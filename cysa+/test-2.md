# Test 2

1.  Ty is reviewing the scan report for a Windows system joined to his organization's domain and finds the vulnerability shown here. What should be Ty's most significant concern related to this vulnerability?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf001.jpg)

    1. The presence of this vulnerability indicates that an attacker may have compromised his network.
    2. The presence of this vulnerability indicates a misconfiguration on the target server.
    3. The presence of this vulnerability indicates that the domain security policy may be lacking appropriate controls.
    4. The presence of this vulnerability indicates a critical flaw on the target server that must be addressed immediately.

    Answer:

    C. The presence of this vulnerability does indicate a misconfiguration on the targeted server, but that is not the most significant concern that Ty should have. Rather, he should be alarmed that the domain security policy does not prevent this configuration and should know that many other systems on the network may be affected. This vulnerability is not an indicator of an active compromise and does not rise to the level of a critical flaw.
2.  Heidi runs a vulnerability scan of the management interface of her organization's virtualization platform and finds the severity 1 vulnerability shown here. What circumstance, if present, should increase the severity level of this vulnerability to Heidi?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf002.jpg)

    1. Lack of encryption
    2. Missing security patch
    3. Exposure to external networks
    4. Out-of-date antivirus signatures

    Answer:

    C. This vulnerability has a low severity, but that could be dramatically increased if the management interface is exposed to external networks. If that were the case, it is possible that an attacker on a remote network would be able to eavesdrop on administrative connections and steal user credentials. Out-of-date antivirus definitions and missing security patches may also be severe vulnerabilities, but they do not increase the severity of this specific vulnerability. The lack of encryption is already known because of the nature of this vulnerability, so confirming that fact would not change the severity assessment.
3.  Rowan ran a port scan against a network switch located on her organization's internal network and discovered the results shown here. She ran the scan from her workstation on the employee VLAN. Which one of the following results should be of greatest concern to her?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf003.jpg)

    1. Port 22
    2. Port 23
    3. Port 80
    4. Ports 8192 to 8194

    Answer:

    B. Both ports 22 and 23 should be of concern to Rowan because they indicate that the network switch is accepting administrative connections from a general-use network. Instead, the switch should accept administrative connections only from a network management VLAN. Of these two results, port 23 should be of the greatest concern because it indicates that the switch is allowing unencrypted telnet connections that may be subject to eavesdropping. The results from ports 80 and 8192 to 8194 are of lesser concern because they are being filtered by a firewall.
4.  Evan is troubleshooting a vulnerability scan issue on his network. He is conducting an external scan of a website located on the web server shown in the diagram. After checking the web server logs, he saw no sign of the scan requests. Which one of the following causes is the least likely issue for him to troubleshoot?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf004.jpg)

    1. The scans are being blocked by an intrusion prevention system.
    2. The scans are being blocked by a rule within the web server application.
    3. The scans are being blocked by a network firewall.
    4. The scans are being blocked by a host firewall.

    Answer:

    B. All of the scenarios described here could result in failed vulnerability scans and are plausible on this network. However, the fact that the web server logs do not show any denied requests indicates that the issue is not with the web server application itself. If this were the case, Evan would see evidence of it in the web server logs.
5.  Sam is looking for evidence of software that was installed on a Windows system. He believes that the programs were deleted and that the suspect used both registry and log cleaners to hide evidence. What Windows feature can't he use to find evidence of the use of these programs?

    1. The MFT
    2. Volume shadow copies
    3. The shim (application compatibility) cache
    4. Prefetch files

    Answer:

    C. The shim cache is used by Windows to track scripts and programs that need specialized compatibility settings. It is stored in the registry at shutdown, which means that a thorough registry cleanup will remove program references from it. The master file table (MFT), volume shadow copies, and prefetch files can all contain evidence of deleted applications.
6.  Mila is evaluating the security of an application developed within her organization. She would like to assess the application's security by supplying it with invalid inputs. What technique is Mila planning to use?

    1. Fault injection
    2. Stress testing
    3. Mutation testing
    4. Fuzz testing

    Answer:

    D. Fuzz testing involves sending invalid or random data to an application to test its ability to handle unexpected data. Fault injection directly inserts faults into error-handling paths, particularly error-handling mechanisms that are rarely used or might otherwise be missed during normal testing. Mutation testing is related to fuzzing and fault injection, but rather than changing the inputs to the program or introducing faults to it, mutation testing makes small modifications to the program itself. Stress testing is a performance test that ensures applications and the systems that support them can stand up to the full production load.
7.  A port scan conducted during a security assessment shows the following results. What type of device has most likely been scanned?

    `Nmap scan report for EXAMPLE (192.168.1.79) Host is up (1.00s latency). Not shown: 992 closed ports PORT STATE 21/tcp open 23/tcp open 80/tcp open 280/tcp open 443/tcp open 515/tcp open 631/tcp open 9100/tcp open Nmap done: 1 IP address (1 host up) scanned in 124.20 seconds`

    1. A wireless access point
    2. A server
    3. A printer
    4. A switch

    Answer:

    C. Although TCP ports 21, 23, 80, and 443 are all common ports, 515 and 9100 are commonly associated with printers.
8.  Which of the following is _not_ one of the major categories of security event indicators described by NIST 800-61?

    1. Alerts from IDS, IPS, SIEM, AV, and other security systems
    2. Logs generated by systems, services, and applications
    3. Exploit developers
    4. Internal and external sources

    Answer:

    C. NIST identifies four major categories of security event indicators: alerts, logs, publicly available information, and people both inside and outside the organization. Exploiting developers may provide some information but is not a primary source of security event information.
9.  During an `nmap` scan of a network, Charles receives the following response from `nmap`:

    `Starting Nmap 7.80 ( https://nmap.org ) Nmap done: 256 IP addresses (0 hosts up) scanned in 29.74 seconds`

    What can Charles deduce about the network segment from these results?

    1. There are no active hosts in the network segment.
    2. All hosts on the network segment are firewalled.
    3. The scan was misconfigured.
    4. Charles cannot determine if there are hosts on the network segment from this scan.

    Answer:

    D. A host that is not running any services or that has a firewall enabled that prevents responses can be invisible to `nmap`. Charles cannot determine whether there are hosts on this network segment and may want to use other means such as ARP queries, DHCP logs, and other network layer checks to determine whether there are systems on the network.
