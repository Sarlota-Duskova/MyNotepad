# Test 1

1.  While reviewing network flow logs, John sees that network flow on a particular segment suddenly dropped to zero. What is the most likely cause of this?

    1. A denial-of-service attack
    2. A link failure
    3. High bandwidth consumption
    4. Beaconing

    Answer:

    B. The sudden drop to zero is most likely to be an example of link failure. A denial-of-service attack could result in this type of drop but is less likely for most organizations. High bandwidth consumption and beaconing both show different traffic patterns than shown in this example.
2.  Saanvi is conducting the recovery process after his organization experienced a security incident. During that process, he plans to apply patches to all of the systems in his environment. Which one of the following should be his highest priority for patching?

    1. Windows systems
    2. Systems involved in the incident
    3. Linux systems
    4. Web servers

    Answer:

    B. During an incident recovery effort, patching priority should be placed on systems that were directly involved in the incident. This is one component of remediating known issues that were actively exploited.
3.  Susan's organization suffered from a major breach that was attributed to an advanced persistent threat (APT) that used exploits of zero-day vulnerabilities to gain control of systems on her company's network. Which of the following is the least appropriate solution for Susan to recommend to help prevent future attacks of this type?

    1. Heuristic attack detection methods
    2. Signature-based attack detection methods
    3. Segmentation
    4. Leverage threat intelligence

    Answer:

    B. Signature-based attack detection methods rely on knowing what an attack or malware looks like. Zero-day attacks are unlikely to have an existing signature, making them a poor choice to prevent them. Heuristic (behavior) detection methods can indicate compromises despite the lack of signatures for the specific exploit. Building a well-designed and segmented network can limit the impact of compromises or even prevent them. Leveraging threat intelligence to understand new attacks and countermeasures is an important part of defense against zero-day attacks.
4.  During his investigation of a Windows system, Eric discovered that files were deleted and he wants to determine whether a specific file previously existed on the computer. Which of the following is the least likely to be a potential location to discover evidence supporting that theory?

    1. Windows registry
    2. Master File Table
    3. INDX files
    4. Event logs

    Answer:

    D. The Windows registry, Master File Tables, and INDX files all contain information about files, often including removed or deleted files. Event logs are far less likely to contain information about a specific file location.
5.  As part of her SOC analyst duties, Emily is tasked with monitoring intrusion detection systems that cover her employer's corporate headquarters network. During her shift, Emily's IDS alarms report that a network scan has occurred from a system with IP address 10.0.11.19 on the organization's WPA3 Enterprise wireless network aimed at systems in the finance division. What data source should she check first?

    1. Host firewall logs
    2. AD authentication logs
    3. Wireless authentication logs
    4. WAF logs

    Answer:

    C. Since Emily's organization uses WPA3 Enterprise, users must authenticate to use the wireless network. Associating the scan with an authenticated user will help incident responders identify the device that conducted the scan.
6.  Casey's incident response process leads her to a production server that must stay online for her company's business to remain operational. What method should she use to capture the data she needs?

    1. Live image to an external drive.
    2. Live image to the system's primary drive.
    3. Take the system offline and image to an external drive.
    4. Take the system offline, install a write blocker on the system's primary drive, and then image it to an external drive.

    Answer:

    A. Normally, forensic images are collected from systems that are offline to ensure that a complete copy is made. In cases like this where keeping the system online is more important than the completeness of the forensic image, a live image to an external drive using a portable forensic tool such as FTK Imager Lite, `dd`, or similar is the correct choice.
7.  What does the Nmap response “filtered” mean in port scan results?

    1. Nmap cannot tell whether the port is open or closed.
    2. A firewall was detected.
    3. An IPS was detected.
    4. There is no application listening, but there may be one at any time.

    Answer:

    A. When Nmap returns a response of “filtered,” it indicates that Nmap cannot tell whether the port is open or closed. Filtered results are often the result of a firewall or other network device, but a response of filtered does not indicate that a firewall or IPS was detected. When Nmap returns a “closed” result, it means that there is no application listening at that moment.
8.  During her review of incident logs, Deepa discovers the initial entry via SSH on a front-facing bastion host (A) at 8:02 a.m. If the network that Deepa is responsible for is designed as shown here, what is the most likely diagnosis if the second intrusion shows up on host B at 7:15 a.m.?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf001.jpg)

    1. Internal host B was previously compromised.
    2. Host A was compromised; then host B was compromised.
    3. Neither host B nor host A are synchronized to NTP properly.
    4. An internal threat compromised host B and then host A.

    Answer:

    C. The likeliest issue is a problem with the Network Time Protocol (NTP) synchronization for both of the hosts, because of an improperly set time zone or another time issue. The ruleset only allows traffic initiated by host A, making it impossible for host B to be the source of a compromise of A. The other options are possible, but the most likely issue is an NTP problem.
9.  Matt recently ran a vulnerability scan of his organization's network and received the results shown here. He would like to remediate the server with the highest number of the most serious vulnerabilities first. Which one of the following servers should be on his highest priority list?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf002.jpg)

    1. Server A
    2. Server B
    3. Server C
    4. Server D

    Answer:

    D. The most serious vulnerabilities shown in this report are medium-severity vulnerabilities. Server D has the highest number (8) of vulnerabilities at that severity level.
10. Saanvi has been tasked with conducting a risk assessment for the midsize bank that he works at because of a recent compromise of their online banking web application. Saanvi has chosen to use the NIST 800-30 risk assessment framework shown here. What likelihood of occurrence should he assign to breaches of the web application?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf003.jpg)

    1. Low
    2. Medium
    3. High
    4. Cannot be determined from the information given

    Answer:

    C. When an event of the type that is being analyzed has occurred within the recent past (often defined as a year), assessments that review that event will normally classify the likelihood of occurrence as high since it has already occurred.
11. Hank's boss recently came back from a CEO summit event where he learned about the importance of cybersecurity and the role of vulnerability scanning. He asked Hank about the vulnerability scans conducted by the organization and suggested that instead of running weekly scans that they simply configure the scanner to start a new scan immediately after the prior scan completes. How should Hank react to this request?

    1. Hank should inform the CEO that this would have a negative impact on system performance and is not recommended.
    2. Hank should immediately implement the CEO's suggestion.
    3. Hank should consider the request and work with networking and engineering teams on possible implementation.
    4. Hank should inform the CEO that there is no incremental security benefit from this approach and that he does not recommend it.

    Answer:

    C. The CEO's suggestion is a reasonable approach to vulnerability scanning that is used in some organizations, often under the term _continuous scanning_. He should consider the request and the impact on systems and networks to determine a reasonable course of action.
