# Questions

1.  During the reconnaissance stage of a penetration test, Cynthia needs to gather information about the target organization's network infrastructure without causing an IPS to alert the target to her information gathering. Which of the following is her best option?

    1. Perform a DNS brute-force attack.
    2. Use an Nmap ping sweep.
    3. Perform a DNS zone transfer.
    4. Use an Nmap stealth scan.

    Answer:

    A. Although it may seem strange, a DNS brute-force attack that queries a list of IP addresses, common subdomains, or other lists of targets will often bypass intrusion detection and prevention systems that do not pay particular attention to DNS queries. Cynthia may even be able to find a DNS server that is not protected by the organization's IPS! Nmap scans are commonly used during reconnaissance, and Cynthia can expect them to be detected since they are harder to conceal. Cynthia shouldn't expect to be able to perform a DNS zone transfer, and if she can, a well-configured IPS should immediately flag the event.
2.  A port scan of a remote system shows that port 3306 is open on a remote database server. What database is the server most likely running?

    1. Oracle
    2. Postgres
    3. MySQL
    4. Microsoft SQL

    Answer:

    C. MySQL uses port 3306 as its default port. Oracle uses 1521, Postgres uses 5432, and Microsoft SQL uses 1433/1434.
3.  During a port scan of her network, Cynthia discovers a workstation that shows the following ports open. What should her next action be?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf001.jpg)

    1. Determine the reason for the ports being open.
    2. Investigate the potentially compromised workstation.
    3. Run a vulnerability scan to identify vulnerable services.
    4. Reenable the workstation's local host firewall.

    Answer:

    A. Cynthia's first action should be to determine whether there is a legitimate reason for the workstation to have the listed ports open.
4.  Which one of the following threats is the most pervasive in modern computing environments?

    1. Zero-day attacks
    2. Advanced persistent threats
    3. Malware
    4. Insider threats

    Answer:

    C. All of the threats described here are serious threats that exist in modern enterprises. However, the most pervasive threat is standard malware, which threatens essentially every computing environment on an almost constant basis.
5.  Nara is concerned about the risk of attackers conducting a brute-force attack against her organization. Which one of the following factors is Nara most likely to be able to control?

    1. Attack vector
    2. Adversary capability
    3. Likelihood
    4. Total attack surface

    Answer:

    D. Nara can reduce the number of services in her environment that are exposed to a brute-force attack. This is a means of reducing the total attack surface. She can't alter characteristics of her adversary, such as the adversary's capability, choice of attack vectors, or likelihood of launching an attack.
6.  What is the default Nmap scan type when Nmap is not provided with a scan type flag?

    1. A TCP FIN scan
    2. A TCP connect scan
    3. A TCP SYN scan
    4. A UDP scan

    Answer:

    C. By default, Nmap uses a TCP SYN scan. If the user does not have proper socket privileges (such as root on a Linux system), it will use a TCP connect scan.
7.  Lakshman wants to limit what potential attackers can gather during passive or semipassive reconnaissance activities. Which of the following actions will typically most reduce his organization's footprint?

    1. Limit information available via the organizational website without authentication.
    2. Use a secure domain registration.
    3. Limit technology references in job postings.
    4. Purge all document metadata before posting.

    Answer:

    A. Limiting the information available about an organization by requiring authentication will strongly limit the ability of potential attackers to gather information. Secure domain registration may conceal the registration contact's information but does not provide any real additional protection. Limiting technologies listed in a job posting can help limit what attackers may find out, but most organizations would prefer to better match candidates. Finally, purging all metadata can help protect information about internal systems and devices but is difficult to enforce, and document metadata is not a primary source of information about most organizations.
8.  Cassandra's Nmap scan of an open wireless network (192.168.10/24) shows the following host at IP address 192.168.1.1. Which of the following is most likely to be the type of system at that IP address based on the scan results shown?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf002.jpg)

    1. A virtual machine
    2. A wireless router
    3. A broadband router
    4. A print server

    Answer:

    B. Since Cassandra is scanning a wireless network and the system is using an IP address that is commonly used for commodity wireless routers, her best guess should be that this is a wireless router that can be accessed via SSH and that is providing a web management interface and print services. The actual host scanned is an Asus router running open source firmware and additional software.
9.  Several organizations recently experienced security incidents when their AWS secret keys were published in public GitHub repositories. What is the most significant threat that could arise from this improper key management?

    1. Total loss of confidentiality
    2. Total loss of integrity
    3. Total loss of availability
    4. Total loss of confidentiality, integrity, and availability

    Answer:

    D. Depending on the level of access associated with the key, this error could give anyone discovering the key total control of an organization's AWS account, resulting in a complete loss of confidentiality, integrity, and availability.
10. After Kristen received a copy of an Nmap scan run by a penetration tester that her company hired, she knows that the tester used the `-O` flag. What type of information should she expect to see included in the output other than open ports?

    1. OCMP status
    2. Other ports
    3. Objective port assessment data in verbose mode
    4. Operating system and Common Platform Enumeration (CPE) data

    Answer:

    D. Nmap provides Common Platform Enumeration data when the `-O` (OS fingerprinting) and verbose flags are used. If Kristen had seen the `-sV` flag instead, she would have expected service version information.
11. Andrea wants to conduct a passive footprinting exercise against a target company. Which of the following techniques is not suited to a passive footprinting process?

    1. WHOIS lookups
    2. Banner grabbing
    3. BGP looking glass usage
    4. Registrar checks

    Answer:

    B. Banner grabbing is an active process and requires a connection to a remote host to grab the banner. The other methods are all passive and use third-party information that does not require a direct lookup against a remote host.
12. Alex wants to scan a protected network and has gained access to a system that can communicate to both his scanning system and the internal network, as shown in the image here. What type of Nmap scan should Alex conduct to leverage this host if he cannot install Nmap on system A?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf003.jpg)

    1. A reflection scan
    2. A proxy scan
    3. A randomized host scan
    4. A ping-through scan

    Answer:

    B. Nmap supports the use of both HTTP and SOCKS4 proxies, allowing Alex to configure the remote host as an HTTP proxy and bounce his scans through it. This can allow Nmap users to leverage their scanning tools without installing them on a protected host or network.
13. Maddox is conducting an inventory of access permissions on cloud-based object buckets, such as those provided by the AWS S3 service. What threat is he seeking to mitigate?

    1. Insecure APIs
    2. Improper key management
    3. Unprotected storage
    4. Insufficient logging and monitoring

    Answer:

    C. Maddox's actions could identify improperly secured storage buckets that require remediation. While the other vulnerabilities could exist in Maddox's cloud environment, they are not likely to be discovered during a permissions inventory.
14. Alex has been asked to assess the likelihood of reconnaissance activities against her organization (a small, regional business). Her first assignment is to determine the likelihood of port scans against systems in her organization's screened subnet (otherwise known as a DMZ). How should she rate the likelihood of this occurring?

    1. Low.
    2. Medium.
    3. High.
    4. There is not enough information for Alex to provide a rating.

    Answer:

    C. Alex knows that systems that are exposed to the Internet like screened subnet (DMZ) systems are constantly being scanned. She should rate the likelihood of the scan occurring as high. In fact, there is a good chance that a scan will be occurring while she is typing up her report!
15. Lucy recently detected a cross-site scripting (XSS) vulnerability in her organization's web server. The organization operates a support forum where users can enter HTML tags and the resulting code is displayed to other site visitors. What type of cross-site scripting vulnerability did Lucy discover?

    1. Persistent
    2. Reflected
    3. DOM-based
    4. Blind

    Answer:

    A. This type of XSS vulnerability, where the attack is stored on a server for later users, is a persistent vulnerability. The scenario does not tell us that the code is immediately displayed to the user submitting it, so there is no indication of a reflected attack. The attack is stored on the server, rather than in the browser, so it is not a DOM-based attack. Blind XSS attacks do not exist.
16. Florian discovered a vulnerability in a proprietary application developed by his organization. The application has a flaw that allows users to log into the system by providing a valid username and leaving the password blank. What term best describes this overflow?

    1. Directory traversal
    2. Stack overflow
    3. Injection flaw
    4. Broken access control

    Answer:

    D. This is an example of a broken access control system. The system is clearly intended to require that users provide a valid password during the authentication process. This approach is broken, however, because the user is able to log in without providing the password.
17. The company that Dan works for has recently migrated to an SaaS provider for its enterprise resource planning (ERP) software. In its traditional on-site ERP environment, Dan conducted regular port scans to help with security validation for the systems. What will Dan most likely have to do in this new environment?

    1. Use a different scanning tool.
    2. Rely on vendor testing and audits.
    3. Engage a third-party tester.
    4. Use a VPN to scan inside the vendor's security perimeter.

    Answer:

    B. Most SaaS providers do not want their customers conducting port scans of their service, and many are glad to provide security assertions and attestations including audits, testing information, or contractual language that addresses potential security issues. Using a different scanning tool, engaging a third-party tester, or even using a VPN are not typically valid answers in a scenario like this.
18. Which one of the following languages is least susceptible to an injection attack?

    1. HTML
    2. SQL
    3. STIX
    4. XML

    Answer:

    C. STIX is a language used to define security threat information and is not a common target of injection attacks. SQL injection and XML injection attacks commonly take place against applications using those languages. Cross-site scripting (XSS) attacks are a common example of an injection attack against HTML documents.
19. Which one of the following types of malware would be most useful in a privilege escalation attack?

    1. Rootkit
    2. Worm
    3. Virus
    4. RAT

    Answer:

    A. Rootkits are specifically designed for privilege escalation attacks, providing the ability to escalate a normal user account into an administrative account.
20. Abdul is conducting a security audit of a multicloud computing environment that incorporates resources from AWS and Microsoft Azure. Which one of the following tools will be least useful to him?

    1. ScoutSuite
    2. Pacu
    3. Prowler
    4. CloudSploit

    Answer:

    B. Pacu is an AWS-specific tool that will not be useful in a multi-cloud environment. ScoutSuite, Prowler, and CloudSploit can all test both AWS and Azure environments.
21. Greg is concerned about the use of DDoS attack tools against his organization, so he purchased a mitigation service from his ISP. What portion of the threat model did Greg reduce?

    1. Likelihood
    2. Total attack surface
    3. Impact
    4. Adversary capability

    Answer:

    C. By purchasing a mitigation service, Greg is reducing the potential impact of a DDoS attack. This service can't reduce the likelihood that an attacker will launch an attack or the capability of that adversary. Greg did not change his own infrastructure, so he did not reduce the total attack surface.
22. Carrie needs to lock down a Windows workstation that has recently been scanned using Nmap with the results shown here. She knows that the workstation needs to access websites and that the system is part of a Windows domain. What ports should she allow through the system's firewall for externally initiated connections?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf004.jpg)

    1. 80, 135, 139, and 445.
    2. 80, 445, and 3389.
    3. 135, 139, and 445.
    4. No ports should be open.

    Answer:

    D. The uses described for the workstation that Carrie is securing do not require inbound access to the system on any of these ports. Web browsing and Active Directory domain membership traffic can be handled by traffic initiated by the system.
23. Adam's port scan returns results on six TCP ports: 22, 80, 443, 515, 631, and 9100. If Adam needs to guess what type of device this is based on these ports, what is his best guess?

    1. A web server
    2. An FTP server
    3. A printer
    4. A proxy server

    Answer:

    C. Whereas the first three ports are common to many of the devices listed, TCP 515 is the LPR/LPD port, 631 is the IPP port commonly used by many print servers, and TCP port 9100 is the RAW, or direct, IP port. Although this could be another type of device, it is most likely a network-connected printer.
24. In his role as the SOC operator, Manish regularly scans a variety of servers in his organization. After two months of reporting multiple vulnerabilities on a Windows file server, Manish recently escalated the issue to the server administrator's manager.

    At the next weekly scan window, Manish noticed that all the vulnerabilities were no longer active; however, ports 137, 139, and 445 were still showing as open. What most likely happened?

    1. The server administrator blocked the scanner with a firewall.
    2. The server was patched.
    3. The vulnerability plug-ins were updated and no longer report false positives.
    4. The system was offline.

    Answer:

    B. The system is showing normal ports for a Windows file server. It is most likely that Manish's escalation to management resulted in action by the server administrator.
25. While conducting reconnaissance, Piper discovers what she believes is an SMTP service running on an alternate port. What technique should she use to manually validate her guess?

    1. Send an email via the open port.
    2. Send an SMTP probe.
    3. Telnet to the port.
    4. SSH to the port.

    Use the following network diagram and scenario to answer questions 26–28.

    Marta is a security analyst who has been tasked with performing Nmap scans of her organization's network. She is a new hire and has been given this logical diagram of the organization's network but has not been provided with any additional detail.

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf005.jpg)

    Answer:

    C. Using telnet to connect to remote services to validate their response is a useful technique for service validation. It doesn't always work, but it can allow you to interact with the service to gather information manually. While telnet is an insecure service and should not typically be used, the `telnet` command is a valuable way to test connectivity to an SMTP server. A more secure tool that uses encryption, such as SSH, would not provide visibility into the SMTP service because SMTP is not set up to accept SSH connections.
26. Marta wants to determine what IP addresses to scan from location A. How can she find this information?

    1. Scan the organization's web server and then scan the other 255 IP addresses in its subnet.
    2. Query DNS and WHOIS to find her organization's registered hosts.
    3. Contact ICANN to request the data.
    4. Use `traceroute` to identify the network that the organization's domain resides in.

    Answer:

    B. Marta's best option from this list is to query DNS using WHOIS. She might also choose to use a BGP looking glass, but most of the information she will need will be in WHOIS. If she simply scans the network the web server is in, she may end up scanning a third-party hosting provider or other systems that aren't owned by her organization in the `/24` subnet range. Contacting ICANN isn't necessary with access to WHOIS, and depending on what country Marta is in, ICANN may not have the data she wants. Finally, using `traceroute` will only show the IP address of the system she queries; she needs more data to perform a useful scan in most instances.
27. If Marta runs a scan from location B that targets the servers on the datacenter network and then runs a scan from location C, what differences is she most likely to see between the scans?

    1. The scans will match.
    2. Scans from location C will show no open ports.
    3. Scans from location C will show fewer open ports.
    4. Scans from location C will show more open ports.

    Answer:

    C. Scans from location C will show fewer open ports because most datacenter firewalls are configured to only allow the ports for publicly accessible services through to other networks. Location C is on an internal network, so Marta will probably see more ports than if she tried to scan datacenter systems from location A, but it is likely that she will see far fewer ports than a port scan of the datacenter from inside the datacenter firewall will show.
28. Marta wants to perform regular scans of the entire organizational network but only has a budget that supports buying hardware for a single scanner. Where should she place her scanner to have the most visibility and impact?

    1. Location A
    2. Location B
    3. Location C
    4. Location D

    Answer:

    B. Marta will see the most important information about her organization at location B, which provides a view of datacenter servers behind the datacenter firewall. To get more information, she should request that the client network firewall ruleset include a rule allowing her scanner to scan through the firewall to all ports for all systems on all protocols.
29. Chris wants to gather as much information as he can about an organization using DNS harvesting techniques. Which of the following methods will easily provide the most useful information if they are all possible to conduct on the network he is targeting?

    1. DNS record enumeration
    2. Zone transfer
    3. Reverse lookup
    4. Domain brute-forcing

    Answer:

    B. If Chris can perform a zone transfer, he can gather all of the organization's DNS information, including domain servers, hostnames, MX and CNAME records, time to live records, zone serial number data, and other information. This is the easiest way to gather the most information about an organization via DNS if it is possible. Unfortunately, for penetration testers (and attackers!), few organizations allow untrusted systems to perform zone transfers.
30. Geoff wants to perform passive reconnaissance as part of an evaluation of his organization's security controls. Which of the following techniques is a valid technique to perform as part of a passive DNS assessment?

    1. A DNS forward or reverse lookup
    2. A zone transfer
    3. A WHOIS query
    4. Using maltego

    Answer:

    C. Performing a WHOIS query is the only passive reconnaissance technique listed. Each of the other techniques performs an active reconnaissance task.
31. Mike's penetration test requires him to use passive mapping techniques to discover network topology. Which of the following tools is best suited to that task?

    1. Wireshark
    2. `nmap`
    3. `netcat`
    4. Angry IP Scanner

    Answer:

    A. Passive network mapping can be done by capturing network traffic using a sniffing tool like Wireshark. Active scanners including `nmap`, the Angry IP Scanner, and `netcat` (with the `-z` flag for port scanning) could all set off alarms as they scan systems on the network.
32. When Scott performs an `nmap` scan with the `-T` flag set to 5, what variable is he changing?

    1. How fast the scan runs
    2. The TCP timeout flag it will set
    3. How many retries it will perform
    4. How long the scan will take to start up

    Answer:

    A. The `nmap -T` command accepts a setting between 0 (or “paranoid”) and 5 (or “insane”). When Scott sets his scan to use the insane setting, it will perform the fastest scanning it can, which will likely set off any IDS or IPS that is watching for scans.
33. While application vulnerability scanning one of her target organizations web servers, Andrea notices that the server's hostname is resolving to a [`cloudflare.com`](http://cloudflare.com/) host. What does Andrea know about her scan?

    1. It is being treated like a DDoS attack.
    2. It is scanning a CDN-hosted copy of the site.
    3. It will not return useful information.
    4. She cannot determine anything about the site based on this information.

    Answer:

    B. Cloudflare, Akamai, and other content distribution networks (CDNs) use a network of distributed servers to serve information closer to requesters. In some cases, this may make parts of a vulnerability scan less useful, whereas others may remain valid. Here, Andrea simply knows that the content is hosted in a CDN and that she may not get all the information she wants from a scan.
34. Part of Tracy's penetration testing assignment is to evaluate the WPA3 Enterprise protected wireless networks of her target organization. What major differences exist between reconnaissances of a wired network versus a wireless network?

    1. Encryption and physical accessibility
    2. Network access control and encryption
    3. Port security and physical accessibility
    4. Authentication and encryption

    Answer:

    A. Tracy knows that most wired networks do not use end-to-end encryption by default and that wireless networks are typically more easily accessible than a wired network that requires physical access to a network jack or a VPN connection from an authorized account. Without more detail, she cannot determine whether authentication is required for both networks, but NAC is a common security feature of wired networks, and WPA3 Enterprise requires authentication as well. Port security is used only for wired network connections.
35. Ian's company has an internal policy requiring that they perform regular port scans of all of their servers. Ian has been part of a recent effort to move his organization's servers to an infrastructure as a service (IaaS) provider. What change will Ian most likely need to make to his scanning efforts?

    1. Change scanning software.
    2. Follow the service provider's scan policies.
    3. Sign a security contract with the provider.
    4. Discontinue port scanning.

    Answer:

    B. Most infrastructure as a service (IaaS) providers will allow their customers to perform security scans as long as they follow the rules and policies for such scans. Ian should review his vendor's security documentation and contact them for details if he has questions.
36. Lauren wants to identify all the printers on the subnets she is scanning with `nmap`. Which of the following `nmap` commands will not provide her with a list of likely printers?

    1. `nmap -sS -p 9100,515,631 10.0.10.15/22 -oX printers.txt`
    2. `nmap -O 10.0.10.15/22 -oG - | grep printer >> printers.txt`
    3. `nmap -sU -p 9100,515,631 10.0.10.15/22 -oX printers.txt`
    4. `nmap -sS -O 10.0.10.15/22 -oG | grep >> printers.txt`

    Answer:

    C. Using a UDP scan, as shown in option C with the `-sU` flag, will not properly identify printers since print service ports are TCP ports. The other commands will properly scan and identify many printers based on either their service ports (515, 631, 9100) or their OS version.
37. What services will the following `nmap` scan test for?

    `nmap -sV -p 22,25,53,389 192.168.2.50/27`

    1. Telnet, SMTP, DHCP, MS-SQL
    2. SSH, SMTP, DNS, LDAP
    3. Telnet, SNMP, DNS, LDAP
    4. SSH, SNMP, DNS, RDP

    Answer:

    B. This `nmap` scan will scan for SSH (22), SMTP (25), DNS (53), and LDAP (389) on their typical ports. If the services are running on an alternate port, this scan will completely miss those and any other services.
38. While conducting a topology scan of a remote web server, Susan notes that the IP addresses returned for the same DNS entry change over time. What has she likely encountered?

    1. A route change
    2. Fast-flux DNS
    3. A load balancer
    4. An IP mismatch

    Answer:

    C. Load balancers can alias multiple servers to the same hostname. This can be confusing when conducting scans, because it may appear that multiple IP addresses or hosts are responding for the same system.
39. Nihar wants to conduct an `nmap` scan of a firewalled subnet. Which of the following is not an `nmap` firewall evasion technique he could use?

    1. Fragmenting packets
    2. Changing packet header flags
    3. Spoofing the source IP
    4. Appending random data

    Answer:

    B. `nmap` supports quite a few firewall evasion techniques including spoofing the MAC (hardware) address, appending random data, setting scan delays, using decoy IP addresses, spoofing the source IP or port, modifying the MTU size, or intentionally fragmenting packets.
40. When Casey scanned a network host, she received the results shown here. What does she know based on the scan results?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf006.jpg)

    1. The device is a Cisco device.
    2. The device is running Red Hat Linux.
    3. The device was built by IBM.
    4. None of the above.

    Answer:

    D. Casey knows that she saw three open ports and that `nmap` took its best guess at what was running on those ports. In this case, the system is actually a CentOS Linux system. This is not a Cisco device, it is not running Red Hat Linux, and it was not built by IBM.
41. Aidan operates the point-of-sale network for a company that accepts credit cards and is thus required to be compliant with PCI DSS. During his regular assessment of the point-of-sale terminals, he discovers that a recent Windows operating system vulnerability exists on all of them. Since they are all embedded systems that require a manufacturer update, he knows that he cannot install the available patch. What is Aidan's best option to stay compliant with PCI DSS and protect his vulnerable systems?

    1. Replace the Windows embedded point-of-sale terminals with standard Windows systems.
    2. Build a custom operating system image that includes the patch.
    3. Identify, implement, and document compensating controls.
    4. Remove the POS terminals from the network until the vendor releases a patch.

    Answer:

    C. When a vulnerability exists and a patch has not been released or cannot be installed, compensating controls can provide appropriate protection. In the case of PCI DSS (and other compliance standards), documenting what compensating controls were put in place and making that documentation available are important steps for compliance.
42. What occurs when Mia uses the following command to perform an `nmap` scan of a network?

    `nmap -sP 192.168.2.0/24`

    1. A secure port scan of all hosts in the 192.168.0.0 to 192.168.2.255 network range
    2. A scan of all hosts that respond to ping in the 192.168.0.0 to 192.168.255.255 network range
    3. A scan of all hosts that respond to ping in the 192.168.2.0 to 192.168.2.255 network range
    4. A SYN-based port scan of all hosts in the 192.168.2.0 to 192.168.2.255 network range

    Answer:

    C. The `-sP` flag for `nmap` indicates a ping scan, and `/24` indicates a range of 255 addresses. In this case, that means `nmap` will scan for hosts that respond to ping in the 192.168.2.0 to 192.168.2.255 IP address range.
43. Amir's remote scans of a target organization's class C network block using the `nmap` command (`nmap -sS 10.0.10.1/24`) show only a single web server. If Amir needs to gather additional reconnaissance information about the organization's network, which of the following scanning techniques is most likely to provide additional detail?

    1. Use a UDP scan.
    2. Perform a scan from on-site.
    3. Scan using the `-p 1-65535` flag.
    4. Use Nmap's IPS evasion techniques.

    Answer:

    B. Performing a scan from an on-site network connection is the most likely to provide more detail. Many organizations have a strong external network defense but typically provide fewer protections for on-site network connections to allow internal users to access services. It is possible that the organization uses services found only on less common ports or UDP only services, but both of these options have a lower chance of being true than for an on-site scan to succeed. Nmap does provide firewall and IPS evasion capabilities, but this is also a less likely scenario.
44. Damian wants to limit the ability of attackers to conduct passive fingerprinting exercises on his network. Which of the following practices will help to mitigate this risk?

    1. Implement an IPS.
    2. Implement a firewall.
    3. Disable promiscuous mode for NICs.
    4. Enable promiscuous mode for NICs.

    Answer:

    C. Passive fingerprinting relies on the ability of a system to capture traffic to analyze. Preventing systems from using promiscuous mode will provide attackers with very little data when performing passive fingerprinting. Both intrusion prevention systems and firewalls can help with active fingerprinting but will do nothing to stop passive fingerprinting.