10. Oskar is designing a vulnerability management program for his company, a hosted service provider. He would like to check all relevant documents for customer requirements that may affect his scanning. Which one of the following documents is _least_ likely to contain this information?

    1. BPA
    2. SLA
    3. MOU
    4. BIA

    Answer:

    D. The business impact assessment (BIA) is an internal document used to identify and assess risks. It is unlikely to contain customer requirements. Service level agreements (SLAs), business partner agreements (BPAs), and memorandums of understanding (MOUs) are much more likely to contain this information.
11. During a port scan of a server, Gwen discovered that the following ports are open on the internal network:

    TCP port 25.

    TCP port 80.

    TCP port 110.

    TCP port 443.

    TCP port 1521.

    TCP port 3389.

    Of the services listed here, for which one does the scan _not_ provide evidence that it is likely running on the server?

    1. Web
    2. Database
    3. SSH
    4. Email

    Answer:

    C. Web servers commonly run on ports 80 (for HTTP) and 443 (for HTTPS). Database servers commonly run on ports 1433 (for Microsoft SQL Server), 1521 (for Oracle), or 3306 (for MySQL). Remote Desktop Protocol services commonly run on port 3389. Simple Mail Transfer Protocol (SMTP) runs on port 25. There is no evidence that SSH, which uses port 22, is running on this server.
12. As part of her forensic analysis of a wiped thumb drive, Selah runs Scalpel to carve data from the image she created. After running Scalpel, she sees the following in the `audit.log` file created by the program. What should Selah do next?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf005.jpg)

    1. Run a data recovery program on the drive to retrieve the files.
    2. Run Scalpel in filename recovery mode to retrieve the actual filenames and directory structures of the files.
    3. Review the contents of the `scalpelout` folder.
    4. Use the identified filenames to process the file using a full forensic suite.

    Answer:

    C. You may not be familiar with Scalpel or other programs you encounter on the exam. In many cases, the problem itself will provide clues that can help you narrow down your answer. Here, pay close attention to the command-line flags, and note the `-o` flag, a common way to denote an output file. In practice, Scalpel automatically creates directories for each of the file types that it finds. Selah simply needs to visit those directories to review the files that she has recovered. She does not need to use another program. The filenames and directory structures may not be recoverable when carving files.
13. Lonnie ran a vulnerability scan of a server that he recently detected in his organization that is not listed in the organization's configuration management database. One of the vulnerabilities detected is shown here. What type of service is most likely running on this server?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf006.jpg)

    1. Database
    2. Web
    3. Time
    4. Network management

    Answer:

    B. The PHP language is used for the development of dynamic web applications. The presence of PHP on this server indicates that it is a web server. It may also be running database, time, or network management services, but the scan results provide no evidence of this.
14. Jorge would like to use a standardized system for evaluating the severity of security vulnerabilities. What SCAP component offers this capability?

    1. CPE
    2. CVE
    3. CVSS
    4. CCE

    Answer:

    C. The Common Vulnerability Scoring System (CVSS) provides a standardized method for rating the severity of security vulnerabilities.
15. When performing threat-hunting activities, what are cybersecurity analysts most directly seeking?

    1. Vulnerabilities
    2. Indicators of compromise
    3. Misconfigurations
    4. Unpatched systems

    Answer:

    B. The defining characteristic of threat hunting is that you are searching out compromises that have already occurred. Therefore, you are looking for indicators of compromise (IoCs). Vulnerabilities, unpatched systems, and misconfigurations are all things that vulnerability management activities, rather than threat-hunting activities, would seek to identify.
16. Taylor is preparing to run vulnerability scans of a web application server that his organization recently deployed for public access. He would like to understand what information is available to a potential external attacker about the system as well as what damage an attacker might be able to cause on the system. Which one of the following scan types would be least likely to provide this type of information?

    1. Internal network vulnerability scan
    2. Port scan
    3. Web application vulnerability scan
    4. External network vulnerability scan

    Answer:

    A. An internal network vulnerability scan will provide an insider's perspective on the server's vulnerabilities. It may provide useful information, but it will not meet Taylor's goal of determining what an external attacker would see.
17. While analyzing a packet capture in Wireshark, Chris finds the packet shown here. Which of the following is he unable to determine from this packet?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf007.jpg)

    1. That the username used was `gnome`
    2. That the protocol used was FTP
    3. That the password was `gnome123`
    4. That the remote system was 137.30.120.40

    Answer:

    A. FTP sends the username in a separate packet. Chris can determine that this was an FTP connection, that the password was `gnome123`, and that the FTP server was 137.30.120.40.
18. Cynthia's review of her network traffic focuses on the graph shown here. What occurred in late June?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf008.jpg)

    1. Beaconing
    2. High network bandwidth consumption
    3. A denial-of-service attack
    4. A link failure

    Answer:

    B. The spike shown just before July appears to be out of the norm for this network since it is almost four times higher than normal. Cynthia may want to check to see what occurred during that time frame to verify whether it was normal traffic for her organization.
19. Carlos arrived at the office this morning to find a subpoena on his desk requesting electronic records in his control. What type of procedure should he consult to determine appropriate next steps, including the people he should consult and the technical process he should follow?

    1. Evidence production procedure
    2. Monitoring procedure
    3. Data classification procedure
    4. Patching procedure

    Answer:

    A. Evidence production procedures describe how the organization will respond to subpoenas, court orders, and other legitimate requests to produce digital evidence. Monitoring procedures describe how the organization will perform security monitoring activities, including the possible use of continuous monitoring technology. Data classification procedures describe the processes to follow when implementing the organization's data classification policy. Patching procedures describe the frequency and process of applying patches to applications and systems under the organization's care.
20. Which stage of the incident response process includes activities such as adding IPS signatures to detect new attacks?

    1. Detection and analysis
    2. Containment, eradication, and recovery
    3. Postincident activity
    4. Preparation

    Answer:

    D. Adding new signatures (prior to an incident) is part of the preparation phase because it prepares an organization to detect attacks.
21. Gloria is configuring vulnerability scans for a new web server in her organization. The server is located on the screened subnet (DMZ) network, as shown here. What type of scans should Gloria configure for best results?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf009.jpg)

    1. Gloria should not scan servers located in the screened subnet (DMZ).
    2. Gloria should perform only internal scans of the server.
    3. Gloria should perform only external scans of the server.
    4. Gloria should perform both internal and external scans of the server.

    Answer:

    D. For best results, Gloria should combine both internal and external vulnerability scans because this server has both public and private IP addresses. The external scan provides an “attacker's eye view” of the web server, while the internal scan may uncover vulnerabilities that would be exploitable only by an insider or an attacker who has gained access to another system on the network.