12. Selah's organization suffers an outage of its point-to-point encrypted VPN because of a system compromise at its ISP. What type of issue is this?

    1. Confidentiality
    2. Availability
    3. Integrity
    4. Accountability

    Answer:

    B. This is an example of an availability issue. If data had been modified, it would have been an integrity issue, while exposure of data would have been a confidentiality issue. Accountability from the outsourced vendor isn't discussed in the question.
13. Garrett is working with a database administrator to correct security issues on several servers managed by the database team. He would like to extract a report for the DBA that will provide useful information to assist in the remediation effort. Of the report templates shown here, which would be most useful to the DBA team?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf004.jpg)

    1. Qualys Top 20 Report
    2. Payment Card Industry (PCI) Technical Report
    3. Executive Report
    4. Technical Report

    Answer:

    D. The Technical Report will contain detailed information on a specific host and is designed for an engineer seeking to remediate the system. The PCI Technical Report would focus on credit card compliance issues, and there is no indication that this server is used for credit card processing. The Qualys Top 20 Report and Executive Report would contain summary information more appropriate for a management audience and would cover an entire network, rather than providing detailed information on a single system.
14. Jiang's SolarWinds network monitoring tools provide data about a system hosted in Amazon's AWS environment. When Jiang checks his server's average response time, he sees the results shown here.

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf005.jpg)

    What action should Jiang take based on this information?

    1. He should increase the speed of his network link.
    2. He should check for scheduled tasks at the times he sees spikes.
    3. He should ensure that his network card has the proper latency settings.
    4. He should perform additional diagnostics to determine the cause of the latency.

    Answer:

    D. Jiang needs to perform additional diagnostics to determine the cause of the latency.

    Unfortunately for Jiang, this chart does not provide enough information to determine why the maximum response time rises to high levels on a periodic basis. Since the events are not regularly timed, it is relatively unlikely that a scheduled task is causing the issue. Network cards do not have latency settings; latency is caused by network traffic, system response times, and similar factors. Increasing the speed of a network link may help with latency, but you do not have enough information to make that determination.
15. Alex notices the traffic shown here during a Wireshark packet capture. What is the host with IP address 10.0.2.11 most likely doing?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf006.jpg)

    1. UDP-based port scanning
    2. Network discovery via TCP
    3. SYN-based port scanning
    4. DNS-based discovery

    Answer:

    C. This image shows a SYN-based port scan. The traffic is primarily made up of TCP SYN packets to a variety of common ports, which is typical of a SYN-based port scan.
16. Jake is building a forensic image of a compromised drive using the `dd` command with its default settings. He finds that the imaging is going very slowly. What parameter should he adjust first?

    1. `if`
    2. `bs`
    3. `of`
    4. `count`

    Answer:

    B. The most likely cause of this slowness is an incorrect block size. Block size is set using the `bs` flag and is defined in bytes. By default, `dd` uses a 512-byte block size, but this is far smaller than the block size of most modern disks. Using a larger block size will typically be much faster, and if you know the block size for the device you are copying, using its native block size can provide huge speed increases. This is set using a flag like `bs = 64k`. The `if` and `of` flags adjust the input and output files, respectively, but there is no indication that these are erroneous. The count flag adjusts the number of blocks to copy and should not be changed if Jake wants to image the entire disk.
17. What purpose does a honeypot system serve when placed on a network as shown here?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf007.jpg)

    1. It prevents attackers from targeting production servers.
    2. It provides information about the techniques attackers are using.
    3. It slows down attackers like sticky honey.
    4. It provides real-time input to IDSs and IPSs.

    Answer:

    B. A honeypot is used by security researchers and practitioners to gather information about techniques and tools used by attackers. A honeypot will not prevent attackers from targeting other systems, and unlike a tarpit, it is not designed to slow down attackers. Typically, honeypot data must be analyzed to provide useful information that can be used to build IDS and IPS rules.
18. Munju's security team has found consistent evidence of system compromise over a period of weeks, with additional evidence pointing to the systems they are investigating being compromised for years. Despite her team's best efforts, Munju has found that her team cannot seem to track down and completely remove the compromise. What type of attack is Munju likely dealing with?

    1. A Trojan horse
    2. An APT
    3. A rootkit
    4. A zero-day attack

    Answer:

    B. Advanced persistent threats (APTs) are highly skilled attackers with advanced capabilities who are typically focused on specific objectives. To accomplish those objectives, they often obtain and maintain long-term access to systems and networks using powerful tools that allow them to avoid detection and to stay ahead of responders who attempt to remove them.
19. Which one of the following metrics would be most useful in determining the effectiveness of a vulnerability remediation program?

    1. Number of critical vulnerabilities resolved
    2. Time to resolve critical vulnerabilities
    3. Number of new critical vulnerabilities per month
    4. Time to complete vulnerability scans

    Answer:

    B. Of these choices, the most useful metric would be the time required to resolve critical vulnerabilities. This is a metric that is entirely within the control of the vulnerability remediation program and demonstrates the responsiveness of remediation efforts and the time that a vulnerability was present. The number of vulnerabilities resolved and the number of new vulnerabilities each month are not good measures of the program's effectiveness because they depend on the number of systems and services covered by the scan and the nature of those services.
20. Mike's Nmap scan of a system using the command `nmap 192.168.1.100` does not return any results. What does Mike know about the system if he is sure of its IP address, and why?

    1. The system is not running any open services.
    2. All services are firewalled.
    3. There are no TCP services reachable on Nmap's default 1000 TCP ports.
    4. There are no TCP services reachable on Nmap's default 65535 TCP ports.

    Answer:

    C. By default Nmap scans 1,000 of the most common TCP ports. Mike only knows that the system he scanned had no reachable (open, filtered, or closed) TCP ports in that list.
21. What is the purpose of creating a hash value for a drive during the forensic imaging process?

    1. To prove that the drive's contents were not altered
    2. To prove that no data was deleted from the drive
    3. To prove that no files were placed on the drive
    4. All of the above

    Answer:

    D. Once they are connected via a write blocker, a checksum is created (using SHA-2, SHA-3 or a similar hashing algorithm). If this hash matches the hash of forensic images, they exactly match, meaning that the drive's contents were not altered and that no files were added to or deleted from the drive.