45. As part of his active reconnaissance activities, Frank is provided with a shell account accessible via SSH. If Frank wants to run a default `nmap` scan on the network behind the firewall shown here, how can he accomplish this?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf007.jpg)

    1. `ssh -t 192.168.34.11 nmap 192.168.34.0/24`
    2. `ssh -R 8080:192.168.34.11:8080 [remote account:remote password]`
    3. `ssh -proxy 192.168.11 [remote account:remote password]`
    4. Frank cannot scan multiple ports with a single `ssh` command.

    Answer:

    D. While SSH port forwarding and SSH tunneling are both useful techniques for pivoting from a host that allows access, `nmap` requires a range of ports open for default scans. He could write a script and forward the full range of ports that `nmap` checks, but none of the commands listed will get him there. If Frank has access to proxy chains, he could do this with two commands.
46. Angela captured the following packets during a reconnaissance effort run by her organization's red team. What type of information are they looking for?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf008.jpg)

    1. Vulnerable web applications
    2. SQL injection
    3. Directory traversal attacks
    4. Passwords

    Answer:

    C. Angela has captured part of a Nikto scan that targets a vulnerable ASP script that allows directory traversal attacks. If it was successful, the contents of files like `/etc/passwd` would be accessible using the web server.
47. Stacey encountered a system that shows as “filtered” and “firewalled” during an `nmap` scan. Which of the following techniques should she not consider as she is planning her next scan?

    1. Packet fragmentation
    2. Spoofing the source address
    3. Using decoy scans
    4. Spoofing the destination address

    Answer:

    D. `nmap` has a number of built-in antifirewall capabilities, including packet fragmentation, decoy scans, spoofing of the source IP address and source port, and scan timing techniques that make detection less likely. Spoofing the target IP address won't help; her packets still need to get to the actual target.
48. Kim is preparing to deploy a new vulnerability scanner and wants to ensure that she can get the most accurate view of configuration issues on laptops belonging to traveling salespeople. Which technology will work best in this situation?

    1. Agent-based scanning
    2. Server-based scanning
    3. Passive network monitoring
    4. Noncredentialed scanning

    Answer:

    A. Using an agent-based scanning approach will provide Kim with the most reliable results for systems that are not always connected to the network. The agent can run the scans and then report results the next time the agent is connected to a network. The other technologies all require that the system be connected to the network during the scan.
49. Carla runs a vulnerability scan of a new appliance that engineers are planning to place on her organization's network and finds the results shown here. Of the actions listed, which would correct the highest criticality vulnerability?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf009.jpg)

    1. Block the use of TLS v1.0.
    2. Replace the expired SSL certificate.
    3. Remove the load balancer.
    4. Correct the information leakage vulnerability.

    Answer:

    B. As Carla reads this report, she should note that the bottom three vulnerabilities have a status of Fixed. This indicates that the information leakage vulnerability is already corrected and that the server no longer supports TLS v1.0. The alert about the load balancer is severity 1, and Carla should treat it as informational. This leaves a severity 2 vulnerability for the expired SSL certificate as the highest-severity issue of the choices presented.
50. Sadiq is responsible for the security of a network used to control systems within his organization's manufacturing plant. The network connects manufacturing equipment, sensors, and controllers. He runs a vulnerability scan on this network and discovers that several of the controllers are running out-of-date firmware that introduces security issues. The manufacturer of the controllers is out of business. What action can Sadiq take to best remediate this vulnerability in an efficient manner?

    1. Develop a firmware update internally and apply it to the controllers.
    2. Post on an Internet message board seeking other organizations that have developed a patch.
    3. Ensure that the ICS is on an isolated network.
    4. Use an intrusion prevention system on the ICS network.

    Answer:

    C. Sadiq should ensure that the industrial control system (ICS) is on an isolated network, unreachable from any Internet-connected system. This greatly reduces the risk of exploitation. It would not be cost-effective to develop a patch himself, and Sadiq should not trust any software that he obtains from an Internet forum. An intrusion prevention system, while a good idea, is not as strong a control as network isolation.
51. Vic scanned a Windows server used in his organization and found the result shown here. The server is on an internal network with access limited to IT staff and is not part of a domain. How urgently should Vic remediate this vulnerability?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf010.jpg)

    1. Vic should drop everything and remediate this vulnerability immediately.
    2. While Vic does not need to drop everything, this vulnerability requires urgent attention and should be addressed quickly.
    3. This is a moderate vulnerability that can be scheduled for remediation at a convenient time.
    4. This vulnerability is informational in nature and may be left in place.

    Answer:

    C. This vulnerability has a severity rating of 3/5 and is further mitigated by the fact that the server is on an internal network, accessible only to trusted staff. This rises above the level of an informational report and should be addressed, but it does not require urgent attention.
52. Rob's manager recently asked him for an overview of any critical security issues that exist on his network. He looks at the reporting console of his vulnerability scanner and sees the options shown here. Which of the following report types would be his best likely starting point?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf011.jpg)

    1. Technical Report
    2. High Severity Report
    3. Qualys Patch Report
    4. Unknown Device Report

    Answer:

    B. The High Severity Report is the most likely report of the choices given that will summarize critical security issues. The Technical Report will likely contain too much detail for Rob's manager. The Patch Report will indicate systems and applications that are missing patches but omit other security issues. The Unknown Device Report will focus on systems detected during the scan that are not registered with the organization's asset management system.
53. Wendy is the security administrator for a membership association that is planning to launch an online store. As part of this launch, she will become responsible for ensuring that the website and associated systems are compliant with all relevant standards. What regulatory regime specifically covers credit card information?

    1. PCI DSS
    2. FERPA
    3. HIPAA
    4. SOX

    Answer:

    A. The Payment Card Industry Data Security Standard (PCI DSS) regulates credit and debit card information. The Family Educational Rights and Privacy Act (FERPA) applies to student educational records. The Health Insurance Portability and Accountability Act (HIPAA) regulates protected health information. The Sarbanes–Oxley (SOX) Act requires controls around the handling of financial records for public companies.
54. During a port scan of a server, Miguel discovered that the following ports are open on the internal network:

    * TCP port 25
    * TCP port 80
    * TCP port 110
    * TCP port 443
    * TCP port 1433
    * TCP port 3389

    The scan results provide evidence that a variety of services are running on this server. Which one of the following services is _not_ indicated by the scan results?

    1. Web
    2. Database
    3. SSH
    4. RDP

    Answer:

    C. Web servers commonly run on ports 80 (for HTTP) and 443 (for HTTPS). Database servers commonly run on ports 1433 (for Microsoft SQL Server), 1521 (for Oracle), or 3306 (for MySQL). Remote Desktop Protocol services commonly run on port 3389. There is no evidence that SSH, which uses port 22, is running on this server.
55. Nina is a software developer, and she receives a report from her company's cybersecurity team that a vulnerability scan detected a SQL injection vulnerability in one of her applications. She examines her code and makes a modification in a test environment that she believes corrects the issue. What should she do next?

    1. Deploy the code to production immediately to resolve the vulnerability.
    2. Request a scan of the test environment to confirm that the issue is corrected.
    3. Mark the vulnerability as resolved and close the ticket.
    4. Hire a consultant to perform a penetration test to confirm that the vulnerability is resolved.

    Answer:

    B. Nina should perform testing of her code before deploying it to production. Because this code was designed to correct an issue in a vulnerability scan, Nina should ask the security team to rerun the scan to confirm that the vulnerability scan was resolved as one component of her testing. A penetration test is overkill and not necessary in this situation. Nina should not deploy the code to production until it is tested. She should not mark the issue as resolved until it is verified to work in production.
56. George recently ran a port scan on a network device used by his organization. Which one of the following open ports represents the most significant possible security vulnerability?

    1. 22
    2. 23
    3. 161
    4. 443

    Use the following scenario to answer questions 57–59.

    Harold runs a vulnerability scan of a server that he is planning to move into production and finds the vulnerability shown here.

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf012.jpg)

    Answer:

    B. Port 23 is used by telnet, an insecure unencrypted communications protocol. George should ensure that telnet is disabled and blocked. Secure shell (SSH) runs on port 22 and serves as a secure alternative. Port 161 is used by the Simple Network Management Protocol (SNMP), and port 443 (HTTPS) is used for secure web connections.
57. What operating system is most likely running on the server in this vulnerability scan report?

    1. macOS
    2. Windows
    3. Kali
    4. RHEL

    Answer:

    B. This system is exposing a service on port 3389. This port is typically used for remote administrative access to Windows servers.
58. Harold is preparing to correct the vulnerability. What service should he inspect to identify the issue?

    1. SSH
    2. HTTPS
    3. RDP
    4. SFTP

    Answer:

    C. The issue identified in this scan report is with a service running on port 3389. Windows systems use port 3389 for the Remote Desktop Protocol (RDP). Therefore, Harold should turn to this service first.
59. Harold would like to secure the service affected by this vulnerability. Which one of the following protocols/versions would be an acceptable way to resolve the issue?

    1. SSL v2.0
    2. SSL v3.0
    3. TLS v1.0
    4. None of the above

    Answer:

    D. None of the protocols and versions listed in this question is an acceptable way to correct this vulnerability. All versions of SSL contain critical vulnerabilities and should no longer be used. TLS v1.0 also contains a vulnerability that would allow an attacker to downgrade the cryptography used by the server. Harold should upgrade the server to support at least TLS v1.2.
60. Seth found the vulnerability shown here in one of the systems on his network. What component requires a patch to correct this issue?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf013.jpg)

    1. Operating system
    2. VPN concentrator
    3. Network router or switch
    4. Hypervisor

    Answer:

    D. VMware is a virtualization platform that is widely used to run multiple guest operating systems on the same hardware platform. This vulnerability indicates a vulnerability in VMware itself, which is the hypervisor that moderates access to physical resources by those guest operating systems.
61. Quentin ran a vulnerability scan of a server in his organization and discovered the results shown here. Which one of the following actions is _not_ required to resolve one of the vulnerabilities on this server?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf014.jpg)

    1. Reconfigure cipher support.
    2. Apply Window security patches.
    3. Obtain a new SSL certificate.
    4. Enhance account security policies.

    Answer:

    B. Quentin should reconfigure cipher support to resolve the issues surrounding the weak cipher support of SSL/TLS and RDP. He should also obtain a new SSL certificate to resolve multiple issues with the current certificate. He should add account security requirements to resolve the naming of guest accounts and the expiration of administrator passwords. There is no indication that any Windows patches are missing on this system.
62. The presence of \_\_\_\_\_\_\_\_\_\_\_\_ triggers specific vulnerability scanning requirements based on law or regulation.

    1. Credit card information
    2. Protected health information
    3. Personally identifiable information
    4. Trade secret information

    Use the scenario to answer questions 63–65.

    Stella is analyzing the results of a vulnerability scan and comes across the vulnerability shown here on a server in her organization. The SharePoint service in question processes all of the organization's work orders and is a critical part of the routine business workflow.

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf015.jpg)

    Answer:

    A. Although all of these categories of information should trigger vulnerability scanning for assets involved in their storage, processing, or transmission, only credit card information has specific regulations covering these scans. The Payment Card Industry Data Security Standard (PCI DSS) contains detailed requirements for vulnerability scanning.
63. What priority should Stella place on remediating this vulnerability?

    1. Stella should make this vulnerability one of her highest priorities.
    2. Stella should remediate this vulnerability within the next several weeks.
    3. Stella should remediate this vulnerability within the next several months.
    4. Stella does not need to assign any priority to remediating this vulnerability.

    Answer:

    A. Stella should remediate this vulnerability as quickly as possible because it is rated by the vendor as a Critical vulnerability. The description of the vulnerability indicates that an attacker could execute arbitrary code on the server and use this vulnerability to achieve escalation of privilege. Therefore, this should be one of Stella's highest priorities for remediation.
64. What operating system is most likely running on the server in this vulnerability scan report?

    1. macOS
    2. Windows
    3. Kali
    4. RHEL

    Answer:

    B. This system is running SharePoint. This application runs only on Microsoft Windows servers.
65. What is the best way that Stella can correct this vulnerability?

    1. Deploy an intrusion prevention system.
    2. Apply one or more application patches.
    3. Apply one or more operating system patches.
    4. Disable the service.

    Answer:

    B. The vulnerability report indicates that SharePoint application patches are available to correct the vulnerability on a variety of versions of SharePoint. This should be Stella's first course of action since it will correct the underlying issue. Deploying an intrusion prevention system may also prevent attackers from exploiting the vulnerability, but it will depend on the positioning of the IPS and the attacker's location on the network and will not correct the underlying issue. There is no indication that an operating system patch will correct the issue. Disabling the service will prevent an attacker from exploiting the vulnerability but will also disable the business-critical service.
66. Harry is developing a vulnerability scanning program for a large network of sensors used by his organization to monitor a transcontinental gas pipeline. What term is commonly used to describe this type of sensor network?

    1. WLAN
    2. VPN
    3. P2P
    4. SCADA

    Answer:

    D. A supervisory control and data acquisition (SCADA) network is a form of industrial control system (ICS) that is used to maintain sensors and control systems over a large geographic area.
67. This morning, Eric ran a vulnerability scan in an attempt to detect a vulnerability that was announced by a software manufacturer yesterday afternoon. The scanner did not detect the vulnerability although Eric knows that at least two of his servers should have the issue. Eric contacted the vulnerability scanning vendor, who assured him that they released a signature for the vulnerability overnight. What should Eric do as a next step?

    1. Check the affected servers to verify a false positive.
    2. Check the affected servers to verify a false negative.
    3. Report a bug to the vendor.
    4. Update the vulnerability signatures.

    Answer:

    D. The most likely issue is that Eric's scanner has not pulled the most recent signatures from the vendor's vulnerability feed. Eric should perform a manual update and rerun the scan before performing an investigation of the servers in question or filing a bug report.
68. Natalie ran a vulnerability scan of a web application recently deployed by her organization, and the scan result reported a blind SQL injection. She reported the vulnerability to the developers, who scoured the application and made a few modifications but did not see any evidence that this attack was possible. Natalie reran the scan and received the same result. The developers are now insisting that their code is secure. What is the most likely scenario?

    1. The result is a false positive.
    2. The code is deficient and requires correction.
    3. The vulnerability is in a different web application running on the same server.
    4. Natalie is misreading the scan report.

    Answer:

    A. Blind SQL injection vulnerabilities are difficult to detect and are a notorious source of false positive reports. Natalie should verify the results of the tests performed by the developers but should be open to the possibility that this is a false positive report, since that is the most likely scenario.
69. Kasun discovers a missing Windows security patch during a vulnerability scan of a server in his organization's datacenter. Upon further investigation, he discovers that the system is virtualized. Where should he apply the patch?

    1. To the virtualized system
    2. The patch is not necessary
    3. To the domain controller
    4. To the virtualization platform

    Answer:

    A. Virtualized systems run full versions of operating systems. If Kasun's scan revealed a missing operating system patch when he scanned a virtualized server, the patch should be applied directly to that guest operating system.
70. Joaquin is frustrated at the high level of false positive reports produced by his vulnerability scans and is contemplating a series of actions designed to reduce the false positive rate. Which one of the following actions is _least_ likely to have the desired effect?

    1. Moving to credentialed scanning
    2. Moving to agent-based scanning
    3. Integrating asset information into the scan
    4. Increasing the sensitivity of scans

    Answer:

    D. Joaquin can improve the quality and quantity of information available to the scanner by moving to credentialed scanning, moving to agent-based scanning, and integrating asset information into the scans. Any of these actions is likely to reduce the false positive rate. Increasing the sensitivity of scans would likely have the opposite effect, causing the scanner to report even more false positives.
71. Joe is conducting a network vulnerability scan against his datacenter and receives reports from system administrators that the scans are slowing down their systems. There are no network connectivity issues, only performance problems on individual hosts. He looks at the scan settings shown here. Which setting would be most likely to correct the problem?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf016.jpg)

    1. Scan IP addresses in a random order
    2. Network timeout (in seconds)
    3. Max simultaneous checks per host
    4. Max simultaneous hosts per scan

    Answer:

    C. Of the choices presented, the maximum number of simultaneous checks per host is the only setting that would affect individual systems. Changing the number of simultaneous hosts per scan and the network timeout would have an effect on the broader network. Randomizing IP addresses would not have a performance impact.
72. Isidora runs a vulnerability scan of the management interface for her organization's DNS service. She receives the vulnerability report shown here. What should be Isidora's next action?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf017.jpg)

    1. Disable the use of cookies on this service.
    2. Request that the vendor rewrite the interface to avoid this vulnerability.
    3. Investigate the contents of the cookie.
    4. Shut down the DNS service.

    Answer:

    C. This report simply states that a cookie used by the service is not encrypted. Before raising any alarms, Isidora should investigate the contents of the cookie to determine whether the compromise of its contents would introduce a security issue. This might be the case if the cookie contains session or authentication information. However, if the cookie does not contain any sensitive contents, Isidora may be able to simply leave the service as is.
73. Zara is prioritizing vulnerability scans and would like to base the frequency of scanning on the information asset value. Which of the following criteria would be most appropriate for her to use in this analysis?

    1. Cost of hardware acquisition
    2. Cost of hardware replacement
    3. Types of information processed
    4. Depreciated hardware cost

    Answer:

    C. Information asset value refers to the value that the organization places on data stored, processed, or transmitted by an asset. In this case, the types of information processed (e.g., regulated data, intellectual property, personally identifiable information) helps to determine information asset value. The cost of server acquisition, cost of hardware replacement, and depreciated cost all refer to the financial value of the hardware, which is a different concept than information asset value.
74. Laura is working to upgrade her organization's vulnerability management program. She would like to add technology that is capable of retrieving the configurations of systems, even when they are highly secured. Many systems use local authentication, and she wants to avoid the burden of maintaining accounts on all of those systems. What technology should Laura consider to meet her requirement?

    1. Credentialed scanning
    2. Uncredentialed scanning
    3. Server-based scanning
    4. Agent-based scanning

    Answer:

    D. Laura should consider deploying vulnerability scanning agents on the servers she wants to scan. These agents can retrieve configuration information and send it to the scanner for analysis. Credentialed scanning would also be able to retrieve this information, but it would require that Laura manage accounts on each scanned system. Server-based scanning would not be capable of retrieving configuration information from the host unless run in credentialed mode. Uncredentialed scans would not have the access required to retrieve detailed configuration information from scan targets.
75. Javier discovered the vulnerability shown here in a system on his network. He is unsure what system component is affected. What type of service is causing this vulnerability?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf018.jpg)

    1. Backup service
    2. Database service
    3. File sharing
    4. Web service

    Answer:

    B. The vulnerability report states that the issue is with SQL Server. SQL Server is a database platform provided by Microsoft.
76. Alicia runs a vulnerability scan of a server being prepared for production and finds the vulnerability shown here. Which one of the following actions is _least_ likely to reduce this risk?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf019.jpg)

    1. Block all connections on port 22.
    2. Upgrade OpenSSH.
    3. Disable AES-GCM in the server configuration.
    4. Install a network IPS in front of the server.

    Answer:

    D. It is unlikely that a network IPS would resolve this issue because it would not be able to view the contents of an encrypted SSH session. Disabling port 22 would correct the issue, although it may cause business disruption. Disabling AES-GCM is listed in the solution section as a feasible workaround, whereas upgrading OpenSSH is the ideal solution.
77. After scanning his organization's email server, Singh discovered the vulnerability shown here. What is the most effective response that Singh can take in this situation?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf020.jpg)

    1. Upgrade to the most recent version of Microsoft Exchange.
    2. Upgrade to the most recent version of Microsoft Windows.
    3. Implement the use of strong encryption.
    4. No action is required.

    Answer:

    D. Unfortunately, Singh cannot take any action to remediate this vulnerability. He could consider restricting network access to the server, but this would likely have an undesirable effect on email access. The use of encryption would not correct this issue. The vulnerability report indicates that “There is no known fix at this time,” meaning that upgrading Windows or Exchange would not correct the problem.
78. A SQL injection exploit typically gains access to a database by exploiting a vulnerability in a(n)\_\_\_\_\_\_\_\_\_\_.

    1. Operating system
    2. Web application
    3. Database server
    4. Firewall

    Use the following scenario to answer questions 79–81.

    Ryan ran a vulnerability scan of one of his organization's production systems and received the report shown here. He would like to understand this vulnerability better and then remediate the issue.

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf021.jpg)

    Answer:

    B. SQL injection vulnerabilities target the data stored in enterprise databases, but they do so by exploiting flaws in client-facing applications. These flaws are most commonly, but not exclusively, found in web applications.
79. Ryan will not be able to correct the vulnerability for several days. In the meantime, he would like to configure his intrusion prevention system to watch for issues related to this vulnerability. Which one of the following protocols would an attacker use to exploit this vulnerability?

    1. SSH
    2. HTTPS
    3. FTP
    4. RDP

    Answer:

    B. This vulnerability exists in Microsoft Internet Information Services (IIS), which is a web server. The fact that the vulnerability could result in cross-site scripting issues also points to a web server. Web servers use the HTTP and HTTPS protocols. Ryan could configure IPS rules to filter HTTP/HTTPS access to this server.
80. Which one of the following actions could Ryan take to remediate the underlying issue without disrupting business activity?

    1. Disable the IIS service.
    2. Apply a security patch.
    3. Modify the web application.
    4. Apply IPS rules.

    Answer:

    B. Applying a security patch would correct the issue on this server. The fact that the header for this vulnerability includes a Microsoft security bulletin ID indicates that Microsoft likely released a patch for the vulnerability. Disabling the IIS service would disrupt business activity on the server. Modifying the web application would not likely address this issue as the report indicates that it is an issue with the underlying IIS server and not a specific web application. IPS rules may prevent an attacker from exploiting the vulnerability, but they would not correct the underlying issue.
81. If an attacker is able to exploit this vulnerability, what is the probable result that will have the highest impact on the organization?

    1. Administrative control of the server
    2. Complete control of the domain
    3. Access to configuration information
    4. Access to web application logs

    Answer:

    A. Since this is an escalation of privilege vulnerability, it is likely that an attacker could gain complete control of the system. There is no indication that control of this system would then lead to complete control of the domain. Administrative control of the server would grant access to configuration information and web application logs, but these issues are not as serious as an attacker gaining complete control of the server.
82. Ted is configuring vulnerability scanning for a file server on his company's internal network. The server is positioned on the network as shown here. What types of vulnerability scans should Ted perform to balance the efficiency of scanning effort with expected results?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf022.jpg)

    1. Ted should not perform scans of servers on the internal network.
    2. Ted should perform only internal vulnerability scans.
    3. Ted should perform only external vulnerability scans.
    4. Ted should perform both internal and external vulnerability scans.

    Answer:

    B. This server is located on an internal network and has only a private IP address. Therefore, the only scan that would provide any valid results is an internal scan. The external scanner would not be able to reach the file server through a valid IP address.
83. Zahra is attempting to determine the next task that she should take on from a list of security priorities. Her boss told her that she should focus on activities that have the most “bang for the buck.” Of the tasks shown here, which should she tackle first?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf023.jpg)

    1. Task 1
    2. Task 2
    3. Task 3
    4. Task 4

    Answer:

    A. Task 1 strikes the best balance between criticality and difficulty. It allows Zahra to remediate a medium criticality issue with an investment of only six hours of time. Task 2 is higher criticality but would take three weeks to resolve. Task 3 is the same criticality but would require two days to fix. Task 4 is lower criticality but would require the same amount of time to resolve as Task 1.
84. Morgan is interpreting the vulnerability scan from her organization's network, shown here. She would like to determine which vulnerability to remediate first. Morgan would like to focus on vulnerabilities that are most easily exploitable by someone outside her organization. Assuming the firewall is properly configured, which one of the following vulnerabilities should Morgan give the highest priority?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf024.jpg)

    1. Severity 5 vulnerability in the workstation
    2. Severity 1 vulnerability in the file server
    3. Severity 5 vulnerability in the web server
    4. Severity 1 vulnerability in the mail server

    Answer:

    C. If the firewall is properly configured, the workstation and file server are not accessible by an external attacker. Of the two remaining choices, the web server vulnerability (at severity 5) is more severe than the mail server vulnerability (at severity 1). Most organizations do not bother to remediate severity 1 vulnerabilities because they are usually informational in nature.
