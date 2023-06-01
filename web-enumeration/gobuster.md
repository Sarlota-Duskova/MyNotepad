# Gobuster

`GoBuster` is a tool used to brute-force URIs (directories and files), DNS subdomains and virtual host names.

### "dir" Mode

`gobuster dir` for directory search

`gobuster dir -u http://10.10.10.10 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt`

<table><thead><tr><th width="99" align="center">Flag</th><th width="226" align="center">Long Flag</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">-c</td><td align="center">--cookies</td><td align="center">Cookies to use for requests</td></tr><tr><td align="center">-x</td><td align="center">--extensions</td><td align="center">File extension(s) to search for</td></tr><tr><td align="center">-H</td><td align="center">--headers</td><td align="center">Specify HTTP headers, -H 'Header1: val1' -H 'Header2: val2'</td></tr><tr><td align="center">-k</td><td align="center">--no-tls-validation</td><td align="center">Skip TLS certificate verification</td></tr><tr><td align="center">-n</td><td align="center">--no-status</td><td align="center">Don't print status codes</td></tr><tr><td align="center">-P</td><td align="center">--password</td><td align="center">Password for Basic Auth</td></tr><tr><td align="center">-s</td><td align="center">--status-codes</td><td align="center">Positive status codes</td></tr><tr><td align="center">-b</td><td align="center">--status-codes-blacklist</td><td align="center">Negative status codes</td></tr><tr><td align="center">-U</td><td align="center">--username</td><td align="center">Username for Basic Auth</td></tr></tbody></table>

`curl -s http://10.10.10.10/whatever` `echo -n "neco==" | base64 -d`

### "dns" Mode

`gobuster dns` for brute-force subdomain

`gobuster dns -d mydomain.thm -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt`

### "vhost" Mode

`gobuster vhost` for brute-force virtual hosts. Virtual hosts are different websites on the same machine.

`gobuster vhost -u http://example.com -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt`
