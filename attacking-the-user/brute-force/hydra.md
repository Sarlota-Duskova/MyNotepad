# Hydra

**Hydra has the ability to bruteforce the following protocols:** Asterisk, AFP, Cisco AAA, Cisco auth, Cisco enable, CVS, Firebird, FTP, HTTP-FORM-GET, HTTP-FORM-POST, HTTP-GET, HTTP-HEAD, HTTP-POST, HTTP-PROXY, HTTPS-FORM-GET, HTTPS-FORM-POST, HTTPS-GET, HTTPS-HEAD, HTTPS-POST, HTTP-Proxy, ICQ, IMAP, IRC, LDAP, MS-SQL, MYSQL, NCP, NNTP, Oracle Listener, Oracle SID, Oracle, PC-Anywhere, PCNFS, POP3, POSTGRES, RDP, Rexec, Rlogin, Rsh, RTSP, SAP/R3, SIP, SMB, SMTP, SMTP Enum, SNMP v1+v2+v3, SOCKS5, SSH (v1 and v2), SSHKEY, Subversion, Teamspeak (TS2), Telnet, VMware-Auth, VNC and XMPP.

`hydra -l user -P passlist.txt ftp://MACHINE_IP`

#### SSH

`hydra -l <username> -P <full path to pass> MACHINE_IP -t 4 ssh`

<table><thead><tr><th width="171.5" align="center">Option</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">-l</td><td align="center">single username</td></tr><tr><td align="center">-L</td><td align="center">use a list of usernames</td></tr><tr><td align="center">-p</td><td align="center">single password</td></tr><tr><td align="center">-P</td><td align="center">use a list of passwords</td></tr><tr><td align="center">-t</td><td align="center">specifes the number of threads to use</td></tr></tbody></table>

#### Post Web Form

`hydra -l <username> -P <wordlist> 10.10.126.20 http-post-form "/:username=^USER^&password=^PASS^:F=incorrect" -V`

<table><thead><tr><th width="168.5" align="center">Option</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">http-post-form</td><td align="center">indicates the type of form (post)</td></tr><tr><td align="center">/login url</td><td align="center">the login page URL</td></tr><tr><td align="center">:username</td><td align="center">the form field where the username is entered</td></tr><tr><td align="center">^USER^</td><td align="center">tells Hydra to use the username</td></tr><tr><td align="center">password</td><td align="center">the form field where the password is entered</td></tr><tr><td align="center">^PASS^</td><td align="center">tells Hydra to use the password list supplied earlier</td></tr><tr><td align="center">Login</td><td align="center">indicates to Hydra the Login failed message</td></tr><tr><td align="center">Login failed</td><td align="center">is the login failure message that the form returns</td></tr><tr><td align="center">F=incorrect</td><td align="center">If this word appears on the page, its incorrect</td></tr><tr><td align="center">-V or -vV</td><td align="center">Show the username and password combinations being tried</td></tr><tr><td align="center">-d</td><td align="center">Display debugging output if the verbose output is not helping</td></tr></tbody></table>