85. Mike runs a vulnerability scan against his company's virtualization environment and finds the vulnerability shown here in several of the virtual hosts. What action should Mike take?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf025.jpg)

    1. No action is necessary because this is an informational report.
    2. Mike should disable HTTPS on the affected devices.
    3. Mike should upgrade the version of OpenSSL on the affected devices.
    4. Mike should immediately upgrade the hypervisor.

    Answer:

    A. This is an informational-level report that will be discovered on any server that supports the `OPTIONS` method. This is not a serious issue and is listed as an informational item, so Mike does not need to take any action to address it.
86. Juan recently scanned a system and found that it was running services on ports 139 and 445. What operating system is this system most likely running?

    1. Ubuntu
    2. macOS
    3. Kali
    4. Windows

    Answer:

    D. Ports 139 and 445 are associated with Windows systems that support file and printer sharing.
87. Gene is concerned about the theft of sensitive information stored in a database. Which one of the following vulnerabilities would pose the most direct threat to this information?

    1. SQL injection
    2. Cross-site scripting
    3. Buffer overflow
    4. Denial of service

    Answer:

    A. Although a buffer overflow attack could theoretically have an impact on information stored in the database, a SQL injection vulnerability poses a more direct threat by allowing an attacker to execute arbitrary SQL commands on the database server. Cross-site scripting attacks are primarily user-based threats that would not normally allow database access. A denial-of-service attack targets system availability, rather than information disclosure.
88. Which one of the following protocols is not likely to trigger a vulnerability scan alert when used to support a virtual private network (VPN)?

    1. IPsec
    2. SSL v2
    3. PPTP
    4. SSL v3

    Answer:

    A. IPsec is a secure protocol for establishing VPN links. Organizations should no longer use the obsolete Secure Sockets Layer (SSL) or Point-to-Point Tunneling Protocol (PPTP) for VPN connections or other secure connections.
89. Rahul ran a vulnerability scan of a server that will be used for credit card processing in his environment and received a report containing the vulnerability shown here. What action must Rahul take?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf026.jpg)

    1. Remediate the vulnerability when possible.
    2. Remediate the vulnerability prior to moving the system into production and rerun the scan to obtain a clean result.
    3. Remediate the vulnerability within 90 days of moving the system to production.
    4. No action is required.

    Use the following scenario to answer questions 90–91.

    Aaron is scanning a server in his organization's datacenter and receives the vulnerability report shown here. The service is exposed only to internal hosts.

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf027.jpg)

    Answer:

    D. Rahul does not need to take any action on this vulnerability because it has a severity rating of 2 on a five-point scale. PCI DSS only requires the remediation of vulnerabilities with at least a “medium” rating, and this vulnerability does not clear that threshold.
90. What is the normal function of the service with this vulnerability?

    1. File transfer
    2. Web hosting
    3. Time synchronization
    4. Network addressing

    Answer:

    C. This vulnerability is with the Network Time Protocol (NTP), a service that runs on UDP port 123. NTP is responsible for providing synchronizing for the clocks of servers, workstations, and other devices in the organization.
91. What priority should Aaron place on remediating this vulnerability?

    1. Aaron should make this vulnerability his highest priority.
    2. Aaron should remediate this vulnerability urgently but does not need to drop everything.
    3. Aaron should remediate this vulnerability within the next month.
    4. Aaron does not need to assign any priority to remediating this vulnerability.

    Answer:

    D. Aaron should treat this vulnerability as a fairly low priority and may never get around to remediating it if there are more critical issues on his network. The vulnerability has a severity rating of 2 (out of 5), and the vulnerability is further mitigated by the fact that the server is accessible only from the local network.
92. Without access to any additional information, which one of the following vulnerabilities would you consider the most severe if discovered on a production web server?

    1. CGI generic SQL injection
    2. Web application information disclosure
    3. Web server uses basic authentication without HTTPS
    4. Web server directory enumeration

    Answer:

    A. The SQL injection attack could be quite serious, since it may allow an attacker to retrieve and/or modify information stored in the back-end database. The second-highest priority should be resolving the use of unencrypted authentication, because it may allow the theft of user credentials. The remaining two vulnerabilities are less serious, because they pose only a reconnaissance risk.
93. Gina ran a vulnerability scan on three systems that her organization is planning to move to production and received the results shown here. How many of these issues should Gina require be resolved before moving to production?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf028.jpg)

    1. 0\.
    2. 1\.
    3. 3\.
    4. All of these issues should be resolved.

    Answer:

    A. The report notes that all of the vulnerabilities for these three servers are in Fixed status. This indicates that the vulnerabilities existed but have already been remediated and no additional work is required.
94. Ji-won recently restarted an old vulnerability scanner that had not been used in more than a year. She booted the scanner, logged in, and configured a scan to run. After reading the scan results, she found that the scanner was not detecting known vulnerabilities that were detected by other scanners. What is the most likely cause of this issue?

    1. The scanner is running on an outdated operating system.
    2. The scanner's maintenance subscription is expired.
    3. Ji-won has invalid credentials on the scanner.
    4. The scanner does not have a current, valid IP address.

    Answer:

    B. The most likely issue is that the maintenance subscription for the scanner expired while it was inactive and the scanner is not able to retrieve current signatures from the vendor's vulnerability feed. The operating system of the scanner should not affect the scan results. Ji-won would not be able to access the scanner at all if she had invalid credentials or the scanner had an invalid IP address.
95. Isabella runs both internal and external vulnerability scans of a web server and detects a possible SQL injection vulnerability. The vulnerability appears only in the internal scan and does not appear in the external scan. When Isabella checks the server logs, she sees the requests coming from the internal scan and sees some requests from the external scanner but no evidence that a SQL injection exploit was attempted by the external scanner. What is the most likely explanation for these results?

    1. A host firewall is blocking external network connections to the web server.
    2. A network firewall is blocking external network connections to the web server.
    3. A host IPS is blocking some requests to the web server.
    4. A network IPS is blocking some requests to the web server.

    Answer:

    D. The most likely scenario is that a network IPS is blocking SQL injection attempts sent to this server, and the internal scanner is positioned on the network in such a way that it is not filtered by the network IPS. If a host IPS were blocking the requests, the vulnerability would likely not appear on internal scans either. If a firewall were blocking the requests, then no external scanner entries would appear in the log file.
96. Rick discovers the vulnerability shown here in a server running in his datacenter. What characteristic of this vulnerability should concern him the most?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf029.jpg)

    1. It is the subject of a recent security bulletin.
    2. It has a CVSS score of 7.8.
    3. There are multiple Bugtraq and CVE IDs.
    4. It affects kernel-mode drivers.

    Answer:

    D. The fact that this vulnerability affects kernel-mode drivers is very serious, because it indicates that an attacker could compromise the core of the operating system in an escalation of privilege attack. The other statements made about this vulnerability are all correct, but they are not as serious as the kernel-mode issue.
97. Carl runs a vulnerability scan of a mail server used by his organization and receives the vulnerability report shown here. What action should Carl take to correct this issue?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf030.jpg)

    1. Carl does not need to take any action because this is an informational report.
    2. Carl should replace SSL with TLS on this server.
    3. Carl should disable weak ciphers.
    4. Carl should upgrade OpenSSL.

    Answer:

    D. This is an example of the POODLE vulnerability that exploits weaknesses in the OpenSSL encryption library. While replacing SSL with TLS and disabling weak ciphers are good practices, they will not correct this issue. Carl should upgrade OpenSSL to a more current version that does not contain this vulnerability.
98. Renee is configuring a vulnerability scanner that will run scans of her network. Corporate policy requires the use of daily vulnerability scans. What would be the best time to configure the scans?

    1. During the day when operations reach their peak to stress test systems
    2. During the evening when operations are minimal to reduce the impact on systems
    3. During lunch hour when people have stepped away from their systems but there is still considerable load
    4. On the weekends when the scans may run unimpeded

    Answer:

    B. According to corporate policy, Renee must run the scans on a daily basis, so the weekend is not a viable option. The scans should run when they have the least impact on operations, which, in this scenario, would be in the evening. The purpose of vulnerability scans is to identify known vulnerabilities in systems and not to perform load testing of servers.
99. Ahmed is reviewing the vulnerability scan report from his organization's central storage service and finds the results shown here. Which action can Ahmed take that will be effective in remediating the highest-severity issue possible?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf031.jpg)

    1. Upgrade to SNMP v3.
    2. Disable the use of RC4.
    3. Replace the use of SSL with TLS.
    4. Disable remote share enumeration.

    Use the following scenario to answer questions 100–101.

    Glenda ran a vulnerability scan of workstations in her organization. She noticed that many of the workstations reported the vulnerability shown here. She would like to not only correct this issue but also prevent the likelihood of similar issues occurring in the future.

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf032.jpg)

    Answer:

    A. The highest-severity vulnerability in this report is the use of an outdated version of SNMP. Ahmed can correct this issue by disabling the use of SNMP v1 and SNMP v2, which contain uncorrectable security issues, and replacing them with SNMP v3. The other actions offered as choices in this question would remediate other vulnerabilities shown in the report, but they are all of lower severity than the SNMP issue.
100.    What action should Glenda take to achieve her goals?

        1. Glenda should uninstall Chrome from all workstations and replace it with Internet Explorer.
        2. Glenda should manually upgrade Chrome on all workstations.
        3. Glenda should configure all workstations to automatically upgrade Chrome.
        4. Glenda does not need to take any action.

        Answer:

        C. Glenda can easily resolve this issue by configuring workstations to automatically upgrade Chrome. It is reasonable to automatically deploy Chrome updates to workstations because of the fairly low impact of a failure and the fact that users could switch to another browser in the event of a failure. Manually upgrading Chrome would also resolve the issue, but it would not prevent future issues. Replacing Chrome with Internet Explorer would resolve this issue but create others, since Internet Explorer is no longer supported by Microsoft. This is a serious issue, so Glenda should not ignore the report.
101.    What priority should Glenda place on remediating this vulnerability?

        1. Glenda should make this vulnerability her highest priority.
        2. Glenda should remediate this vulnerability urgently but does not need to drop everything.
        3. Glenda should remediate this vulnerability within the next several months.
        4. Glenda does not need to assign any priority to remediating this vulnerability.

        Answer:

        B. Glenda should remediate this vulnerability as quickly as possible because it occurs widely throughout her organization and has a significant severity (4 on a five-point scale). If an attacker exploits this vulnerability, they could take control of the affected system by executing arbitrary code on it.
102.    After reviewing the results of a vulnerability scan, Gabriella discovered a flaw in her Oracle database server that may allow an attacker to attempt a direct connection to the server. She would like to review NetFlow logs to determine what systems have connected to the server recently. What TCP port should Gabriella expect to find used for this communication?

        1. 443
        2. 1433
        3. 1521
        4. 8080

        Answer:

        C. Oracle database servers use port 1521 for database connections. Port 443 is used for HTTPS connections to a web server. Microsoft SQL Server uses port 1433 for database connections. Port 8080 is a nonstandard port for web services.
103.    Terry recently ran a vulnerability scan against his organization's credit card processing environment that found a number of vulnerabilities. Which vulnerabilities must he remediate to have a “clean” scan under PCI DSS standards?

        1. Critical vulnerabilities
        2. Critical and high vulnerabilities
        3. Critical, high, and medium vulnerabilities
        4. Critical, high, medium, and low vulnerabilities

        Answer:

        C. The PCI DSS standard requires that merchants and service providers present a clean scan result that shows no critical, high, or medium vulnerabilities in order to maintain compliance.
104.    Himari discovers the vulnerability shown here on several Windows systems in her organization. There is a patch available, but it requires compatibility testing that will take several days to complete. What type of file should Himari be watchful for because it may directly exploit this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf033.jpg)

        1. Private key files
        2. Word documents
        3. Image files
        4. Encrypted files

        Answer:

        C. The vulnerability shown here affects PNG processing on systems running Windows. PNG is an acronym for Portable Network Graphics and is a common image file format.
105.    Aaron is configuring a vulnerability scan for a Class C network and is trying to choose a port setting from the list shown here. He would like to choose a scan option that will efficiently scan his network but also complete in a reasonable period of time. Which setting would be most appropriate?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf034.jpg)

        1. None
        2. Full
        3. Standard Scan
        4. Light Scan

        Answer:

        C. The standard scan of 1,900 common ports is a reasonably thorough scan that will conclude in a realistic period of time. If Aaron knows of specific ports used in his organization that are not included in the standard list, he could specify them using the Additional section of the port settings. A full scan of all 65,535 ports would require an extremely long period of time on a Class C network. Choosing the Light Scan setting would exclude a large number of commonly used ports, whereas the None setting would not scan any ports.
106.    Haruto is reviewing the results of a vulnerability scan, shown here, from a web server in his organization. Access to this server is restricted at the firewall so that it may not be accessed on port 80 or 443. Which of the following vulnerabilities should Haruto still address?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf035.jpg)

        1. OpenSSL version.
        2. Cookie information disclosure.
        3. TRACK/TRACE methods.
        4. Haruto does not need to address any of these vulnerabilities because they are not exposed to the outside world.

        Answer:

        A. From the information given in the scenario, you can conclude that all of the HTTP/HTTPS vulnerabilities are not exploitable by an attacker because of the firewall restrictions. However, OpenSSL is an encryption package used for other services, in addition to HTTPS. Therefore, it may still be exposed via SSH or other means. Haruto should replace it with a current, supported version because running an end-of-life (EOL) version of this package exposes the organization to potentially unpatchable security vulnerabilities.
107.    Brian is considering the use of several different categories of vulnerability plug-ins. Of the types listed here, which is the most likely to result in false positive reports?

        1. Registry inspection
        2. Banner grabbing
        3. Service interrogation
        4. Fuzzing

        Answer:

        B. Banner grabbing scans are notorious for resulting in false positive reports because the only validation they do is to check the version number of an operating system or application against a list of known vulnerabilities. This approach is unable to detect any remediation activities that may have taken place that do not alter the version number.
108.    Binh conducts a vulnerability scan and finds three different vulnerabilities, with the CVSS scores shown here. Which vulnerability should be his highest priority to fix, assuming all three fixes are of equal difficulty?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf036.jpg)

        1. Vulnerability 1.
        2. Vulnerability 2.
        3. Vulnerability 3.
        4. Vulnerabilities 1 and 3 are equal in priority.

        Answer:

        C. Vulnerability 3 has a CVSS score of 10.0 because it received the highest possible ratings on all portions of the CVSS vector. All three vulnerabilities have ratings of “high” for the confidentiality, integrity, and availability impact metrics. Vulnerabilities 1 and 2 have lower values for one or more of the exploitability metrics, meaning that weaponization of those vulnerabilities would likely be more difficult.
109.    Which one of the following is not an appropriate criterion to use when prioritizing the remediation of vulnerabilities?

        1. Network exposure of the affected system.
        2. Difficulty of remediation.
        3. Severity of the vulnerability.
        4. All of these are appropriate.

        Answer:

        D. A cybersecurity analyst should consider all of these factors when prioritizing remediation of vulnerabilities. The severity of the vulnerability is directly related to the risk involved. The likelihood of the vulnerability being exploited may be increased or reduced based on the affected system's network exposure. The difficulty of remediation may impact the team's ability to correct the issue with a reasonable commitment of resources.
110.    Landon is preparing to run a vulnerability scan of a dedicated Apache server that his organization is planning to move into a screened subnet (DMZ). Which one of the following vulnerability scans is _least_ likely to provide informative results?

        1. Web application vulnerability scan
        2. Database vulnerability scan
        3. Port scan
        4. Network vulnerability scan

        Answer:

        B. There is no indication in the scenario that the server is running a database; in fact, the scenario indicates that the server is dedicated to running the Apache web service. Therefore, it is unlikely that a database vulnerability scan would yield any results. Landon should run the other three scans, and if they indicate the presence of a database server, he could follow up with a specialized database vulnerability scan.
111.    Ken recently received the vulnerability report shown here that affects a file server used by his organization. What is the primary nature of the risk introduced by this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf037.jpg)

        1. Confidentiality
        2. Integrity
        3. Availability
        4. Nonrepudiation

        Answer:

        C. The vulnerability report's impact statement reads as follows: “If successfully exploited, this vulnerability could lead to intermittent connectivity problems, or the loss of all NetBIOS functionality.” This is a description of an availability risk.
112.    Aadesh is creating a vulnerability management program for his company. He has limited scanning resources and would like to apply them to different systems based on the sensitivity and criticality of the information that they handle. What criteria should Aadesh use to determine the vulnerability scanning frequency?

        1. Data remanence
        2. Data privacy
        3. Data classification
        4. Data sovereignty

        Answer:

        C. Data classification is a set of labels applied to information based on their degree of sensitivity and/or criticality. It would be the most appropriate choice in this scenario. Data retention requirements dictate the length of time that an organization should maintain copies of records. Data remanence is an issue where information thought to be deleted may still exist on systems. Data privacy may contribute to data classification but does not encompass the entire field of data sensitivity and criticality in the same manner as data classification. For example, a system may process proprietary business information that would be very highly classified and require frequent vulnerability scanning. Unless that system also processed personally identifiable information, it would not trigger scans under a system based solely on data privacy. Data sovereignty issues relate to what jurisdiction(s) regulate data and are not relevant in this scenario.
113.    Tom recently read a media report about a ransomware outbreak that was spreading rapidly across the Internet by exploiting a zero-day vulnerability in Microsoft Windows. As part of a comprehensive response, he would like to include a control that would allow his organization to effectively recover from a ransomware infection. Which one of the following controls would best achieve Tom's objective?

        1. Security patching
        2. Host firewalls
        3. Backups
        4. Intrusion prevention systems

        Answer:

        C. In this scenario, a host firewall may be an effective way to prevent infections from occurring in the first place, but it will not expedite the recovery of a system that is already infected. Intrusion prevention systems and security patches will generally not be effective against a zero-day attack and also would not serve as a recovery control. Backups would provide Tom with an effective way to recover information that was encrypted during a ransomware attack.
114.    Kaitlyn discovered the vulnerability shown here on a workstation in her organization. Which one of the following is not an acceptable method for remediating this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf038.jpg)

        1. Upgrade WinRAR.
        2. Upgrade Windows.
        3. Remove WinRAR.
        4. Replace WinRAR with an alternate compression utility.

        Answer:

        B. There is no reason to believe that upgrading the operating system will resolve this application vulnerability. All of the other solutions presented are acceptable ways to address this risk.
115.    Brent ran a vulnerability scan of several network infrastructure devices on his network and obtained the result shown here. What is the extent of the impact that an attacker could have by exploiting this vulnerability directly?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf039.jpg)

        1. Denial of service
        2. Theft of sensitive information
        3. Network eavesdropping
        4. Reconnaissance

        Answer:

        D. This is a serious vulnerability because it exposes significant network configuration information to attackers and could be used to wage other attacks on this network. However, the direct impact of this vulnerability is limited to reconnaissance of network configuration information.
116.    Yashvir runs the cybersecurity vulnerability management program for his organization. He sends a database administrator a report of a missing database patch that corrects a high severity security issue. The DBA writes back to Yashvir that he has applied the patch. Yashvir reruns the scan, and it still reports the same vulnerability. What should he do next?

        1. Mark the vulnerability as a false positive.
        2. Ask the DBA to recheck the database server.
        3. Mark the vulnerability as an exception.
        4. Escalate the issue to the DBA's manager.

        Answer:

        B. In this case, Yashvir should ask the DBA to recheck the server to ensure that the patch was properly applied. It is not yet appropriate to mark the issue as a false positive report until Yashvir performs a brief investigation to confirm that the patch is applied properly. This is especially true because the vulnerability relates to a missing patch, which is not a common source of false positive reports. There was no acceptance of this vulnerability, so Yashvir should not mark it as an exception. He should not escalate this issue to management because the DBA is working with him in good faith.
117.    Manya is reviewing the results of a vulnerability scan and identifies the issue shown here in one of her systems. She consults with developers who check the code and assure her that it is not vulnerable to SQL injection attacks. An independent auditor confirms this for Manya. What is the most likely scenario?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf040.jpg)

        1. This is a false positive report.
        2. The developers are wrong, and the vulnerability exists.
        3. The scanner is malfunctioning.
        4. The database server is misconfigured.

        Answer:

        A. This is most likely a false positive report. The vulnerability description says “note that this script is experimental and may be prone to false positives.” It is less likely that the developers and independent auditors are all incorrect. The scanner is most likely functioning properly, and there is no indication that either it or the database server is misconfigured.
118.    Erik is reviewing the results of a vulnerability scan and comes across the vulnerability report shown here. Which one of the following services is _least_ likely to be affected by this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf041.jpg)

        1. HTTPS
        2. HTTP
        3. SSH
        4. VPN

        Use the following scenario to answer questions 119–120.

        Larry recently discovered a critical vulnerability in one of his organization's database servers during a routine vulnerability scan. When he showed the report to a database administrator, the administrator responded that they had corrected the vulnerability by using a vendor-supplied workaround because upgrading the database would disrupt an important process. Larry verified that the workaround is in place and corrects the vulnerability.

        Answer:

        B. X.509 certificates are used to exchange public keys for encrypted communications. They are a fundamental part of the SSL and TLS protocols, and an issue in an X.509 certificate may definitely affect HTTPS, SSH, and VPN communications that depend on public key cryptography. HTTP does not use encryption and would not be subject to this vulnerability.
119.    How should Larry respond to this situation?

        1. Mark the report as a false positive.
        2. Insist that the administrator apply the vendor patch.
        3. Mark the report as an exception.
        4. Require that the administrator submit a report describing the workaround after each vulnerability scan.

        Answer:

        A. This is an example of a false positive report. The administrator demonstrated that the database is not subject to the vulnerability because of the workaround, and Larry went a step further and verified this himself. Therefore, he should mark the report as a false positive in the vulnerability scanner.
120.    What is the most likely cause of this report?

        1. The vulnerability scanner requires an update.
        2. The vulnerability scanner depends on version detection.
        3. The database administrator incorrectly applied the workaround.
        4. Larry misconfigured the scan.

        Answer:

        B. False positive reports like the one described in this scenario are common when a vulnerability scanner depends on banner grabbing and version detection. The primary solution to this issue is applying a patch that the scanner would detect by noting a new version number. However, the administrator performed the perfectly acceptable action of remediating the vulnerability in a different manner without applying the patch, but the scanner is unable to detect that remediation activity and is reporting a false positive result.
121.    Mila ran a vulnerability scan of a server in her organization and found the vulnerability shown here. What is the use of the service affected by this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf042.jpg)

        1. Web server
        2. Database server
        3. Email server
        4. Directory server

        Answer:

        C. The Post Office Protocol v3 (POP3) is used for retrieving email from an email server.
122.    Margot discovered that a server in her organization has a SQL injection vulnerability. She would like to investigate whether attackers have attempted to exploit this vulnerability. Which one of the following data sources is _least_ likely to provide helpful information?

        1. NetFlow logs
        2. Web server logs
        3. Database logs
        4. IDS logs

        Answer:

        A. Margot can expect to find relevant results in the web server logs because they would contain records of HTTP requests to the server. Database server logs would contain records of the queries made against the database. IDS logs may contain logs of SQL injection alerts. NetFlow logs would not contain useful information because they record only traffic flows, not the details of the communications.
123.    Krista is reviewing a vulnerability scan report and comes across the vulnerability shown here. She comes from a Linux background and is not as familiar with Windows administration. She is not familiar with the `runas` command mentioned in this vulnerability. What is the closest Linux equivalent command?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf043.jpg)

        1. `sudo`
        2. `grep`
        3. `su`
        4. `ps`

        Answer:

        A. The `runas` command allows an administrator to execute a command using the privileges of another user. Linux offers the same functionality with the `sudo` command. The Linux `su` command is similar but allows an administrator to switch user identities, rather than simply execute a command using another user's identity. The `ps` command in Linux lists active processes, whereas the `grep` command is used to search for text matching a pattern.
124.    After scanning a web application for possible vulnerabilities, Barry received the result shown here. Which one of the following best describes the threat posed by this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf044.jpg)

        1. An attacker can eavesdrop on authentication exchanges.
        2. An attacker can cause a denial-of-service attack on the web application.
        3. An attacker can disrupt the encryption mechanism used by this server.
        4. An attacker can edit the application code running on this server.

        Answer:

        A. Plain-text authentication sends credentials “in the clear,” meaning that they are transmitted in unencrypted form and are vulnerable to eavesdropping by an attacker with access to a network segment between the client and server.