22. Pranab is preparing to reuse media that contained data that his organization classifies as having “moderate” value. If he wants to follow NIST SP 800-88's guidelines, what should he do to the media if the media will not leave his organization's control?

    1. Reformat it
    2. Clear it
    3. Purge it
    4. Destroy it

    Answer:

    B. NIST SP 800-88 recommends clearing media and then validating and documenting that it was cleared. Clearing uses logical techniques to sanitize data in user-addressable storage locations and protects against noninvasive data recovery techniques. This level of security is appropriate to moderately sensitive data contained on media that will remain in an organization.
23. Susan is building an incident response program and intends to implement NIST's recommended actions to improve the effectiveness of incident analysis. Which of the following items is _not_ an NIST-recommended incident analysis improvement?

    1. Perform behavioral baselining.
    2. Create and implement a logging policy.
    3. Set system BIOS/UEFI clocks regularly.
    4. Maintain an organizationwide system configuration database.

    Answer:

    C. NIST recommends the usage of NTP to synchronize clocks throughout organizational infrastructure, thus allowing logs, alerts, and other data to be analyzed more easily during incident response. Manually setting clocks results in time skew, incorrect clocks, and other time-related problems.
24. Jim's nmap port scan of a remote system showed the following list of ports:

    `PORT STATE SERVICE 80/tcp open http 135/tcp open msrpc 139/tcp open netbios-ssn 445/tcp open microsoft-ds 902/tcp open iss-realsecure 912/tcp open apex-mesh 3389/tcp open ms-wbt-server`

    What operating system is the remote system most likely running?

    1. Windows
    2. Linux
    3. An embedded OS
    4. macOS

    Answer:

    A. TCP 135, 139, and 445 are all common Windows ports. The addition of 3389, the remote desktop port for Windows, makes it most likely that this is a Windows server.
25. Helen is seeking to protect her organization against attacks that involve the theft of user credentials. In most organizations, which one of the following threats poses the greatest risk of credential theft?

    1. DNS poisoning
    2. Phishing
    3. Telephone-based social engineering
    4. Shoulder surfing

    Answer:

    B. Although all the techniques listed may be used to engage in credential theft, phishing is, by far, the most common way that user accounts become compromised in most organizations.
26. As part of her duties as a security operations center (SOC) analyst, Emily is tasked with monitoring intrusion detection sensors that cover her employer's corporate headquarters network. During her shift, Emily's IDS reports that a network scan has occurred from a system with IP address 10.1. 1.19 on the organization's unauthenticated guest wireless network aimed at systems on an external network. What should Emily's first step be?

    1. Report the event to the impacted third parties.
    2. Report the event to law enforcement.
    3. Check the system's MAC address against known assets.
    4. Check authentication logs to identify the logged-in user.

    Answer:

    C. In most organizations, Emily's first action should be to verify that the system is not one that belongs to the organization by checking it against her organization's asset inventory. If the system is a compromised system on the wrong network, she or her team will need to address it. In most jurisdictions, there is no requirement to notify third parties or law enforcement of outbound scans, and since the guest wireless is specifically noted as being unauthenticated, there will not be authentication logs to check.
27. Sai works in an environment that is subject to the Payment Card Industry Data Security Standard (PCI DSS). He realizes that technical constraints prevent the organization from meeting a specific PCI DSS requirement and wants to implement a compensating control. Which one of the following statements is _not_ true about proper compensating controls?

    1. The control must include a clear audit mechanism.
    2. The control must meet the intent and rigor of the original requirement.
    3. The control must provide a similar level of defense as the original requirement provides.
    4. The control must be above and beyond other requirements.

    Answer:

    A. The PCI DSS compensating control procedures do not require that compensating controls have a clearly defined audit mechanism, although this is good security practice. They do require that the control meet the intent and rigor of the original requirement, provide a similar level of defense as the original requirement, and be above and beyond other requirements.
28. Lou recently scanned a web server in his environment and received the vulnerability report shown here. What action can Lou take to address this vulnerability?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf010.jpg)

    1. Configure TLS.
    2. Replace the certificate.
    3. Unblock port 443.
    4. Block port 80.

    Answer:

    B. This error indicates that the digital certificate presented by the server is not valid. Lou should replace the certificate with a certificate from a trusted certificate authority (CA) to correct the issue.
29. Which of the following factors is _not_ typically considered when determining whether evidence should be retained?

    1. Media life span
    2. Likelihood of civil litigation
    3. Organizational retention policies
    4. Likelihood of criminal prosecution

    Answer:

    A. Incident data should be retained as necessary regardless of media life span. Retention is often driven by the likelihood of civil or criminal action, as well as by organizational standards.
30. Match each of the following with the appropriate element of the CIA triad:

    1. A hard drive failure resulting in a service outage
    2. A termination letter that is left on a printer and read by others in the department
    3. Modification of an email's content by a third party
    4. 1\. Integrity, 2. Confidentiality, 3. Confidentiality
    5. 1\. Integrity, 2. Confidentiality, 3. Availability
    6. 1\. Availability, 2. Availability, 3. Confidentiality
    7. 1\. Availability, 2. Confidentiality, 3. Integrity

    Answer:

    D. An outage is an availability issue, data exposures are confidentiality issues, and the integrity of the email was compromised when it was changed.
31. Niesha discovered the vulnerability shown here on a server running in her organization. What would be the best way for Niesha to resolve this issue?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf011.jpg)

    1. Disable the use of AES-GCM.
    2. Upgrade OpenSSH.
    3. Upgrade the operating system.
    4. Update antivirus signatures.

    Answer:

    B. The best way to resolve this issue would be to upgrade OpenSSH, as stated in the solution section of the report. Disabling the use of AES-GCM is an acceptable workaround, but upgrading to a more current version of OpenSSH is likely to address additional security issues not described in this particular vulnerability report. There is no indication that an operating system upgrade would correct the problem. The vulnerability report states that there is no malware associated with this vulnerability, so antivirus signature updates would not correct it.
32. As part of her postincident recovery process, Alicia creates a separate virtual network as shown here to contain compromised systems she needs to investigate. What containment technique is she using?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf012.jpg)

    1. Segmentation
    2. Isolation
    3. Removal
    4. Reverse engineering

    Answer:

    A. The firewall rules continue to allow access to the compromised systems, while preventing them from attacking other systems. This is an example of segmentation. Segmentation via VLANs, firewall rules, or other logical methods can help to protect other systems, while allowing continued live analysis.