22. After completing his unsuccessful forensic analysis of the hard drive from a workstation that was compromised by malware, Ben sends it to be re-imaged and patched by his company's desktop support team. Shortly after the system returns to service, the device once again connects to the same botnet. What action should Ben take as part of his next forensic review if this is the only system showing symptoms like this?

    1. Verify that all patches are installed.
    2. Destroy the system.
    3. Validate the BIOS hash against a known good version.
    4. Check for a system with a duplicate MAC address.

    Answer:

    C. Although BIOS infections are relatively rare, some malware does become resident in the system's firmware or BIOS. Once there, analysis of the hard drive will not show the infection. If the desktop support team at Ben's company has fully patched the system and no other systems are similarly infected, Ben's next step should be to validate that elements of the system he did not check before, such as the BIOS, are intact.
23. Part of the forensic data that Susan was provided for her investigation was a Wireshark packet capture. The investigation is aimed at determining what type of media an employee was consuming during work. What is the more detailed analysis that Susan can do if she is provided with the data shown here?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf008.jpg)

    1. She can determine that the user was viewing a GIF.
    2. She can manually review the TCP stream to see what data was sent.
    3. She can export and view the GIF.
    4. She cannot determine what media was accessed using this data set.

    Answer:

    C. Wireshark includes the ability to export packets. In this case, Susan can select the GIF89a detail by clicking that packet and then export the actual image to a file that she can view.
24. Which one of the following models traces the steps that an attacker would commonly perform during an intrusion?

    1. MITRE ATT\&CK
    2. Diamond
    3. Cyber Kill Chain
    4. STIX

    Answer:

    C. The Lockheed Martin Cyber Kill Chain traces the steps used to conduct an attack. The Diamond model and the MITRE ATT\&CK model are used to classify attacks. STIX is a standard format for describing threats.
25. Mika wants to run an Nmap scan that includes all TCP ports and uses service detection. Which of the following `nmap` commands should she execute?

    1. `nmap -p0 -all -SC`
    2. `nmap -p 1-32768 -sVS`
    3. `nmap -p 1-65535 -sV -sS`
    4. `nmap -all -sVS`

    Answer:

    C. Scanning the full range of TCP ports can be done using a SYN scan (`-sS`) and declaring the full range of possible ports (1-65535). Service version identification is enabled with the `-sV` flag.
26. Which one of the following cloud service models relies on the cloud service provider to implement the greatest number of security controls?

    1. SaaS
    2. PaaS
    3. FaaS
    4. IaaS

    Answer:

    A. The software-as-a-service (SaaS) model requires the cloud service provider to secure the entire service stack. Other models provide customers with greater degrees of control and responsibility over security.
27. Dan is a cybersecurity analyst for a healthcare organization. He ran a vulnerability scan of the VPN server used by his organization. His scan ran from inside the datacenter against a VPN server also located in the datacenter. The complete vulnerability report is shown here. What action should Dan take next?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf009.jpg)

    1. Dan should immediately remediate this vulnerability.
    2. Dan should schedule the vulnerability for remediation within the next 30 days.
    3. Dan should rerun the scan because this is likely a false positive report.
    4. Dan should take no action.

    Answer:

    D. Dan does not need to take any action. This is a very low criticality vulnerability (1/5), and it is likely not exploitable from outside the datacenter. It is not necessary to remediate this vulnerability, and there is no indication that it is a false positive report. Overall, this is a clean scan result for a VPN server.
28. Kwame received an alert from his organization's SIEM that it detected a potential attack against a web server on his network. However, he is unsure whether the traffic generating the alert actually entered the network from an external source or whether it came from inside the network. The NAT policy at the network perimeter firewall rewrites public IP addresses, making it difficult to assess this information based on IP addresses. Kwame would like to perform a manual log review to locate the source of the traffic. Where should he turn for the best information?

    1. Application server logs
    2. Database server logs
    3. Firewall logs
    4. Antimalware logs

    Answer:

    C. All of the data sources listed in this question may provide Kwame with further information about the attack. However, firewall logs would be best positioned to answer his specific question about the source of the attack. Since the firewall is performing network address translation (NAT), it would likely have a log entry of the original (pre-NAT) source IP address of the traffic.
29. Which one of the following types of vulnerability scans would provide the least information about the security configuration of a system?

    1. Agent-based scan
    2. Credentialed scan
    3. Uncredentialed internal scan
    4. Uncredentialed external scan

    Answer:

    D. An uncredentialed scan provides far less information than a credentialed scan or an agent-based scan because both credentialed and agent-based scans are able to gather configuration information from the target systems. External scans also provide less information than internal scans because they are filtered by border firewalls and other security devices. Therefore, an uncredentialed external scan would provide the least information.
30. After finishing a forensic case, Sam needs to wipe a magnetic hard drive (HDD) that he is using to prepare it for the next case. Which of the following methods is best suited to preparing the hard drive that he will use if he wants to be in compliance with NIST SP 800-88?

    1. Degauss the drive.
    2. Zero-write the drive.
    3. Seven rounds: all ones, all zeros, and five rounds of random values.
    4. Use the ATA Secure Erase command.

    Answer:

    B. NIST SP800-88, along with many forensic manuals, requires a complete zero wipe of the drive but does not require multiple rounds of wiping. Degaussing is primarily used for magnetic media-like tapes and may not completely wipe a hard drive (and may, in fact, damage it). Using the ATA Secure Erase command is commonly used for SSDs.
31. After reading the NIST standards for incident response, Mateo spends time configuring the NTP service on each of his servers, workstations, and appliances throughout his network. What phase of the incident response process is he working to improve?

    1. Preparation
    2. Detection and analysis
    3. Containment, eradication, and recovery
    4. Post-incident activity

    Answer:

    B. NIST recommends that clock synchronization is performed for all devices to improve the ability of responders to conduct analysis, part of the detection and analysis phase of the NIST incident response process. Although this might occur in the preparation phase, it is intended to improve the analysis process.
32. Latisha is the ISO for her company and is notified that a zero-day exploit has been released that can result in remote code execution on all Windows workstations on her network because of an attack against Windows domain services. She wants to limit her exposure to this exploit but needs the systems to continue to be able to access the Internet. Which of the following approaches is best for her response?

    1. Firewalling
    2. Patching
    3. Isolation
    4. Segmentation

    Answer:

    A. Latisha knows that Windows domain services can be blocked using a network firewall. As long as she builds the correct ruleset, she can prevent external systems from sending this type of traffic to her Windows workstations. She may still want to segment her network to protect the most important workstations, but her first move should be to use her firewalls to prevent the traffic from reaching the workstations.