125.    Javier ran a vulnerability scan of a network device used by his organization and discovered the vulnerability shown here. What type of attack would this vulnerability enable?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf045.jpg)

        1. Denial of service
        2. Information theft
        3. Information alteration
        4. Reconnaissance

        Answer:

        D. Fingerprinting vulnerabilities disclose information about a system and are used in reconnaissance attacks. This vulnerability would allow an attacker to discover the operating system and version running on the target server.
126.    Akari scans a Windows server in her organization and finds that it has multiple critical vulnerabilities, detailed in the report shown here. What action can Akari take that will have the most significant impact on these issues without creating a long-term outage?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf046.jpg)

        1. Configure the host firewall to block inbound connections.
        2. Apply security patches.
        3. Disable the guest account on the server.
        4. Configure the server to only use secure ciphers.

        Answer:

        B. The majority of the most serious issues in this scan report relate to missing security updates to Windows and applications installed on the server. Akari should schedule a short outage to apply these updates. Blocking inbound connections at the host firewall would prevent the exploitation of these vulnerabilities, but it would also prevent users from accessing the server. Disabling the guest account and configuring the use of secure ciphers would correct several vulnerabilities, but they are not as severe as the vulnerabilities related to patches.
127.    During a recent vulnerability scan of workstations on her network, Andrea discovered the vulnerability shown here. Which one of the following actions is _least_ likely to remediate this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf047.jpg)

        1. Remove JRE from workstations.
        2. Upgrade JRE to the most recent version.
        3. Block inbound connections on port 80 using the host firewall.
        4. Use a web content filtering system to scan for malicious traffic.

        Answer:

        C. This vulnerability is exploited by the user running a Java applet and does not require any inbound connections to the victim system, so a host firewall would not be an effective control. The best options to correct this vulnerability are either removing the JRE if it is no longer necessary or upgrading it to a recent, secure version. A web content filtering solution, though not the ideal solution, may be able to block malicious GIF files from exploiting this vulnerability.
128.    Doug is preparing an RFP for a vulnerability scanner for his organization. He needs to know the number of systems on his network to help determine the scanner requirements. Which one of the following would not be an easy way to obtain this information?

        1. ARP tables
        2. Asset management tool
        3. Discovery scan
        4. Results of scans recently run by a consultant

        Answer:

        A. Although ARP tables may provide the necessary information, this is a difficult way to enumerate hosts and is prone to error. Doug would have much greater success if he consulted the organization's asset management tool, ran a discovery scan, or looked at the results of other recent scans.
129.    Mary runs a vulnerability scan of her entire organization and shares the report with another analyst on her team. An excerpt from that report appears here. Her colleague points out that the report contains only vulnerabilities with severities of 3, 4, or 5. What is the most likely cause of this result?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf048.jpg)

        1. The scan sensitivity is set to exclude low-importance vulnerabilities.
        2. Mary did not configure the scan properly.
        3. Systems in the datacenter do not contain any level 1 or 2 vulnerabilities.
        4. The scan sensitivity is set to exclude high-impact vulnerabilities.

        Answer:

        A. The most likely reason for this result is that the scan sensitivity is set to exclude low-impact vulnerabilities rated as 1 or 2. There is no reason to believe that Mary configured the scan improperly because this is a common practice to limit information overload and is likely intentional. It is extremely unlikely that systems in the datacenter contain no low-impact vulnerabilities when they have high-impact vulnerabilities. If Mary excluded high-impact vulnerabilities, the report would not contain any vulnerabilities rated 4 or 5.
130.    Mikhail is reviewing the vulnerability shown here, which was detected on several servers in his environment. What action should Mikhail take?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf049.jpg)

        1. Block TCP/IP access to these servers from external sources.
        2. Upgrade the operating system on these servers.
        3. Encrypt all access to these servers.
        4. No action is necessary.

        Answer:

        D. This vulnerability is presented as an Info level vulnerability and, therefore, does not represent an actual threat to the system. Mikhail can safely ignore this issue.
131.    Which one of the following approaches provides the most current and accurate information about vulnerabilities present on a system because of the misconfiguration of operating system settings?

        1. On-demand vulnerability scanning
        2. Continuous vulnerability scanning
        3. Scheduled vulnerability scanning
        4. Agent-based monitoring

        Use the following scenario to answer questions 132–134.

        Pete recently conducted a broad vulnerability scan of all the servers and workstations in his environment. He scanned the following three networks:

        * Screened subnet (DMZ) network that contains servers with public exposure
        * Workstation network that contains workstations that are allowed outbound access only
        * Internal server network that contains servers exposed only to internal systems

        He detected the following vulnerabilities:

        * Vulnerability 1: A SQL injection vulnerability on a screened subnet (DMZ) server that would grant access to a database server on the internal network (severity 5/5)
        * Vulnerability 2: A buffer overflow vulnerability on a domain controller on the internal server network (severity 3/5)
        * Vulnerability 3: A missing security patch on several hundred Windows workstations on the workstation network (severity 2/5)
        * Vulnerability 4: A denial-of-service vulnerability on a screened subnet (DMZ) server that would allow an attacker to disrupt a public-facing website (severity 2/5)
        * Vulnerability 5: A denial-of-service vulnerability on an internal server that would allow an attacker to disrupt an internal website (severity 4/5)

        Note that the severity ratings assigned to these vulnerabilities are directly from the vulnerability scanner and were not assigned by Pete.

        Answer:

        D. Vulnerability scans can only provide a snapshot in time of a system's security status from the perspective of the vulnerability scanner. Agent-based monitoring provides a detailed view of the system's configuration from an internal perspective and is likely to provide more accurate results, regardless of the frequency of vulnerability scanning.
132.    Absent any other information, which one of the vulnerabilities in the report should Pete remediate first?

        1. Vulnerability 1
        2. Vulnerability 2
        3. Vulnerability 3
        4. Vulnerability 4

        Answer:

        A. The SQL injection vulnerability is clearly the highest priority for remediation. It has the highest severity (5/5) and also exists on a server that has public exposure because it resides on the screened subnet (DMZ) network.
133.    Pete is working with the desktop support manager to remediate vulnerability 3. What would be the most efficient way to correct this issue?

        1. Personally visit each workstation to remediate the vulnerability.
        2. Remotely connect to each workstation to remediate the vulnerability.
        3. Perform registry updates using a remote configuration tool.
        4. Apply the patch using a GPO.

        Answer:

        D. Pete and the desktop support team should apply the patch using a Group Policy Object (GPO) or other centralized configuration management tool. This is much more efficient than visiting each workstation individually, either in person or via remote connection. There is no indication in the scenario that a registry update would remediate this issue.
134.    Pete recently conferred with the organization's CISO, and the team is launching an initiative designed to combat the insider threat. They are particularly concerned about the theft of information by employees seeking to exceed their authorized access. Which one of the vulnerabilities in this report is of greatest concern given this priority?

        1. Vulnerability 2
        2. Vulnerability 3
        3. Vulnerability 4
        4. Vulnerability 5

        Answer:

        A. An insider would have the network access required to connect to a system on the internal server network and exploit this buffer overflow vulnerability. Buffer overflow vulnerabilities typically allow the execution of arbitrary code, which may allow an attacker to gain control of the server and access information above their authorization level. Vulnerability 3 may also allow the theft of information, but it has a lower severity level than vulnerability 2. Vulnerabilities 4 and 5 are denial-of-service vulnerabilities that would allow the disruption of service, not the theft of information.
135.    Wanda recently discovered the vulnerability shown here on a Windows server in her organization. She is unable to apply the patch to the server for six weeks because of operational issues. What workaround would be most effective in limiting the likelihood that this vulnerability would be exploited?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf050.jpg)

        1. Restrict interactive logins to the system.
        2. Remove Microsoft Office from the server.
        3. Remove Internet Explorer from the server.
        4. Apply the security patch.

        Answer:

        A. Wanda should restrict interactive logins to the server. The vulnerability report states that “The most severe of these vulnerabilities could allow remote code execution if a user either visits a specially crafted website or opens a specially crafted document.” If Wanda restricts interactive login, it greatly reduces the likelihood of this type of activity. Removing Internet Explorer or Microsoft Office might lower some of the risk, but it would not be as effective as completely restricting logins. Applying the security patch is not an option because of the operational concerns cited in the question.
136.    Garrett is configuring vulnerability scanning for a new web server that his organization is deploying on its screened subnet (DMZ) network. The server hosts the company's public website. What type of scanning should Garrett configure for best results?

        1. Garrett should not perform scanning of screened subnet (DMZ) systems.
        2. Garrett should perform external scanning only.
        3. Garrett should perform internal scanning only.
        4. Garrett should perform both internal and external scanning.

        Answer:

        D. For best results, Garret should combine both internal and external vulnerability scans. The external scan provides an “attacker's eye view” of the web server, whereas the internal scan may uncover vulnerabilities that would only be exploitable by an insider or an attacker who has gained access to another system on the network.
137.    Frank recently ran a vulnerability scan and identified a POS terminal that contains an unpatchable vulnerability because of running an unsupported operating system. Frank consults with his manager and is told that the POS is being used with full knowledge of management and, as a compensating control, it has been placed on an isolated network with no access to other systems. Frank's manager tells him that the merchant bank is aware of the issue. How should Frank handle this situation?

        1. Document the vulnerability as an approved exception.
        2. Explain to his manager that PCI DSS does not permit the use of unsupported operating systems.
        3. Decommission the POS system immediately to avoid personal liability.
        4. Upgrade the operating system immediately.

        Answer:

        A. The scenario describes an acceptable use of a compensating control that has been reviewed with the merchant bank. Frank should document this as an exception and move on with his scans. Other actions would go against his manager's wishes and are not required by the situation.
138.    James is configuring vulnerability scans of a dedicated network that his organization uses for processing credit card transactions. What types of scans are least important for James to include in his scanning program?

        1. Scans from a dedicated scanner on the card processing network.
        2. Scans from an external scanner on his organization's network.
        3. Scans from an external scanner operated by an approved scanning vendor.
        4. All three types of scans are equally important.

        Answer:

        D. All three of these scan types provide James with important information and/or are needed to meet regulatory requirements. The external scan from James's own network provides information on services accessible outside of the payment card network. The internal scan may detect vulnerabilities accessible to an insider or someone who has breached the network perimeter. The approved scanning vendor (ASV) scans are required to meet PCI DSS obligations. Typically, ASV scans are run infrequently and do not provide the same level of detailed reporting as scans run by the organization's own external scans, so James should include both in his program.
139.    Helen performs a vulnerability scan of one of the internal LANs within her organization and finds a report of a web application vulnerability on a device. Upon investigation, she discovers that the device in question is a printer. What is the most likely scenario in this case?

        1. The printer is running an embedded web server.
        2. The report is a false positive result.
        3. The printer recently changed IP addresses.
        4. Helen inadvertently scanned the wrong network.

        Answer:

        A. Any one of the answer choices provided is a possible reason that Helen received this result. However, the most probable scenario is that the printer is actually running a web server and this is a true positive result. Printers commonly provide administrative web interfaces, and those interfaces may be the source of vulnerabilities.
140.    Julian recently detected the vulnerability shown here on several servers in his environment. Because of the critical nature of the vulnerability, he would like to block all access to the affected service until it is resolved using a firewall rule. He verifies that the following TCP ports are open on the host firewall. Which one of the following does Julian _not_ need to block to restrict access to this service?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf051.jpg)

        1. 137
        2. 139
        3. 389
        4. 445

        Answer:

        C. Port 389 is used by the Lightweight Directory Access Protocol (LDAP) and is not part of the SMB communication. SMB may be accessed directly over TCP port 445 or indirectly by using NetBIOS over TCP/IP on TCP ports 137 and 139.
141.    Ted recently ran a vulnerability scan of his network and was overwhelmed with results. He would like to focus on the most important vulnerabilities. How should Ted reconfigure his vulnerability scanner?

        1. Increase the scan sensitivity.
        2. Decrease the scan sensitivity.
        3. Increase the scan frequency.
        4. Decrease the scan frequency.

        Answer:

        B. Ted can reduce the number of results returned by the scan by decreasing the scan sensitivity. This will increase the threshold for reporting, only returning the most important results. Increasing the scan sensitivity would have the opposite effect, increasing the number of reported vulnerabilities. Changing the scan frequency would not alter the number of vulnerabilities reported.
142.    Sunitha discovered the vulnerability shown here in an application developed by her organization. What application security technique is most likely to resolve this issue?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf052.jpg)

        1. Input validation
        2. Network segmentation
        3. Parameter handling
        4. Tag removal

        Answer:

        A. Buffer overflow vulnerabilities occur when an application attempts to put more data in a memory location than was allocated for that use, resulting in unauthorized writes to other areas of memory. Input validation verifies that user-supplied input does not exceed the maximum allowable length before storing it in memory.
143.    Sherry runs a vulnerability scan and receives the high-level results shown here. Her priority is to remediate the most important vulnerabilities first. Which system should be her highest priority?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf053.jpg)

        1. A
        2. B
        3. C
        4. D

        Answer:

        D. System D is the only system that contains a critical vulnerability, as shown in the scan results. Therefore, Sherry should begin with this system as it has the highest-priority vulnerability.
144.    Victor is configuring a new vulnerability scanner. He set the scanner to run scans of his entire datacenter each evening. When he went to check the scan reports at the end of the week, he found that they were all incomplete. The scan reports noted the error “Scan terminated due to start of preempting job.” Victor has no funds remaining to invest in the vulnerability scanning system. He does want to cover the entire datacenter. What should he do to ensure that scans complete?

        1. Reduce the number of systems scanned.
        2. Increase the number of scanners.
        3. Upgrade the scanner hardware.
        4. Reduce the scanning frequency.

        Answer:

        D. The problem Victor is experiencing is that the full scan does not complete in the course of a single day and is being cancelled when the next full scan tries to run. He can fix this problem by reducing the scanning frequency. For example, he could set the scan to run once a week so that it completes. Reducing the number of systems scanned would not meet his requirement to scan the entire datacenter. He cannot increase the number of scanners or upgrade the hardware because he has no funds to invest in the system.
145.    Vanessa ran a vulnerability scan of a server and received the results shown here. Her boss instructed her to prioritize remediation based on criticality. Which issue should she address first?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf054.jpg)

        1. Remove the POP server.
        2. Remove the FTP server.
        3. Upgrade the web server.
        4. Remove insecure cryptographic protocols.

        Answer:

        C. The only high-criticality issue on this report (and all but one of the medium-criticality issues) relates to an outdated version of the Apache web server. Vanessa should upgrade this server before taking any other remediation action.
146.    Terry is reviewing a vulnerability scan of a Windows server and came across the vulnerability shown here. What is the risk presented by this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf055.jpg)

        1. An attacker may be able to execute a buffer overflow and execute arbitrary code on the server.
        2. An attacker may be able to conduct a denial-of-service attack against this server.
        3. An attacker may be able to determine the operating system version on this server.
        4. There is no direct vulnerability, but this information points to other possible vulnerabilities on the server.

        Answer:

        D. This scan result does not directly indicate a vulnerability. However, it does indicate that the server is configured for compatibility with 16-bit applications, and those applications may have vulnerabilities. It is an informational result that does not directly require action on Terry's behalf.
147.    Andrea recently discovered the vulnerability shown here on the workstation belonging to a system administrator in her organization. What is the major likely threat that should concern Andrea?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf056.jpg)

        1. An attacker could exploit this vulnerability to take control of the administrator's workstation.
        2. An attacker could exploit this vulnerability to gain access to servers managed by the administrator.
        3. An attacker could exploit this vulnerability to prevent the administrator from using the workstation.
        4. An attacker could exploit this vulnerability to decrypt sensitive information stored on the administrator's workstation.

        Answer:

        B. PuTTY is a commonly used remote login application used by administrators to connect to servers and other networked devices. If an attacker gains access to the SSH private keys used by PuTTY, the attacker could use those keys to gain access to the systems managed by that administrator. This vulnerability does not necessarily give the attacker any privileged access to the administrator's workstation, and the SSH key is not normally used to encrypt stored information.
148.    Avik recently conducted a PCI DSS vulnerability scan of a web server and noted a critical PHP vulnerability that required an upgrade to correct. She applied the update. How soon must Avik repeat the scan?

        1. Within 30 days
        2. At the next scheduled quarterly scan
        3. At the next scheduled annual scan
        4. Immediately

        Answer:

        D. Avik is required to rerun the vulnerability scan until she receives a clean result that may be submitted for PCI DSS compliance purposes.
149.    Chandra's organization recently upgraded the firewall protecting the network where they process credit card information. This network is subject to the provisions of PCI DSS. When is Chandra required to schedule the next vulnerability scan of this network?

        1. Immediately
        2. Within one month
        3. Before the start of next month
        4. Before the end of the quarter following the upgrade

        Answer:

        A. PCI DSS requires that networks be scanned quarterly or after any “significant change in the network.” A firewall upgrade definitely qualifies as a significant network change, and Chanda should schedule a vulnerability scan immediately to maintain PCI DSS compliance.
150.    Fahad is concerned about the security of an industrial control system (ICS) that his organization uses to monitor and manage systems in their factories. He would like to reduce the risk of an attacker penetrating this system. Which one of the following security controls would best mitigate the vulnerabilities in this type of system?

        1. Network segmentation
        2. Input validation
        3. Memory protection
        4. Redundancy

        Answer:

        A. Network segmentation is one of the strongest controls that may be used to protect ICS and supervisory control and data acquisition (SCADA) systems by isolating them from other systems on the network. Input validation and memory protection may provide some security, but the mitigating effect is not as strong as isolating these sensitive systems from other devices and preventing an attacker from connecting to them in the first place. Redundancy may increase uptime from accidental failures but would not protect the systems from attack.
151.    Raphael discovered during a vulnerability scan that an administrative interface to one of his storage systems was inadvertently exposed to the Internet. He is reviewing firewall logs and would like to determine whether any access attempts came from external sources. Which one of the following IP addresses reflects an external source?

        1. 10.15.1.100
        2. 12.8.1.100
        3. 172.16.1.100
        4. 192.168.1.100

        Answer:

        B. Any addresses in the 10._x_._x_._x_, 172.16._x_._x_, and 192.168._x_._x_ ranges are private IP addresses that are not routable over the Internet. Therefore, of the addresses listed, only 12.8.1.100 could originate outside the local network.
152.    Nick is configuring vulnerability scans for his network using a third-party vulnerability scanning service. He is attempting to scan a web server that he knows exposes a CIFS file share and contains several significant vulnerabilities. However, the scan results only show ports 80 and 443 as open. What is the most likely cause of these scan results?

        1. The CIFS file share is running on port 443.
        2. A firewall configuration is preventing the scan from succeeding.
        3. The scanner configuration is preventing the scan from succeeding.
        4. The CIFS file share is running on port 80.

        Answer:

        B. The most likely issue here is that there is a network firewall between the server and the third-party scanning service. This firewall is blocking inbound connections to the web server and preventing the external scan from succeeding. CIFS generally runs on port 445, not port 80 or 443. Those ports are commonly associated with web services. The scanner is not likely misconfigured because it is successfully detecting other ports on the server. Nick should either alter the firewall rules to allow the scan to succeed or, preferably, place a scanner on a network in closer proximity to the web server.
153.    Thomas learned this morning of a critical security flaw that affects a major service used by his organization and requires immediate patching. This flaw was the subject of news reports and is being actively exploited. Thomas has a patch and informed stakeholders of the issue and received permission to apply the patch during business hours. How should he handle the change management process?

        1. Thomas should apply the patch and then follow up with an emergency change request after work is complete.
        2. Thomas should initiate a standard change request but apply the patch before waiting for approval.
        3. Thomas should work through the standard change approval process and wait until it is complete to apply the patch.
        4. Thomas should file an emergency change request and wait until it is approved to apply the patch.

        Answer:

        A. Change management processes should always include an emergency change procedure. This procedure should allow applying emergency security patches without working through the standard change process. Thomas has already secured stakeholder approval on an informal basis, so he should proceed with the patch and then file a change request after the work is complete. Taking the time to file the change request before completing the work would expose the organization to a critical security flaw during the time required to complete the paperwork.
154.    After running a vulnerability scan of systems in his organization's development shop, Mike discovers the issue shown here on several systems. What is the best solution to this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf057.jpg)

        1. Apply the required security patches to this framework.
        2. Remove this framework from the affected systems.
        3. Upgrade the operating system of the affected systems.
        4. No action is necessary.

        Answer:

        B. The vulnerability description indicates that this software has reached its end-of-life (EOL) and, therefore, is no longer supported by Microsoft. Mike's best solution is to remove this version of the framework from the affected systems. No patches will be available for future vulnerabilities. There is no indication from this result that the systems require operating system upgrades. Mike should definitely take action because of the critical severity (5 on a five-point scale) of this vulnerability.
155.    Tran is preparing to conduct vulnerability scans against a set of workstations in his organization. He is particularly concerned about system configuration settings. Which one of the following scan types will give him the best results?

        1. Unauthenticated scan
        2. Credentialed scan
        3. External scan
        4. Internal scan

        Answer:

        B. Credentialed scans are able to log on to the target system and directly retrieve configuration information, providing the most accurate results of the scans listed. Unauthenticated scans must rely on external indications of configuration settings, which are not as accurate. The network location of the scanner (external versus internal) will not have a direct impact on the scanner's ability to read configuration information.
156.    Brian is configuring a vulnerability scan of all servers in his organization's datacenter. He is configuring the scan to detect only the highest-severity vulnerabilities. He would like to empower system administrators to correct issues on their servers but also have some insight into the status of those remediations. Which approach would best serve Brian's interests?

        1. Give the administrators access to view the scans in the vulnerability scanning system.
        2. Send email alerts to administrators when the scans detect a new vulnerability on their servers.
        3. Configure the vulnerability scanner to open a trouble ticket when they detect a new vulnerability on a server.
        4. Configure the scanner to send reports to Brian who can notify administrators and track them in a spreadsheet.

        Answer:

        C. The best path for Brian to follow would be to leverage the organization's existing trouble ticket system. Administrators likely already use this system on a regular basis, and it can handle reporting and escalation of issues. Brian might want to give administrators access to the scanner and/or have emailed reports sent automatically as well, but those will not provide the tracking that he desires.
157.    Xiu Ying is configuring a new vulnerability scanner for use in her organization's datacenter. Which one of the following values is considered a best practice for the scanner's update frequency?

        1. Daily
        2. Weekly
        3. Monthly
        4. Quarterly

        Answer:

        A. Vulnerability scanners should be updated as often as possible to allow the scanner to retrieve new vulnerability signatures as soon as they are released. Xiu Ying should choose daily updates.
158.    Ben’s manager recently assigned him to begin the remediation work on the most vulnerable server in his organization. A portion of the scan report appears here. What remediation action should Ben take first?

        1. Install patches for Adobe Flash.
        2. Install patches for Firefox.
        3. Run Windows Update.
        4. Remove obsolete software.

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf058.jpg)

        Answer:

        C. Ben is facing a difficult challenge and should likely perform all of the actions described in this question. However, the best starting point would be to run Windows Update to install operating system patches. Many of the critical vulnerabilities relate to missing Windows patches. The other actions may also resolve critical issues, but they all involve software that a user must run on the server before they can be exploited. This makes them slightly lower priorities than the Windows flaws that may be remotely exploitable with no user action.
159.    Zhang Wei completed a vulnerability scan of his organization's virtualization platform from an external host and discovered the vulnerability shown here. How should he react?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf059.jpg)

        1. This is a critical issue that requires immediate adjustment of firewall rules.
        2. This issue has a very low severity and does not require remediation.
        3. This issue should be corrected as time permits.
        4. This is a critical issue, and Zhang Wei should shut down the platform until it is corrected.

        Answer:

        A. Although the vulnerability scan report does indicate that this is a low-severity vulnerability, Zhang Wei must take this information in context. The management interface of a virtualization platform should never be exposed to external hosts, and it also should not use unencrypted credentials. In that context, this is a critical vulnerability that could allow an attacker to take control of a large portion of the computing environment. He should work with security and network engineers to block this activity at the firewall as soon as possible. Shutting down the virtualization platform is not a good alternative because it would be extremely disruptive, and the firewall adjustment is equally effective from a security point of view.