33. Jennifer is reviewing her network monitoring configurations and sees the following chart for a system she runs remotely in Amazon's Web Services (AWS) environment more than 400 miles away. What can she use this data for?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf013.jpg)

    1. Incident response; she needs to determine the issue causing the spikes in response time.
    2. The high packet loss must be investigated, since it may indicate a denial-of-service attack.
    3. She can use this data to determine a reasonable response time baseline.
    4. The high response time must be investigated, since it may indicate a denial-of-service attack.

    Answer:

    C. Jennifer can use this information to help build her baseline for response times for the AWS server. A 200 ms response time for a remotely hosted server is well within a reasonable range. There is nothing in this chart that indicates an issue.
34. The Windows system that Abdul is conducting live forensics on shows a partition map, as shown here. If Abdul believes that a hidden partition was deleted resulting in the unallocated space, which of the following type of tool is best suited to identifying the data found in the unallocated space?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf014.jpg)

    1. File carving
    2. Wiping
    3. Partitioning
    4. Disk duplication

    Answer:

    A. A file carving tool, such as Scalpel, is designed to identify files in a partition or volume that is missing its index or file allocation table. A wiping tool is used to completely remove data from a disk. Partitioning tools are used to modify the volume structure of a disk. Disk duplication tools are used to create forensic images, among other purposes.
35. During a postmortem forensic analysis of a Windows system that was shut down after its user saw strange behavior, Pranab concludes that the system he is reviewing was likely infected with a memory-resident malware package. What is his best means of finding the malware?

    1. Search for a core dump or hibernation file to analyze.
    2. Review the INDX files and Windows registry for signs of infection.
    3. Boot the system and then use a tool like the Volatility Framework to capture live memory.
    4. Check volume shadow copies for historic information prior to the reboot.

    Answer:

    A. Pranab's best option is to look for a hibernation file or core dump that may contain evidence of the memory-resident malware. Once a system has been shut down, a memory-resident malware package will be gone until the system is re-infected, making reviews of the registry, INDX files, and volume shadow copies unlikely to be useful. Since the system was shut down, he won't get useful memory forensics from a tool like the Volatility Framework unless the machine is re-infected.
36. Juliette's organization recently suffered a cross-site scripting attack, and she plans to implement input validation to protect against the recurrence of such attacks in the future. Which one of the following HTML tags should be most carefully scrutinized when it appears in user input?

    1. `<SCRIPT>`
    2. `<XSS>`
    3. `<B>`
    4. `<EM>`

    Answer:

    A. The `<SCRIPT>` tag is used to mark the beginning of a code element, and its use is indicative of a cross-site scripting attack. `<XSS>` is not a valid HTML tag. The `<B>` (for bold text) and `<EM>` (for emphasis) tags are commonly found in normal HTML input.
37. Jessie needs to prevent port scans like the scan shown here. Which of the following is a valid method for preventing port scans?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf015.jpg)

    1. Not registering systems in DNS
    2. Using a firewall to restrict traffic to only ports required for business purposes
    3. Using a heuristic detection rule on an IPS
    4. Implementing port security

    Answer:

    C. An intrusion prevention system (or other device or software with similar capabilities) to block port scans based on behavior is the most effective method listed. Not registering systems in DNS won't stop IP-based scans, and port scans will still succeed on the ports that firewalls allow through. Port security is a network switch–based technology designed to limit which systems can use a physical network port.
38. What information can be gathered by observing the distinct default values of the following TCP/IP fields during reconnaissance activities: initial packet size, initial TTL, window size, maximum segment size, and flags?

    1. The target system's TCP version.
    2. The target system's operating system.
    3. The target system's MAC address.
    4. These fields are useful only for packet analysis.

    Answer:

    B. Operating system fingerprinting relies on the differences between how each operating system (and sometimes OS versions) handles and sets various TCP/IP fields, including initial packet size, initial TTL, window size, maximum segment size, and the `don't fragment`, `SACK OK`, and `nop options`.
39. Brooke would like to find a technology platform that automates workflows across a variety of security tools, including the automated response to security incidents. What category of tool best meets this need?

    1. SIEM
    2. NIPS
    3. SOAR
    4. DLP

    Answer:

    C. Although any of these tools may provide some security automation capability, the purpose of a security orchestration, automation, and response (SOAR) platform is to perform this type of automation across other solutions.
40. Miray needs to identify the device or storage type that has the lowest order of volatility. Which of the following is the least volatile?

    1. Network traffic
    2. A solid-state drive
    3. A spinning hard drive
    4. A DVD-ROM

    Answer:

    D. The order of volatility of common storage locations is as follows:

    1. CPU cache, registers, running processes, and RAM
    2. Network traffic
    3. Disk drives (both spinning and magnetic)
    4. Backups, printouts, and optical media (including DVD-ROMs and CDs)

    Thus, the least volatile storage listed is the DVD-ROM.
41. After receiving complaints about a system on Anastasia's network not performing correctly, she decides to investigate the issue by capturing traffic with Wireshark. The captured traffic is shown here. What type of issue is Anastasia most likely seeing?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf016.jpg)

    1. A link failure
    2. A failed three-way handshake
    3. A DDoS
    4. A SYN flood

    Answer:

    D. The repeated SYN packets are likely a SYN flood that attempts to use up resources on the target system. A failed three-way handshake might initially appear similar but will typically not show this volume of attempts. A link failure would not show traffic from a remote system, and a DDoS would involve more than one system sending traffic.
42. After finishing a forensic case, Lucas needs to wipe the media that he is using to prepare it for the next case. Which of the following methods is best suited to preparing the SSD that he will use?

    1. Degauss the drive.
    2. Zero-write the drive.
    3. Use a PRNG.
    4. Use the ATA Secure Erase command.

    Answer:

    D. The ATA Secure Erase command wipes all of an SSD, including host-protected area partitions and remapped spare blocks. Degaussing is used for magnetic media such as tapes and is not effective on SSDs, whereas zero writing or using a pseudorandom number generator to fill the drive will not overwrite data in the host-protected area or spare blocks, which are used to wear-level most SSDs.
43. Luis is creating a vulnerability management program for his company. He only has the resources to conduct daily scans of approximately 10 percent of his systems, and the rest will be scheduled for weekly scans. He would like to ensure that the systems containing the most sensitive information receive scans on a more frequent basis. What criterion is Luis using?

    1. Data privacy
    2. Data remanence
    3. Data retention
    4. Data classification

    Answer:

    D. Data classification is a set of labels applied to information based upon their degree of sensitivity and/or criticality. It would be the most appropriate choice in this scenario. Data retention requirements dictate the length of time that an organization should maintain copies of records. Data remanence is an issue where information thought to be deleted may still exist on systems. Data privacy may contribute to data classification but does not encompass the entire field of data sensitivity and criticality in the same manner as data classification. For example, a system may process proprietary business information that would be very highly classified and require frequent vulnerability scanning. Unless that system also processed personally identifiable information, it would not trigger scans under a system based solely upon data privacy.
