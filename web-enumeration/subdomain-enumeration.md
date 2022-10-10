# Subdomain enumeration

### Brute Force

Bruteforce DNS (Domain Name System)

### OSINT (Open-Source Intelligence)

#### SSL/TLS Certificates (Secure Sockets Layer/Transport Layer Security)

https://crt.sh

* When an SSL/TLS certificate is created for a domain by a CA (Certificate Authority), CA's take part in what's called "Certificate Transparency (CT) logs".
* These are publicly accessible logs of every SSL/TLS certificate created for a domain name.
* The purpose of Certificate Transparency logs is to stop malicious and accidentally made certificates from being used.

#### Search Engines

On Google use the search term -site:www.tryhackme.com site:\*.tryhackme.com

#### Sublist3r

`./sublist3r.py -d tryhackme.com`

### Virtual Host

`ffuf -w /usr/share/wordlists/SecLists/Discovery/DNS/namelist.txt -H "Host: FUZZ.acmeitsupport.thm" -u http://10.10.97.97 -fs 503`
