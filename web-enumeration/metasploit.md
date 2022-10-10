# Metasploit

`msfconsole` command

* **Exploit**
  * A piece of code that uses a vulnerability present on the target system.
* **Vulnerability**
  * A design, coding, or logic flaw affecting the target system.
  * The exploitation of a vulnerability can result in disclosing confidential information or allowing the attacker to execute code on the target system.
* **Payload**
  * An exploit will take advantage of a vulnerability.
  * However, if we want the exploit to have the result we want (gaining access to the target system, read confidential information, etc.), we need to use a payload.
  * Payloads are the code that will run on the target system.

**Three different directories under payloads:**

* **Singles:** Self-contained payloads (add user, launch notepad.exe, etc.) that do not need to download an additional component to run.
* **Stagers:** Responsible for setting up a connection channel between Metasploit and the target system. Useful when working with staged payloads. “Staged payloads” will first upload a stager on the target system then download the rest of the payload (stage). This provides some advantages as the initial size of the payload will be relatively small compared to the full payload sent at once.
* **Stages:** Downloaded by the stager. This will allow you to use larger sized payloads.

**Auxiliary:** Any supporting module, such as scanners, crawlers and fuzzers

**Encoders:** Encoders will allow you to encode the exploit and payload in the hope that a signature-based antivirus solution may miss them

**Evasion:** While encoders will encode the payload, they should not be considered a direct attempt to evade antivirus software.

**Exploits:** Exploits, neatly organized by target system.

**NOPs:** NOPs (No OPeration) do nothing, literally.

**Payloads:** Payloads are codes that will run on the target system.

`exploit/windows/smb/ms17_010_eternalblue` command

* The "EternalBlue" is an exploit allegedly developed by the U.S. National Security Agency (N.S.A.)
* The SMB (Server Message Block) is widely used in Windows networks for file sharing and even for sending files to printers.

`show options` `back` command will leave to msf `search` command

Parameters:

* **RHOSTS:** “Remote host”, the IP address of the target system. A single IP address or a network range can be set. This will support the CIDR (Classless Inter-Domain Routing) notation (/24, /16, etc.) or a network range (10.10.10.x – 10.10.10.y).
* **RPORT:** “Remote port”, the port on the target system the vulnerable application is running on.
* **PAYLOAD:** The payload you will use with the exploit.
* **LHOST:** “Localhost”, the attacking machine (your AttackBox or Kali Linux) IP address.
* **LPORT:** “Local port”, the port you will use for the reverse shell to connect back to. This is a port on your attacking machine, and you can set it to any port not used by any other application.
* **SESSION:** Each connection established to the target system using Metasploit will have a session ID. You will use this with post-exploitation modules that will connect to the target system using an existing connection.

The difference is that if you use the `set` command to set a value using a module and you switch to another module, you will need to set the value again. The `setg` command allows you to set the value so it can be used by default across different modules. You can clear any value set with `setg` using `unsetg`

`exploit` command The`exploit -z` command will run the exploit and background the session as soon as it opens.

Some modules support the `check` option. This will check if the target system is vulnerable without exploiting it.

The `background` command to background the session prompt and go back to the msfconsole prompt.

The `sessions` command can be used from the msfconsole prompt or any context to see the existing sessions.

To interact with any session, the `sessions -i` command followed by the desired session number.

## Metasploit Databases

`systemctl start postgresql` Then you will need to initialize the Metasploit Database using the `msfdb init` command. now launch `msfconsole` and check the database status using the `db_status` command. list available workspaces using the `workspace` command

* add a workspace using the `-a` parameter
* delete a workspace using the `-d` paramete

the `workspace -h` command to list available options for the `workspace` command Nmap scan using the `db_nmap` `db_nmap -sV -p- IP_ADDRESS` `hosts` and `services` commands

the `vnc_login` module can help us find login details for the VNC service