44. Peter is designing a vulnerability scanning program for the large chain of retail stores where he works. The store operates point-of-sale terminals in its retail stores as well as an e-commerce website. Which one of the following statements about PCI DSS compliance is _not_ true?

    1. Peter's company must hire an approved scanning vendor to perform vulnerability scans.
    2. The scanning program must include, at a minimum, weekly scans of the internal network.
    3. The point-of-sale terminals and website both require vulnerability scans.
    4. Peter may perform some required vulnerability scans on his own.

    Answer:

    B. PCI DSS requires scanning on at least a quarterly basis and after any significant changes. Weekly scanning is a best practice but is not required by the standard. Peter must hire an approved scanning vendor to perform the required quarterly external scans but may conduct the internal scans himself. All systems in the cardholder data environment, including both the website and point-of-sale terminals, must be scanned.
45. Rachel discovered the vulnerability shown here when scanning a web server in her organization. Which one of the following approaches would best resolve this issue?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf017.jpg)

    1. Patching the server
    2. Performing input validation
    3. Adjusting firewall rules
    4. Rewriting the application code

    Answer:

    A. The vulnerability description mentions that this is a cross-site scripting (XSS) vulnerability. Normally, XSS vulnerabilities are resolved by performing proper input validation in the web application code. However, in this particular case, the XSS vulnerability exists within Microsoft IIS server itself and not in a web application. Therefore, it requires a patch from Microsoft to correct it.
46. What `nmap` feature is enabled with the `-O` flag?

    1. OS detection
    2. Online/offline detection
    3. Origami attack detection
    4. Origination port validation

    Answer:

    A. The `-O` flag enables operating system detection for `nmap`.
47. Jose is working with his manager to implement a vulnerability management program for his company. His manager tells him that he should focus on remediating critical and high-severity risks to externally accessible systems. He also tells Jose that the organization does not want to address risks on systems without any external exposure or risks rated medium or lower. Jose disagrees with this approach and believes that he should also address critical and high-severity risks on internal systems. How should he handle the situation?

    1. Jose should recognize that his manager has made a decision based upon the organization's risk appetite and should accept it and carry out his manager's request.
    2. Jose should discuss his opinion with his manager and request that the remediation criteria be changed.
    3. Jose should ask his manager's supervisor for a meeting to discuss his concerns about the manager's approach.
    4. Jose should carry out the remediation program in the manner that he feels is appropriate because it will address all of the risks identified by the manager as well as additional risks.

    Answer:

    B. The most appropriate step for Jose to take is to discuss his opinion with his manager and see whether the manager is willing to change the guidelines. As a security professional, it is Jose's ethical responsibility to share his opinion with his manager. It would not be appropriate for Jose to act against his manager's wishes. Jose should also not ask to speak with his manager's supervisor until he has had an opportunity to discuss the issue thoroughly with his manager.
48. Susan needs to test thousands of submitted binaries. She needs to ensure that the applications do not contain malicious code. What technique is best suited to this need?

    1. Sandboxing
    2. Implementing a honeypot
    3. Decompiling and analyzing the application code
    4. Fagan testing

    Answer:

    A. Susan's best option is to use an automated testing sandbox that analyzes the applications for malicious or questionable behavior. While this may not catch every instance of malicious software, the only other viable option is decompiling the applications and analyzing the code, which would be incredibly time-consuming. Since she doesn't have the source code, Fagan inspection won't work (and would take a long time too), and running a honeypot is used to understand hacker techniques, not to directly analyze application code.
49. When conducting a quantitative risk assessment, what term describes the total amount of damage expected to occur as a result of one incident?

    1. EF
    2. SLE
    3. AV
    4. ALE

    Answer:

    B. The single loss expectancy (SLE) is the amount of damage expected from a single occurrence of an incident. The annualized loss expectancy (ALE) is the amount of loss expected from a risk during a given year. The exposure factor (EF) is the percentage of an asset that is expected to be damaged during an incident, and the asset value (AV) is the total value of the asset in question.
50. Rhonda recently configured new vulnerability scans for her organization's datacenter. Completing the scans according to current specifications requires that they run all day, every day. After the first day of scanning, Rhonda received complaints from administrators of network congestion during peak business hours. How should Rhonda handle this situation?

    1. Adjust the scanning frequency to avoid scanning during peak times.
    2. Request that network administrators increase available bandwidth to accommodate scanning.
    3. Inform the administrators of the importance of scanning and ask them to adjust the business requirements.
    4. Ignore the request because it does not meet security objectives.

    Answer:

    A. The most reasonable response is for Rhonda to adjust the scanning parameters to avoid conflicts with peak business periods. She could ask for additional network bandwidth, but this is likely an unnecessary expense. Adjusting the business requirements is not a reasonable response, as security objectives should be designed to add security in a way that allows the business to operate efficiently, not the other way around. Ignoring the request would be very harmful to the business relationship.
51. After restoring a system from 30-day-old backups after a compromise, administrators at Piper's company return the system to service. Shortly after that, Piper detects similar signs of compromise again. Why is restoring a system from a backup problematic in many cases?

    1. Backups cannot be tested for security issues.
    2. Restoring from backup may reintroduce the original vulnerability.
    3. Backups are performed with the firewall off and are insecure after restoration.
    4. Backups cannot be properly secured.

    Answer:

    B. When restoring from a backup after a compromise, it is important to ensure that the flaw that allowed attackers in is patched or otherwise remediated. In many environments, backups can be restored to a protected location where they can be patched, validated, and tested before they are restored to service.
52. Captured network traffic from a compromised system shows it reaching out to a series of five remote IP addresses that change on a regular basis. Since the system is believed to be compromised, the system's Internet access is blocked, and the system is isolated to a quarantine VLAN.

    When forensic investigators review the system, no evidence of malware is found. Which of the following scenarios is most likely?

    1. The system was not infected, and the detection was a false positive.
    2. The beaconing behavior was part of a web bug.
    3. The beaconing behavior was due to a misconfigured application.
    4. The malware removed itself after losing network connectivity.

    Answer:

    D. Recurring beaconing behavior with a changing set of systems is a common characteristic of more advanced malware packages. It is most likely that this system was compromised with malware that deleted itself when its ability to check in with a command-and-control (C2) system was removed, thus preventing the malware from being captured and analyzed by incident responders.
