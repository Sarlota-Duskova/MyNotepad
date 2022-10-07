# Basics of Windows

### Alternate Data Streams (ADS)

* Is a file attribute specific to Windows NTFS (New Technology File System).
* Every file has at least one data stream ($DATA), and ADS allows files to contain more than one stream of data.
* The system environment variable for the Windows directory is %windir%.
* The System Configuration utility (MSConfig)&#x20;
* The Computer Management (compmgmt)&#x20;
* The Local Users and Groups (lusrmgr.msc)
* The Performance Monitor (perfmon)
* The System Information (msinfo32)
* The Resource Monitor (resmon)
* The command prompt (cmd)
  * Ipconfig /? Shows a help
  * Whoami
  * Hostname
  * Cls stand for clear
  * Netstat
* the Registry Editor (regedit)

**Windows Update** could run from cmd `control /name Microsoft.WindowsUpdate`

Windows Defender Firewall is `WF.msc`

**the Volume Shadow Copy Service (VSS)**

* Coordinates the required actions to create a consistent shadow copy (also known as a snapshot or a point-in-time copy) of the data that is to be backed up.&#x20;

**smss.exe (Session Manager Subsystem) = Windows Session Manager**

* Smss.exe starts csrss.exe (Windows subsystem) and wininit.exe in Session 0, an isolated Windows session for the operating system, and csrss.exe and winlogon.exe for Session 1, which is the user session.
* The first child instance creates child instances in new sessions.
* This is done by smss.exe copying itself into the new session and self-terminating.

**csrss.exe (Client Server Runtime Process)**

* This process is responsible for the Win32 console window and process thread creation and deletion.
* For each instance csrsrv.dll, basesrv.dll, and winsrv.dll are loaded (along with others).&#x20;

**The Windows Initialization Process, wininit.exe**

* Is responsible for launching services.exe (Service Control Manager), lsass.exe (Local Security Authority), and lsaiso.exe within Session 0.
* This is another critical Windows process that runs in the background, along with its child processes.&#x20;

&#x20;**the Service Control Manager (SCM)**

* Which is services.exe.
* Its primary responsibility is to handle system services: loading services, interacting with services, starting/ending services, etc.
* It maintains a database that can be queried using a Windows built-in utility, 'sc.exe.'&#x20;

**The Service Host (Host Process for Windows Services)**

* svchost.exe, is responsible for hosting and managing Windows services.&#x20;
* Since svchost.exe will always have multiple running processes on any Windows system, this process has been a target for malicious use.
* Adversaries create malware to masquerade as this process and try to hide amongst the legitimate svchost.exe processes.
* They can name the malware svchost.exe or misspell it slightly, such as scvhost.exe.
* By doing so the intention is to go under the radar.
* Another tactic is to install/call a malicious service (DLL). &#x20;

**Local Security Authority Subsystem Service (LSASS)**

* Is a process in Microsoft Windows operating systems that is responsible for enforcing the security policy on the system.
* It verifies users logging on to a Windows computer or server, handles password changes, and creates access tokens.
* It also writes to the Windows Security Log.
* It creates security tokens for SAM (Security Account Manager), AD (Active Directory), and NETLOGON.
* It uses authentication packages specified in HKLM\System\CurrentControlSet\Control\Lsa.
* Parrent proces sis wininit.exe

**The Windows Logon, winlogon.exe**

* Is responsible for handling the Secure Attention Sequence (SAS).
* This is the ALT+CTRL+DELETE key combination users press to enter their username & password.&#x20;
* This process is also responsible for loading the user profile.
* This is done by loading the user's NTUSER.DAT into HKCU and via userinit.exe loads the user's shell.

**the Windows Explorer, explorer.exe**

* This is the process that gives the user access to their folders and files.
* It also provides functionality to other features such as the Start Menu, Taskbar, etc.&#x20;