160.    Elliott runs a vulnerability scan of one of the servers belonging to his organization and finds the results shown here. Which one of these statements is _not_ correct?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf060.jpg)

        1. This server requires one or more Linux patches.
        2. This server requires one or more Oracle database patches.
        3. This server requires one or more Firefox patches.
        4. This server requires one or more MySQL patches.

        Answer:

        A. The server described in this report requires multiple Red Hat Linux and Firefox patches to correct serious security issues. One of those Red Hat updates also affects the MySQL database service. Although there are Oracle patches listed on this report, they relate to Oracle Java, not an Oracle database.
161.    Tom runs a vulnerability scan of the file server shown here.

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf061.jpg)

        He receives the vulnerability report shown next. Assuming that the firewall is configured properly, what action should Tom take immediately?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf062.jpg)

        1. Block RDP access to this server from all hosts.
        2. Review and secure server accounts.
        3. Upgrade encryption on the server.
        4. No action is required.

        Answer:

        B. The scan report shows two issues related to server accounts: a weak password policy for the Administrator account and an active Guest account. Tom should remediate these issues to protect against the insider threat. The server also has an issue with weak encryption, but this is a lower priority given that the machine is located on an internal network.
162.    Dave is running a vulnerability scan of a client's network for the first time. The client has never run such a scan and expects to find many results. What security control is likely to remediate the largest portion of the vulnerabilities discovered in Dave's scan?

        1. Input validation
        2. Patching
        3. Intrusion prevention systems
        4. Encryption

        Answer:

        B. Although all the solutions listed may remediate some of the vulnerabilities discovered by Dave's scan, the vast majority of issues in an unmaintained network result from missing security updates. Applying patches will likely resolve quite a few vulnerabilities, if not the majority of them.
163.    Kai is planning to patch a production system to correct a vulnerability detected during a scan. What process should she follow to correct the vulnerability but minimize the risk of a system failure?

        1. Kai should deploy the patch immediately on the production system.
        2. Kai should wait 60 days to deploy the patch to determine whether bugs are reported.
        3. Kai should deploy the patch in a sandbox environment to test it prior to applying it in production.
        4. Kai should contact the vendor to determine a safe timeframe for deploying the patch in production.

        Answer:

        C. Kai should deploy the patch in a sandbox environment and then thoroughly test it prior to releasing it in production. This reduces the risk that the patch will not work well in her environment. Simply asking the vendor or waiting 60 days may identify some issues, but it does not sufficiently reduce the risk because the patch will not have been tested in her company's environment.
164.    Given no other information, which one of the following vulnerabilities would you consider the greatest threat to information confidentiality?

        1. HTTP TRACE/TRACK methods enabled
        2. SSL Server with SSL v3 enabled vulnerability
        3. phpinfo information disclosure vulnerability
        4. Web application SQL injection vulnerability

        Answer:

        D. Although all these vulnerabilities do pose a confidentiality risk, the SQL injection vulnerability poses the greatest threat because it may allow an attacker to retrieve the contents of a backend database. The HTTP TRACK/TRACE methods and PHP information disclosure vulnerabilities may provide reconnaissance information but would not directly disclose sensitive information. SSL v3 is no longer considered secure but is much more difficult to exploit for information theft than a SQL injection issue.
165.    Ling recently completed the security analysis of a web browser deployed on systems in her organization and discovered that it is susceptible to a zero-day integer overflow attack. Who is in the best position to remediate this vulnerability in a manner that allows continued use of the browser?

        1. Ling
        2. The browser developer
        3. The network administrator
        4. The domain administrator

        Answer:

        B. Ling or the domain administrator could remove the software from the system, but this would not allow continued use of the browser. The network administrator could theoretically block all external web browsing, but this is not a practical solution. The browser developer is the only one in a good situation to correct an overflow error because it is a flaw in the code of the web browser.
166.    Jeff's team is preparing to deploy a new database service, and he runs a vulnerability scan of the test environment. This scan results in the four vulnerability reports shown here. Jeff is primarily concerned with correcting issues that may lead to a confidentiality breach. Which vulnerability should Jeff remediate first?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf063.jpg)

        1. Rational ClearCase Portscan Denial of Service vulnerability
        2. Non-Zero Padding Bytes Observed in Ethernet Packets
        3. Oracle Database TNS Listener Poison Attack vulnerability
        4. Hidden RPC Services

        Answer:

        C. Jeff should begin by looking at the highest-severity vulnerabilities and then identify whether they are confidentiality risks. The highest-severity vulnerability on this report is the Rational ClearCase Portscan Denial of Service vulnerability. However, a denial-of-service vulnerability affects availability, rather than confidentiality. The next highest-severity report is the Oracle Database TNS Listener Poison Attack vulnerability. A poisoning vulnerability may cause hosts to connect to an illegitimate server and could result in the disclosure of sensitive information. Therefore, Jeff should address this issue first.
167.    Eric is a security consultant and is trying to sell his services to a new client. He would like to run a vulnerability scan of their network prior to their initial meeting to show the client the need for added security. What is the most significant problem with this approach?

        1. Eric does not know the client's infrastructure design.
        2. Eric does not have permission to perform the scan.
        3. Eric does not know what operating systems and applications are in use.
        4. Eric does not know the IP range of the client's systems.

        Answer:

        B. Although all these concerns are valid, the most significant problem is that Eric does not have permission from the potential client to perform the scan and may wind up angering the client (at best) or violating the law (at worst).
168.    Renee is assessing the exposure of her organization to the denial-of-service vulnerability in the scan report shown here. She is specifically interested in determining whether an external attacker would be able to exploit the denial-of-service vulnerability. Which one of the following sources of information would provide her with the best information to complete this assessment?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf064.jpg)

        1. Server logs
        2. Firewall rules
        3. IDS configuration
        4. DLP configuration

        Answer:

        B. The firewall rules would provide Renee with information about whether the service is accessible from external networks. Server logs would contain information on actual access but would not definitively state whether the server is unreachable from external addresses. Intrusion detection systems may detect an attack in progress but are not capable of blocking traffic and would not be relevant to Renee's analysis. Data loss prevention systems protect against confidentiality breaches and would not be helpful against an availability attack.
169.    Mary is trying to determine what systems in her organization should be subject to vulnerability scanning. She would like to base this decision on the criticality of the system to business operations. Where should Mary turn to best find this information?

        1. The CEO
        2. System names
        3. IP addresses
        4. Asset inventory

        Answer:

        D. Mary should consult the organization's asset inventory. If properly constructed and maintained, this inventory should contain information about asset criticality. The CEO may know some of this information, but it is unlikely that they would have all the necessary information or the time to review it. System names and IP addresses may contain some hints to asset criticality but would not be as good a source as an asset inventory that clearly identifies criticality.
170.    Paul ran a vulnerability scan of his vulnerability scanner and received the result shown here. What is the simplest fix to this issue?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf065.jpg)

        1. Upgrade Nessus.
        2. Remove guest accounts.
        3. Implement TLS encryption.
        4. Renew the server certificate.

        Answer:

        A. The vulnerability description indicates that this is a vulnerability that exists in versions of Nessus earlier than 6.6. Upgrading to a more recent version of Nessus would correct the issue.
171.    Kamea is designing a vulnerability management system for her organization. Her highest priority is conserving network bandwidth. She does not have the ability to alter the configuration or applications installed on target systems. What solution would work best in Kamea's environment to provide vulnerability reports?

        1. Agent-based scanning
        2. Server-based scanning
        3. Passive network monitoring
        4. Port scanning

        Answer:

        C. Passive network monitoring meets Kamea's requirements to minimize network bandwidth consumption while not requiring the installation of an agent. Kamea cannot use agent-based scanning because it requires application installation. She should not use server-based scanning because it consumes bandwidth. Port scanning does not provide vulnerability reports.
172.    Aki is conducting a vulnerability scan when he receives a report that the scan is slowing down the network for other users. He looks at the performance configuration settings shown here. Which setting would be most likely to correct the issue?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf066.jpg)

        1. Enable safe checks.
        2. Stop scanning hosts that become unresponsive during the scan.
        3. Scan IP addresses in random order.
        4. Max simultaneous hosts per scan.

        Answer:

        D. Of the answers presented, the maximum number of simultaneous hosts per scan is most likely to have an impact on the total bandwidth consumed by the scan. Enabling safe checks and stopping the scanning of unresponsive hosts is likely to resolve issues where a single host is negatively affected by the scan. Randomizing IP addresses would only change the order of scanning systems.
173.    Laura received a vendor security bulletin that describes a zero-day vulnerability in her organization's main database server. This server is on a private network but is used by publicly accessible web applications. The vulnerability allows the decryption of administrative connections to the server. What reasonable action can Laura take to address this issue as quickly as possible?

        1. Apply a vendor patch that resolves the issue.
        2. Disable all administrative access to the database server.
        3. Require VPN access for remote connections to the database server.
        4. Verify that the web applications use strong encryption.

        Answer:

        C. The issue raised by this vulnerability is the possibility of eavesdropping on administrative connections to the database server. Requiring the use of a VPN would add strong encryption to this connection and negate the effect of the vulnerability. A patch is not an option because this is a zero-day vulnerability, meaning that a patch is not yet available. Disabling administrative access to the database server would be unnecessarily disruptive to the business. The web server's encryption level is irrelevant to the issue as it would affect connections to the web server, not the database server.
174.    Emily discovered the vulnerability shown here on a server running in her organization. What is the most likely underlying cause for this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf067.jpg)

        1. Failure to perform input validation
        2. Failure to use strong passwords
        3. Failure to encrypt communications
        4. Failure to install antimalware software

        Answer:

        A. In a remote code execution attack, the attacker manages to upload arbitrary code to a server and run it. These attacks are often because of the failure of an application or operating system component to perform input validation.
175.    Rex recently ran a vulnerability scan of his organization's network and received the results shown here. He would like to remediate the server with the highest number of the most serious vulnerabilities first. Which one of the following servers should be on his highest priority list?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf068.jpg)

        1. 10.0.102.58
        2. 10.0.16.58
        3. 10.0.46.116
        4. 10.0.69.232

        Answer:

        A. The server with IP address 10.0.102.58 is the only server among the possible answers that has a Level 5 vulnerability. Level 5 vulnerabilities have the highest severity and should be prioritized. The server at 10.0.16.58 has the most overall vulnerabilities but does not have any Level 5 vulnerabilities. The servers at 10.0.46.116 and 10.0.69.232 have only Level 3 vulnerabilities, which are less severe than Level 5 vulnerabilities.
176.    Abella is configuring a vulnerability scanning tool. She recently learned about a privilege escalation vulnerability that requires the user already have local access to the system. She would like to ensure that her scanners are able to detect this vulnerability as well as future similar vulnerabilities. What action can she take that would best improve the scanner's ability to detect this type of issue?

        1. Enable credentialed scanning.
        2. Run a manual vulnerability feed update.
        3. Increase scanning frequency.
        4. Change the organization's risk appetite.

        Answer:

        A. Enabling credentialed scanning would increase the likelihood of detecting vulnerabilities that require local access to a server. Credentialed scans can read deep configuration settings that might not be available with an uncredentialed scan of a properly secured system. Updating the vulnerability feed manually may add a signature for this particular vulnerability but would not help with future vulnerabilities. Instead, Abella should configure automatic feed updates. Increasing the scanning frequency may increase the speed of detection but would not impact the scanner's ability to detect the vulnerability. The organization's risk appetite affects what vulnerabilities they choose to accept but would not change the ability of the scanner to detect a vulnerability.
177.    Kylie reviewed the vulnerability scan report for a web server and found that it has multiple SQL injection and cross-site scripting vulnerabilities. What would be the least difficult way for Kylie to address these issues?

        1. Install a web application firewall.
        2. Recode the web application to include input validation.
        3. Apply security patches to the server operating system.
        4. Apply security patches to the web server service.

        Answer:

        A. Applying patches to the server will not correct SQL injection or cross-site scripting flaws, since these reside within the web applications themselves. Kylie could correct the root cause by recoding the web applications to use input validation, but this is the more difficult path. A web application firewall would provide immediate protection with lower effort.
178.    Karen ran a vulnerability scan of a web server used on her organization's internal network. She received the report shown here. What circumstances would lead Karen to dismiss this vulnerability as a false positive?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf069.jpg)

        1. The server is running SSL v2.
        2. The server is running SSL v3.
        3. The server is for internal use only.
        4. The server does not contain sensitive information.

        Answer:

        C. This error indicates that the vulnerability scanner was unable to verify the signature on the digital certificate used by the web server. If the organization is using a self-signed digital certificate for this internal application, this would be an expected result.
179.    Which one of the following vulnerabilities is the most difficult to confirm with an external vulnerability scan?

        1. Cross-site scripting
        2. Cross-site request forgery
        3. Blind SQL injection
        4. Unpatched web server

        Answer:

        C. Cross-site scripting and cross-site request forgery vulnerabilities are normally easy to detect with vulnerability scans because the scanner can obtain visual confirmation of a successful attack. Unpatched web servers are often identified by using publicly accessible banner information. Although scanners can often detect many types of SQL injection vulnerabilities, it is often difficult to confirm blind SQL injection vulnerabilities because they do not return results to the attacker but rely on the silent (blind) execution of code.
180.    Holly ran a scan of a server in her datacenter, and the most serious result was the vulnerability shown here. What action is most commonly taken to remediate this vulnerability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf070.jpg)

        1. Remove the file from the server.
        2. Edit the file to limit information disclosure.
        3. Password protect the file.
        4. Limit file access to a specific IP range.

        Answer:

        A. The phpinfo file is a testing file often used by web developers during the initial configuration of a server. Although any of the solutions provided here may remediate this vulnerability, the most common course of action is to simply remove this file before the server is moved into production or made publicly accessible.
181.    During a recent vulnerability scan, Mark discovered a flaw in an internal web application that allows cross-site scripting attacks. He spoke with the manager of the team responsible for that application and was informed that he discovered a known vulnerability and the manager worked with other leaders and determined that the risk is acceptable and does not require remediation. What should Mark do?

        1. Object to the manager's approach and insist on remediation.
        2. Mark the vulnerability as a false positive.
        3. Schedule the vulnerability for remediation in six months.
        4. Mark the vulnerability as an exception.

        Answer:

        D. The manager has thought about the risk and, in consultation with others, determined that it is acceptable. Therefore, Mark should not press the matter and demand remediation, either now or in six months. He should mark this vulnerability as an approved exception in the scanner to avoid future alerts. It would not be appropriate to mark this as a false positive because the vulnerability detection was accurate.
182.    Jacquelyn recently read about a new vulnerability in Apache web servers that allows attackers to execute arbitrary code from a remote location. She verified that her servers have this vulnerability, but this morning's OpenVAS vulnerability scan report shows that the servers are secure. She contacted the vendor and determined that they have released a signature for this vulnerability and it is working properly at other clients. What action can Jacquelyn take that will most likely address the problem efficiently?

        1. Add the web servers to the scan.
        2. Reboot the vulnerability scanner.
        3. Update the vulnerability feed.
        4. Wait until tomorrow's scan.

        Answer:

        C. Jacquelyn should update the vulnerability feed to obtain the most recent signatures from the vendor. She does not need to add the web servers to the scan because they are already appearing in the scan report. Rebooting the scanner would not necessarily update the feed. If she waits until tomorrow, the scanner may be configured to automatically update the feed, but this is not guaranteed and is not as efficient as simply updating the feed now.
183.    Sharon is designing a new vulnerability scanning system for her organization. She must scan a network that contains hundreds of unmanaged hosts. Which of the following techniques would be most effective at detecting system configuration issues in her environment?

        1. Agent-based scanning
        2. Credentialed scanning
        3. Server-based scanning
        4. Passive network monitoring

        Use the following scenario to answer questions 184–186.

        Arlene ran a vulnerability scan of a VPN server used by contractors and employees to gain access to her organization's network. An external scan of the server found the vulnerability shown here.

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf071.jpg)

        Answer:

        C. It would be difficult for Sharon to use agent-based or credentialed scanning in an unmanaged environment because she would have to obtain account credentials for each scanned system. Of the remaining two technologies, server-based scanning is more effective at detecting configuration issues than passive network monitoring.
184.    Which one of the following hash algorithms would _not_ trigger this vulnerability?

        1. MD4
        2. MD5
        3. SHA-1
        4. SHA-256

        Answer:

        D. To be used in a secure manner, certificates must take advantage of a hash function that is not prone to collisions. The MD2, MD4, MD5, and SHA-1 algorithms all have demonstrated weaknesses and would trigger a vulnerability. The SHA-256 algorithm is still considered secure.
185.    What is the most likely result of failing to correct this vulnerability?

        1. All users will be able to access the site.
        2. All users will be able to access the site, but some may see an error message.
        3. Some users will be unable to access the site.
        4. All users will be unable to access the site.

        Answer:

        B. This vulnerability should not prevent users from accessing the site, but it will cause their browsers to display a warning that the site is not secure.
186.    How can Arlene correct this vulnerability?

        1. Reconfigure the VPN server to only use secure hash functions.
        2. Request a new certificate.
        3. Change the domain name of the server.
        4. Implement an intrusion prevention system.

        Answer:

        B. This error is a vulnerability in the certificate itself and may be corrected only by requesting a new certificate from the certificate authority (CA) that uses a secure hash algorithm in the certificate signature.
187.    After reviewing the results of a vulnerability scan, Bruce discovered that many of the servers in his organization are susceptible to a brute-force SSH attack. He would like to determine what external hosts attempted SSH connections to his servers and is reviewing firewall logs. What TCP port would relevant traffic most likely use?

        1. 22
        2. 636
        3. 1433
        4. 1521

        Answer:

        A. Secure shell (SSH) traffic flows over TCP port 22. Port 636 is used by the Lightweight Directory Access Protocol Secure (LDAPS). Port 1433 is used by Microsoft SQL Server. Port 1521 is used by Oracle databases.
188.    Joaquin runs a vulnerability scan of the network devices in his organization and sees the vulnerability report shown here for one of those devices. What action should he take?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf072.jpg)

        1. No action is necessary because this is an informational report.
        2. Upgrade the version of the certificate.
        3. Replace the certificate.
        4. Verify that the correct ciphers are being used.

        Answer:

        C. This error occurs when the server name on a certificate does not match the name of the server in question. It is possible that this certificate was created for another device or that the device name is slightly different than that on the certificate. Joaquin should resolve this error by replacing the certificate with one containing the correct server name.
189.    Lori is studying vulnerability scanning as she prepares for the CySA+ exam. Which of the following is _not_ one of the principles she should observe when preparing for the exam to avoid causing issues for her organization?

        1. Run only nondangerous scans on production systems to avoid disrupting a production service.
        2. Run scans in a quiet manner without alerting other IT staff to the scans or their results to minimize the impact of false information.
        3. Limit the bandwidth consumed by scans to avoid overwhelming an active network link.
        4. Run scans outside of periods of critical activity to avoid disrupting the business.

        Answer:

        B. Lori should absolutely not try to run scans without the knowledge of other IT staff. She should inform her team of her plans and obtain permission for any scans that she runs. She should limit scans of production systems to safe plug-ins while she is learning. She should also limit the bandwidth consumed by her scans and the time of her scans to avoid impacts on production environments.
190.    Meredith is configuring a vulnerability scan and would like to configure the scanner to perform credentialed scans. Of the menu options shown here, which will allow her to directly configure this capability?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf073.jpg)

        1. Manage Discovery Scans
        2. Configure Scan Settings
        3. Configure Search Lists
        4. Set Up Host Authentication

        Answer:

        D. Credentialed scans are also known as authenticated scans and rely on having credentials to log on to target hosts and read their configuration settings. Meredith should choose this option.
191.    Norman is working with his manager to implement a vulnerability management program for his company. His manager tells him that he should focus on remediating critical and high-severity risks and that the organization does not want to spend time worrying about risks rated medium or lower. What type of criteria is Norman's manager using to make this decision?

        1. Risk appetite
        2. False positive
        3. False negative
        4. Data classification

        Answer:

        A. Norman's manager is deciding to use the organization's risk appetite (or risk tolerance) to make this decision. He is stating that the organization will tolerate medium severity risks but will not accept critical or high-severity risks. This is not a case of a false positive or false negative error, since they are not discussing a specific vulnerability. The decision is not based on data classification because the criticality or sensitivity of information processed on systems was not discussed.
192.    Sara's organization has a well-managed test environment. What is the most likely issue that Sara will face when attempting to evaluate the impact of a vulnerability remediation by first deploying it in the test environment?

        1. Test systems are not available for all production systems.
        2. Production systems require a different type of patch than test systems.
        3. Significant configuration differences exist between test and production systems.
        4. Test systems are running different operating systems than production systems.

        Answer:

        A. In a well-managed test environment, the test systems should be configured in a near-identical manner to production systems. They should be running the same operating systems and require the same patches. However, in almost every organization, there are systems running in production that do not have mirror deployments in test environments because of cost, legacy system issues, and other reasons.
193.    How many vulnerabilities listed in the report shown here are significant enough to warrant immediate remediation in a typical operating environment?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf074.jpg)

        1. 22
        2. 14
        3. 5
        4. 0

        Answer:

        D. The vulnerability scan of this server has fairly clean results. All of the vulnerabilities listed are severity 3 or lower. In most organizations, immediate remediation is required only for severity 4 or 5 vulnerabilities.
194.    Which one of the following types of data is subject to regulations in the United States that specify the minimum frequency of vulnerability scanning?

        1. Driver's license numbers
        2. Insurance records
        3. Credit card data
        4. Medical records

        Answer:

        C. Credit card information is subject to the Payment Card Industry Data Security Standard (PCI DSS), which contains specific provisions that dictate the frequency of vulnerability scanning. Although the other data types mentioned in the question are regulated, none of those regulations contains specific provisions that identify a required vulnerability scanning frequency.
195.    Chang is responsible for managing his organization's vulnerability scanning program. He is experiencing issues with scans aborting because the previous day's scans are still running when the scanner attempts to start the current day's scans. Which one of the following solutions is _least_ likely to resolve Chang's issue?

        1. Add a new scanner.
        2. Reduce the scope of the scans.
        3. Reduce the sensitivity of the scans.
        4. Reduce the frequency of the scans.

        Answer:

        C. Chang could resolve this issue by adding additional scanners to balance the load, reducing the frequency of scans or reducing the scope (number of systems) of the scan. Changing the sensitivity level would not likely have a significant impact on the scan time.
196.    Bhanu is scheduling vulnerability scans for her organization's datacenter. Which one of the following is a best practice that Bhanu should follow when scheduling scans?

        1. Schedule scans so that they are spread evenly throughout the day.
        2. Schedule scans so that they run during periods of low activity.
        3. Schedule scans so that they all begin at the same time.
        4. Schedule scans so that they run during periods of peak activity to simulate performance under load.

        Answer:

        B. If possible, Bhanu should schedule the scans during periods of low activity to reduce the impact they have on business operations. The other approaches all have a higher risk of causing a disruption.
197.    Alan recently reviewed a vulnerability report and determined that an insecure direct object reference vulnerability existed on the system. He implemented a remediation to correct the vulnerability. After doing so, he verifies that his actions correctly mitigated the vulnerability. What term best describes the initial vulnerability report?

        1. True positive
        2. True negative
        3. False positive
        4. False negative

        Answer:

        A. This report is best classified as a true positive report because the vulnerability did exist on the system, even though it was later remediated. A true negative report occurs when a vulnerability scanner correctly reports that a vulnerability does not exist. A false positive report occurs when a scanner incorrectly reports that a vulnerability exists, while a false negative report occurs when a scanner incorrectly reports that no vulnerability exists.
198.    Gwen is reviewing a vulnerability report and discovers that an internal system contains a serious flaw. After reviewing the issue with her manager, they decide that the system is sufficiently isolated and they will take no further action. What risk management strategy are they adopting?

        1. Risk avoidance
        2. Risk mitigation
        3. Risk transference
        4. Risk acceptance

        Use the following scenario for questions 199–201.

        Mike is in charge of the software testing process for his company. They perform a complete set of tests for each product throughout its life span. Use your knowledge of software assessment methods to answer the following questions.

        Answer:

        D. Gwen and her manager are choosing to take no further action and, therefore, are choosing to accept the remaining risk.
199.    A new web application has been written by the development team in Mike's company. They used an Agile process and built a tool that fits all of the user stories that the participants from the division that asked for the application outlined. If they want to ensure that the functionality is appropriate for all users in the division, what type of testing should Mike perform?

        1. Stress testing
        2. Regression testing
        3. Static testing
        4. User acceptance testing

        Answer:

        D. Mike needs to conduct user acceptance testing (UAT) with a broad group of users to validate the functionality and usability of the software.
