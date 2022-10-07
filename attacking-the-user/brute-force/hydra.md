# Hydra

**Hydra has the ability to bruteforce the following protocols:** Asterisk, AFP, Cisco AAA, Cisco auth, Cisco enable, CVS, Firebird, FTP, HTTP-FORM-GET, HTTP-FORM-POST, HTTP-GET, HTTP-HEAD, HTTP-POST, HTTP-PROXY, HTTPS-FORM-GET, HTTPS-FORM-POST, HTTPS-GET, HTTPS-HEAD, HTTPS-POST, HTTP-Proxy, ICQ, IMAP, IRC, LDAP, MS-SQL, MYSQL, NCP, NNTP, Oracle Listener, Oracle SID, Oracle, PC-Anywhere, PCNFS, POP3, POSTGRES, RDP, Rexec, Rlogin, Rsh, RTSP, SAP/R3, SIP, SMB, SMTP, SMTP Enum, SNMP v1+v2+v3, SOCKS5, SSH (v1 and v2), SSHKEY, Subversion, Teamspeak (TS2), Telnet, VMware-Auth, VNC and XMPP.

`hydra -l user -P passlist.txt ftp://MACHINE_IP`

#### SSH

`hydra -l <username> -P <full path to pass> MACHINE_IP -t 4 ssh`

| Option |              Description              |
| :----: | :-----------------------------------: |
|   -l   |            single username            |
|   -L   |        use a list of usernames        |
|   -p   |            single password            |
|   -P   |        use a list of passwords        |
|   -t   | specifes the number of threads to use |

#### Post Web Form

`hydra -l <username> -P <wordlist> 10.10.126.20 http-post-form "/:username=^USER^&password=^PASS^:F=incorrect" -V`

|     Option     |                          Description                          |
| :------------: | :-----------------------------------------------------------: |
| http-post-form |               indicates the type of form (post)               |
|   /login url   |                       the login page URL                      |
|    :username   |          the form field where the username is entered         |
|     ^USER^     |                tells Hydra to use the username                |
|    password    |          the form field where the password is entered         |
|     ^PASS^     |     tells Hydra to use the password list supplied earlier     |
|      Login     |          indicates to Hydra the Login failed message          |
|  Login failed  |       is the login failure message that the form returns      |
|   F=incorrect  |        If this word appears on the page, its incorrect        |
|    -V or -vV   |    Show the username and password combinations being tried    |
|       -d       | Display debugging output if the verbose output is not helping |