33. When Saanvi was called in to help with an incident recovery effort, he discovered that the network administrator had configured the network as shown here. What type of incident response action best describes what Saanvi has encountered?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf010.jpg)

    1. Segmentation
    2. Isolation
    3. Removal
    4. Network locking

    Answer:

    B. The systems in the containment network are fully isolated from the rest of the network using logical controls that prevent any access. To work with the systems that he needs to access, Saanvi will need to either have firewall rules added to allow him remote access to the systems or physically work with them.
34. As part of the forensic investigation of a Linux workstation, Alex needs to determine what commands may have been issued on the system. If no anti-forensic activities have taken place, what is the best location for Alex to check for a history of commands issued on the system?

    1. `/var/log/commands.log`
    2. `$HOME/.bash_history`
    3. `$HOME/.commands.sqlite`
    4. `/var/log/authactions.log`

    Answer:

    B. On Linux systems that use the Bash shell, `$home/.bash_history` will contain a log of recently performed actions. Each of the others was made up for this question.
35. Ben recently completed a risk analysis and determined that he should implement a new set of firewall rules to filter traffic from known suspect IP addresses. What type of risk management activity is he performing?

    1. Risk avoidance
    2. Risk acceptance
    3. Risk transference
    4. Risk mitigation

    Answer:

    D. Implementing firewall rules is an attempt to reduce the likelihood of a risk occurring. This is, therefore, an example of a risk mitigation strategy.
36. Crystal is attempting to determine the next task that she should take on from a list of security priorities. Her boss told her that she should focus on activities that have the most “bang for the buck.” Of the tasks shown here, which should she tackle first?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf011.jpg)

    1. Task 1
    2. Task 2
    3. Task 3
    4. Task 4

    Answer:

    C. Task 3 strikes the best balance between criticality and difficulty. It allows Crystal to remediate a medium criticality issue with an investment of only 6 hours of time. Task 2 is higher criticality but would take 12 weeks to resolve. Task 1 is the same criticality but would require a full day to fix. Task 4 is lower criticality but would require the same amount of time to resolve as Task 1.
37. During the analysis of an incident that took place on her network, Sofia discovered that the attacker used a stolen cookie to access a web application. Which one of the following attack types most likely occurred?

    1. On-path (man-in-the-middle)
    2. Privilege escalation
    3. Cross-site scripting
    4. Session hijacking

    Answer:

    D. The use of a stolen cookie is the hallmark of a session hijacking attack. These attacks focus on taking over an already existing session, either by acquiring the session key or cookies used by the remote server to validate the session or by causing the session to pass through a system the attacker controls, allowing them to participate in the session.
38. Curt is conducting a forensic analysis of a Windows system and needs to determine whether a program was set to automatically run. Which of the following locations should he check for this information?

    1. NTFS INDX files
    2. The registry
    3. Event logs
    4. Prefetch files

    Answer:

    B. The registry contains autorun keys that are used to make programs run at startup. In addition, scheduled tasks, individual user startup folders, and DLLs placed in locations that will be run by programs (typically malicious DLLs) are all locations where files will automatically run at startup or user login.
39. What concept measures how easy data is to lose?

    1. Order of volatility
    2. Data transience
    3. Data loss prediction
    4. The Volatility Framework

    Answer:

    A. The order of volatility of data measures how easy the data is to lose. The Volatility Framework is a forensic tool aimed at memory forensics, while data transience and data loss prediction are not common terms.
40. Steps like those listed here are an example of what type of incident response preparation?

    1. Visit [`otx.alienvault.com`](http://otx.alienvault.com/) and the suspected C\&C system's IP address on the top search input field.
    2. If the IP address is associated with malware C\&C activity, create a ticket in the incident response tracking system.
    3. Creating a CSIRT
    4. Creating a playbook
    5. Creating an incident response plan
    6. Creating an IR-FAQ

    Answer:

    B. Playbooks contain specific procedures used during a particular type of cybersecurity incident. In this case, the playbook entry addresses malware command and control traffic validation. Creating a CSIRT or IR plan occurs at a higher level, and IR-FAQs is not a common industry term.
41. While analyzing the vulnerability scan from her web server, Kristen discovers the issue shown here. Which one of the following solutions would best remedy the situation?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf012.jpg)

    1. Move from TLS 1.0 to SSL 3.0.
    2. Require IPsec connections to the server.
    3. Disable the use of TLS.
    4. Move from TLS 1.0 to TLS 1.3.

    Answer:

    D. Kristen should upgrade the web server to the most current secure version of TLS: TLS 1.3. SSL 3.0 has vulnerabilities similar to those in TLS 1.0 and is not a suitable alternative. IPsec is not effective for web communications. Disabling the use of TLS would jeopardize the security of information sent to and from the server and would create additional risk, rather than remedying the situation.
42. Charles is building an incident response playbook for his organization that will address command-and-control client-server traffic detection and response. Which of the following information sources is least likely to be part of his playbook?

    1. DNS query logs
    2. Threat intelligence feeds
    3. Honeypot data
    4. Notifications from internal staff about suspicious behavior

    Answer:

    C. Relatively few organizations run honeypots because of the effort required to maintain and analyze the data they generate. DNS queries and other traffic logs, threat intelligence feeds, and notifications from staff are all common information sources for a variety of types of incident detection.
43. Carol recently fell victim to a phishing attack. When she clicked the link in an email message that she received, she was sent to her organization's central authentication service and logged in successfully. She did verify the URL and certificate to validate that the authentication server was genuine. After authenticating, she was sent to a form that collected sensitive personal information that was sent to an attacker. What type of vulnerability did the attacker most likely exploit?

    1. Buffer overflow
    2. Session hijacking
    3. IP spoofing
    4. Open redirect

    Answer:

    D. In an open redirect attack, users may be sent to a genuine authentication server and then redirected to an untrusted server through the OAuth flow. This occurs when the authentication server does not validate OAuth server requests prior to redirection.