200.    Mike's development team wants to expand the use of the software to the whole company, but they are concerned about its performance. What type of testing should they conduct to ensure that the software will not fail under load?

        1. Stress testing
        2. Regression testing
        3. Static testing
        4. User acceptance testing

        Answer:

        A. Mike's team should stress test the application by loading it beyond what its maximum expected load is. They should validate that it performs as expected and that their infrastructure can handle the load of broad usage by the company. Stress testing often tests to a multiple of the maximum expected load to ensure that the application will handle unexpected load conditions.
201.    Two years after deployment, Mike's team is ready to roll out a major upgrade to their web application. They have pulled code from the repository that it was checked into but are worried that old bugs may have been reintroduced because they restored additional functionality based on older code that had been removed in a release a year ago. What type of testing does Mike's team need to perform?

        1. Stress testing
        2. Regression testing
        3. Static testing
        4. User acceptance testing

        Answer:

        B. Regression testing checks to ensure that old flaws have not been reintroduced. Mike's team needs to regression test their application, particularly because they reintroduced old code that may have flaws.
202.    Padma is evaluating the security of an application developed within her organization. She would like to assess the application's security by supplying it with invalid inputs. What technique is Padma planning to use?

        1. Fault injection
        2. Stress testing
        3. Mutation testing
        4. Fuzz testing

        Answer:

        D. Fuzz testing involves sending invalid or random data to an application to test its ability to handle unexpected data. Fault injection directly inserts faults into error handling paths, particularly error handling mechanisms that are rarely used or might otherwise be missed during normal testing. Mutation testing is related to fuzzing and fault injection, but rather than changing the inputs to the program or introducing faults to it, mutation testing makes small modifications to the program itself. Stress testing is a performance test that ensures applications and the systems that support them can stand up to the full production load.
203.    Which software development life cycle model is illustrated in the image?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf075.jpg)

        1. Waterfall
        2. Spiral
        3. Agile
        4. RAD

        Answer:

        C. The Agile software development methodology is characterized by multiple sprints, each producing a concrete result. The Waterfall model follows a series of sequential steps, whereas the Spiral model uses multiple passes through four phases. Rapid Application Development (RAD) uses a five-phase approach in an iterative format.
204.    The Open Worldwide Application Security Project (OWASP) maintains an application called Orizon. This application reviews Java classes and identifies potential security flaws. What type of tool is Orizon?

        1. Fuzzer
        2. Static code analyzer
        3. Web application assessor
        4. Fault injector

        Answer:

        B. As stated in the question, Orizon performs a review of Java classes, indicating that it is performing a source code review. Techniques that perform source code review are grouped into the category of static code analyzers. The other testing techniques listed in this question are all examples of dynamic code analysis, where the testing application actually executes the code.
205.    Barney's organization mandates fuzz testing for all applications before deploying them into production. Which one of the following issues is this testing methodology most likely to detect?

        1. Incorrect firewall rules
        2. Unvalidated input
        3. Missing operating system patches
        4. Unencrypted data transmission

        Answer:

        B. Fuzz testing works by dynamically manipulating input to an application in an effort to induce a flaw. This technique is useful for detecting places where an application does not perform proper input validation.
206.    Mia would like to ensure that her organization's cybersecurity team reviews the architecture of a new ERP application that is under development. During which SDLC phase should Mia expect the security architecture to be completed?

        1. Analysis and Requirements Definition
        2. Design
        3. Development
        4. Testing and Integration

        Answer:

        B. Security artifacts created during the Design phase include security architecture documentation and data flow diagrams.
207.    Which one of the following security activities is _not_ normally a component of the Operations and Maintenance phase of the SDLC?

        1. Vulnerability scans
        2. Disposition
        3. Patching
        4. Regression testing

        Use the following scenario for questions 208–210.

        Olivia has been put in charge of performing code reviews for her organization and needs to determine which code analysis models make the most sense based on specific needs her organization has. Use your knowledge of code analysis techniques to answer the following questions.

        Answer:

        B. Disposition is a separate SDLC phase that is designed to ensure that data is properly purged at the end of an application life cycle. Operations and maintenance activities include ongoing vulnerability scans, patching, and regression testing after upgrades.
208.    Olivia's security team has identified potential malicious code that has been uploaded to a webserver. If she wants to review the code without running it, what technique should she use?

        1. Dynamic analysis
        2. Fagan analysis
        3. Regression analysis
        4. Static analysis

        Answer:

        D. Olivia needs to review the code without running it, which means she needs to perform a static analysis. Static analysis is often performed with an automated tool, but her security analysts may also choose to review the code manually to identify potential details about the threat actors or what the code may have been specifically intended to do.
209.    Olivia's next task is to test the code for a new mobile application. She needs to test it by executing the code and intends to provide the application with input based on testing scenarios created by the development team as part of their design work. What type of testing will Olivia conduct?

        1. Dynamic analysis
        2. Fagan analysis
        3. Regression analysis
        4. Static analysis

        Answer:

        A. Olivia will conduct dynamic code analysis, which tests the code by running it while providing appropriate test inputs.
210.    After completing the first round of tests for her organization's mobile application, Olivia has discovered indications that the application may not handle unexpected data well. What type of testing should she conduct if she wants to test it using an automated tool that will check for this issue?

        1. Fault injection
        2. Fagan testing
        3. Fuzzing
        4. Failure injection

        Answer:

        C. Fuzz testing involves sending random or invalid data to an application to test its ability to handle the unexpected data. Olivia should identify a fuzzer (a fuzz testing tool) and run it against the application.
211.    Which one of the following characters would not signal a potential security issue during the validation of user input to a web application?

        1. `<`
        2. `'`
        3. `>`
        4. `$`

        Answer:

        D. The `$` character does not necessarily represent a security issue. The greater than/less than brackets (`<>`) are used to enclose HTML tags and require further inspection to determine whether they are part of a cross-site scripting attack. The single quotation mark (`'`) could be used as part of a SQL injection attack.
212.    The Open Worldwide Application Security Project (OWASP) maintains a listing of the most important web application security controls. Which one of these items is _least_ likely to appear on that list?

        1. Implement identity and authentication controls.
        2. Implement appropriate access controls.
        3. Obscure web interface locations.
        4. Leverage security frameworks and libraries.

        Answer:

        C. Security through obscurity is not a good practice. You should not rely on the secrecy of the control (e.g., the location of the web interface) as a security measure. Therefore, obscuring web interface locations is not included on the OWASP security controls list.
213.    Kyle is developing a web application that uses a database back end. He is concerned about the possibility of an SQL injection attack against his application and is consulting the OWASP proactive security controls list to identify appropriate controls. Which one of the following OWASP controls is _least_ likely to prevent a SQL injection attack?

        1. Parameterize queries.
        2. Validate all input.
        3. Encode data.
        4. Implement logging and intrusion detection.

        Answer:

        D. Query parameterization, input validation, and data encoding are all ways to prevent the database from receiving user-supplied input that injects unwanted commands into an SQL query. Logging and intrusion detection are important controls, but they would detect, rather than prevent, a SQL injection attack.
214.    Jill's organization has adopted an asset management tool. If she wants to identify systems on the network based on a unique identifier per machine that will not normally change over time, which of the following options can she use for network-based discovery?

        1. IP address
        2. Hostname
        3. MAC address
        4. None of the above

        Answer:

        C. A machine's MAC, or hardware address, will not typically change over time. MAC addresses can also provide useful information like the manufacturer's name, allowing Jill to have a useful guess about what type of device she has discovered during a discovery scan for asset tracking.
215.    Which software development methodology is illustrated in the diagram?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf076.jpg)

        1. Spiral
        2. RAD
        3. Agile
        4. Waterfall

        Answer:

        D. The Waterfall model follows a series of sequential steps, as shown in the diagram. The Agile software development methodology is characterized by multiple sprints, each producing a concrete result. The Spiral model uses multiple passes through four phases, resulting in a spiral-like diagram. Rapid Application Development (RAD) uses a five-phase approach in an iterative format.
216.    Claire knows that a web application that her organization needs to have in production has vulnerabilities due to a recent scan using a web application security scanner. What is her best protection option if she knows that the vulnerability is a known SQL injection flaw?

        1. A firewall
        2. An IDS
        3. A WAF
        4. DLP

        Use the following scenario to answer questions 217–219.

        Donna has been assigned as the security lead for a DevSecOps team building a new web application. As part of the effort, she has to oversee the security practices that the team will use to protect the application. Use your knowledge of secure coding practices to help Donna guide her team through this process.

        Answer:

        C. A web application firewall (WAF) can often be used to address the specific SQL injection attack. Claire can either write a rule based on the SQL injection attack or use a broader SQL injection prevention ruleset. An IDS would only detect the attack and would not stop it, whereas data loss prevention (DLP) tools might help if data was being stolen but won't stop SQL injection. Some firewalls may have WAF functionality built in, but here the best option is the dedicated web application firewall.
217.    A member of Donna's team recommends building a blocklist to avoid dangerous characters like `'` and `<script>` tags. How could attackers bypass a blocklist that individually identified those characters?

        1. They can use a binary attack.
        2. They can use alternate encodings.
        3. They can use different characters with the same meaning.
        4. The characters could be used together to avoid the blocklist.

        Answer:

        B. Using Unicode encoding to avoid blocklists is a common technique. OWASP recommends you avoid attempting to detect potentially dangerous characters and patterns of characters with a blocklist.
218.    The design of the application calls for client-side validation of input. What type of tool could an attacker use to bypass this?

        1. An XSS injector
        2. A web proxy
        3. A JSON interpreter
        4. A SQL injector

        Answer:

        B. A web proxy is a commonly used tool for web application attacks and allows data to be changed after client-side validation. In general, client-side validation is not a secure technique because of this.
219.    A member of Donna's security team suggests that output encoding should also be considered. What type of attack is the team member most likely attempting to prevent?

        1. Cross-site scripting
        2. SQL injection
        3. Cross-site request forgery
        4. All of the above

        Answer:

        A. Cross-site scripting is the primary threat that is created by not using secure output encoding. Allowing users to enter arbitrary input and then displaying it to other users can result in a cross-site scripting attack. SQL injection is most common as a direct attack, whereas cross-site request forgery normally relies on users clicking a malicious link.
220.    Nathan downloads a BIOS/UEFI update from Dell's website, and when he attempts to install it on the PC, he receives an error that the hash of the download does not match the hash stored on Dell's servers. What type of protection is this?

        1. Full-disk encryption
        2. Firmware protection
        3. Operating system protection
        4. None of the above

        Answer:

        B. BIOS and UEFI are the firmware that controls system startup. In Dell's implementation of this technology, a SHA-256 hash of the new firmware is compared to a known good hash on Dell's servers. If an issue is detected, administrators are notified so that they can take appropriate action.
221.    What practice is typical in a DevSecOps organization as part of a CI/CD pipeline?

        1. Automating some security gates
        2. Programmatic implementation of zero-day vulnerabilities
        3. Using security practitioners to control the flow of the CI/CD pipeline
        4. Removing security features from the IDE

        Answer:

        A. DevSecOps makes security a shared responsibility throughout the development and operations life cycle, and automating some security gates is a common practice to make this happen without causing slowdowns. This means that practitioners must consider both application and infrastructure security constantly from the beginning of the workflow to deployment and support. Implementing zero-day vulnerabilities would be a terrible idea, and having security practitioners exert more control rather than collaboratively making flows work more effectively and removing security features from the integrated development environment aren't great ideas either.
222.    Valerie wants to prevent potential cross-site scripting attacks from being executed when previously entered information is displayed in user's browsers. What technique should she use to prevent this?

        1. A firewall
        2. A HIDS
        3. Output encoding
        4. String randomization

        Answer:

        C. Output encoding translates special characters to an equivalent that will not be interpreted as part of a script or other significant character by a user's browser (or other endpoint application). A HIDS would only alarm on potential attacks, rather than stop them; a firewall will not parse the data; and string randomization was made up for this question—but if it did exist, randomized data wouldn't be useful in most applications when displaying input to a user.
223.    While developing a web application, Chris sets his session ID length to 128 bits based on OWASP's recommended session management standards. What reason would he have for needing such a long session ID?

        1. To avoid duplication
        2. To allow for a large group of users
        3. To prevent brute-forcing
        4. All of the above

        Answer:

        C. OWASP recommends a large session ID value to avoid brute-force attacks. 2^128 is 340,282,366,920,938,463,463,374,607,431,768,211,456, a number that is far larger than you would need to avoid duplication of numbers, even for very large groups of users across the entire world. If you encounter a question like this and don't know the answer, you can apply logic. In this case, the number is so large that it doesn't make sense to use it for simply duplication avoidance, and any reasonable number of users—including the entire population of the world—would require fewer bits.
224.    Robert is reviewing a web application, and the developers have offered four different responses to incorrect logins. Which of the following four responses is the most secure option?

        1. Login failed for user; invalid password
        2. Login failed; invalid user ID or password
        3. Login failed; invalid user ID
        4. Login failed; account does not exist

        Answer:

        B. The answer that provides the least specific information to potential attackers is the best answer here: login failed; invalid user ID or password does not tell an attacker which option they have wrong or provide hints about which accounts may or may not exist.
225.    Nathan is reviewing PHP code for his organization and finds the following code in the application he is assessing. What technique is the developer using?

        `$stmt = $dbh->prepare(“INSERT INTO REGISTRY (var1, var2) VALUES (:var1, :var2)”); $stmt->bindParam(‘:var1’, $var1); $stmt->bindParam(‘:var2’, $var2);`

        1. Dynamic binding
        2. Parameterized queries
        3. Variable limitation
        4. None of the above

        Answer:

        B. This code is an example of one way to parameterize queries. Here, the `var1` and `var2` variables are bound to specific data objects. In some cases, the CySA+ exam may show you examples of code or configurations that you may not be familiar with. In that case, you should read the example carefully for useful context like the statement `bindParam` here. That should give you a clue to the parameterized queries answer being the correct option.
226.    Christina wants to check the firmware she has been provided to ensure that it is the same firmware that the manufacturer provides. What process should she follow to validate that the firmware is trusted firmware?

        1. Download the same file from the manufacturer and compare file size.
        2. Compare a hash of the file to a hash provided by the manufacturer.
        3. Run strings against the firmware to find any evidence of tempering.
        4. Submit the firmware to a malware scanning site to verify that it does not contain malware.

        Answer:

        B. The most effective means of checking most firmware to validate that it is a trusted firmware update is to compare the hash of the file that you have against the provided hash values from the manufacturer website.
227.    What type of attack is the use of query parameterization intended to prevent?

        1. Buffer overflows
        2. Cross-site scripting
        3. SQL injection
        4. Denial-of-service attacks

        Answer:

        C. SQL injection is regularly rated as one of the top web application vulnerabilities, and parameterizing queries is an important way to help prevent it. Parameterized queries, or prepared statements, require developers to define the SQL code they will use, then pass in each parameter to the query. This prevents attackers from changing the intent of the query and allows the query to be used only as intended if properly implemented.
228.    What type of attack is output encoding typically used against?

        1. DoS
        2. XSS
        3. XML
        4. DDoS

        Use the following scenario for questions 229–231.

        Scott has been asked to select a software development model for his organization and knows that there are a number of models that may make sense for what he has been asked to accomplish. Use your knowledge of SDLC models to identify an appropriate model for each of the following requirements.

        Answer:

        B. Output encoding is frequently used to prevent cross-site scripting (XSS) attacks by replacing potentially dangerous characters in previously input user data with harmless equivalents.
229.    Scott's organization needs basic functionality of the effort to become available as soon as possible and wants to involve the teams that will use it heavily to ensure that their needs are met. What model should Scott recommend?

        1. Waterfall
        2. Spiral
        3. Agile
        4. Rapid Application Development

        Answer:

        C. The Agile method is heavily driven by user stories and customer involvement. Sprints deliver functional code, meaning that some elements of the product may be ready early.
230.    A parallel coding effort needs to occur; however, this effort involves a very complex system and errors could endanger human lives. The system involves medical records and drug dosages, and the organization values stability and accuracy over speed. Scott knows the organization often adds design constraints throughout the process and that the model he selects must also deal with that need. What model should he choose?

        1. Waterfall
        2. Spiral
        3. Agile
        4. Rapid Application Development

        Answer:

        B. Spiral places a heavy emphasis on risk assessment and improves from Waterfall by repeating the identification/design/build/evaluation process. This will handle both the complexity that Scott is aware will be involved as well as the late addition of design requirements.
231.    At the end of his development cycle, what SDLC phase will Scott enter as the new application is installed and replaces the old code?

        1. User acceptance testing
        2. Testing and integration
        3. Disposition
        4. Redesign

        Answer:

        C. The disposition phase of SDLC addresses what occurs when a product or system reaches the end of its life. Scott will need to decommission systems and services, identify what will happen to data and other artifacts, and make other decisions before the system can be shut down.
232.    The OWASP Session Management Cheatsheet advises that session IDs are meaningless and recommends that they should be used only as an identifier on the client side. Why should a session ID not have additional information encoded in it like the IP address of the client, their username, or other information?

        1. Processing complex session IDs will slow down the service.
        2. Session IDs cannot contain this information for legal reasons.
        3. Session IDs are sent to multiple different users, which would result in a data breach.
        4. Session IDs could be decoded, resulting in data leakage.

        Answer:

        D. Session IDs should be associated with information needed by the application like userID, client IP address, session timeout and session start time information, or other details on the server side, typically in a session management database or repository. If the session ID had this information encoded in it, it could be reverse engineered and decoded, possibly resulting in data leakage. Complex session IDs are not a processing concern, unless there is sensitive information covered by law (which isn't listed in the question) and then legal limitations would not apply. Session IDs are sent to the application and user whose session they belong to, so they would not breach data simply by being sent.
233.    Bounds checking, removing special characters, and forcing strings to match a limited set of options are all examples of what web application security technique?

        1. SQL injection prevention
        2. Input validation
        3. XSS prevention
        4. Fuzzing

        Answer:

        B. Input validation involves a variety of techniques, including checking the minimum and maximum range for numeric input, checking the length of input strings, removing special characters, and providing limited options for drop-down menus and other strings.
234.    Abigail is performing input validation against an input field and uses the following regular expression:

        `^(AA|AE|AP|AL|AK|AS|AZ|AR|CA|CO|CT|DE|DC|FM|FL|GA|GU| HI|ID|IL|IN|IA|KS|KY|LA|ME|MH|MD|MA|MI|MN|MS|MO|MT|NE| NV|NH|NJ|NM|NY|NC|ND|MP|OH|OK|OR|PW|PA|PR|RI|SC|SD|TN| TX|UT|VT|VI|VA|WA|WV|WI|WY)$`

        What is she checking with the regular expression?

        1. She is removing all typical special characters found in SQL injection.
        2. She is checking for all U.S. state names.
        3. She is removing all typical special characters for cross-site scripting attacks.
        4. She is checking for all U.S. state name abbreviations.

        Answer:

        D. This regular expression will match all U.S. state abbreviations. Even if you're not familiar with regular expressions, you may be asked to read unfamiliar code and determine what function it is performing. Here, reading the list should give you a good clue based on the two-letter pairings.
235.    Jennifer uses an application to send randomized data to her application to determine how it responds to unexpected input. What type of tool is she using?

        1. A UAT tool
        2. A stress testing tool
        3. A fuzzer
        4. A regression testing tool

        Answer:

        C. Fuzzers are tools that send unexpected input, testing whether an application can handle data that does not match what it expects. User acceptance testing (UAT) is a type of testing that helps to ensure that users can properly use a tool and that it performs the functions they expect. A stress testing tool typically puts very high loads onto an infrastructure or application to see how it performs when stressed. Regression testing is done to ensure that old flaws are not reintroduced to an application.
236.    Greg wants to prevent SQL injection in a web application he is responsible for. Which of the following is _not_ a common defense against SQL injection?

        1. Prepared statements with parameterized queries
        2. Output validation
        3. Stored procedures
        4. Escaping all user-supplied input

        Answer:

        B. Validating the output will not prevent SQL injection from occurring. Using prepared statements with parameterized queries, stored procedures, escaping all user-supplied input, input validation, and applying least privilege to the application and database accounts are all useful techniques to prevent successful SQL injection.
237.    While reviewing code that generates a SQL query, Aarav notices that the “address” field is appended to the query without input validation or other techniques applied. What type of attack is most likely to be successful against code like this?

        1. DoS
        2. XSS
        3. SQL injection
        4. Teardrop

        Use the following diagram and scenario for questions 238–240.

        Amanda has been assigned to lead the development of a new web application for her organization. She is following a standard SDLC model as shown here. Use the model and your knowledge of the software development life cycle to answer the following questions.

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c02uf077.jpg)

        Answer:

        C. Unvalidated parameters in a SQL query are likely to allow SQL injection attacks. An attacker could inject arbitrary SQL code into that parameter, thus gaining additional access to the database and the data stored in it.
238.    Amanda's first task is to determine if there are alternative solutions that are more cost effective than in-house development. What phase is she in?

        1. Design
        2. Operations and maintenance
        3. Feasibility
        4. Analysis and requirements definition

        Answer:

        C. The feasibility phase of a project like this looks into whether the project should occur and also looks for alternative solutions as well as the costs for each solution proposed.
239.    What phase of the SDLC typically includes the first code analysis and unit testing in the process?

        1. Analysis and requirements definition
        2. Design
        3. Coding
        4. Testing and integration

        Answer:

        C. Although it may seem like code analysis and unit testing should occur in the testing and integration phase, remember that unit testing occurs on individual program components, which means it will occur as the code is written. The same holds true for code analysis, and thus, the first time this happens will be in the coding stage.
240.    After making it through most of the SDLC process, Amanda has reached point E on the diagram. What occurs at point E?

        1. Disposition
        2. Training and transition
        3. Unit testing
        4. Testing and integration

        Answer:

        B. Before an application can enter ongoing operations and maintenance, users must be trained and the application must be transitioned to the team that will maintain it for its life cycle. Disposition occurs when a product or system hits the end of its life cycle. Unit testing is often part of the coding phase. Testing and integration occur just before training and transition (point D).
241.    Angela wants to prevent buffer overflow attacks on a Windows system. What two built-in technologies should she consider?

        1. The memory firewall and the stack guard
        2. ASLR and DEP
        3. ASLR and DLP
        4. The memory firewall and the buffer guard

        Answer:

        B. Windows has support for both data execution prevention (DEP) and address space location randomization (ASLR). These combine to help prevent buffer overflows by preventing items in memory location tagged as data from being executed and by randomizing the memory space Windows uses to make it harder to take advantage of known memory locations with an overflow.
242.    Amanda has been assigned to reduce the attack surface area for her organization, and she knows that the current network design relies on allowing systems throughout her organization to access the Internet directly via public IP addresses they are assigned. What should her first step be to reduce her organization's attack surface quickly and without large amounts of time invested?

        1. Install host firewalls on the systems.
        2. Move to a NAT environment.
        3. Install an IPS.
        4. None of the above.

        Answer:

        B. Moving to a network address translation (NAT) environment will make the systems inaccessible from the outside world, massively reducing the organization's attack surface. Installing host firewalls would be a great second step but could involve significant amounts of work to install and tune the firewalls.
243.    Matt believes that developers in his organization deployed code that did not implement cookies in a secure way. What type of attack would be aided by this security issue?

        1. SQL injection
        2. A denial-of-service attack
        3. Session hijacking
        4. XSS

        Answer:

        C. Session hijacking of insecurely implemented session cookies is the likely result from this type of issue. Matt should spend time with his developers to ensure that they have reviewed resources like the OWASP guides to secure session creation and maintenance.
244.    Chris operates the point-of-sale (POS) network for a company that accepts credit cards and is thus required to be compliant with PCI DSS. During his regular assessment of the POS terminals, he discovers that a recent Windows operating system vulnerability exists on all of them. Since they are all embedded systems that require a manufacturer update, he knows that he cannot install the available patch. What is Chris's best option to stay compliant with PCI DSS and protect his vulnerable systems?

        1. Replace the Windows embedded point-of-sale terminals with standard Windows systems.
        2. Build a custom operating system image that includes the patch.
        3. Identify, implement, and document compensating controls.
        4. Remove the POS terminals from the network until the vendor releases a patch.

        Answer:

        C. When a vulnerability exists and a patch has not been released or cannot be installed, compensating controls can provide appropriate protection. In the case of PCI DSS (and other compliance standards), documenting what compensating controls were put in place and making that documentation available is an important step for compliance.
245.    Tracy is validating the web application security controls used by her organization. She wants to ensure that the organization is prepared to conduct forensic investigations of future security incidents. Which one of the following OWASP control categories is most likely to contribute to this effort?

        1. Implement logging.
        2. Validate all inputs.
        3. Parameterize queries.
        4. Error and exception handling.

        Answer:

        A. Logging of application and server activity may provide valuable evidence during a forensic investigation. The other three controls listed are proactive controls designed to reduce the risk of an incident occurring and are less likely to directly provide information during a forensic investigation.
246.    While reviewing his Apache logs, Oscar discovers the following entry. What has occurred?

        `10.1.1.1 - - [27/Jun/2023:11:42:22 -0500] "GET /query.php?searchterm=stuff&%20lid=1%20UNION%20SELECT%200, username,user_id,password,name,%20email,%20FROM%20users HTTP/1.1" 200 9918 "-" "Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.1; SV1; .NET CLR 1.1.4322)"`

        1. A successful database query
        2. A PHP overflow attack
        3. A SQL injection attack
        4. An unsuccessful database query

        Answer:

        C. This shows an attempted SQL injection attack. The query reads `1' UNION SELECT 0` and then looks for username, user\_id, password, and email from the `users` table.
