# Gobuster

`GoBuster` is a tool used to brute-force URIs (directories and files), DNS subdomains and virtual host names.

### "dir" Mode

`gobuster dir` for directory search

`gobuster dir -u http://10.10.10.10 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt`

| Flag |         Long Flag        |                         Description                         |
| :--: | :----------------------: | :---------------------------------------------------------: |
|  -c  |         --cookies        |                 Cookies to use for requests                 |
|  -x  |       --extensions       |               File extension(s) to search for               |
|  -H  |         --headers        | Specify HTTP headers, -H 'Header1: val1' -H 'Header2: val2' |
|  -k  |    --no-tls-validation   |              Skip TLS certificate verification              |
|  -n  |        --no-status       |                   Don't print status codes                  |
|  -P  |        --password        |                   Password for Basic Auth                   |
|  -s  |      --status-codes      |                    Positive status codes                    |
|  -b  | --status-codes-blacklist |                    Negative status codes                    |
|  -U  |        --username        |                   Username for Basic Auth                   |

`curl -s http://10.10.10.10/whatever` `echo -n "neco==" | base64 -d`

### "dns" Mode

`gobuster dns` for brute-force subdomain

`gobuster dns -d mydomain.thm -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt`

### "vhost" Mode

`gobuster vhost` for brute-force virtual hosts. Virtual hosts are different websites on the same machine.

`gobuster vhost -u http://example.com -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt`