44. As a penetration tester, Max uses Wireshark to capture all of his testing traffic. Which of the following is not a reason that Max would capture packets during penetration tests?

    1. To document the penetration test
    2. To scan for vulnerabilities
    3. To gather additional information about systems and services
    4. To troubleshoot issues encountered when connecting to targets

    Answer:

    B. Although packet capture can help Max document his penetration test and gather additional information about remote systems through packet analysis, as well as help troubleshoot connection and other network issues, sniffers aren't useful for scanning for vulnerabilities on their own.
45. Rich recently configured new vulnerability scans for his organization's business intelligence systems. The scans run late at night when users are not present. Rich received complaints from the business intelligence team that the performance burden imposed by the scanning is causing their overnight ETL jobs to run too slowly and they are not completing before business hours. How should Rich handle this situation?

    1. Rich should inform the team that they need to run the ETL jobs on a different schedule.
    2. Rich should reconfigure the scans to run during business hours.
    3. Rich should inform the team that they must resize the hardware to accommodate both requirements.
    4. Rich should work with the team to find a mutually acceptable solution.

    Answer:

    D. Rich should not attempt to solve this problem on his own or dictate a specific solution. Instead, he should work with the business intelligence team to find a way to both meet their business requirements and accomplish the security goals achieved by scanning.
46. Javier ran a vulnerability scan of a new web application created by developers on his team and received the report shown here. The developers inspected their code carefully and do not believe that the issue exists. They do have a strong understanding of SQL injection issues and have corrected similar vulnerabilities in other applications. What is the most likely scenario in this case?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf013.jpg)

    1. Javier misconfigured the scan.
    2. The code is deficient and requires correction.
    3. The vulnerability is in a different web application running on the same server.
    4. The result is a false positive.

    Answer:

    D. Blind SQL injection vulnerabilities are difficult to detect and are a notorious source of false positive reports. Javier should verify the results of the tests performed by the developers but should be open to the possibility that this is a false positive report, as that is the most likely scenario.
47. During an incident investigation, Mateo is able to identify the IP address of the system that was used to compromise multiple systems belonging to his company. What can Mateo determine from this information?

    1. The identity of the attacker
    2. The country of origin of the attacker
    3. The attacker's domain name
    4. None of the above

    Answer:

    D. Although it may be tempting to assign blame based on an IP address, attackers frequently use compromised systems for attacks. Some may also use cloud services and hosting companies where they can purchase virtual machines or other resources using stolen credit cards. Thus, knowing the IP address from which an attack originated will typically not provide information about an attacker. In some cases, deeper research can identify where an attack originated, but even then, knowing the identity of an attacker is rarely certain.
48. After a major compromise involving what appears to be an APT, Jaime needs to conduct a forensic examination of the compromised systems. Which containment method should he recommend to ensure that he can fully investigate the systems that were involved while minimizing the risk to his organization's other production systems?

    1. Sandboxing
    2. Removal
    3. Isolation
    4. Segmentation

    Answer:

    B. Completely removing the systems involved in the compromise will ensure that they cannot impact the organization's other production systems. Although attackers may be able to detect this change, it provides the best protection possible for the organization's systems.
49. Piper is attempting to remediate a security vulnerability and must apply a patch to a production database server. The database administration team is concerned that the patch will disrupt business operations. How should Piper proceed?

    1. She should deploy the patch immediately on the production system.
    2. She should wait 60 days to deploy the patch to determine whether bugs are reported.
    3. She should deploy the patch in a sandbox environment to test it prior to applying it in production.
    4. She should contact the vendor to determine a safe time frame for deploying the patch in production.

    Answer:

    C. Piper should deploy the patch in a sandbox environment and then thoroughly test it prior to releasing it in production. This reduces the risk that the patch will not work well in her environment. Simply asking the vendor or waiting 60 days may identify some issues, but it does not sufficiently reduce the risk because the patch will not have been tested in her company's environment.
50. Kent ran a vulnerability scan of an internal CRM server that is routinely used by employees, and the scan reported that no services were accessible on the server. Employees continued to use the CRM application over the Web without difficulty during the scan. What is the most likely source of Kent's result?

    1. The server requires strong authentication.
    2. The server uses encryption.
    3. The scan was run from a different network perspective than user traffic.
    4. The scanner's default settings do not check the ports used by the CRM application.

    Answer:

    C. The most likely scenario is that Kent ran the scan from a network that does not have access to the CRM server. Even if the server requires strong authentication and/or encryption, this would not prevent ports from appearing as open on the vulnerability scan. The CRM server runs over the web, as indicated in the scenario. Therefore, it is most likely using ports 80 and/or 443, which are part of the default settings of any vulnerability scanner.
51. Steve needs to perform an Nmap scan of a remote network and wants to be as stealthy as possible. Which of the following `nmap` commands will provide the stealthiest approach to his scan?

    1. `nmap -P0 -sT 10.0.10.0/24`
    2. `nmap -sT -T0 10.0.10.0/24`
    3. `nmap -P0 -sS 10.0.10.0/24`
    4. `nmap -P0 -sS -T0 10.0.10.0/24`

    Answer:

    D. Nmap provides multiple scan modes, including a TCP SYN scan, denoted by the `-sS` flag. This is far stealthier than the full TCP connect scan, which uses the `-sT` flag. Turning off pings with the `-P0` flag helps with stealth, and setting the scan speed using the `-T` flag to either a 0 for paranoid or a 1 for sneaky will help bypass many IDSs by falling below their detection threshold.
52. After performing threat hunting, Lakshman determines that it would be appropriate to disable some services on his organization's database servers. What activity is Lakshman engaging in?

    1. Establishing a hypothesis
    2. Gathering evidence
    3. Reducing the attack surface
    4. Executable process analysis

    Answer:

    C. Disabling unnecessary services reduces the attack service by decreasing the number of possible attack vectors for gaining access to a server.
53. Jenna is configuring the scanning frequency for her organization's vulnerability scanning program. Which one of the following is the _least_ important criteria for Jenna to consider?

    1. Sensitivity of information stored on systems
    2. Criticality of the business processes handled by systems
    3. Operating system installed on systems
    4. Exposure of the system to external networks

    Answer:

    C. Of the criteria listed, the operating system installed on the systems is the least likely to have a significant impact on the likelihood and criticality of discovered vulnerabilities. All operating systems are susceptible to security issues.