247.    Joan is working as a security consultant to a company that runs a critical web application. She discovered that the application has a serious SQL injection vulnerability, but the company cannot take the system offline during the two weeks required to revise the code. Which one of the following technologies would serve as the best compensating control?

        1. IPS
        2. WAF
        3. Vulnerability scanning
        4. Encryption

        Answer:

        B. Vulnerability scanning would not serve as a compensating control because it would only detect, rather than correct, security flaws. There is no indication that encryption is not in place on this server or that it would address a SQL injection vulnerability. Both an intrusion prevention system (IPS) and a web application firewall (WAF) have the ability to serve as a compensating control and block malicious requests. Of the two, a WAF would be the best solution in this case because it is purpose-built for protecting against the exploitation of web application vulnerabilities.
248.    After conducting an `nmap` scan of his network from outside of his network, James notes that a large number of devices are showing three TCP ports open on public IP addresses: 9100, 515, and 631. What type of devices has he found, and how could he reduce his organization's attack surface?

        1. Wireless access points, disable remote administration
        2. Desktop workstations, enable the host firewall
        3. Printers, move the printers to an internal-only IP address range
        4. Network switches, enable encrypted administration mode

        Answer:

        C. You may not remember every common TCP port, but you'll want to make sure you have a good command of a few of them, including things like the LPR (515), IPP (631), and RAW (9100) ports common to many printers. Since these ports need to be open for printing services, the best option would be to move them to a protected subnet or IP range. RFC 1918 nonroutable IP addresses are often used for this purpose, but James may want to look into why devices like this are exposed to the Internet. He may have a deeper problem!
249.    Alex is working to understand his organization's attack surface. Services, input fields in a web application, and communication protocols are all examples of what component of an attack surface evaluation?

        1. Threats
        2. Attack vectors
        3. Risks
        4. Surface tension

        Answer:

        B. Services, input fields, protocols, APIs, and other potential targets are all examples of attack vectors. Threats are possible dangers that might exploit a vulnerability, and risks are the exposure to loss or harm that results from breaches or attacks. Surface tension is a term from physics, not cybersecurity.
250.    Michelle wants to implement a static application security testing (SAST) tool into her continuous integration pipeline. What challenge could she run into if her organization uses multiple programming languages for components of their application stack that will be tested?

        1. They will have to ensure the scanner works with all of the languages chosen.
        2. They will have to compile all of the code to the same binary output language.
        3. They will have to run the applications in a sandbox.
        4. They will have to run the applications under the same execution environment.

        Answer:

        A. Static code analysis requires access to the source code, meaning that the SAST tool will need to be compatible with all the languages that Michelle needs to have tested. Binary output language was made up for this question, while options C and D both refer to dynamic testing because the application would be run in both options.
251.    Ken learns that an APT group is targeting his organization. What term best describes this situation?

        1. Risk
        2. Threat
        3. Countermeasure
        4. Vulnerability

        Answer:

        B. The advanced persistent threat (APT) group is an example of an external threat to the organization. If there is also some vulnerability in the organization's security defenses that might allow that APT to successfully attack the organization, then a risk exists.
252.    Which one of the following activities is _least_ likely to occur during the risk identification process?

        1. Network segmentation
        2. Threat intelligence
        3. Vulnerability scanning
        4. System assessments

        Answer:

        A. Network segmentation is a risk mitigation activity. Threat intelligence, vulnerability scanning, and systems assessments are all valuable tools in helping an organization identify risks.
253.    What two factors are weighted most heavily when determining the severity of a risk?

        1. Probability and magnitude
        2. Likelihood and probability
        3. Magnitude and impact
        4. Impact and control

        Answer:

        A. The two factors that determine the severity of a risk are its probability and magnitude. Impact is a synonym for magnitude. Likelihood is a synonym for probability. Controls are a risk mitigation technique that might be applied to reduce the magnitude and/or probability after determining the severity of a risk.
254.    Preemployment background screening is an example of what type of security control?

        1. Detective
        2. Preventive
        3. Corrective
        4. Compensating

        Answer:

        B. This background screening is taking place prior to employment. Therefore, it is a preventive control, designed to prevent the organization from hiring someone who might pose a security risk.
255.    Roland received a security assessment report from a third-party assessor, and it indicated that one of the organization's web applications is susceptible to an OAuth redirect attack. What type of attack would this vulnerability allow an attacker to wage?

        1. Privilege escalation
        2. Cross-site scripting
        3. SQL injection
        4. Impersonation

        Questions 256–258 refer to the following scenario.

        Gary recently conducted a comprehensive security review of his organization. He identified the 25 top risks to the organization and is pursuing different risk management strategies for each of these risks. In some cases, he is using multiple strategies to address a single risk. His goal is to reduce the overall level of risk so that it lies within his organization's risk tolerance.

        Answer:

        D. OAuth redirects are an authentication attack that allows an attacker to impersonate another user.
256.    Gary decides that the organization should integrate a threat intelligence feed with the firewall. What type of risk management strategy is this?

        1. Risk mitigation
        2. Risk acceptance
        3. Risk transference
        4. Risk avoidance

        Answer:

        A. The use of a threat intelligence feed to block connections at the firewall reduces the likelihood of a successful attack and is, therefore, a risk mitigation activity.
257.    Gary discovers that his organization is storing some old files in a cloud service that are exposed to the world. He deletes those files. What type of risk management strategy is this?

        1. Risk mitigation
        2. Risk acceptance
        3. Risk transference
        4. Risk avoidance

        Answer:

        D. Gary is changing business practices to eliminate the risk entirely. This is, therefore, an example of risk avoidance.
258.    Gary is working with his financial team to purchase a cyber-liability insurance policy to cover the financial impact of a data breach. What type of risk management strategy is he using?

        1. Risk mitigation
        2. Risk acceptance
        3. Risk transference
        4. Risk avoidance

        Answer:

        C. Purchasing insurance is the most common example of risk transference—it's shifting liability to a third party.
259.    Which one of the following risk management strategies is _most_ likely to limit the probability of a risk occurring?

        1. Risk acceptance
        2. Risk avoidance
        3. Risk transference
        4. Risk mitigation

        Answer:

        B. This is a tricky question because two options—risk avoidance and risk mitigation—can both limit the probability of a risk occurring. However, risk avoidance is _more_ likely to do so because it eliminates the circumstances that created the risk, whereas risk mitigation simply introduces controls to reduce the likelihood or impact of a risk. Risk acceptance does not change the probability or magnitude of a risk. Risk transference limits the potential magnitude by transferring financial responsibility to another organization but does not impact probability.
260.    Saanvi would like to reduce the probability of a data breach that affects sensitive personal information. Which one of the following compensating controls is _most_ likely to achieve that objective?

        1. Minimizing the amount of data retained and the number of places where it is stored
        2. Limiting the purposes for which data may be used
        3. Purchasing cyber-risk insurance
        4. Installing a new firewall

        Answer:

        A. This question forces you to choose from several good options, as do many questions on the exam. We can rule out insurance because that does not alter the probability of a risk occurring. The remaining three options all do reduce the likelihood, but the best choice is minimizing the amount of data retained and the number of locations where it is stored, since this removes that data from the potential of a breach.
261.    Kwame recently completed a risk assessment and is concerned that the level of residual risk exceeds his organization's risk tolerance. What should he do next?

        1. Have a discussion with his manager.
        2. Implement new security controls.
        3. Modify business processes to lower risk.
        4. Purge data from systems.

        Questions 262–267 refer to the following scenario.

        Alan is a risk manager for Acme University, a higher education institution located in the western United States. He is concerned about the threat that an earthquake will damage his organization's primary datacenter. He recently undertook a replacement cost analysis and determined that the datacenter is valued at $10 million.

        After consulting with seismologists, Alan determined that an earthquake is expected in the area of the datacenter once every 200 years. Datacenter specialists and architects helped him determine that an earthquake would likely cause $5 million in damage to the facility.

        Answer:

        A. Kwame should take action to communicate the risk factors to management and facilitate a risk-informed discussion about possible courses of action. He should do this prior to taking any more aggressive action.
262.    Based on the information in this scenario, what is the exposure factor (EF) for the effect of an earthquake on Acme University's datacenter?

        1. 10 percent
        2. 25 percent
        3. 50 percent
        4. 75 percent

        Answer:

        C. The exposure factor (EF) is the percentage of the facility that risk managers expect will be damaged if the risk materializes. It is calculated by dividing the amount of damage by the asset value. In this case, that is $5 million in damage divided by the $10 million facility value, or 50 percent.
263.    Based on the information in this scenario, what is the annualized rate of occurrence (ARO) for an earthquake at the datacenter?

        1. .0025
        2. .005
        3. .01
        4. .015

        Answer:

        B. The annualized rate of occurrence (ARO) is the number of times that risk analysts expect a risk to happen in any given year. In this case, the analysts expect an earthquake once every 200 years, or 0.005 times per year.
264.    Based on the information in this scenario, what is the annualized loss expectancy (ALE) for an earthquake at the datacenter?

        1. $25,000
        2. $50,000
        3. $250,000
        4. $500,000

        Answer:

        A. The annualized loss expectancy (ALE) is calculated by multiplying the single loss expectancy (SLE) by the annualized rate of occurrence (ARO). In this case, the SLE is $5,000,000, and the ARO is 0.005. Multiplying these numbers together gives you the ALE of $25,000.
265.    Referring to the previous scenario, if Alan's organization decides to move the datacenter to a location where earthquakes are not a risk, what risk management strategy are they using?

        1. Risk mitigation
        2. Risk avoidance
        3. Risk acceptance
        4. Risk transference

        Answer:

        B. Moving the datacenter to a location where earthquakes are not a risk is an example of risk avoidance, because it is completely avoiding the risk. If the location simply had a lower risk of earthquake, then this strategy would be risk mitigation.
266.    Referring to the previous scenario, if the organization decides not to relocate the datacenter but instead purchases an insurance policy to cover the replacement cost of the datacenter, what risk management strategy are they using?

        1. Risk mitigation
        2. Risk avoidance
        3. Risk acceptance
        4. Risk transference

        Answer:

        D. Purchasing insurance is always an example of risk transference, as it transfers risk from the entity purchasing the policy to the insurance company.
267.    Referring to the previous scenario, assume that the organization decides that relocation is too difficult and the insurance is too expensive. They instead decide that they will carry on despite the risk of earthquake and handle the impact if it occurs. What risk management strategy are they using?

        1. Risk mitigation
        2. Risk avoidance
        3. Risk acceptance
        4. Risk transference

        Answer:

        C. Risk acceptance is the deliberate decision to not take any other risk management action and simply to carry on with normal activity in spite of the risk.
268.    Colin would like to implement a detective security control in his accounting department, which is specifically designed to identify cases of fraud that are able to occur despite the presence of other security controls. Which one of the following controls is best suited to meet Colin's need?

        1. Separation of duties
        2. Least privilege
        3. Dual control
        4. Mandatory vacations

        Answer:

        D. Mandatory vacations are designed to force individuals to take time away from the office to allow fraudulent activity to come to light in their absence. The other controls listed here (separation of duties, least privilege, and dual control) are all designed to prevent, rather than detect, fraud.
269.    Rob is an auditor reviewing the managerial controls used in an organization. He is examining the payment process used by the company to issue checks to vendors. He notices that Helen, a staff accountant, is the person responsible for creating new vendors. Norm, another accountant, is responsible for issuing payments to vendors. Helen and Norm are cross-trained to provide backup for each other. What security issue, if any, exists in this situation?

        1. Least privilege violation
        2. Separation of duties violation
        3. Dual control violation
        4. No issue

        Answer:

        B. This situation violates the principle of separation of duties. The company appears to have designed the controls to separate the creation of vendors from the issuance of payments, which is a good fraud-reduction practice. However, the fact that they are cross-trained to back each other up means that they have the permissions assigned to violate this principle.
270.    Mei recently completed a risk management review and identified that the organization is susceptible to an on-path (also known as man-in-the-middle) attack. After review with her manager, they jointly decided that accepting the risk is the most appropriate strategy. What should Mei do next?

        1. Implement additional security controls.
        2. Design a remediation plan.
        3. Repeat the business impact assessment.
        4. Document the decision.

        Answer:

        D. After accepting a risk, the organization takes no action other than to document the risk as accepted. Implementing additional security controls or designing a remediation plan would not be risk acceptance but would instead fit into the category of risk mitigation. There is no need to repeat the business impact assessment.
271.    Robin is planning to conduct a risk assessment in her organization. She is concerned that it will be difficult to perform the assessment because she needs to include information about both tangible and intangible assets. What would be the most effective risk assessment strategy for her to use?

        1. Quantitative risk assessment
        2. Qualitative risk assessment
        3. Combination of quantitative and qualitative risk assessment
        4. Neither quantitative nor qualitative risk assessment

        Answer:

        C. Robin would achieve the best results by combining elements of quantitative and qualitative risk assessment. Quantitative risk assessment excels at analyzing tangible, financial risks, whereas qualitative risk assessment is good for intangible risks. Combining the two techniques provides a well-rounded risk picture.
272.    Barry's organization is running a security exercise and Barry was assigned to conduct offensive operations. What term best describes Barry's role in the process?

        1. Red team
        2. Purple team
        3. Blue team
        4. White team

        Answer:

        A. In a security exercise, the red team is responsible for offensive operations, whereas the blue team is responsible for defensive operations. The white team serves as the neutral referees, whereas the purple team combines elements of the red team and blue team.
273.    Vlad's organization recently underwent a security audit that resulted in a finding that the organization fails to promptly remove the accounts associated with users who have left the organization. This resulted in at least one security incident where a terminated user logged into a corporate system and took sensitive information. What identity and access management control would best protect against this risk?

        1. Automated deprovisioning
        2. Quarterly user account reviews
        3. Separation of duties
        4. Two-person control

        Answer:

        A. Automated deprovisioning ties user account removal to human resources systems. Once a user is terminated in the human resources system, the identity and access management infrastructure automatically removes the account. Quarterly user access reviews may identify accounts that should have been disabled, but they would take a long time to do so, so they are not the best solution to the problem. Separation of duties and two-person control are designed to limit the authority of a user account and would not remove access.
274.    Jay is the CISO for his organization and is responsible for conducting periodic reviews of the organization's information security policy. The policy was written three years ago and has undergone several minor revisions after audits and assessments. Which one of the following would be the most reasonable frequency to conduct formal reviews of the policy?

        1. Monthly
        2. Quarterly
        3. Annually
        4. Every five years

        Answer:

        C. Annual reviews of security policies are an industry standard and are sufficient unless there are special circumstances, such as a new policy or major changes in the environment. Monthly or quarterly reviews would occur too frequently, whereas waiting five years for the review is likely to miss important changes in the environment.
275.    Terri is undertaking a risk assessment for her organization. Which one of the following activities would normally occur first?

        1. Risk identification
        2. Risk calculation
        3. Risk mitigation
        4. Risk management

        Answer:

        A. The first step in performing a risk assessment is to undertake the risk identification process.
276.    Kai is attempting to determine whether he can destroy a cache of old records that he discovered. What type of policy would most directly answer his question?

        1. Data ownership
        2. Data classification
        3. Data minimization
        4. Data retention

        Answer:

        D. The most relevant policy here is the organization's data retention policy, which should outline the standards for keeping records before destruction or disposal.
277.    Fences are a widely used security control that can be described by several different control types. Which one of the following control types would _least_ describe a fence?

        1. Deterrent
        2. Corrective
        3. Preventive
        4. Physical

        Answer:

        B. Fences are preventive controls because a tall fence can prevent an intruder from gaining access to a secure facility. They are also deterrent controls because the presence of a fence may deter an intruder from attempting to gain access. They are physical security controls because they restrict physical access. They are not corrective controls because they do not play a role after a physical intrusion occurs.
278.    Ian is designing an authorization scheme for his organization's deployment of a new accounting system. He is considering putting a control in place that would require that two accountants approve any payment request over $100,000. What security principle is Ian seeking to enforce?

        1. Security through obscurity
        2. Least privilege
        3. Separation of duties
        4. Dual control

        Answer:

        D. It is sometimes difficult to distinguish between cases of least privilege, separation of duties, and dual control. Least privilege means that an employee should only have the access rights necessary to perform their job. That is not the case in this scenario because accountants need to be able to approve payments. Separation of duties occurs when the same employee does not have permission to perform two different actions that, when combined, could undermine security. That is not the case here because both employees are performing the same action: approving the payment. Dual control occurs when two employees must jointly authorize the same action. That is the case in this scenario. Security through obscurity occurs when the security of a control depends on the secrecy of its mechanism.
279.    Carmen is working with a new vendor on the design of a penetration test. She would like to ensure that the vendor does not conduct any physical intrusions as part of their testing. Where should Carmen document this requirement?

        1. Rules of engagement
        2. Service level objectives
        3. Nondisclosure agreement
        4. Counterparty agreement

        Answer:

        A. The rules of engagement for a penetration test outline the activities that are (and are not) permissible during a test. Carmen should include her requirement in the penetration test's rules of engagement.
280.    Gavin is drafting a document that provides a detailed step-by-step process that users may follow to connect to the VPN from remote locations. Alternatively, users may ask IT to help them configure the connection. What term best describes this document?

        1. Policy
        2. Procedure
        3. Standard
        4. Guideline

        Answer:

        B. A procedure offers a step-by-step process for completing a cybersecurity activity. The VPN instructions that Gavin is creating are best described using this term.
281.    Which one of the following security controls is designed to help provide continuity for security responsibilities?

        1. Succession planning
        2. Separation of duties
        3. Mandatory vacation
        4. Dual control

        Answer:

        A. Succession planning is designed to create a pool of reserve candidates ready to step into positions when a vacancy occurs. This is an important continuity control. The other security controls may have the incidental side effect of exposing employees to other responsibilities, but they are not designed to meet this goal.
282.    After conducting a security review, Oskar determined that his organization is not conducting regular backups of critical data. What term best describes the type of control gap that exists in Oskar's organization?

        1. Preventive
        2. Corrective
        3. Detective
        4. Deterrent

        Answer:

        B. Backups are used to recover operations in the wake of a security incident. Therefore, they are best described as corrective controls.
283.    Carla is reviewing the cybersecurity policies used by her organization. What policy might she put in place as a failsafe to cover employee behavior situations where no other policy directly applies?

        1. Data monitoring policy
        2. Account management policy
        3. Code of conduct
        4. Data ownership policy

        Answer:

        C. An organization's code of conduct or ethics describes expected behavior of employees and affiliates and serves as a backstop for situations not specifically addressed in policy.
284.    Which one of the following items is _not_ normally included in a request for an exception to security policy?

        1. Description of a compensating control
        2. Description of the risks associated with the exception
        3. Proposed revision to the security policy
        4. Business justification for the exception

        Answer:

        C. Requests for an exception to a security policy would not normally include a proposed revision to the policy. Exceptions are documented variances from the policy because of specific technical and/or business requirements. They do not alter the original policy, which remains in force for systems not covered by the exception.
285.    What policy should contain provisions for removing user access upon termination?

        1. Data ownership policy
        2. Data classification policy
        3. Data retention policy
        4. Account management policy

        Questions 286–288 refer to the following scenario:

        Karen is the CISO of a major manufacturer of industrial parts. She is currently performing an assessment of the firm's financial controls, with an emphasis on implementing security practices that will reduce the likelihood of theft from the firm.

        Answer:

        D. Account management policies describe the account life cycle from provisioning through active use and decommissioning, including removing access upon termination. Data ownership policies clearly state the ownership of information created or used by the organization. Data classification policies describe the classification structure used by the organization and the process used to properly assign classifications to data. Data retention policies outline what information the organization will maintain and the length of time different categories of information will be retained prior to destruction.
286.    Karen would like to ensure that the same individual is not able to both create a new vendor in the system and authorize a payment to that vendor. She is concerned that an individual who could perform both of these actions would be able to send payments to false vendors. What type of control should Karen implement?

        1. Mandatory vacations
        2. Separation of duties
        3. Job rotation
        4. Two-person control

        Answer:

        B. Separation of duties is a principle that prevents individuals from having two different privileges that, when combined, could be misused. Separating the ability to create vendors and authorize payments is an example of two-person control.
287.    The accounting department has a policy that requires the signatures of two individuals on checks valued over $5,000. What type of control do they have in place?

        1. Mandatory vacations
        2. Separation of duties
        3. Job rotation
        4. Two-person control

        Answer:

        D. Two-person control is a principle that requires the concurrence of two different employees to perform a single sensitive action. Requiring two signatures on a check is an example of a two-person control.
288.    Karen would also like to implement controls that would help detect potential malfeasance by existing employees. Which one of the following controls is _least_ likely to detect malfeasance?

        1. Mandatory vacations
        2. Background investigations
        3. Job rotation
        4. Privilege use reviews

        Answer:

        B. Mandatory vacations and job rotation plans are able to detect malfeasance by requiring an employee's absence from his or her normal duties and exposing them to other employees. Privilege use reviews have a manager review the actions of an employee with privileged system access and would detect misuse of those privileges. Background investigations uncover past acts and would not be helpful in detecting active fraud. They are also typically performed only for new hires.
289.    Kevin is conducting a security exercise for his organization that uses both offensive and defensive operations. His role is to serve as the moderator of the exercise and to arbitrate disputes. What role is Kevin playing?

        1. White team
        2. Red team
        3. Swiss team
        4. Blue team

        Answer:

        A. The role of the white team is to control the exercise, serving as a neutral party to facilitate events and moderate disputes. The red team is responsible for offensive operations, whereas the blue team is responsible for defensive operations. The term _Swiss team_ is not used in security exercises.
290.    Bohai is concerned about access to the main account for a cloud service that his company uses to manage payment transactions. He decides to implement a new process for multifactor authentication to that account where an individual on the IT team has the password to the account, while an individual in the accounting group has the token. What security principle is Bohai using?

        1. Dual control
        2. Separation of duties
        3. Least privilege
        4. Security through obscurity

        Answer:

        A. This is an example of dual control (or two-person control) where performing a sensitive action (logging onto the payment system) requires the cooperation of two individuals. Separation of duties is related but would involve not allowing the same person to perform two actions that, when combined, could be harmful.
291.    Tina is preparing for a penetration test and is working with a new vendor. She wants to make sure that the vendor understands exactly what technical activities are permitted within the scope of the test. Where should she document these requirements?

        1. MOA
        2. Contract
        3. RoE
        4. SLA

        Answer:

        C. The rules of engagement (RoE) for a penetration test outline the permissible and impermissible activities for testers. If there are any systems, techniques, or information that is off-limits, this should be clearly stated in the RoE.
292.    Azra is reviewing a draft of the Domer Doodads information security policy and finds that it contains the following statements. Which one of these statements would be more appropriately placed in a different document?

        1. Domer Doodads designates the chief information security officer as the individual with primary responsibility for information security.
        2. The chief information security officer is granted the authority to create specific requirements that implement this policy.
        3. All access to financial systems must use multifactor authentication for remote connections.
        4. Domer Doodads considers cybersecurity and compliance to be of critical importance to the business.

        Answer:

        C. It is normal to find statements in an information security policy that declare the importance of cybersecurity to the organization, designate a specific individual as responsible for the cybersecurity function, and grant that individual authority over cybersecurity. Specific requirements, such as requiring multifactor authentication for financial systems would be more appropriately placed in a standard than a policy.