53. Which one of the following ISO standards provides guidance on the development and implementation of information security management systems?

    1. ISO 27001
    2. ISO 9000
    3. ISO 11120
    4. ISO 23270

    Answer:

    A. ISO 27001 provides guidance on information security management systems. ISO 9000 applies to quality management. ISO 11120 applies to gas cylinders. ISO 23270 applies to programming languages.
54. Mika's forensic examination of a compromised Linux system is focused on determining what level of access attackers may have achieved using a compromised `www` account. Which of the following is _not_ useful if she wants to check for elevated privileges associated with the `www` user?

    1. `/etc/passwd`
    2. `/etc/shadow`
    3. `/etc/sudoers`
    4. `/etc/group`

    Answer:

    B. `/etc/shadow` contains password hashes but does not provide information about privileges. Unlike `/etc/passwd`, it does not contain user ID or group ID information and instead contains only the username and hashed password.

    The `/etc/sudoers` file contains a list of users who may use the `sudo` command. The `/etc/group` file contains the membership listing for system groups.
55. Tracy is validating the web application security controls used by her organization. She wants to ensure that the organization is prepared to conduct forensic investigations of future security incidents. Which one of the following OWASP control categories is most likely to contribute to this effort?

    1. Implement logging.
    2. Validate all inputs.
    3. Parameterize queries.
    4. Error and exception handling.

    Answer:

    A. Logging of application and server activity may provide valuable evidence during a forensic investigation. The other three controls listed are proactive controls designed to reduce the risk of an incident occurring and are less likely to directly provide information during a forensic investigation.
56. Jamal is using agent-based scanning to assess the security of his environment. Every time that Jamal runs a vulnerability scan against a particular system, it causes the system to hang. He spoke with the system administrator, who provided him with a report showing that the system is current with patches and has a properly configured firewall that allows access from only a small set of trusted internal servers. Jamal and the server administrator both consulted the vendor, and they are unable to determine the cause of the crashes and suspect that it may be a side effect of the agent. What would be Jamal's most appropriate course of action?

    1. Approve an exception for this server.
    2. Continue scanning the server each day.
    3. Require that the issue be corrected in 14 days and then resume scanning.
    4. Decommission the server.

    Answer:

    A. This is an appropriate case for an exception to the scanning policy. The server appears to be secure, and the scanning itself is causing a production issue. Jamal should continue to monitor the situation and consider alternative forms of scanning, but it would not be appropriate to continue the scanning or set an artificial deadline that is highly unlikely to be met. Decommissioning the server is an excessive action as there is no indication that it is insecure, and the issue may, in fact, be a problem with the scanner itself.
57. During an `nmap` port scan using the `-sV` flag to determine service versions, Ling discovers that the version of SSH on the Linux system she is scanning is not up-to-date. When she asks the system administrators, they inform her that the system is fully patched and that the SSH version is current. What issue is Ling most likely experiencing?

    1. The system administrators are incorrect.
    2. The `nmap` version identification is using the banner to determine the service version.
    3. `nmap` does not provide service version information, so Ling cannot determine version levels in this way.
    4. The systems have not been rebooted since they were patched.

    Answer:

    B. Although `nmap` provides service version identification, it relies heavily on the information that the services provide. In some cases, fully patched services may provide banner information that does not show the minor version or may not change banners after a patch, leading to incorrect version identification.
58. Tyler scans his organization's mail server for vulnerabilities and finds the result shown here. What should be his next step?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c06uf018.jpg)

    1. Shut down the server immediately.
    2. Initiate the change management process.
    3. Apply the patch.
    4. Rerun the scan.

    Answer:

    B. Tyler should initiate his organization's change management process to begin the patching process. This is a medium severity vulnerability, so there is no need to apply the patch in an emergency fashion that would bypass change management. Similarly, shutting down the server would cause a serious disruption, and the level of severity does not justify that. Finally, there is no need to rerun the scan because there is no indication that it is a false positive result.
59. Carla is performing a penetration test of a web application and would like to use a software package that allows her to modify requests being sent from her system to a remote web server. Which one of the following tools would _not_ meet Carla's needs?

    1. Nessus
    2. Burp Suite
    3. Zed Attack Proxy (ZAP)
    4. Tamper Data

    Answer:

    A. Carla is looking for a tool from a category known as interception proxies. They run on the tester's system and intercept requests being sent from the web browser to the web server before they are released onto the network. This allows the tester to manually manipulate the request to attempt the injection of an attack. Burp Suite, ZAP, and Tamper Data are all examples of interception proxies. Nessus is a vulnerability scanner and, while useful in penetration testing, does not serve as an interception proxy.
60. Alex learns that a recent Microsoft patch covers a zero-day exploit in Microsoft Office that occurs because of incorrect memory handling. The flaw is described as potentially resulting in memory corruption and arbitrary code execution in the context of the current privilege level. Exploitation of the flaws can occur if victims open a specifically crafted Office document in a vulnerable version of Microsoft Office.

    If Alex finds out that approximately 15 of the workstations in his organization have been compromised by this malware, including one workstation belonging to a domain administrator, what phase of the incident response process should he enter next?

    1. Preparation
    2. Detection and analysis
    3. Containment, eradication, and recovery
    4. Postincident activity

    Answer:

    C. Alex needs to quickly move into containment mode by limiting the impact of the compromise. He can then gather the evidence and data needed to support the incident response effort, allowing him to work with his organization's desktop and IT support teams to return the organization to normal function.
61. Maria wants to use a security benchmark that is widely used throughout the industry to baseline her systems as part of a hardening process. Which of the following organizations provides a set of freely available benchmarks for operating systems?

    1. The Center for Internet Security
    2. CompTIA
    3. PCI SSC
    4. OWASP

    Answer:

    A. The Center for Internet Security (CIS) provides a range of free security baselines for Windows, Linux, macOS, and applications and services of many types. CompTIA, the Payment Card Industry Security Standards Council (PCI SSC), and the Open Worldwide Application Security Project (OWASP) do not.
