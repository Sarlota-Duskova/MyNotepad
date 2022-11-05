# Passive recon

* `whois` - find names, email addresses, postal addresses, and phone numbers, the authoritative name servers for the domain in question.
* DNS queries can be executed with `nslookup`
* `dig` Domain Information Groper.  Provides a lot of query options and even allows you to specify a different DNS server to use.&#x20;
* `host` is another useful alternative for querying DNS servers for DNS records.&#x20;
* &#x20;Unix-like systems is `traceroute`, or on MS Windows systems, `tracert`. Traces the route taken by the packets from our system to the target host.

### Advanced searching

| Symbol / Syntax                  | Function                                            |
| -------------------------------- | --------------------------------------------------- |
| `"search phrase"`                | Find results with exact search phrase               |
| `OSINT filetype:pdf`             | Find files of type `PDF` related to a certain term. |
| `salary site:blog.tryhackme.com` | Limit search results to a specific site.            |
| `pentest -site:example.com`      | Exclude a specific site from results                |
| `walkthrough intitle:TryHackMe`  | Find pages with a specific term in the page title.  |
| `challenge inurl:tryhackme`      | Find pages with a specific term in the page URL.    |

{% embed url="https://web.archive.org" %}
Internet archiv
{% endembed %}

{% embed url="https://www.exploit-db.com/google-hacking-database" %}
Exploit DB
{% endembed %}

### View DNS info

{% embed url="https://viewdns.info" %}
Website
{% endembed %}

### Threat Intelligence Platform

Provide a domain name or an IP address, and it will launch a series of tests from malware checks to WHOIS and DNS queries.

{% embed url="https://threatintelligenceplatform.com" %}
Website
{% endembed %}

### **Censys**

Can provide a lot of information about IP addresses and domains.

{% embed url="https://search.censys.io" %}
Website
{% endembed %}