293.    Which one of the following security policy framework documents _never_ includes mandatory employee compliance?

        1. Policy
        2. Guideline
        3. Procedure
        4. Standard

        Answer:

        B. Guidelines are optional advice, by definition. Policies and standards are always mandatory. Procedures may be mandatory or optional, depending on the organizational context.
294.    Kaitlyn is on the red team during a security exercise, and she has a question about whether an activity is acceptable under the exercise's rules of engagement. Who would be the most appropriate person to answer her question?

        1. Red team leader.
        2. White team leader.
        3. Blue team leader.
        4. Kaitlyn should act without external advice.

        Questions 295–299 refer to the following scenario.

        Seamus is conducting a business impact assessment for his organization. He is attempting to determine the risk associated with a denial-of-service attack against his organization's datacenter.

        Seamus consulted with various subject-matter experts (SMEs) and determined that the attack would not cause any permanent damage to equipment, applications, or data. The primary damage would come in the form of lost revenue. Seamus believes that the organization would lose $75,000 in revenue during a successful attack.

        Seamus also consulted with his threat management vendor, who considered the probability of a successful attack against his organization and determined that there is a 10 percent chance of a successful attack in the next 12 months.

        Answer:

        B. The white team is responsible for interpreting rules and arbitrating disputes during a security exercise. The white team leader would be the most appropriate person from this list to answer Kaitlyn's question.
295.    What is the ARO for this assessment?

        1. 8 percent
        2. 10 percent
        3. 12 percent
        4. 100 percent

        Answer:

        B. The annualized rate of occurrence (ARO) is calculated as the number of times an attack should be expected in a given year. This may be expressed as a decimal or percentage. The scenario tells us that there is a 10 percent chance of an attack in a given year. This could be described as an ARO of 10 percent, or 0.1.
296.    What is the SLE for this scenario?

        1. $625
        2. $6,250
        3. $7,500
        4. $75,000

        Answer:

        D. The single loss expectancy (SLE) is the amount of damage expected to occur as the result of a single successful attack. In this case, the scenario provides this information as $75,000.
297.    What is the ALE for this scenario?

        1. $625
        2. $6,250
        3. $7,500
        4. $75,000

        Answer:

        C. The annualized loss expectancy (ALE) is the amount of damage expected in any given year. It is calculated by multiplying the SLE ($75,000) by the ARO (10 percent) to get the ALE ($7,500).
298.    Seamus is considering purchasing a DDoS protection system that would reduce the likelihood of a successful attack. What type of control is he considering?

        1. Detective
        2. Corrective
        3. Preventive
        4. Deterrent

        Answer:

        C. Determining the single best category for a control is always tricky, as many controls can cross categories in terms of their purpose. In this case, we are told that the control exists to reduce the likelihood of an attack, making it a preventive control.
299.    Seamus wants to make sure that he can accurately describe the category of the DDoS protection service to auditors. Which term best describes the category of this control?

        1. Compensating
        2. Physical
        3. Operational
        4. Technical

        Questions 300 and 301 refer to the following scenario:

        Piper's organization handles credit card information and is, therefore, subject to the Payment Card Industry Data Security Standard (PCI DSS). She is working to implement the PCI DSS requirements.

        Answer:

        D. A DDoS mitigation service takes action to reduce the load on the network by blocking unwanted traffic. This is a technical intervention and is best described as a technical control.
300.    As Piper attempts to implement PCI DSS requirements, she discovers that she is unable to meet one of the requirements because of a technical limitation in her point-of-sale system. She decides to work with regulators to implement a second layer of logical isolation to protect this system from the Internet to allow its continued operation despite not meeting one of the requirements. What term best describes the type of control Piper has implemented?

        1. Physical control
        2. Operational control
        3. Compensating control
        4. Deterrent control

        Answer:

        C. PCI DSS allows organizations that cannot meet a specific PCI DSS requirement to implement a compensating control that mitigates the risk. This is the process Piper is following in this scenario.
301.    When Piper implements this new isolation technology, what type of risk management action is she taking?

        1. Risk acceptance
        2. Risk avoidance
        3. Risk transference
        4. Risk mitigation

        Answer:

        D. The purpose of this control is to reduce the probability of an attack. Implementing controls designed to reduce the probability or magnitude of a risk is a risk mitigation activity.
302.    Ruth is helping a business leader determine the appropriate individuals to consult about sharing information with a third-party organization. Which one of the following policies would likely contain the most relevant guidance for her?

        1. Data retention policy
        2. Information security policy
        3. Data validation policy
        4. Data ownership policy

        Answer:

        D. Sharing data outside the organization normally requires the consent of the data owner. Ruth should consult the data ownership policy for assistance in determining the identities of the appropriate data owner(s) that she should consult.
303.    Samantha is investigating a cybersecurity incident where an internal user used his computer to participate in a denial-of-service attack against a third party. What type of policy was most likely violated?

        1. AUP
        2. SLA
        3. BCP
        4. Information classification policy

        Answer:

        A. This activity is almost certainly a violation of the organization's acceptable use policy (AUP), which should contain provisions describing appropriate use of networks and computing resources belonging to the organization.
304.    Ryan is compiling a list of allowable encryption algorithms for use in his organization. What type of document would be most appropriate for this list?

        1. Policy
        2. Standard
        3. Guideline
        4. Procedure

        Answer:

        B. Standards describe specific security controls that must be in place for an organization. Ryan would not include a list of algorithms in a high-level policy document, and this information is too general to be useful as a procedure. Guidelines are not mandatory, so they would not be applicable in this scenario.
305.    During the design of an identity and access management authorization scheme, Katie took steps to ensure that members of the security team who can approve database access requests do not have access to the database themselves. What security principle is Katie most directly enforcing?

        1. Least privilege
        2. Separation of duties
        3. Dual control
        4. Security through obscurity

        Answer:

        B. It is sometimes difficult to distinguish between cases of least privilege, separation of duties, and dual control. Least privilege means that an employee should only have the access rights necessary to perform their job. While this may be true in this scenario, you do not have enough information to make that determination because you do not know whether access to the database would help the security team perform their duties. Separation of duties occurs when the same employee does not have permission to perform two different actions that, when combined, could undermine security. That is the case here because a team member who had the ability to both approve access and access the database may be able to grant themselves access to the database. Dual control occurs when two employees must jointly authorize the same action. Security through obscurity occurs when the security of a control depends on the secrecy of its mechanism.
306.    Which one of the following controls is useful to both facilitate the continuity of operations and serve as a deterrent to fraud?

        1. Succession planning
        2. Dual control
        3. Cross-training
        4. Separation of duties

        Answer:

        C. Succession planning and cross-training both serve to facilitate continuity of operations by creating a pool of candidates for job vacancies. Of these, only cross-training encompasses actively involving other people in operational processes, which may also help detect fraud. Dual control and separation of duties are both controls that deter fraud, but they do not facilitate the continuity of operations.
307.    Which one of the following requirements is often imposed by organizations as a way to achieve their original control objective when they approve an exception to a security policy?

        1. Documentation of scope
        2. Limited duration
        3. Compensating control
        4. Business justification

        Answer:

        C. Organizations may require all of these items as part of an approved exception request. However, the documentation of scope, duration of the exception, and business justification are designed to clearly describe and substantiate the exception request. The compensating control, on the other hand, is designed to ensure that the organization meets the intent and rigor of the original requirement.
308.    Berta is reviewing the security procedures surrounding the use of a cloud-based online payment service by her company. She set the access permissions for this service so that the same person cannot add funds to the account and transfer funds out of the account. What security principle is most closely related to Berta's action?

        1. Least privilege
        2. Security through obscurity
        3. Separation of duties
        4. Dual control

        Answer:

        C. This is an example of separation of duties. Someone who has the ability to transfer funds into the account and issue payments could initiate a very large fund transfer, so Berta has separated these responsibilities into different roles. Separation of duties goes beyond least privilege by intentionally changing jobs to minimize the access that an individual has, rather than granting them the full permissions necessary to perform their job. This is not an example of dual control because a single individual can still perform each action.
309.    Thomas found himself in the middle of a dispute between two different units in his business that are arguing over whether one unit may analyze data collected by the other. What type of policy would most likely contain guidance on this issue?

        1. Data ownership policy
        2. Data classification policy
        3. Data retention policy
        4. Account management policy

        Answer:

        A. Data ownership policies clearly state the ownership of information created or used by the organization. Data classification policies describe the classification structure used by the organization and the process used to properly assign classifications to data. Data retention policies outline what information the organization will maintain and the length of time different categories of information will be retained prior to destruction. Account management policies describe the account life cycle from provisioning through active use and decommissioning.
310.    Mara is designing a new data mining system that will analyze access control logs for signs of unusual login attempts. Any suspicious logins will be automatically locked out of the system. What type of control is Mara designing?

        1. Physical control
        2. Operational control
        3. Managerial control
        4. Technical control

        Answer:

        D. The automatic blocking of logins is a technical activity and this is, therefore, a technical control. Physical controls are security controls that impact the physical world. Operational controls include the processes that we put in place to manage technology in a secure manner. Managerial controls are procedural mechanisms that an organization follows to implement sound security management practices.
311.    Which one of the following elements is _least_ likely to be found in a data retention policy?

        1. Minimum retention period for data
        2. Maximum retention period for data
        3. Description of information to retain
        4. Classification of information elements

        Answer:

        D. Data retention policies describe what information the organization will maintain and the length of time different categories of information will be retained prior to destruction, including both minimum and maximum retention periods. Data classification would be covered by the data classification policy.
312.    Kevin leads the IT team at a small business and does not have a dedicated security team. He would like to develop a security baseline of his organization's system configurations but does not have a team of security experts available to assist him. Which of the following is the most appropriate tool for Kevin to use?

        1. Penetration testing tool
        2. Patch management tool
        3. Vulnerability scanning tool
        4. Network monitoring tool

        Answer:

        C. A vulnerability scanner is the most appropriate tool for Kevin to use to conduct security baseline scans. Vulnerability scanners are automated tools that can identify known vulnerabilities and misconfigurations on a system. They can scan a wide range of systems, including servers, workstations, and network devices. They are designed to be easy to use, even for IT professionals who are not security experts.

        Kevin might be able to obtain similar information using a penetration testing tool, but those tools tend to require skilled cybersecurity professionals to operate and analyze the results.

        Patch management and network monitoring tools are useful security tools, but they do not develop a baseline of system configurations.
313.    Jenna is helping her organization choose a set of security standards that will be used to secure a variety of operating systems. She is looking for industry guidance on the appropriate settings to use for Windows and Linux systems. Which one of the following tools will serve as the best resource?

        1. ISO 27001
        2. OWASP
        3. PCI DSS
        4. CIS benchmarks

        Answer:

        D. All of these resources provide valuable information to security professionals seeking to design a security program according to industry standards. However, only the Center for Internet Security (CIS) provides detailed baseline standards that include step-by-step instructions for configuring systems to meet specific security requirements. The CIS benchmarks are widely used as a resource for securing systems in various industries.

        ISO 27001 is a standard for information security management systems (ISMS), which outlines a framework for managing and protecting sensitive information. While it may include some guidance on securing systems, it is not specific to Windows or Linux and is more focused on overall information security management.

        Open Worldwide Application Security Project (OWASP) is a nonprofit organization that provides a variety of resources for web application security, including a list of the top 10 most critical web application security risks. While it may include some guidance on securing systems, it is not specific to Windows or Linux and is more focused on web application security.

        Payment Card Industry Data Security Standard (PCI DSS) is a standard for securing credit card information. There is no indication in the scenario that Jenna's organization handles credit card data, so this would not be an appropriate standard for her to use.
314.    Linda is attempting to configure Angry IP Scanner on her Linux scanning workstation and is receiving errors about missing required software. What component must be installed prior to using Angry IP Scanner?

        1. `nmap`
        2. Java
        3. `gcc`
        4. Nessus

        Answer:

        B. The Angry IP scanner is a multiplatform tool that is written in the Java language. It does require a Java runtime to function properly. It does not require other scanning tools, such as `nmap` or Nessus. It also does not require a C compiler, such as `gcc`.
315.    Chris is investigating a malware outbreak and would like to reverse engineer the code. Which one of the following tools is specifically designed for this task?

        1. Immunity debugger
        2. ZAP
        3. Recon-ng
        4. GDB

        Answer:

        A. The Immunity debugger is designed specifically to support penetration testing and the reverse engineering of malware.

        GNU debugger (GDB) is a widely used open source debugger for Linux that works with a variety of programming languages. It may assist Chris in this work, but it is not specifically designed for reverse engineering malware, so it is not as good an answer as Immunity.

        Recon-ng and ZAP are tools designed to assist in website penetration tests. Recon-ng automates web application reconnaissance, while ZAP serves as an interception proxy. Neither is likely to be useful in reverse engineering malware.
316.    Jim is working with a penetration testing contractor who proposes using Metasploit as part of his penetration testing effort. What should Jim expect to occur when Metasploit is used?

        1. Systems will be scanned for vulnerabilities.
        2. Systems will have known vulnerabilities exploited.
        3. Services will be probed for buffer overflow and other unknown flaws.
        4. Systems will be tested for zero-day exploits.

        Answer:

        B. Metasploit is an exploitation package that is designed to assist penetration testers. A tester using Metasploit can exploit known vulnerabilities for which an exploit has been created or can create their own exploits using the tool. While Metasploit provides built-in access to some vulnerability scanning functionality, a tester using Metasploit should primarily be expected to perform actual tests of exploitable vulnerabilities. Similarly, Metasploit supports creating buffer overflow attacks, but it is not a purpose-built buffer overflow testing tool, and of course testing systems for zero-day exploits doesn't work unless they have been released.
317.    Which one of the following best describes recon-ng as a security tool?

        1. Vulnerability scanner
        2. Web application reconnaissance tool
        3. Network mapper
        4. Password cracker

        Answer:

        B. Recon-ng is an automated web application reconnaissance tool that helps penetration testers and attackers discover information about a web environment in advance of trying to exploit that environment.
318.    Ashley is investigating an attack that compromised an account of one of her users. In the attack, the attacker forced the submission of an authenticated request to a third-party site by exploiting trust relationships in the user's browser. What type of attack most likely took place?

        1. XSS
        2. CSRF
        3. SQL injection
        4. Session hijacking

        Answer:

        B. Cross-site request forgery (XSRF or CSRF) attacks exploit the trust that sites have in a user's browser by attempting to force the submission of authenticated requests to third-party sites. Cross-site scripting (XSS) uses reflected input to trick a user's browser into executing untrusted code from a trusted site. SQL injection directly attacks a database through a web application. Session hijacking attacks attempt to steal previously authenticated sessions but do not force the browser to submit requests.
319.    Juanita is a cybersecurity professional who works with data scientists at a company that uses machine learning (ML) models to predict customer behavior. She believes that their work has been the target of a data poisoning attack.

        Which of the following actions should she take to address the situation?

        1. Ignore the problem as it is unlikely to have an operational effect.
        2. Remove affected data from the training dataset and generate a new model.
        3. Generate a new model using the same dataset and machine learning algorithm.
        4. Generate a new model using the same dataset and a different machine learning algorithm.

        Answer:

        B. Data poisoning, the act of injecting false or misleading data into a machine learning model's training dataset, can cause the model to make incorrect predictions or decisions. By removing the false data and retraining the model, Juanita can ensure that the model is not basing its predictions or decisions on faulty or malicious data.

        Juanita should not ignore the problem because it is likely to have had an effect on the accuracy of the model. She should not use the same dataset to generate a new model (regardless of algorithm choice) because that model would still be based upon the poisoned data.
320.    Joshua is concerned about insecure software design practices and is developing a software threat modeling program for his organization. Which of the following is not an appropriate goal for this program?

        1. To reduce the number of security-related design flaws
        2. To reduce the number of security-related coding flaws
        3. To reduce the severity of non-security-related flaws
        4. To reduce the number of threat vectors

        Answer:

        D. Software threat modeling is designed to reduce the number of security-related design and coding flaws as well as the severity of other flaws. The developer or evaluator of software has no control over the threat environment, because it is external to the organization.
321.    Gavin works as a cybersecurity analyst and notices that issues continually arise in his organization where system administrators modify system configuration files without providing advance notice to other teams. In several situations, this resulted in a security misconfiguration. What control would best prevent these issues from recurring in the future?

        1. Change management program
        2. Security-enhanced operating system
        3. Configuration lockdown
        4. File integrity monitoring

        Answer:

        A. There are many potential solutions to this problem. Locking down configurations might prevent unauthorized changes, but it would also likely disrupt authorized changes. File integrity monitoring systems may identify an unauthorized change but only after it occurred. A security-enhanced operating system is designed to implement advanced security controls and does not address this specific risk.

        The underlying problem here is that system administrators are making changes without properly coordinating them with other teams. A strong change management program would directly address this root cause.
322.    Brenda maintains a web application and learned that the application contains a remote code execution vulnerability that is triggered by sending a carefully crafted message to a logging service that runs on the underlying server. What action should Brenda take to best address this risk?

        1. Modify the code of the web application to eliminate the vulnerability.
        2. Install an intrusion detection system.
        3. Check for and apply patches from the logging vendor.
        4. Ignore the issue because the logging service is not her responsibility.

        Answer:

        C. The vulnerability that exists in this situation is in the code for the logging service. Modifying the code of the web application is unlikely to correct this problem. The code of the underlying logging service is the issue, so Brenda should check for a patch from the vendor who created that service and apply the patch promptly.

        An intrusion detection system would only identify that the vulnerability was being exploited and not correct the issue.

        Brenda should not ignore this issue as remote code execution vulnerabilities are extremely serious.
323.    Viola is analyzing an attack that occurred against her organization. The attacker was able to manipulate a web application to display a confidential data file that was stored on the server by traversing the directory structure in the URL. What term best describes this type of attack?

        1. SQL injection
        2. Server-side request forgery
        3. Local file inclusion
        4. Remote file inclusion

        Answer:

        C. You might find this question a little confusing because the scenario seems to describe a directory traversal attack, and that is not one of the answer choices. The key to successfully answering this question is understanding that a directory traversal attack is a type of local file inclusion (LFI) attack. LFI attacks allow a remote user to access files stored on a server. Directory traversal achieves the attacker's goal of LFI by navigating the directory structure with navigation commands such as `..` and `/` in the URL. Remote file inclusion (RFI) attacks use a similar approach but allow the attacker to execute code that is hosted on their own computer using the targeted server.
324.    Melissa is concerned that users in her organization are connecting to corporate systems over insecure networks and begins a security awareness campaign designed to encourage them to use the VPN. What category of control has Melissa implemented?

        1. Compensating
        2. Technical
        3. Operational
        4. Managerial

        Answer:

        D. Security awareness training is an example of a managerial security control because it is an administrative practice. The subject of the training is the use of the VPN, which is a technical control, but the training itself is managerial in nature.
325.    The company Chris works for has notifications posted at each door reminding employees to be careful not to allow people to enter when they do. Which type of control is this?

        1. Detective
        2. Responsive
        3. Preventive
        4. Corrective

        Answer:

        C. Notifications and procedures like the signs posted at the company Chris works for are examples of preventive controls because they are designed to stop unauthorized activity from occurring in the first place. They do not identify security incidents, as a detective control would. They do not respond to active security incidents, as a responsive control would, and they do not correct the effects of a security incident, as a corrective control would.
326.    Kevin has discovered a security vulnerability in one of his organization's business-critical systems. He evaluates the situation and determines that it presents a low risk to the organization but would like to correct it. There is a patch available from the vendor. When should Kevin plan to apply the patch?

        1. Immediately
        2. During the next scheduled maintenance window
        3. As soon as possible outside of normal business hours
        4. During the next major system upgrade

        Answer:

        B. A maintenance window is a period of time during which routine maintenance and updates are scheduled to be performed on systems, devices, and infrastructure. This can include software updates, security patches, hardware replacements, and other types of maintenance activities. This is a low-risk vulnerability so Kevin can wait until the next maintenance window to apply it.
327.    Ben is responsible for the security of payment card information stored in a database. Policy directs that he remove the information from the database, but he cannot do this for operational reasons. He obtained an exception to policy and is seeking an appropriate compensating control to mitigate the risk. What would be his best option?

        1. Purchasing insurance
        2. Encrypting the database contents
        3. Removing the data
        4. Objecting to the exception

        Answer:

        B. Ben should encrypt the data to provide an additional layer of protection as a compensating control. The organization has already made a policy exception, so he should not react by objecting to the exception or removing the data without authorization. Purchasing insurance may transfer some of the risk but is not a mitigating control.
328.    Isabelle wants to prevent privilege escalation attacks via her organization's service accounts. Which of the following security practices is best suited to this?

        1. Remove unnecessary rights.
        2. Disable interactive login for service accounts.
        3. Limit when accounts can log in.
        4. Use meaningless or randomized names for service accounts.

        Answer:

        A. The most important step in securing service accounts is to ensure that they have only the rights that are absolutely needed to accomplish the task they are designed for. Disabling interactive logins is important as well and would be the next best answer. Limiting when accounts can log in and using randomized or meaningless account names can both be helpful in some circumstances but are far less important.
329.    Brandon is validating the security of systems and devices in his organization, but he is permitted to use only passive techniques. Which one of the following actions would be considered passive discovery?

        1. Monitoring network traffic and analyzing the contents for signs of unpatched systems and applications
        2. Running vulnerability scans of an organization's servers
        3. Running port scans of an organization's servers
        4. Using carefully scoped penetration testing techniques to identify vulnerabilities

        Answer:

        A. Passive discovery techniques involve no interaction with the target system. Monitoring network traffic would, therefore, be a passive technique because it does not actively engage the target system.

        Vulnerability scanners, port scanners, and penetration testing techniques are active tools that directly interact with the target system.
330.    Ryan's organization wants to ensure that proper account management is occurring but does not have a central identity and access management tool in place. Ryan has a limited amount of time to do his verification process. What is his best option to test the account management process as part of an internal audit?

        1. Validate all accounts changed in the past 90 days.
        2. Select high value administrative accounts for validation.
        3. Validate all accounts changed in the past 180 days.
        4. Validate a random sample of accounts.

        Answer:

        D. Random sampling of accounts is the recommended best practice if all accounts cannot be validated. Selecting only recently changed accounts will not identify long-term issues or historic issues, and checking only high-value accounts will not show if there are issues or bad practices with other account types.
331.    Which one of the following security testing programs is designed to attract the participation of external testers and incentivize them to uncover security flaws?

        1. Penetration test
        2. Internal vulnerability scan
        3. Bug bounty
        4. External vulnerability scan

        Answer:

        C. Bug bounty programs are specifically designed to solicit bug reports from external security testers. Vulnerability scans (whether internal or external) and penetration tests are run by, or on behalf of, an organization's own security team.
332.    Frank's team is testing a new API that his company's developers have built for their application infrastructure. Which of the following is not a common API issue that you would expect Frank's team to find?

        1. Improper encryption
        2. Object level authorization issues
        3. User authentication issues
        4. Lack of rate limiting

        Answer:

        A. APIs typically transfer data for web application via HTTPS, meaning that the API itself is not responsible for encryption. If Frank's team discovers that TLS is not enabled, they will need to work with the infrastructure or systems administration team to ensure that TLS is enabled and in use rather than making API changes. Authorization for object access, authentication weaknesses, and rate limiting are all common API issues. If you're not familiar with the types of issues you might encounter in APIs, you can read more about them in the OWASP API security top 10 at `https://github.com/OWASP/API-Security/raw/master/2019/en/dist/owasp-api-security-top-10.pdf`.
333.    Ryan is considering the use of fuzz testing in his web application testing program. Which one of the following statements about fuzz testing is true?

        1. Fuzzers find only complex faults.
        2. Testers must manually generate input.
        3. Fuzzers may not fully cover the code.
        4. Fuzzers can't reproduce errors.

        Answer:

        C. Fuzz testers are capable of automatically generating input sequences to test an application. Therefore, testers do not need to manually generate input, although they may do so if they wish. Fuzzers can reproduce errors (and thus, “fuzzers can't reproduce errors” is not an issue) but typically don't fully cover the code—code coverage tools are usually paired with fuzzers to validate how much coverage was possible. Fuzzers are often limited to simple errors because they won't handle business logic or attacks that require knowledge from the application user.