62. Sally's organization wants to prioritize their vulnerability remediation efforts. Which of the following items is not typically critical to prioritization of remediation efforts?

    1. A list of affected hosts
    2. The risk score of the vulnerability
    3. The vulnerability's name or CVE
    4. The organization or individual that discovered the vulnerability

    Answer:

    D. Figuring out which vulnerabilities should receive attention first means that organizations need to understand the scope and impact of the vulnerability, both of which can be more easily determined with a risk score and a list of affected hosts. Knowing the vulnerability's name, or even better its CVE identifier, allows it to be researched. Who discovered it is not relevant to remediation prioritization.
63. Chris is reviewing network flow data from systems in his organization and notices that a number of the systems are contacting a remote IP address periodically through the day. He suspects the systems may be compromised. What type of behavior is he most likely seeing?

    1. Data exfiltration
    2. Port scans
    3. Beaconing
    4. Rogue devices

    Answer:

    C. Chris is most likely seeing beaconing behavior. Beaconing is periodic contact with a command-and-control (C2) server or servers to receive instructions and provide data about the current state of the compromised system. The question does not provide any information to indicate that data is being exfiltrated, port scans typically involve connections to a series of ports, and rogue devices are devices unexpectedly on a network, not potentially compromised organizationally owned devices like these.
64. What concern may drive organizations to communicate with customers impacted by a breach within a specific timeline?

    1. Regulatory compliance
    2. Media awareness
    3. Social media interaction
    4. Police involvement

    Answer:

    A. Regulations and laws may require customer notification in a timely manner or in a specific timeframe once an organization has information about the breach. This frequently drives disclosure. Contractual requirements, while not listed here, are the other primary driver of time-bound disclosures. Media, social media, and police involvement are not primary drivers to a specific timeline but may put pressure on an organization.
65. Yuri wants to check if an IP address is known to be malicious. Which of the following options is the most useful way for him to manually check current information about an IP address or hostname?

    1. The SANS Top 20
    2. AbuseIPDB
    3. WHOIS
    4. Cuckoo Sandbox

    Answer:

    B. The only service that provides reputational information from this list is the AbuseIPDB. The SANS Top 20 are a set of lists of critical controls, vulnerabilities, and other items. WHOIS is a lookup services allowing IP addresses and hostnames to be resolved, and Cuckoo Sandbox is an open-source sandbox tool.
66. Carla's organization is a managed security provider that uses the ITIL, and Carla wants to determine if her team is meeting the service level agreements her organization has agreed to meet for their customers for vulnerability management notifications happening within 24 hours. What is Carla attempting to assess?

    1. A VMO
    2. A SLO
    3. An NDA
    4. A VMS

    Answer:

    B. Carla is managing to a service level objective (SLO). SLOs are agreements that are found in service level agreements (SLAs) that specify a metric such as time to respond or expected uptime. An NDA is a nondisclosure agreement, VMS is a vulnerability management system, and VMO was made up for this question.
67. Joanna's organization has been performing a forensic investigation of a compromised system. Her team's analysis indicates that a number of commonly available tools were used by the attacker and that the attacker was using basic, rather than advanced skills and techniques. What type of threat actor is Joanna most likely dealing with?

    1. A hacktivist
    2. A nation-state actor
    3. A script kiddie
    4. Organized crime

    Answer:

    C. Script kiddies are unsophisticated attackers who use widely available tools without an in-depth understanding or skillset. All of the information that Joanna and her team have indicate they were attacked by a script kiddie. A nation-state actor or organized crime group are more likely to use advanced techniques or customized tools, while a hacktivist will typically have a specific political purpose for an attack that was not described here.
68. Michelle wants to provide metrics for her security team's incident response capabilities. Which of the following is not a common measure for teams like hers?

    1. Mean time to detect
    2. Mean time to respond
    3. Mean time to remediate
    4. Mean time to compromise

    Answer:

    D. Mean time to compromise is not a typical metric or key performance indicator for security teams. Mean time to detect, mean time to respond, and mean time to remediate are all common metrics for teams.
69. Tony is working with information from a closed-source threat feed and combines the feed information with his own organization's vulnerability management data and asset databases. What activity is Tony performing?

    1. IoC analysis
    2. Geolocation
    3. Active defense
    4. Data enrichment

    Answer:

    D. Tony is performing data enrichment by combining threat feeds with additional data to improve his ability to use contextual data from his own organization. IoC analysis would involve using indicators of compromise to identify potential compromises. There is no mention of geographic data for geolocation, and active defenses involve working actively to stop attackers by responding rather than simply combining information with threat feed data.
70. Which of the following is not a common inhibitor to remediation of vulnerabilities?

    1. Legacy systems
    2. Organizational policies
    3. The potential to degrade functionality
    4. Organizational governance processes

    Answer:

    B. Organizational policies are often used to drive remediation processes by defining set timelines for patching for based on risk and other factors. Common inhibitors to remediation include MOUs and SLAs, which may require specific performance or uptime; organizational governance processes that slow down actions; concerns about business process interruptions or degrading functionality, legacy, and proprietary systems.
71. Greg wants to assess the confidence levels for his threat intelligence data. What three common items are most frequently used to determine confidence in threat intelligence?

    1. Timeliness, source quality, and cost
    2. Accuracy, threat actor, and likelihood
    3. Timeliness, relevance, and accuracy
    4. Accuracy, source quality, and cost

    Answer:

    C. Greg knows that timeliness, relevance, and accuracy are the key factors typically used to assess threat intelligence confidence levels.
72. Valerie's incident response process includes moving a compromise system to a separate VLAN that retains access to the Internet but does not allow contact with other systems on her network. What containment process has she implemented?

    1. Segmentation
    2. IoC-based response
    3. Isolation
    4. Sanitization

    Answer:

    A. Valerie has segmented her network to prevent the compromise from spreading, but without fully isolating the system. This can be useful to prevent attackers from knowing that they have been detected. IoC-based response is not a common term, and sanitization is the process of wiping and rebuilding a system to prevent hidden or remnant threats.
73. Isaac wants to view network traffic from a potentially compromised Linux machine. What tool can he use from the command line to view and analyze his network traffic?

    1. Wireshark
    2. `tcpdump`
    3. Ettercap
    4. `cat /dev/eth0`

    Answer:

    B. The `tcpdump` tool is included in many Linux distributions by default and is a command-line tool that can capture network traffic. Isaac can use `tcpdump` to perform his analysis but may want to use Wireshark's graphical user interface if he wants to perform more detailed analysis. Ettercap is an on-path attack tool, and simply using the `cat` (concatenate) command on the Ethernet device won't work to display traffic.