54. Donna is interpreting a vulnerability scan from her organization's network, shown here. She would like to determine which vulnerability to remediate first. Donna would like to focus on the most critical vulnerability according to the potential impact if exploited. Assuming the firewall is properly configured, which one of the following vulnerabilities should Donna give the highest priority?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf014.jpg)

    1. Severity 5 vulnerability in the file server
    2. Severity 3 vulnerability in the file server
    3. Severity 4 vulnerability in the web server
    4. Severity 2 vulnerability in the mail server

    Answer:

    A. In this case, the identity or network location of the server is not relevant. Donna is simply interested in the most critical vulnerability, so she should select the one with the highest severity. In vulnerability severity rating systems, severity 5 vulnerabilities are the most critical, and severity 1 are the least critical. Therefore, Donna should remediate the severity 5 vulnerability in the file server.
55. Which one of the following document categories provides the highest-level authority for an organization's cybersecurity program?

    1. Policy
    2. Standard
    3. Procedure
    4. Framework

    Answer:

    A. Policies are the highest-level component of an organization's governance documentation. They are set at the executive level and provide strategy and direction for the cybersecurity program. Standards and procedures derive their authority from policies. Frameworks are not governance documents but rather provide a conceptual structure for organizing a program. Frameworks are usually developed by third-party organizations, such as ISACA or ITIL.
56. Mateo is planning a vulnerability scanning program for his organization and is scheduling weekly scans of all the servers in his environment. He was approached by a group of system administrators who asked that they be given direct access to the scan reports without going through the security team. How should Mateo respond?

    1. Mateo should provide the administrators with access.
    2. Mateo should deny the administrators access because the information may reveal critical security issues.
    3. Mateo should offer to provide the administrators with copies of the report after they go through a security review.
    4. Mateo should deny the administrators access because it would allow them to correct security issues before they are analyzed by the security team.

    Answer:

    A. Vulnerability scanning information is most effective in the hands of individuals who can correct the issues. The point of scans is not to “catch” people who made mistakes. Mateo should provide the administrators with access. The security team may always monitor the system for unremediated vulnerabilities, but they should not act as a gatekeeper to critical information.
57. While reviewing a report from a vulnerability scan of a web server, Paul encountered the vulnerability shown here. What is the easiest way for Paul to correct this vulnerability with minimal impact on the business?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf015.jpg)

    1. Block ports 80 and 443.
    2. Adjust directory permissions.
    3. Block port 80 only to require the use of encryption.
    4. Remove CGI from the server.

    Answer:

    B. This vulnerability results in an information disclosure issue. Paul can easily correct it by disabling the directory listing permission on the `cgi-bin` directory. This is unlikely to affect any other use of the server because he is not altering permissions on the CGI scripts themselves. Blocking access to the web server and removing CGI from the server would also resolve the vulnerability but would likely have an undesirable business impact.
58. A log showing a successful user authentication is classified as what type of occurrence in NIST's definitions?

    1. A security incident
    2. A security event
    3. An event
    4. An adverse event

    Answer:

    C. Observable occurrences are classified as events in NIST's scheme. Events with negative consequences are considered adverse events, while violations (or event imminent threats of violations) are classified as security incidents.
59. Fran is trying to run a vulnerability scan of a web server from an external network, and the scanner is reporting that there are no services running on the web server. She verified the scan configuration and attempted to access the website running on that server using a web browser on a computer located on the same external network and experienced no difficulty. What is the most likely issue with the scan?

    1. A host firewall is blocking access to the server.
    2. A network firewall is blocking access to the server.
    3. An intrusion prevention system is blocking access to the server.
    4. Fran is scanning the wrong IP address.

    Answer:

    C. The most likely issue is that an intrusion prevention system (IPS) is detecting the scan as an attack and blocking the scanner. If this were a host or network firewall issue, Fran would most likely not be able to access the server using a web browser. It is less likely that the scan is misconfigured given that Fran double-checked the configuration.
60. During a regulatory compliance assessment, Manish discovers that his organization has implemented a multifactor authentication requirement for systems that store and handle highly sensitive data. The system requires that users provide both a password and a four-digit PIN. What should Manish note in his findings about this system?

    1. The multifactor system provides two independent factors and provides an effective security control.
    2. The factors used are both the same type of factor, making the control less effective.
    3. The system uses only two factors and is not a true multifactor system. To qualify as multifactor, it should include at least three factors.
    4. The multifactor system's use of a four-digit PIN does not provide sufficient complexity, and additional length should be required for any PIN for secure environments.

    Answer:

    B. The biggest issue in this scenario is that both factors are knowledge-based factors. A true multifactor system relies on more than one type of distinct factor including something you know, something you have, or something you are (and sometimes somewhere you are). This system relies on two things you know, and attackers are likely to acquire both from the same location in a successful attack.
61. Which one of the following mechanisms may be used to enhance security in a context-based authentication system?

    1. Time of day
    2. Location
    3. Device fingerprint
    4. All of the above

    Answer:

    D. Context-based authentication may leverage a wide variety of information. Potential attributes include time of day, location, device fingerprint, frequency of access, user roles, user group memberships, and IP address/reputation.
62. Latisha's organization has faced a significant increase in successful phishing attacks, resulting in compromised accounts. She knows that she needs to implement additional technical controls to prevent successful attacks. Which of the following controls will be the most effective while remaining relatively simple and inexpensive to deploy?

    1. Increased password complexity requirements
    2. Application or token-based multifactor authentication
    3. Biometric-based multifactor authentication
    4. OAuth-based single sign-on

    Answer:

    B. Application or token-based multifactor authentication ensures that the exposure of a password because of successful phishing email does not result in the compromise of the credential. Password complexity increases fail to add security since complex passwords can still be compromised by phishing attacks, biometric multifactor authentication is typically expensive to implement and requires enrollment, and OAuth-based single sign-on will not prevent phishing attacks; instead, it can make it easier for attackers to move between multiple services.
63. Lauren downloads a new security tool and checks its MD5. What does she know about the software she downloaded if she receives the following message?

    `root@demo:~# md5sum -c demo.md5 demo.txt: FAILED md5sum: WARNING: 1 computed checksum did not match`

    1. The file is corrupted.
    2. Attackers have modified the file.
    3. The files do not match.
    4. The test failed and provided no answer.

    Answer:

    C. Lauren knows that the file she downloaded and computed a checksum for does not match the MD5 checksum that was calculated by the providers of the software. She does not know it the file is corrupted or if attackers have modified the file but may want to contact the providers of the software to let them know about the issue, and she definitely shouldn't execute or trust the file!
