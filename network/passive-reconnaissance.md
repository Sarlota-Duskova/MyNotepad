# Passive Reconnaissance



* `whois DOMAIN_NAME` to query WHOIS servers
* `nslookup OPTIONS DOMAIN_NAME SERVER` to query DNS servers
  * **OPTIONS** `A` for IPv4 addresses and `AAAA` for IPv6 addresses.
  * **SERVER** is the DNS server that you want to query.
    * You can choose any local or public DNS server to query.
    * Cloudflare offers 1.1.1.1 and 1.0.0.1, Google offers 8.8.8.8 and 8.8.4.4, and Quad9 offers 9.9.9.9 and 149.112.112.112.

| Query type |       Result       |
| :--------: | :----------------: |
|      A     |   IPv4 Addresses   |
|    AAAA    |   IPv6 Addresses   |
|    CNAME   |   Canonical Name   |
|     MX     |    Mail Servers    |
|     SOA    | Start of Authority |
|     TX     |     TXT Records    |

`nslookup -type=A tryhackme.com 1.1.1.1`

* `dig @SERVER DOMAIN_NAME TYPE` to query DNS servers

1. Passive Reconnaissance

* In passive reconnaissance, you rely on publicly available knowledge.
* It is the knowledge that you can access from publicly available resources without directly engaging with the target.
* Looking up DNS records of a domain from a public DNS server.
* Checking job ads related to the target website.
* Reading news articles about the target company.

1. Active Reconnaissance

* Connecting to one of the company servers such as HTTP, FTP, and SMTP.
* Calling the company in an attempt to get information (social engineering).
* Entering company premises pretending to be a repairman.