74. Beena wants to ensure that her vulnerability management program is performing as expected. What technique should she use to look at its performance over time so she can see if she has problematic behaviors or practices?

    1. A regularly created list of the top 10 most common vulnerabilities
    2. A report showing remediation and patching trends
    3. A list of zero-day vulnerabilities and the time to remediate them
    4. A list of service level objectives

    Answer:

    B. Trends help to determine if there is a new or increasing problem with patching. Beena can review the trends to see if her organization's performance is stable, improving, or if issues are occurring. A list of the top 10 vulnerabilities does not provide this. A list of zero-day vulnerabilities and the time to remediate them does not help her assess performance, nor does a list of service level objectives without data about whether they were met and how often.
75. Valentine is reviewing network flow logs and sees a 30 GB data transfer between a database server and a system outside of her organization. For reviews, how should she flag the event?

    1. Potential data exfiltration
    2. Potential use of unauthorized privileges
    3. A potential malicious process
    4. Potential high drive capacity consumption

    Answer:

    A. Valentine knows that large data transfer from servers like a database server that should not typically send data to outside systems is likely to be data exfiltration. She should immediately flag the transfer for further investigation. There is no indication of the use of unauthorized privileges, but a malicious process may be found when she digs in further. There is also no indicator of drive capacity consumption.
76. Selah wants to use appropriate metrics to determine how well her incident response process is working. Which of the following metrics is not commonly used to assess incident response processes?

    1. Mean time to remediate
    2. Meant time to detect
    3. Mean time to respond
    4. Mean time to defend

    Answer:

    D. Mean time to detect, respond, and remediate are all commonly used measures. Use of active defenses is less common, and thus mean time to defend is not a commonly used measure; instead, time to respond in general is measured.
77. Gary wants to use NTP to help with his log analysis efforts. What is Gary doing?

    1. Setting appropriate logging levels
    2. Removing unnecessary logs using a trust process
    3. Time synchronization
    4. Validating log entries against the originals

    Answer:

    C. The Network Time Protocol (NTP) is used for time synchronization. This ensures logs have correct timestamps allowing correlation between logs from systems throughout an organization.
78. Nathan's organization has been notified that there is a vulnerability in a legacy system that does not have vendor support. Nathan needs to ensure that the system is not compromised due to the vulnerability. What should Nathan implement to address this issue?

    1. A patching plan
    2. A compensating control
    3. A remediation plan
    4. An alternate patch

    Answer:

    B. Nathan should document and deploy a compensating control. This may also require the vulnerability to be marked in the vulnerability management system to ensure that future detections are not flagged for noncompliance. A patching or remediation plan won't resolve the issue or protect the system, and alternative patches are not commonly available.
79. The endpoint detection and response (EDR) system that Li's organization uses has detected Windows workstations communicating between each other on the network on port 8944. What should Li flag this traffic as?

    1. Beaconing
    2. A port scan
    3. Unexpected bandwidth consumption
    4. Irregular peer-to-peer communication

    Answer:

    D. Li knows that port 8944 is not a commonly used Windows port for communication and that this could be a malicious process. She should flag it as irregular peer-to-peer communication and ensure that it is investigated.
80. What phase of incident response needs to happen before customer communications can occur?

    1. Perform stakeholder identification.
    2. Document lessons learned.
    3. Prepare a timeline.
    4. Conduct a root-cause analysis.

    Answer:

    A. Before communications occur with external parties such as customers, the stakeholders must be identified to ensure that communications go to the appropriate people or organizations. Since communications often happen during the investigation, having lessons learned, a timeline, or a root-cause analysis ready may not occur until after at least some customer communication has needed to happen.
81. Jake wants to ensure that only authorized IP addresses can send email on behalf of his organization but doesn't want to require certificates and signatures for the validation. What should he implement?

    1. DKIM
    2. DMARC
    3. S/MIME
    4. SPF

    Answer:

    D. The Sender Policy Framework (SPF) allows you to create a list of authorized IP addresses that can send emails on an organization's behalf. This is done by publishing and checking a SPF record maintained by the organization. DomainKeys Identified Mail (DKIM) uses public key cryptography and uses a private key to sign email headers. Domain-based Message Authentication, Reporting, and Conformance (DMARC) combines SPF and DKIM to validate senders and take actions based on a policy. S/MIME is a protocol for sending messages using digital signatures and encryption.
82. Katie has been reviewing her organization's vulnerability management reports and notices that systems that are part of a cloud-hosted cluster continue to show a recurring issue where vulnerabilities re-appear when the cluster is scaled up to handle higher loads. What is the most likely issue that Katie should ask the system administrators about?

    1. Reinstallation of the same software package instead of a patched version
    2. A lack of update to the original cluster image
    3. Patches failing to install
    4. A compromise restoring the system to a vulnerable state

    Answer:

    B. Since auto-scaling clusters often rely on an image for systems as they are instantiated, a base image that does not include the patch can result in exactly this scenario. This is why organizations often use infrastructure-as-code capabilities to allow patching and updates before a system is placed into production. Reinstalling the same software package is often a human error or a problem with scripting and less likely to be repeated. Patches failing to install would also likely be identified after the first this the issue was reported. A compromise is more likely to be allowed by a vulnerability than for a compromise to cause the system to display a new vulnerability.
83. What open source intelligence source is accessible only using a TOR enabled browser or system?

    1. Social media
    2. The Dark Web
    3. Blogs
    4. Government bulletins

    Answer:

    B. The Dark Web is accessible only via The Onion Router (TOR), which provides an alternative, typically unindexed Internet. Other valuable cybersecurity resources, such as social media sites, blogs, and government bulletins, are all available on the Internet and may be accessed using a standard web browser.
84. Bob's organization wants to adopt passwordless authentication. What will they need to provide to users to adopt this solution?

    1. PINs
    2. Biometric identifiers
    3. Hardware tokens
    4. New passwords

    Answer:

    C. Passwordless authentication requires either hardware tokens or authentication applications, typically deployed to mobile devices like phones. PINs are still a knowledge factor, new passwords would not be passwordless, and biometric identifiers are not provided to users; they are set up for users based on their biometric data.
85. Hillary is working on improving her organization's security response processes and wants to integrate security tools from multiple vendors together. What type of integration should she look for to optimize the ability for systems to work together and exchange data?

    1. FTP-based integration
    2. Data scraping from built-in web pages
    3. API-based integration
    4. A single pane of glass design

    Answer:

    C. When working with tools from multiple vendors, Hillary knows that having well-documented and available APIs can be one of the most effective ways to exchange data and information. FTP and data scraping are both slower and less reliable options. While a single pane of glass design is desirable, it doesn't enable data exchange.