64. Peter works for an organization that is joining a consortium of similar organizations that use a federated identity management (FIM) system. He is configuring his identity management system to participate in the federation. Specifically, he wants to ensure that users at his organization will be able to use their credentials to access federated services. What role is Peter configuring?

    1. Relying party
    2. Service provider
    3. Identity provider
    4. Consumer

    Answer:

    C. Identity providers (IDPs) provide identities, make assertions about those identities to relying parties, and release information to relying parties about identity holders. Relying parties (RP), also known as service providers (SP), provide services to members of the federation and should handle the data from both users and identity providers securely. The consumer is the end user of the federated services.
65. Mika uses a security token like the unit shown here and a password to authenticate to her PayPal account. What two types of factors is she using?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf016.jpg)

    1. Something she knows and something she has.
    2. Something she knows and something she is.
    3. Something she is and something she has.
    4. Mika is using only one type of factor because she knows the token code and her password.

    Answer:

    A. Mika is using both a knowledge-based factor in the form of her password and something she has in the form of the token. Possession of the token is the “something she has.”
66. During the account setup for her bank, Deepa is asked to answer a series of questions about her past home addresses, financial transactions, and her credit history. What type of authentication factor is Deepa being asked for?

    1. Location factor
    2. Knowledge factor
    3. Possession factor
    4. Biometric factor

    Answer:

    B. Questions that rely on knowledge that a specific individual should have are an example of a knowledge factor. When institutions want to verify that a new user is who they claim to be, they will sometimes use information that is unlikely to be acquired by third parties like the examples given here.
67. Charles is worried about users conducting SQL injection attacks. Which of the following solutions will best address his concerns?

    1. Using secure session management
    2. Enabling logging on the database
    3. Performing user input validation
    4. Implementing TLS

    Answer:

    C. Charles should perform user input validation to strip out any SQL code or other unwanted input. Secure session management can help prevent session hijacking, logging may provide useful information for incident investigation, and implementing TLS can help protect network traffic, but only input validation helps with the issue described.
68. Which of the following risks is most commonly associated with vulnerability scanning activities?

    1. Attackers may learn about the vulnerabilities.
    2. Services may be crashed by the scanner.
    3. The vulnerability scanner may be exploited by attackers.
    4. Too many vulnerabilities may be detected.

    Answer:

    B. The most common concern with vulnerability scanning is that it may have a service impact due to exploiting a risk or causing a denial-of-service condition. In sensitive environments, scans are sometimes run against nonproduction versions of services to help prevent this, but the most common answer is that if the service cannot survive being scanned, it is not ready to be used!
69. Adam finds entries in his authentication logs for many of the systems in his network that all have logins for the same userID with a variety of passwords. What type of attack has he discovered?

    1. A session hijacking attack
    2. An on-path (man-in-the-middle) attack
    3. A credential stuffing attack
    4. A password spraying attack

    Answer:

    D. Password spraying attacks try many passwords for a limited number of accounts. Credential stuffing attacks try compromised usernames and passwords across many sites to try to use them elsewhere. Session hijacking requires a valid session to try to leverage to conduct malicious activities. An on-path (man-in-the-middle) attack would require the attacker to redirect traffic through a system that they control to allow them to be able to read and/or modify the traffic before it continues on to the legitimate destination. Adam could mitigate the password spraying attack by using back-off algorithms that allow only a limited number of failures before delaying further logins or locking out the account until it is manually unlocked.
70. You are reviewing the methods that your organization uses to communicate with the media during an incident response effort. Which one of the following is not a commonly accepted practice?

    1. Inform the media immediately of developments in the investigation.
    2. Conduct practice sessions for incident responders who communicate with the media.
    3. Establish media briefing procedures in advance of an incident.
    4. Maintain an incident response status document.

    Answer:

    A. Communications with the media should be carefully planned and timed to share relevant information at the appropriate moment. Organizations should not have a default policy of immediately sharing all information, as that might result in adverse publicity, create legal risk, or hinder the investigation. The other activities listed here are all best practices for incident communications.
71. Charles reviews the source code for a web application for vulnerabilities. What type of software assessment is this?

    1. Dynamic analysis
    2. Fuzzing
    3. Static analysis
    4. Reverse engineering

    Answer:

    C. Manual or automated review of source code rather than a running application is static analysis. This can help find bugs that you cannot see in the running application or that may otherwise be missed, but it also does not test the live code.
72. Isaac sees the following entry in his web logs. What type of attack has been attempted?

    `http://example.com/../../../../../etc/shadow`

    1. A buffer overflow attack
    2. An attack on the heap
    3. A session hijacking attack
    4. A directory traversal attack

    Answer:

    D. This query attempts to traverse directories from the directory the web server is running in, until it can access `/etc/shadow`. If the web application does not have appropriate filters or the system does not have appropriate permissions set to prevent this, the attacker will be able to download `/etc/shadow`, the password store for Linux systems. A buffer overflow would typically have data passed to a variable and then code that would be executed once the buffer was overflowed and the additional contents were placed into memory. There is no session data, and there is no indication of data that would be placed on the heap of a system.
73. Precompiled SQL statements that only require variables to be input are an example of what type of application security control?

    1. Parameterized queries
    2. Encoding data
    3. Input validation
    4. Appropriate access controls

    Answer:

    A. A parameterized query (sometimes called a prepared statement) uses a prebuilt SQL statement to prevent SQL-based attacks. Variables from the application are fed to the query, rather than building a custom query when the application needs data. Encoding data helps to prevent cross-site scripting attacks, as does input validation. Appropriate access controls can prevent access to data that the account or application should not have access to, but they don't use precompiled SQL statements.
74. Rob would like to perform a root-cause analysis in the wake of an incident. He will be including the results of that analysis in his incident report. What action should he take first?

    1. Document the analysis.
    2. Differentiate between each of the events and causal factors.
    3. Identify the problems and events that occurred.
    4. Establish a timeline.

    Answer:

    C. Rob should undertake all four of these steps during his root-cause analysis, but he should understand the appropriate sequence:

    1. Identify the problems and events that occurred as part of the incident, and describe them as well as possible.
    2. Establish a timeline of events. This helps to determine what happened and in what order to help identify the root cause (or causes).
    3. Differentiate between each of the events and causal factors. In short, you need to determine which cause is a root cause, which are results of the root cause, and which are causal factors, or events that contributed to the issue but were not the root cause.
    4. Document the root-cause analysis, often through the use of a diagram or chart.
75. What are activities like disabling unnecessary processes, moving systems to internal IP addresses, and using firewalls and other network security devices to protect hosts known as in the context of threat hunting?

    1. Establishing a hypothesis
    2. Conducting a security lockdown
    3. Reducing the attack surface areas
    4. Bundling critical assets

    Answer:

    C. An important part of threat hunting is reducing your own organization's attack surface area. This can involve any activity that reduces the systems or services that an attacker can potentially map or attack. Establishing a hypothesis is part of identifying your threat model but doesn't involve these activities, and bundling critical assets is used to gather similar assets together for assessment and threat modeling activities. Conducting a security lockdown is not a common threat hunting term.
76. Bob is creating a report to management summarizing the result of a recent vulnerability scan. He would like to prioritize the results. Which one of the following tools would provide the most comprehensive assessment of the risk posed by each vulnerability?

    1. CVSS score
    2. Confidentiality rating
    3. Impact rating
    4. Likelihood rating

    Answer:

    A. The Common Vulnerability Scoring System (CVSS) is a standardized approach to assessing the risk posed by a vulnerability. It brings together both likelihood and impact (confidentiality, integrity, and availability) ratings into a single measure and, therefore, is the most comprehensive of these approaches.
77. Kelly's organization recently suffered a security incident where the attacker was present on her network for several months before the SOC identified the attack. Once they saw evidence, they quickly reacted to contain the incident. Which incident response metric would suffer most as a result of this performance?

    1. Mean time to respond
    2. Mean time to remediate
    3. Alert volume
    4. Mean time to detect

    Answer:

    D. The issue in this case is that the SOC did not detect the incident for several months. This would impact the mean time to detect metric. They did quickly respond and remediate the incident once it was detected. This was only a single incident, so it should have no noticeable impact on alert volume.
78. Seth is trying to identify activities in his organization that might be automated to improve efficiency. Which one of the following activities is least likely to benefit from automation?

    1. Threat hunting
    2. Intrusion analysis
    3. Qualitative risk assessment
    4. Data backup

    Answer:

    C. It is likely that Seth's organization will find some efficiencies by adding automation to their technical activities, including threat hunting, intrusion analysis, and data backup. Qualitative risk analysis is a nontechnical activity and focuses on human thought. It is, therefore, the least likely candidate for automation of the activities on this list.
79. Rae wants to detect forged sender addresses to decrease the amount of spam that her organization receives. Which of the following techniques or methods will most directly fit her needs?

    1. Spamhaus
    2. DKIM
    3. SPF
    4. RBL

    Answer:

    B. DomainKeys Identified Mail (DKIM) uses digital signatures to validate that the claimed domain of the sender is the actual sender's domain. Sender Policy Framework (SPF) records identify the mail servers that can send email from your domain but do not prove the sender's domain. Spamhaus is an antispam organization, and an RBL is a real-time black hole list, which is a list of untrusted or spam sending hosts.
80. Your organization recently suffered a series of serious vulnerabilities as a result of the use of legacy software that is no longer supported by the vendor. This software is critical to your organization and can't be removed for at least six more months. What action plan would best address this risk during that six month period?

    1. Awareness, training, and education
    2. Compensating controls
    3. Patch management
    4. Changing business requirements

    Answer:

    B. You should implement compensating controls that mitigate the risk of the legacy systems. For example, you might place the systems on an isolated network where they are less susceptible to direct attack. Awareness, training, and education may be helpful, but it would not address the risk as completely as a compensating control. Patch management is not possible because the software is no longer supported by the vendor, so no new patches will be issued. Changing business requirements is not a feasible solution because the system is needed for six more months. Patch management is not possible because the software is no longer supported by the vendor, so no new patches will be issued.
81. Yolanda received a threat intelligence report and is evaluating it to determine whether her organization runs any of the software affected by the threat. What type of confidence is Yolanda attempting to gain?

    1. Timeliness
    2. Accuracy
    3. Relevancy
    4. Superficial

    Answer:

    C. The three types of confidence in a threat intelligence report are timeliness, relevance, and accuracy. Yolanda is assessing whether this threat affects her organization, which is a measure of relevancy. There is no indication that Yolanda suspects that the report is outdated or inaccurate.
82. Gabby's organization captures sensitive customer information, and salespeople and others often work with that data on local workstations and laptops. After a recent inadvertent breach where a salesperson accidentally sent a spreadsheet of customer information to another customer, her organization is seeking a technology solution that can help prevent similar problems. What should Gabby recommend?

    1. IDS
    2. FSB
    3. DLP
    4. FDE

    Answer:

    C. Data loss prevention (DLP) can tag sensitive data and then scan outbound communications for that data. Once tagged data or data that matches specific patterns such as credit card numbers or Social Security numbers are discovered, DLP can alert the user or take other action. IDS, an intrusion detection system, might be able to detect patterns but could not stop traffic flow. FSB is not a security term, and full-disk encryption (FDE) can help prevent data loss if a system is stolen.
83. Fred is reviewing a checklist used in the automation of his security program and sees the following code:

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c05uf017.jpg)

    What file type from the following list is he most likely reviewing?

    1. Plaintext
    2. JSON
    3. XML
    4. HTML

    Answer:

    C. Fred is most likely reviewing an XML file. JSON uses a series of curly brackets ({ and }), and those do not appear in this sample. Plaintext is generally not structured, and this sample is highly structured. Both XML and HTML use angle brackets (< and >) to indicate code elements. We can eliminate HTML because it uses specific tags, such as \<A>, \<HEAD>, and \<H1> that do not appear in this sample. XML provides a much more flexible format that can use any tags desired by the developer.
84. Cynthia's organization receives a letter from a company they are a service provider for, notifying them of a pending legal case and telling them not to delete or discard documents related to the case. What term describes this?

    1. Legal hold
    2. Litigation priority
    3. Criminal suspension
    4. A data summons

    Answer:

    A. Legal or litigation holds are notifications sent to inform an organization or individual that they should not delete data or destroy records that may be relevant to a new or pending legal case. The remainder of the answers for this question are made up.
85. As part of his forensic investigation, Alex signs and notes in his log when the drive copy he prepared is transferred to legal counsel. What is this process known as?

    1. Handoff documentation
    2. Chain of custody tracking
    3. Asset tracking
    4. Forensic certification

    Answer:

    B. Chain of custody tracking determines who has access to and authority over drives, devices, and forensic data throughout its life cycle. This is a critical element in investigations that may end up in court or that will involve law enforcement.
