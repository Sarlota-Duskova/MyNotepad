# Questions

1.  Consider the threat modeling analysis shown here. What attack framework was used to develop this analysis?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf001.jpg)

    1. ATT\&CK
    2. Cyber Kill Chain
    3. STRIDE
    4. Diamond

    Answer:

    D. This analysis used the Diamond model of intrusion analysis, which describes a sequence where an adversary deploys a capability targeted at an infrastructure against a victim. The Diamond model draws its name from the shape of the diagram created during the analysis.
2.  As part of an organization-wide red team exercise, Frank is able to use a known vulnerability to compromise an Apache web server. Frank knows that the Apache service is running under a limited user account. Once he has gained access, what should his next step be if he wants to use the system to pivot to protected systems behind the screened subnet (DMZ) that the web server resides in?

    1. Vulnerability scanning
    2. Privilege escalation
    3. Patching
    4. Installing additional tools

    Answer:

    B. By default Apache does not run as an administrative user. In fact, it typically runs as a limited user. To take further useful action, Frank should look for a privilege escalation path that will allow him to gain further access.
3.  Helen is using the Lockheed Martin Cyber Kill Chain to analyze an attack that took place against her organization. During the attack, the perpetrator attached a malicious tool to an email message that was sent to the victim. What phase of the Cyber Kill Chain includes this type of activity?

    1. Weaponization
    2. Delivery
    3. Exploitation
    4. Actions on objectives

    Answer:

    B. Delivery occurs when the adversary deploys their tool either directly against targets or via release that relies on staff at the target interacting with it such as in an email payload, on a USB stick, or via websites that they visit.
4.  Betty wants to review the security logs on her Windows workstation. What tool should she use to do this?

    1. `Secpol.msc`
    2. Event Viewer
    3. Log Viewer
    4. `Logview.msc`

    Answer:

    B. The Windows Event Viewer is a built-in tool for Windows systems that can be used to view application, security, setup, system, and other events and logs. `Secpol.msc` is the Local Security Policy snap-in, and `logview.msc` is not a built-in Windows tool or a snap-in.
5.  The ATT\&CK framework defines which of the following as “the specifics behind how the adversary would attack the target?”

    1. The threat actor
    2. The targeting method
    3. The attack vector
    4. The organizational weakness

    Answer:

    C. The MITRE ATT\&CK framework defines the attack vector as the specifics behind how the adversary would attack the target. You don't have to memorize ATT\&CK to pass the exam, but you should be prepared to encounter questions that you need to narrow down based on what knowledge you do have. Here you can rule out the threat actor and targeting method and then decide between the attack vector and organizational weakness.
6.  Jamal wants to leverage a framework to improve his threat hunting for network defense. What threat-hunting framework should he select to help his team categorize and analyze threats more effectively?

    1. MOPAR
    2. CVSS
    3. MITRE ATT\&CK
    4. CAPEC

    Answer:

    C. The ATT\&CK framework is focused on network defense and broadly covers threat hunting. CAPEC is focused on application security. CVSS is the Common Vulnerability Scoring System, and Mopar is a parts, service, and customer care organization that is part of Fiat Chrysler.
7.  Maria is an Active Directory domain administrator for her company, and she knows that a quickly spreading botnet relies on a series of domain names for command and control and that preventing access to those domain names will cause the malware infection that connects to the botnet to fail to take further action. Which of the following actions is her best option if she wants to prevent offsite Windows users from connecting to botnet command-and-control systems?

    1. Force a BGP update.
    2. Set up a DNS sinkhole.
    3. Modify the hosts file.
    4. Install an antimalware application.

    Answer:

    C. Maria can push an updated hosts file to her domain connected systems that will direct traffic intended for known bad domains to the localhost or a safe system. She might want to work with a security analyst or other IT staff member to capture queries sent to that system to track any potentially infected workstations. A DNS sinkhole would work only if all of the systems were using local DNS, and offsite users are likely to have DNS settings set by the local networks they connect to. Antimalware applications may not have an update yet, or may fail to detect the malware, and forcing a Border Gateway Protocol (BGP) update for third-party networks is likely a bad idea.
8.  While attempting to stop a rogue service, Monica issues the following Linux command on an Ubuntu system using upstart:

    `service rogueservice stop`

    After a reboot, she discovers the service running again. What happened, and what does she need to do to prevent this?

    1. The service restarted at reboot, so she needs to include the `-p`, or permanent, flag.
    2. The service restarted itself, so she needs to delete the binary associated with the service.
    3. The service restarted at reboot, so she should add an `.override` file to stop the service from starting.
    4. A malicious user restarted the service, so she needs to ensure users cannot restart services.

    Questions 9–12 refer to the following scenario and image.

    Bill is reviewing the authentication logs for a Linux system that he operates and encounters the following log entries:

    `Aug 30 09:46:54 ip-172-30-0-62 sshd[3051]: Accepted publickey for ec2-user from 10.174.238.88 port 57478 ssh2: RSA e5:f5:c1:46:bb:49:a1:43:da:9d:50:c5:37:bd:79:22 Aug 30 09:46:54 ip-172-30-0-62 ssh[3051]: pam_unix[sshd:session]: session opened for user ec2-user by (uid=0) Aug 30 09:48:06 ip-172-30-0-62 sudo: ec2-user : TTY=ps/0 ; PWD=/home/ec2-user ; USER=root; COMMAND=/bin/bash`Answer:

    C. Monica issued a command that only stops a running service. It will restart at reboot unless the scripts that start it are disabled. On modern Ubuntu systems, that is handled by upstart. Other services may use `init.d` scripts. In either case, when asked a question like this, you can quickly identify this as a problem that occurred at reboot and remove the answer that isn't likely to be correct.
9.  What is the IP address of the system where the user was logged in when they initiated the connection?

    1. 172.30.0.62
    2. 62.0.30.172
    3. 10.174.238.88
    4. 9.48.6.0

    Answer:

    C. The first entry in the log indicates that the user authenticated from the system 10.174.238.88.
10. What service did the user use to connect to the server?

    1. HTTPS
    2. PTS
    3. SSH
    4. Telnet

    Answer:

    C. The second log entry indicates that the `sshd` daemon handled the connection. This daemon supports the Secure Shell (SSH) protocol.
11. What authentication technique did the user use to connect to the server?

    1. Password
    2. PKI
    3. Token
    4. Biometric

    Answer:

    B. The first log entry indicates that the user made use of public key encryption (PKI) to authenticate the connection. The user, therefore, possessed the private key that corresponded to a public key stored on the server and associated with the user.
12. What account did the individual use to connect to the server?

    1. root
    2. ec2-user
    3. bash
    4. pam\_unix

    Answer:

    B. The identity of the user making the connection appears in the first log entry: `accepted publickey for ec2-user`. The third log entry that contains the string `USER=root` is recording the fact that the user issued the `sudo` command to create an interactive bash shell with administrative privileges. This is not the account used to create the server connection. The `pam_unix` entry indicates that the session was authenticated using the pluggable authentication module (PAM) facility.
13. Alaina adds the `openphish` URL list to her SOAR tool and sees the following entries:

    `http://13.126.65.8/DocExaDemo/uploads/index.php/bofa/bofa/95843de35406f3cab0b2dcf2b/success.htm http://13.126.65.8/DocExaDemo/uploads/index.php/bofa/bofa/9b094075409d3a723c7ee3d9e/sitekey.php http://13.126.65.8/DocExaDemo/uploads/index.php/bofa/bofa/9b094075409d3a723c7ee3d9e/success.htm http://13.126.65.8/DocExaDemo/uploads/index.php/bofa/bofa/9b094075409d3a723c7ee3d9e/ http://13.126.65.8/DocExaDemo/uploads/index.php/bofa/bofa/95843de35406f3cab0b2dcf2b/ http://13.126.65.8/DocExaDemo/uploads/index.php/bofa/bofa/95843de35406f3cab0b2dcf2b/sitekey.php`

    What action should she take based on phishing URLs like these?

    1. Block the IP address at her border firewall.
    2. Monitor for the IP address using her IDS.
    3. Delete emails with the URL from inbound email.
    4. Nothing, as these have not been confirmed.

    Answer:

    C. Alaina's best option is to delete emails with these URLs from all inbound email. Blocking or monitoring for the IP addresses can help, but mobile and offsite users will not be protected if they do not send their traffic through her firewall or IDSs.
14. Rowan wants to block drive-by-downloads and bot command-and-control channels while redirecting potentially impacted systems to a warning message. What should she implement to do this?

    1. A DNS sinkhole
    2. A WAF
    3. An IDS
    4. A UEBA

    Use the following table and rating information for questions 15–17.

    The U.S. Cybersecurity and Infrastructure Security Agency (CISA) uses a 1–100 scale for incident prioritization, with weight assigned to each of a number of categories. The functional impact score is weighted in their demonstration as follows:

    | Functional Impact                              | Rating |
    | ---------------------------------------------- | ------ |
    | No impact                                      | 0      |
    | No impact to services                          | 20     |
    | Minimal impact to noncritical services         | 35     |
    | Minimal impact to critical services            | 40     |
    | Significant impact to noncritical services     | 50     |
    | Denial of noncritical services                 | 60     |
    | Significant impact to critical services        | 70     |
    | Denial of critical services or loss of control | 100    |

    Answer:

    A. A DNS sinkhole exactly meets Rowan's needs. It can redirect traffic intended for malicious sites and botnet controllers to a landing page, which warns the end user that something went wrong.
15. Nathan discovers a malware package on an end-user workstation. What rating should he give this if he is considering organization impact based on the table shown?

    1. No impact
    2. No impact to services
    3. Denial of noncritical services
    4. Denial of critical services or loss of control

    Answer:

    B. It may be tempting to answer “no impact,” but the better answer here is “no impact to services.” The system will still require remediation, which will consume staff time, so there will not be a total lack of impact.
16. Nathan's organization uses a software-as-a-service (SaaS) tool to manage their customer mailing lists, which they use to inform customers of upcoming sales a week in advance. The organization's primary line of business software continues to function and merchandise can be sold. Because of a service outage, they are unable to add new customers to the list for a full business day. How should Nathan rate this local impact issue during the outage?

    1. Minimal impact to noncritical services
    2. Minimal impact to critical services
    3. Significant impact to noncritical services
    4. Denial of noncritical services

    Answer:

    D. The service is noncritical because it can be used to conduct business as usual after it is restored without a meaningful business impact due to the outage. During the outage, however, this is a denial of a noncritical service.
17. During an investigation into a compromised system, Nathan discovers signs of an advanced persistent threat (APT) resident in his organization's administrative systems. How should he classify this threat?

    1. Significant impact to noncritical services
    2. Denial of noncritical services
    3. Significant impact to critical services
    4. Denial of critical services or loss of control

    Answer:

    D. Discovering an APT in your administrative systems typically indicates that you have lost control of your environment.
18. Melissa is using the US-CERT's scale to measure the impact of the location of observed activity by a threat actor. Which of the following should be the highest rated threat activity location?

    1. Critical system screened subnet (DMZ)
    2. Business network
    3. Business screened subnet (DMZ)
    4. Safety systems

    Answer:

    D. Human safety and human lives are always the most critical system or resource. Here, safety systems should receive the highest rating, and in the US-CERT NCISS demo, they receive 100/100 points on the scale.
19. Derek's organization has been working to recover from a recent malware infection that caused outages across the organization during an important part of their business cycle. To properly triage, what should Derek pay the most attention to first?

    1. The immediate impact on operations so that his team can restore functionality
    2. The total impact of the event so that his team can provide an accurate final report
    3. The immediate impact on operations so that his team can identify the likely threat actor
    4. The total impact of the event so that his team can build a new threat model for future use

    Answer:

    A. During an event, incident responders often have to pay more attention to the immediate impact to triage and prioritize remediation. Once systems are back online and the business is operating, total impact can be assessed and should be included in the report and considered in new controls and practices from the lessons learned analysis of the event.
20. Jeff discovers multiple JPEG photos during his forensic investigation of a computer involved in an incident. When he runs `exiftool` to gather file metadata, which information is not likely to be part of the images even if they have complete metadata intact?

    1. GPS location
    2. Camera type
    3. Number of copies made
    4. Correct date/timestamp

    Answer:

    C. The amount of metadata included in photos varies based on the device used to take them, but GPS location, GPS timestamp-based time (and thus correct, rather than device native), and camera type can all potentially be found. Image files do not track how many times they have been copied!
21. John has designed his network as shown here and places untrusted systems that want to connect to the network into the Guests network segment. What is this type of segmentation called?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf002.jpg)

    1. Proactive network segmentation
    2. Isolation
    3. Quarantine
    4. Removal

    Answer:

    A. John is not responding to an incident, so this is an example of proactive network segmentation. If he discovered a system that was causing issues, he might create a dedicated quarantine network or could isolate or remove the system.
22. The organization that Jamal works for classifies security related events using NIST's standard definitions. Which classification should he use when he discovers key logging software on one of his frequent business travelers' laptop?

    1. An event
    2. An adverse event
    3. A security incident
    4. A policy violation

    Answer:

    C. NIST describes events like this as security incidents because they are a violation or imminent threat of violation of security policies and practices. An adverse event is any event with negative consequences, and an event is any observable occurrence on a system or network.
23. Dan is designing a segmented network that places systems with different levels of security requirements into different subnets with firewalls and other network security devices between them. What phase of the incident response process is Dan in?

    1. Post-incident activity
    2. Detection and analysis
    3. Preparation
    4. Containment, eradication, and recovery

    Answer:

    C. Dan's efforts are part of the preparation phase, which involves activities intended to limit the damage an attacker could cause.
24. Lauren wants to create a backup of Linux permissions before making changes to the Linux workstation she is attempting to remediate. What Linux tool can she use to back up the permissions of an entire directory on the system?

    1. She can use `chbkup`.
    2. She can use `getfacl`.
    3. She can use `aclman`.
    4. There is not a common Linux permission backup tool.

    Answer:

    B. Linux provides a pair of useful ACL backup and restore commands: `getfacl` allows recursive backups of directories, including all permissions to a text file, and `setfacl` restores those permissions from the backup file. Both `aclman` and `chbkup` were made up for this question.
25. While working to restore systems to their original configuration after a long-term APT compromise, Manish has three options.

    1. He can restore from a backup and then update patches on the system.
    2. He can rebuild and patch the system using original installation media and application software using his organization's build documentation.
    3. He can remove the compromised accounts and rootkit tools and then fix the issues that allowed the attackers to access the systems.

    Which option should Manish choose in this scenario?

    1. Option A.
    2. Option B.
    3. Option C.
    4. None of the above. Manish should hire a third party to assess the systems before proceeding.

    Answer:

    B. In cases where an advanced persistent threat (APT) has been present for an unknown period of time, backups should be assumed to be compromised. Since APTs often have tools that cannot be detected by normal anti-malware techniques, the best option that Manish has is to carefully rebuild the systems from the ground up and then ensure that they are fully patched and secured before returning them to service.
26. Jessica wants to access a macOS FileVault 2–encrypted drive. Which of the following methods is not a possible means of unlocking the volume?

    1. Change the FileVault key using a trusted user account.
    2. Retrieve the key from memory while the volume is mounted.
    3. Acquire the recovery key.
    4. Extract the keys from iCloud.

    Answer:

    A. FileVault does allow trusted accounts to unlock the drive but not by changing the key. FileVault 2 keys can be recovered from memory for mounted volumes, and much like BitLocker, it suggests that users record their recovery key, so Jessica may want to ask the user or search their office or materials if possible. Finally, FileVault keys can be recovered from iCloud, providing her with a third way to get access to the drive.
27. Susan discovers the following log entries that occurred within seconds of each other in her Squert (a Sguil web interface) console. What have her network sensors most likely detected?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf003.jpg)

    1. A failed database connection from a server
    2. A denial-of-service attack
    3. A port scan
    4. A misconfigured log source

    Answer:

    C. The series of connection attempts shown is most likely associated with a port scan. A series of failed connections to various services within a few seconds (or even minutes) is common for a port scan attempt. A denial-of-service attack will typically be focused on a single service, whereas an application that cannot connect will be configured to point at only one database service, not many. A misconfigured log source either would send the wrong log information or would not send logs at all in most cases.
28. If Suki wants to purge a drive, which of the following options will accomplish her goal?

    1. Cryptographic erase
    2. Reformat
    3. Overwrite
    4. Repartition

    Answer:

    A. Purging requires complete removal of data, and cryptographic erase is the only option that will fully destroy the contents of a drive from this list. Reformatting leaves the original data in place, overwriting leaves the potential for file remnants in slack space, and repartitioning also leaves data intact in the new partitions.
29. While performing post-rebuild validation efforts, Scott scans a server from a remote network and sees no vulnerabilities. Joanna, the administrator of the machine, runs a scan and discovers two critical vulnerabilities and five moderate issues. What is most likely causing the difference in their reports?

    1. Different patch levels were used during the scans.
    2. They are scanning through a load balancer.
    3. There is a firewall between the remote network and the server.
    4. Scott or Joanna ran the vulnerability scan with different settings.

    Answer:

    C. Local scans often provide more information than remote scans because of network or host firewalls that block access to services. The second most likely answer is that Scott or Joanna used different settings when they scanned.
30. As part of his organization's cooperation in a large criminal case, Adam's forensic team has been asked to send a forensic image of a highly sensitive compromised system in RAW format to an external forensic examiner. What steps should Adam's team take prior to sending a drive containing the forensic image?

    1. Encode in EO1 format and provide a hash of the original file on the drive.
    2. Encode in FTK format and provide a hash of the new file on the drive.
    3. Encrypt the RAW file and transfer a hash and key under separate cover.
    4. Decrypt the RAW file and transfer a hash under separate cover.

    Answer:

    C. A general best practice when dealing with highly sensitive systems is to encrypt copies of the drives before they are sent to third parties. Adam should encrypt the drive image and provide both the hash of the image and the decryption key under separate cover (sent via a separate mechanism) to ensure that losing the drive itself does not expose the data. Once the image is in the third-party examiner's hands, they will be responsible for its security. Adam may want to check on what their agreement says about security.
31. Mika wants to analyze the contents of a drive without causing any changes to the drive. What method is best suited to ensuring this?

    1. Set the “read-only” jumper on the drive.
    2. Use a write blocker.
    3. Use a read blocker.
    4. Use a forensic software package.

    Answer:

    B. A hardware write blocker can ensure that connecting or mounting the drive does not cause any changes to occur on the drive. Mika should create one or more forensic images of the original drive and then work with the copy or copies as needed. She may then opt to use forensic software, possibly including a software write blocker.
32. What type of forensic investigation–related form is shown here?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf004.jpg)

    1. Chain of custody
    2. Report of examination
    3. Forensic discovery log
    4. Policy custody release

    Answer:

    A. This form is a sample chain of custody form. It includes information about the case; copies of drives that were created; and who was in possession of drives, devices, and copies during the investigation.
33. James wants to determine whether other Windows systems on his network are infected with the same malware package that he has discovered on the workstation he is analyzing. He has removed the system from his network by unplugging its network cable, as required by corporate policy. He knows that the system has previously exhibited beaconing behavior and wants to use that behavior to identify other infected systems. How can he safely create a fingerprint for this beaconing without modifying the infected system?

    1. Plug the system into the network and capture the traffic quickly at the firewall using Wireshark or `tcpdump`.
    2. Plug the system into an isolated switch and use a span port or tap and Wireshark/`tcpdump` to capture traffic.
    3. Review the ARP cache for outbound traffic.
    4. Review the Windows Defender Firewall log for traffic logs.

    Answer:

    B. James can temporarily create an untrusted network segment and use a span port or tap to allow him to see traffic leaving the infected workstation. Using Wireshark or `tcpdump`, he can build a profile of the traffic it sends, helping him build a fingerprint of the beaconing behavior. Once he has this information, he can then use it in his recovery efforts to ensure that other systems are not similarly infected.
34. After completing an incident response process and providing a final report to management, what step should Casey use to identify improvement to her incident response plan?

    1. Update system documentation.
    2. Conduct a lessons learned session.
    3. Review patching status and vulnerability scans.
    4. Engage third-party consultants.

    Answer:

    B. Conducting a lessons learned review after using an incident response plan can help to identify improvements and to ensure that the plan is up-to-date and ready to handle new events.
35. During a forensic investigation, Lukas discovers that he needs to capture a virtual machine that is part of the critical operations of his company's website. If he cannot suspend or shut down the machine for business reasons, what imaging process should he follow?

    1. Perform a snapshot of the system, boot it, suspend the copied version, and copy the directory it resides in.
    2. Copy the virtual disk files and then use a memory capture tool.
    3. Escalate to management to get permission to suspend the system to allow a true forensic copy.
    4. Use a tool like the Volatility Framework to capture the live machine completely.

    Answer:

    B. If business concerns override his ability to suspend the system, the best option that Lukas has is to copy the virtual disk files and then use a live memory imaging tool. This will give him the best forensic copy achievable under the circumstances. Snapshotting the system and booting it will result in a loss of live memory artifacts. Escalating may be possible in some circumstances, but the scenario specifies that the system must remain online. Finally, volatility can capture memory artifacts but is not designed to capture a full virtual machine.
36. Mika, a computer forensic examiner, receives a PC and its peripherals that were seized as forensic evidence during an investigation. After she signs off on the chain of custody log and starts to prepare for her investigation, one of the first things she notes is that each cable and port was labeled with a color-coded sticker by the onsite team. Why are the items labeled like this?

    1. To ensure chain of custody
    2. To ensure correct reassembly
    3. To allow for easier documentation of acquisition
    4. To tamper-proof the system

    Answer:

    B. Reassembling the system to match its original configuration can be important in forensic investigations. Color-coding each cable and port as a system is disassembled before moving helps to ensure proper reassembly. Mika should also have photos taken by the onsite investigators to match her reassembly work to the onsite configuration.
37. While reviewing her Nagios logs, Selah discovers the error message shown here. What should she do about this error?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf005.jpg)

    1. Check for evidence of a port scan.
    2. Review the Apache error log.
    3. Reboot the server to restore the service.
    4. Restart the Apache service.

    Answer:

    B. Selah should check the error log to determine what web page or file access resulted in 404 “not found” errors. The errors may indicate that a page is linked incorrectly, but it may also indicate a scan occurring against her web server.
38. Lakshman needs to sanitize hard drives that will be leaving his organization after a lease is over. The drives contained information that his organization classifies as sensitive data that competitors would find valuable if they could obtain it. Which choice is the most appropriate to ensure that data exposure does not occur during this process?

    1. Clear, validate, and document.
    2. Purge the drives.
    3. Purge, validate, and document.
    4. The drives must be destroyed to ensure no data loss.

    Answer:

    C. Since the drives are being returned at the end of a lease, you must assume that the contract does not allow them to be destroyed. This means that purging the drives, validating that the drives have been purged, and documenting the process to ensure that all drives are included are the appropriate actions. Clearing the drives leaves the possibility of data recovery, while purging, as defined by NIST SP 800-88, renders data recovery infeasible.
39. Selah is preparing to collect a forensic image for a Macintosh computer running the Ventura operating system. What hard drive format is she most likely to encounter?

    1. FAT32
    2. MacFAT
    3. APFS
    4. HFS+

    Answer:

    C. The default macOS drive format is Apple File System (APFS) and is the native macOS drive format. macOS does support FAT32 and can read New Technology File System (NTFS) but cannot write to NTFS drives without additional software. HFS+ was the default file system for earlier versions of macOS.
40. During a forensic analysis of an employee's computer as part of a human resources investigation into misuse of company resources, Tim discovers a program called Eraser installed on the PC. What should Tim expect to find as part of his investigation?

    1. A wiped C: drive
    2. Antiforensic activities
    3. All slack space cleared
    4. Temporary files and Internet history wiped

    Answer:

    B. Eraser is a tool used to securely wipe files and drives. If Eraser is not typically installed on his organization's machines, Tim should expect that the individual being investigated has engaged in some antiforensic activities including wiping files that may have been downloaded or used against company policy. This doesn't mean he shouldn't continue his investigation, but he may want to look at Eraser's log for additional evidence of what was removed.
41. Jessica wants to recover deleted files from slack space and needs to identify where the files begin and end. What is this process called?

    1. Slacking
    2. Data carving
    3. Disk recovery
    4. Header manipulation

    Answer:

    B. Data carving is the process of identifying files based on file signatures such as headers and footers and then pulling the information between those locations out as a file. Jessica can use common carving tools or could manually carve files if she knows common header and footer types that she can search for.
42. Latisha is the IT manager for a small company and occasionally serves as the organization's information security officer. Who would be the most appropriate leader for her organization's CSIRT?

    1. Her lead IT support staff technician.
    2. Her organization's legal counsel.
    3. A third-party IR team lead.
    4. She should select herself.

    Answer:

    D. A CSIRT leader must have authority to direct the incident response process and should be able to act as a liaison with organizational management. Although Latisha may not have deep incident response experience, she is in the right role to provide those connections and leadership. She should look at retaining third-party experts for incidents if she needs additional skills or expertise on her IR team.
43. During her forensic analysis of a Windows system, Cynthia accesses the registry and checks `\\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsNT\CurrentVersion\Winlogin` (as shown here). What domain was the system connected to, and what was the username that would appear at login?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf006.jpg)

    1. Admin, administrator
    2. No domain, administrator
    3. Legal, admin
    4. Corporate, no default username

    Answer:

    B. This system is not connected to a domain (default domain name has no value), and the default user is administrator.
44. Alex suspects that an attacker has modified a Linux executable using static libraries. Which of the following Linux commands is best suited to determining whether this has occurred?

    1. `file`
    2. `stat`
    3. `strings`
    4. `grep`

    Answer:

    A. The Linux `file` command shows a file's format, encoding, what libraries it is linked to, and its file type (binary, ASCII text, etc.). Since Alex suspects that the attacker used statically linked libraries, the `file` command is the best command to use for this scenario. `stat` provides the last time accessed, permissions, UID and GID bit settings, and other details. It is useful for checking when a file was last used or modified but won't provide details about linked libraries. `strings` and `grep` are both useful for analyzing the content of a file and may provide Alex with other hints but won't be as useful as the `file` command for this purpose.
45. Because of external factors, Eric has only a limited time period to collect an image from a workstation. If he collects only specific files of interest, what type of acquisition has he performed?

    1. Logical
    2. Bit-by-bit
    3. Sparse
    4. None of the above

    Answer:

    A. A logical acquisition focuses on specific files of interest, such as a specific type of file or files from a specific location. In Eric's case, a logical acquisition meets his needs. A sparse acquisition also collects data from unallocated space. A bit-by-bit acquisition is typically performed for a full drive and will take longer.
46. During a forensic investigation, Kwame records information about each drive, including where it was acquired, who made the forensic copy, the MD5 hash of the drive, and other details. What term describes the process Kwame is using as he labels evidence with details of who acquired and validated it?

    1. Direct evidence
    2. Circumstantial evidence
    3. Incident logging
    4. Chain of custody

    Answer:

    D. The chain of custody for evidence is maintained by logging and labeling evidence. This ensures that the evidence is properly controlled and accessed.
47. Susan needs to perform forensics on a virtual machine. What process should she use to ensure she gets all of the forensic data she may need?

    1. Suspend the machine and copy the contents of the directory it resides in.
    2. Perform a live image of the machine.
    3. Suspend the machine and make a forensic copy of the drive it resides on.
    4. Turn the virtual machine off and make a forensic copy of it.

    Answer:

    A. Suspending a virtual machine will result in the RAM and disk contents being stored to the directory where it resides. Simply copying that folder is then sufficient to provide Susan with all the information she needs. She should not turn the virtual machine off, and creating a forensic copy of the drive is not necessary (but she should still validate hashes for the copied files or directory).
48. Allison wants to access Chrome logs as part of a forensic investigation. What format is information about cookies, history, and saved form responses saved in?

    1. SQLite
    2. Plain text
    3. Base64-encoded text
    4. NoSQL

    Answer:

    A. Chrome stores a broad range of useful forensic information in its SQLite database, including cookies, favicons, history, logins, top sites, web form data, and other details. Knowing how to write SQL queries or having access to a forensic tool that makes these databases easy to access can provide a rich trove of information about the web browsing history of a Chrome user.
49. While Chris is attempting to image a device, he encounters write issues and cannot write the image as currently set (refer to the image shown here). What issue is he most likely encountering?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf007.jpg)

    1. The files need to be compressed.
    2. The destination drive is formatted FAT32.
    3. The destination drive is formatted NTFS.
    4. The files are encrypted.

    Answer:

    B. FTK Imager Light is shown configured to write a single large file that will fail on FAT32-formatted drives where the largest single file is 4 GB. If Chris needs to create a single file, he should format his destination drive as NTFS. In many cases, he should simply create a raw image to a blank disk instead!
50. Saanvi needs to validate the MD5 checksum of a file on a Windows system to ensure that there were no unauthorized changes to the binary file. He is not allowed to install any programs and cannot run files from external media or drives. What Windows utility can he use to get the MD5 hash of the file?

    1. `md5sum`
    2. `certutil`
    3. `sha1sum`
    4. `hashcheck`

    Answer:

    B. Modern versions of Windows include the built-in `certutil` utility. Running `certutil -hashfile [file location] md5` will calculate the MD5 hash of a file. `certutil` also supports SHA1 and SHA256 as well as other less frequently used hashes. `md5sum` and `sha1sum` are Linux utilities, and `hashcheck` is a shell extension for Windows.
51. Forensic investigation shows that the target of an investigation used the Windows Quick Format command to attempt to destroy evidence on a USB thumb drive. Which of the NIST sanitization techniques has the target of the investigation used in their attempt to conceal evidence?

    1. Clear
    2. Purge
    3. Destroy
    4. None of the above

    Answer:

    D. The Windows Quick Format option leaves data in unallocated space on the new volume, allowing the data to be carved and retrieved. This does not meet the requirements for any of the three levels of sanitization defined by NIST.
52. During an incident response process, Susan plugs a system back into the network, allowing it normal network access. What phase of the incident response process is Susan performing?

    1. Preparation
    2. Detection and analysis
    3. Containment, eradication, and recovery
    4. Post-incident activity

    Answer:

    C. Restoring a system to normal function, including removing it from isolation, is part of the containment, eradication, and recovery stage. This may seem to be part of the post-incident activity phase, but that phase includes activities such as reporting and process updates rather than system restoration.
53. Mei's team has completed the initial phases of their incident response process and is assessing the time required to recover from the incident. Using the NIST recoverability effort categories, the team has determined that they can predict the time to recover but will require additional resources. How should she categorize this using the NIST model?

    1. Regular
    2. Supplemented
    3. Extended
    4. Not recoverable

    Answer:

    B. The NIST recoverability effort categories call a scenario in which time to recovery is predictable with additional resources “supplemented.” The key to the NIST levels is to remember that each level of additional unknowns and resources required increases the severity level from regular to supplemented and then to extended. A nonrecoverable situation exists when the event cannot be remediated, such as when data is exposed. At that point, an investigation is launched. In a nongovernment agency, this phase might involve escalating to law enforcement.
54. Janet is attempting to conceal her actions on a company-owned computer. As part of her cleanup attempts, she deletes all the files she downloaded from a corporate file server using a browser in incognito mode. How can a forensic investigator determine what files she downloaded?

    1. Network flows
    2. SMB logs
    3. Browser cache
    4. Drive analysis

    Answer:

    D. A forensic investigator's best option is to seize, image, and analyze the drive that Janet downloaded the files to. Since she only deleted the files, it is likely that the investigator will be able to recover most of the content of the files, allowing them to be identified. Network flows do not provide file information, SMB does not log file downloads, browser caches will typically not contain a list of all downloaded files, and incognito mode is specifically designed to not retain session and cache information.
55. Jose is aware that an attacker has compromised a system on his network but wants to continue to observe the attacker's efforts as they continue their attack. If Jose wants to prevent additional impact on his network while watching what the attacker does, what containment method should he use?

    1. Removal
    2. Isolation
    3. Segmentation
    4. Detection

    Answer:

    B. Jose can choose to isolate the compromised system, either physically or logically, leaving the attacker with access to the system while isolating it from other systems on his network. If he makes a mistake, he could leave his own systems vulnerable, but this will allow him to observe the attacker.
56. When Abdul arrived at work this morning, he found an email in his inbox that read, “Your systems are weak; we will own your network by the end of the week.” How would he categorize this sign of a potential incident if he was using the NIST SP 800-61 descriptions of incident signs?

    1. An indicator
    2. A threat
    3. A risk
    4. A precursor

    Answer:

    D. NIST SP 800-61 categorizes signs of an incident into two categories, precursors and indicators. Precursors are signs that an incident may occur in the future. Since there is not an indicator that an event is in progress, this can be categorized as a precursor. Now Abdul needs to figure out how he will monitor for a potential attack.
57. During an incident response process, Cynthia conducts a lessons learned review. What phase of the incident response process is she in?

    1. Preparation
    2. Detection and analysis
    3. Containment, eradication, and recovery
    4. Post-incident recovery

    Answer:

    D. Lessons learned reviews are typically conducted by independent facilitators who ask questions like “What happened, and at what time?” and “What information was needed, and when?” Lessons learned reviews are conducted as part of the post-incident activity stage of incident response and provide an opportunity for organizations to improve their incident response process.
58. As part of his incident response program, Allan is designing a playbook for zero-day threats. Which of the following should not be in his plan to handle them?

    1. Segmentation
    2. Patching
    3. Using threat intelligence
    4. Allow listing/whitelisting

    Answer:

    B. Although patching is useful, it won't stop zero-day threats. If Allan is building a plan specifically to deal with zero-day threats, he should focus on designing his network and systems to limit the possibility and impact of an unknown vulnerability. That includes using threat intelligence, using segmentation, using allow listing/whitelisting applications, implementing only necessary firewall rules, using behavior and baseline-based intrusion prevention rules and SIEM alerts, and building a plan in advance.
59. As the CISO of her organization, Mei is working on an incident classification scheme and wants to base her design on NIST's definitions. Which of the following options should she use to best describe a user accessing a file that they are not authorized to view?

    1. An incident
    2. An event
    3. An adverse event
    4. A security incident

    Answer:

    C. NIST describes events with negative consequences as adverse events. It might be tempting to immediately call this a security incident; however, this wouldn't be classified that way until an investigation was conducted. If the user accidentally accessed the file, it would typically not change classification. Intentional or malicious access would cause the adverse event to become a security incident.
60. Fred wants to identify digital evidence that can place an individual in a specific place at a specific time. Which of the following types of digital forensic data is not commonly used to attempt to document physical location at specific times?

    1. Cell phone GPS logs
    2. Photograph metadata
    3. Cell phone tower logs
    4. Microsoft Office document metadata

    Answer:

    D. Cell phones contain a treasure trove of location data, including both tower connection log data and GPS location logs in some instances. Photographs taken on mobile devices may also include location metadata. Microsoft Office files do not typically include location information.

    Other potential sources of data include car GPS systems if the individual has a car with built-in GPS, black-box data-gathering systems, social media posts, and fitness software, as well as any other devices that may have built-in GPS or location detection capabilities. In some cases, this can be as simple as determining whether the individual's devices were connected to a specific network at a specific time.
61. Kai has completed the validation process of her media sanitization efforts and has checked a sample of the drives she had purged using a built-in cryptographic wipe utility. What is her next step?

    1. Resample to validate her testing.
    2. Destroy the drives.
    3. Create documentation.
    4. She is done and can send the drives on for disposition.

    Answer:

    C. Documentation is important when tracking drives to ensure that all drives that should be sanitized are being received. Documentation can also provide evidence of proper handling for audits and internal reviews.
62. In his role as a small company's information security manager, Mike has a limited budget for hiring permanent staff. Although his team can handle simple virus infections, he does not currently have a way to handle significant information security incidents. Which of the following options should Mike investigate to ensure that his company is prepared for security incidents?

    1. Outsource to a third-party SOC.
    2. Create an internal SOC.
    3. Hire an internal incident response team.
    4. Outsource to an incident response provider.

    Answer:

    D. Outsourcing to a third-party incident response provider allows Mike to bring in experts when an incident occurs while avoiding the day-to-day expense of hiring a full-time staff member. This can make a lot of financial sense if incidents occur rarely, and even large organizations bring in third-party response providers when large incidents occur. A security operations center (SOC) would be appropriate if Mike needed day-to-day security monitoring and operations, and hiring an internal team does not match Mike's funding model limitations in this scenario.
63. Bohai wants to ensure that media has been properly sanitized. Which of the following options properly lists sanitization descriptions from least to most effective?

    1. Purge, clear, destroy
    2. Eliminate, eradicate, destroy
    3. Clear, purge, destroy
    4. Eradicate, eliminate, destroy

    Answer:

    C. NIST identifies three activities for media sanitization: clearing, which uses logical techniques to sanitize data in all user-addressable storage locations; purging, which applies physical or logical techniques to render data recovery infeasible using state-of-the-art laboratory techniques; and destruction, which involves physically destroying the media.
64. Degaussing is an example of what form of media sanitization?

    1. Clearing.
    2. Purging.
    3. Cryptoshredding.
    4. It is not a form of media sanitization.

    Answer:

    B. Degaussing, which uses a powerful electromagnet to remove data from tape media, is a form of purging.
65. While reviewing storage usage on a Windows system, Brian checks the volume shadow copy storage as shown here:

    `C:\WINDOWS\system32>vssadmin list Shadowstorage vssadmin 1.1 - Volume Shadow Copy Service administrative command-line tool (C) Copyright 2001-2013 Microsoft Corp. Shadow Copy Storage association For volume: (C:)\\?\Volume{c3b53dae-0e54-13e3-97ab-806e6f6e69633}\ Shadow Copy Storage volume: (C:)\\?\Volume{c3b53dae-0e54-13e3-97ab-806e6f6e6963}\ Used Shadow Copy Storage space: 25.6 GB (2%) Allocated Shadow Copy Storage space: 26.0 GB (2%) Maximum Shadow Copy Storage space: 89.4 GB (10%)`

    What purpose does this storage serve, and can he safely delete it?

    1. It provides a block-level snapshot and can be safely deleted.
    2. It provides secure hidden storage and can be safely deleted.
    3. It provides secure hidden storage and cannot be safely deleted.
    4. It provides a block-level snapshot and cannot be safely deleted.

    Answer:

    A. As long as Brian is comfortable relying on another backup mechanism, he can safely disable volume shadow copies and remove the related files. For the drive he is looking at, this will result in approximately 26 GB of storage becoming available.
66. Lauren recovers a number of 16GB and 32GB microSD cards during a forensic investigation. Without checking them manually, what filesystem type is she most likely to find them formatted in as if they were used with a digital camera?

    1. RAW
    2. FAT16
    3. FAT32
    4. APFS

    Answer:

    C. Most portable consumer devices, especially those that generate large files, format their storage as FAT32. FAT16 is limited to 2 GB partitions, RAW is a photo file format, and APFS is the native macOS file system format. Lauren can expect most devices to format media as FAT32 by default because of its broad compatibility across devices and operating systems.
67. After arriving at an investigation site, Brian determines that three powered-on computers need to be taken for forensic examination. What steps should he take before removing the PCs?

    1. Power them down, take pictures of how each is connected, and log each system in as evidence.
    2. Take photos of each system, power them down, and attach a tamper-evident seal to each PC.
    3. Collect live forensic information, take photos of each system, and power them down.
    4. Collect a static drive image, validate the hash of the image, and securely transport each system.

    Answer:

    C. Brian should determine whether he needs live forensic information, but if he is not certain, the safest path for him is to collect live forensic information, take photos so that he knows how each system was set up and configured, and then power them down. He would then log each system as evidence and will likely create forensic copies of the drives once he reaches his forensic work area or may use a portable forensic system to make drive images onsite. Powering a running system down can result in the loss of significant forensic information, meaning that powering a system down before collecting some information is typically not recommended. Collecting a static image of a drive requires powering the system down first.
68. In his role as a forensic examiner, Lukas has been asked to produce forensic evidence related to a civil case. What is this process called?

    1. Criminal forensics
    2. E-discovery
    3. Cyber production
    4. Civil tort

    Answer:

    B. When forensic evidence or information is produced for a legal proceeding, it is called e-discovery. This type of discovery often involves massive amounts of data, including email, files, text messages, and any other electronic evidence that is relevant to the case.
69. As Mika studies her company's computer forensics playbook, she notices that forensic investigators are required to use a chain of custody form. Which of the following best describes the information that she should record on that form if she was conducting a forensic investigation?

    1. The list of individuals who made contact with files leading to the investigation
    2. The list of former owners or operators of the PC involved in the investigation
    3. All individuals who work with evidence in the investigation
    4. The police officers who take possession of the evidence

    Answer:

    C. A chain of custody form is used to record each person who works with or is in contact with evidence in an investigation. Typically, investigative work is also done in a way that fully records all actions taken and sometimes requires two people present to verify actions taken.
70. Scott needs to ensure that the system he just rebuilt after an incident is secure. Which type of scan will provide him with the most useful information to meet his goal?

    1. An authenticated vulnerability scan from a trusted internal network
    2. An unauthenticated vulnerability scan from a trusted internal network
    3. An authenticated scan from an untrusted external network
    4. An unauthenticated scan from an untrusted external network

    Answer:

    A. Since Scott needs to know more about potential vulnerabilities, an authenticated scan from a trusted internal network will provide him with the most information. He will not gain a real attacker's view, but in this case, having more detail is important.
71. What is the primary role of management in the incident response process?

    1. Leading the CSIRT
    2. Acting as the primary interface with law enforcement
    3. Providing authority and resources
    4. Assessing impact on stakeholders

    Answer:

    C. The primary role of management in an incident response effort is to provide the authority and resources required to respond appropriately to the incident. They may also be asked to make business decisions, communicate with external groups, or assess the impact on key stakeholders.
72. Max wants to improve the effectiveness of the incident analysis process he is responsible for as the leader of his organization's CSIRT. Which of the following is not a commonly recommended best practice based on NIST's guidelines?

    1. Profile networks and systems to measure the characteristics of expected activity.
    2. Perform event correlation to combine information from multiple sources.
    3. Maintain backups of every system and device.
    4. Capture network traffic as soon as an incident is suspected.

    Answer:

    C. NIST does not include making backups of every system and device in its documentation. Instead, NIST suggests maintaining an organizationwide knowledge base with critical information about systems and applications. Backing up every device and system can be prohibitively expensive. Backups are typically done only for specific systems and devices, with configuration and restoration data stored for the rest.
73. NIST describes four major phases in the incident response cycle. Which of the following is not one of the four?

    1. Containment, eradication, and recovery
    2. Notification and communication
    3. Detection and analysis
    4. Preparation

    Answer:

    B. NIST identifies four major phases in the IR life cycle: preparation; detection and analysis; containment, eradication, and recovery; and post-incident activity. Notification and communication may occur in multiple phases.
74. Charles wants to perform memory forensics on a Windows system and wants to access `pagefile.sys`. When he attempts to copy it, he receives the following error. What access method is required to access the page file?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf008.jpg)

    1. Run Windows File Explorer as an administrator and repeat the copy.
    2. Open the file using `fmem`.
    3. Run `cmd.exe` as an administrator and repeat the copy.
    4. Shut the system down, remove the drive, and copy it from another system.

    Answer:

    D. The page file, like many system files, is locked while Windows is running. Charles simply needs to shut down the system and copy the page file. Some Windows systems may be set to purge the page file when the system is shut down, so he may need to pull the plug to get an intact page file.
75. Where is slack space found in the following Windows partition map?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf009.jpg)

    1. The System Reserved partition
    2. The System Reserved and Unallocated partitions
    3. The System Reserved and `C:` partitions
    4. The `C:` and unallocated partitions

    Answer:

    C. Slack space is leftover storage that exists because files do not take up the entire space allocated for them. Since the Unallocated partition does not have a filesystem on it, space there should not be considered slack space. Both System Reserved and C: are formatted with NTFS and will have slack space between files.
76. Ty needs to determine the proper retention policy for his organization's incident data. If he wants to follow common industry practices and does not have specific legal or contractual obligations that he needs to meet, what timeframe should he select?

    1. 30 days
    2. 90 days
    3. 1 to 2 years
    4. 7 years

    Answer:

    C. Without other requirements in place, many organizations select a one- to two-year retention period. This allows enough time to use existing information for investigations but does not retain so much data that it cannot be managed. Regardless of the time period selected, organizations should set and consistently follow a retention policy.
77. The system that Alice has identified as the source of beaconing traffic is one of her organization's critical e-commerce servers. To maintain her organization's operations, she needs to quickly restore the server to its original, uncompromised state. What criterion is likely to be impacted the most by this action?

    1. Damage to the system or service
    2. Service availability
    3. Ability to preserve evidence
    4. Time and resources needed to implement the strategy

    Answer:

    C. If Alice focuses on a quick restoration, she is unlikely to preserve all of the evidence she would be able to during a longer incident response process. Since she is focusing on quick restoration, the service should be available more quickly, and the service and system should not be damaged in any significant way by the restoration process. The time required to implement the strategy will typically be less if she does not conduct a full forensic investigation and instead focuses on service restoration.
78. Piper wants to create a forensic image that third-party investigators can use but does not know what tool the third-party investigation team that her company intends to engage will use. Which of the following forensic formats should she choose if she wants almost any forensic tool to be able to access the image?

    1. E01
    2. AFF
    3. RAW
    4. AD1

    Answer:

    C. A RAW image, like those created by `dd`, is Piper's best option for broad compatibility. Many forensic tools support multiple image formats, but RAW files are supported almost universally by forensic tools.
79. As part of his forensic investigation, Scott intends to make a forensic image of a network share that is mounted by the PC that is the focus of his investigation. What information will he be unable to capture?

    1. File creation dates
    2. Deleted files
    3. File permission data
    4. File metadata

    Answer:

    B. When a network share or mounted drive is captured from the system that mounts it, data such as deleted files, unallocated space, and other information that requires direct drive access will not be captured. If Scott needs that information, he will need to create a forensic image of the drive from the host server.
80. What common incident response follow-up activity includes asking questions like “What additional tools or resources are needed to detect or analyze future events?”

    1. Preparation
    2. Lessons learned review
    3. Evidence gathering
    4. Procedural analysis

    Answer:

    B. Questions including what tools and resources are needed to detect, analyze, or mitigate figure incidents, as well as topics such as how information sharing could be improved, what could be done better or differently, and how effective existing processes and policies are, can all be part of the lessons learned review.
81. Suki has been asked to capture forensic data from a Windows PC and needs to ensure that she captures the data in their order of volatility. Which order is correct from most to least volatile?

    1. Network traffic, CPU cache, disk drives, optical media
    2. CPU cache, network traffic, disk drives, optical media
    3. Optical media, disk drives, network traffic, CPU cache
    4. Network traffic, CPU cache, optical media, disk drives

    Answer:

    B. The order of volatility for common storage locations is as follows:

    1. CPU cache, registers, running processes, RAM
    2. Network traffic
    3. Disk drives
    4. Backups, printouts, optical media
82. During an incident response process, Suki heads to a compromised system and disconnects its network cable. What phase of the incident response process is Suki performing?

    1. Preparation
    2. Detection and analysis
    3. Containment, eradication, and recovery
    4. Post-incident activity

    Answer:

    C. Removing a system from the network typically occurs as part of the containment phase of an incident response process. Systems are typically not returned to the network until the end of the recovery phase.
83. Scott needs to verify that the forensic image he has created is an exact duplicate of the original drive. Which of the following methods is considered forensically sound?

    1. Create a MD5 hash
    2. Create a SHA-1 hash
    3. Create a SHA-2 hash
    4. All of the above

    Answer:

    D. MD5, SHA-1, and SHA-2 hashes are all considered forensically sound. Although MD5 and SHA-1 hashes are no longer a secure means of hashing, they are still considered appropriate for validation of forensic images because it is unlikely that an attacker would intentionally create a hash collision to falsify the forensic integrity of a drive.
84. What strategy does NIST suggest for identifying attackers during an incident response process?

    1. Use geographic IP tracking to identify the attacker's location.
    2. Contact upstream ISPs for assistance in tracking down the attacker.
    3. Contact local law enforcement so that they can use law enforcement–specific tools.
    4. Identifying attackers is not an important part of the incident response process.

    Answer:

    D. NIST's Computer Security Incident Handling Guide notes that identifying an attacker can be “time-consuming and futile.” In general, spending time identifying attackers is not a valuable use of incident response time for most organizations.
85. While performing forensic analysis of an iPhone backup, Cynthia discovers that she has only some of the information that she expects the phone to contain. What is the most likely scenario that would result in the backup she is using having partial information?

    1. The backup was interrupted.
    2. The backup is encrypted.
    3. The backup is a differential backup.
    4. The backup is stored in iCloud.

    Answer:

    C. iPhone backups to local systems can be full or differential, and in this scenario the most likely issue is that Cynthia has recovered a differential backup. She should look for additional backup files if she does not have access to the original phone. If the backup was encrypted, she would not be able to access it without a cracking tool, and if it was interrupted, she would be unlikely to have the backup file or have it be in usable condition. iCloud backups require access to the user's computer or account and are less likely to be part of a forensic investigation.
86. Cullen wants to ensure that his chain of custody documentation will stand up to examination in court. Which of the following options will provide him with the best documentary proof of his actions?

    1. A second examiner acting as a witness and countersigning all actions
    2. A complete forensic logbook signed and sealed by a notary public
    3. A documented forensic process with required sign-off
    4. Taking pictures of all independent forensic actions

    Answer:

    A. A second forensic examiner who acts as a witness, countersigning all documentation and helping document all actions, provides both strong documentation and another potential witness in court. Independent forensic action, no matter how well documented, will not be as reliable as having a witness.
87. Cynthia is reviewing her organization's incident response recovery process, which is outlined here. Which of the following recommendations should she make to ensure that further issues do not occur during the restoration process?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf010.jpg)

    1. Change passwords before restoring from backup.
    2. Isolate the system before restoring from backups.
    3. Securely wipe the drive before restoration.
    4. Vulnerability scan before patching.

    Answer:

    B. Although it may seem obvious that the system should be isolated from the network when it is rebuilt, we have seen this exact scenario play out before. In one instance, the system was compromised twice before the system administrator learned their lesson!
88. Saria is reviewing the contents of a drive as part of a forensic effort and notes that the file she is reviewing takes up more space on the disk than its actual size, as shown here. What has she discovered?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf011.jpg)

    1. Slack space
    2. Hidden content
    3. Sparse files
    4. Encryption overhead

    Answer:

    A. The space that Saria sees is the space between the end of the file and the space allocated per cluster or block. This space may contain remnants of previous files written to the cluster or block or may simply contain random data from when the disk was formatted or initialized.
89. Kathleen is restoring a critical business system to operation after a major compromise and needs to validate that the operating system and application files are legitimate and do not have any malicious code included in them. What type of tool should she use to validate this?

    1. A trusted system binary kit
    2. Dynamic code analysis
    3. Static code analysis
    4. File rainbow tables

    Answer:

    A. Trusted system binary kits like those provided by the National Software Reference Library include known good hashes of many operating systems and applications. Kathleen can validate the files on her system using references like the NSRL ([`www.nsrl.nist.gov/new.html`](http://www.nsrl.nist.gov/new.html)).
90. Mel is creating the evidence log for a computer that was part of an attack on an external third-party system. What network-related information should he include in that log if he wants to follow NIST's recommendations?

    1. Subnet mask, DHCP server, hostname, MAC address
    2. IP addresses, MAC addresses, hostname
    3. Domain, hostname, MAC addresses, IP addresses
    4. NIC manufacturer, MAC addresses, IP addresses, DHCP configuration

    Answer:

    B. NIST specifically recommends the hostname, MAC addresses, and IP addresses of the system. Capturing the full output of an `ipconfig` or `ifconfig` command may be useful, but forensic analysis may not permit interaction with a live machine. Additional detail like the domain (or domain membership) may or may not be available for any given machine, and NIC manufacturer and similar data is not necessary under most circumstances.
91. Ryan believes that systems on his network have been compromised by an advanced persistent threat actor. He has observed a number of large file transfers outbound to remote sites via TLS-protected HTTP sessions from systems that do not typically send data to those locations. Which of the following techniques is most likely to detect the APT infections?

    1. Network traffic analysis
    2. Network forensics
    3. Endpoint behavior analysis
    4. Endpoint forensics

    Answer:

    D. Since most APTs (including this one, as specified in the question) send traffic in an encrypted form, performing network forensics or traffic analysis will only provide information about potentially infected hosts. If Ryan wants to find the actual tools that may exist on endpoint systems, he should conduct endpoint forensics. Along the way, he may use endpoint behavior analysis, network forensics, and network traffic analysis to help identify target systems.
92. Ben is investigating a potential malware infection of a laptop belonging to a senior manager in the company he works for. When the manager opens a document, website, or other application that takes user input, words start to appear as though they are being typed. What is the first step that Ben should take in his investigation?

    1. Run an antivirus scan.
    2. Disconnect the system from the network.
    3. Wipe the system and reinstall.
    4. Observe and record what is being typed.

    Answer:

    B. When a system is not a critical business asset that must remain online, the best response is typically to isolate it from other systems and networks that it could negatively impact. By disconnecting it from all networks, Ben can safely investigate the issue without causing undue risk.

    We have actually encountered this situation. After investigating, we found that the user's text-to-speech application was enabled, and the microphone had the gain turned all the way up. The system was automatically typing words based on how it interpreted background noise, resulting in strange text that terrified the unsuspecting user.
93. Kathleen's forensic analysis of a laptop that is believed to have been used to access sensitive corporate data shows that the suspect tried to overwrite the data they downloaded as part of antiforensic activities by deleting the original files and then copying other files to the drive. Where is Kathleen most likely to find evidence of the original files?

    1. The MBR
    2. Unallocated space
    3. Slack space
    4. The FAT

    Answer:

    C. When clusters are overwritten, original data is left in the unused space between the end of the new file and the end of the cluster. This means that copying new files over old files can leave remnant data that may help Kathleen prove that the files were on the system by examining slack space.
94. Angela wants to access the decryption key for a BitLocker-encrypted system, but the system is currently turned off. Which of the following methods is a viable method if a Windows system is turned off?

    1. Hibernation file analysis
    2. Memory analysis
    3. Boot-sector analysis
    4. Brute-force cracking

    Answer:

    A. If the system that Angela is attempting to access had mounted the encrypted volume before going to sleep and there is a hibernation file, Angela can use hibernation file analysis tools to retrieve the BitLocker key. If the system did not hibernate or the volume was not mounted when the system went to sleep, she will not be able to retrieve the keys. Memory analysis won't work with a system that is off, the boot sector does not contain keys, and brute-force cracking is not a viable method of cracking BitLocker keys because of the time involved.
95. Adam believes that a system on his network is infected but does not know which system. To detect it, he creates a query for his network monitoring software based on the following pseudocode. What type of traffic is he most likely trying to detect?

    `destip: [*] and duration < 10 packets and destbytes < 3000 and flowcompleted = true and application = http or https or tcp or unknown and content != uripath:* and content != contentencoding:*`

    1. Users browsing malicious sites
    2. Adware
    3. Beaconing
    4. Outbound port scanning

    Answer:

    C. The pseudocode tells you that Adam is trying to detect outbound packets that are part of short communications (fewer than 10 packets and fewer than 3,000 bytes) and that he believes the traffic may appear to be web traffic, be general TCP traffic, or not match known traffic types. This is consistent with the attributes of beaconing traffic. Adam also is making sure that general web traffic won't be captured by not matching on `uripath` and `contentencoding`.
96. As an employee of the U.S. government, Megan is required to use NIST's information impact categories to classify security incidents. During a recent incident, proprietary information was changed. How should she classify this incident?

    1. As a privacy breach
    2. As an integrity loss
    3. As a proprietary breach
    4. As an availability breach

    Answer:

    B. NIST classifies changes or deletion of sensitive or proprietary information as an integrity loss. Proprietary breaches occur when unclassified proprietary information is accessed or exfiltrated, and privacy breaches involve personally identifiable information (PII) that is accessed or exfiltrated.
97. During what stage of an event is preservation of evidence typically handled?

    1. Preparation
    2. Detection and analysis
    3. Containment, eradication, and recovery
    4. Post-incident activity

    Answer:

    C. Although responders are working to contain the incident, they should also preserve forensic and incident information for future analysis. Restoration of service is often prioritized over analysis during containment activities, but taking the time to create forensic images and to preserve log and other data is important for later investigation.
98. Lukas wants to purge a drive to ensure that data cannot be extracted when it is sent offsite. Which of the following is not a valid option for purging hard drives on a Windows system?

    1. Use the built-in Windows `sdelete` command line.
    2. Use Eraser.
    3. Use DBAN.
    4. Encrypt the drive and then delete the key.

    Answer:

    A. Windows does not include a built-in secure erase tool in the GUI or at the command line. Using a third-party program like Eraser or a bootable tool like DBAN is a reasonable option, and encrypting the entire drive and then deleting the key will have the same effect.
99. Which of the following is not a valid use case for live forensic imaging?

    1. Malware analysis
    2. Encrypted drives
    3. Postmortem forensics
    4. Nonsupported filesystems

    Answer:

    C. Postmortem forensics can typically be done after shutting down systems to ensure that a complete forensic copy is made. Live forensic imaging can help to capture memory-resident malware. It can also aid in the capture of encrypted drives and filesystems when they are decrypted for live usage. Finally, unsupported filesystems can sometimes be imaged while the system is booted by copying data off the system to a supported filesystem type. This won't retain some filesystem-specific data but can allow key forensic activities to take place.
100.    While reviewing the actions taken during an incident response process, Mei is informed by the local desktop support staff person that the infected machine was returned to service by using a Windows System Restore point. Which of the following items will a Windows System Restore return to a previous state?

        1. Personal files
        2. Malware
        3. Windows system files
        4. All installed apps

        Answer:

        C. A Windows System Restore should not be used to rebuild a system after an infection or compromise since it restores only Windows system files, some program files, registry settings, and hardware drivers. This means that personal files and most malware, as well as programs installed or modifications to programs after the restore point is created, will not be restored.
101.    During a major incident response effort, Kobe discovers evidence that a critical application server may have been the data repository and egress point in the compromise he is investigating. If he is unable to take the system offline, which of the following options will provide him with the best forensic data?

        1. Reboot the server and mount the system drive using a USB-bootable forensic suite.
        2. Create an image using a tool like FTK Imager Lite.
        3. Capture the system memory using a tool like Volatility.
        4. Install and run an imaging tool on the live server.

        Answer:

        B. Portable imaging tools like FTK Imager Lite can be run from removable media, allowing a live image to be captured. Kobe may still want to capture the system memory as well, but when systems are used for data gathering and egress, the contents of the disk will be important. Installing a tool or taking the system offline and mounting the drive are both undesirable in this type of scenario when the system must stay online and should not be modified.
102.    Manish finds the following entries on a Linux system in `/var/log/auth.log`. If he is the only user with root privileges, requires two-factor authentication to log in as root, and did not take the actions shown, what should he check for?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf012.jpg)

        1. A hacked root account
        2. A privilege escalation attack from a lower privileged account or service
        3. A malware infection
        4. A RAT

        Answer:

        B. If Manish has good reason to believe he is the only person with root access to the system, he should look for a privilege escalation attack. A remote access trojan would not directly provide root access, and a hacked root account is less likely than a privilege escalation attack. A malware infection is possible, and privilege escalation would be required to take the actions shown.
103.    As part of his forensic analysis of a series of photos, John runs `exiftool` for each photo. He receives the following listing from one photo. What useful forensic information can he gather from this photo?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf013.jpg)

        1. The original creation date, the device type, the GPS location, and the creator's name
        2. The endian order of the file, the file type, the GPS location, and the scene type
        3. The original creation date, the device type, the GPS location, and manufacturer of the device
        4. The MIME type, the GPS time, the GPS location, and the creator's name

        Answer:

        C. The original creation date (as shown by the GPS date), the device type (an iPhone X), the GPS location, and the manufacturer of the device (Apple) can all provide useful forensic information. Here, you know when the photo was taken, where it was taken, and what type of device it was taken on. This can help narrow down who took the photo or may provide other useful clues when combined with other forensic information or theories.
104.    During the preparation phase of his organization's incident response process, Oscar gathers a laptop with useful software including a sniffer and forensics tools, thumb drives and external hard drives, networking equipment, and a variety of cables. What is this type of preprepared equipment commonly called?

        1. A grab bag
        2. A jump kit
        3. A crash cart
        4. A first responder kit

        Answer:

        B. A jump kit is a common part of an incident response plan and provides responders with the tools they will need without having to worry about where key pieces of equipment are during a stressful time. Crash carts are often used in datacenters to connect a keyboard, mouse, and monitor to a server to work on it. First-responder kits are typically associated with medical responders, and a grab bag contains random items.
105.    As John proceeds with a forensic investigation involving numerous images, he finds a directory labeled `Downloaded from Facebook`. The images appear relevant to his investigation, so he processes them for metadata using `exiftool`. The following image shows the data provided. What forensically useful information can John gather from this output?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf014.jpg)

        1. The original file creation date and time.
        2. The device used to capture the image.
        3. The original digest (hash) of the file, allowing comparison to the original.
        4. None; Facebook strips almost all useful metadata from images.

        Answer:

        D. Facebook, as well as many other social media sites, now strip image metadata to help protect user privacy. John would need to locate copies of the photos that have not had the metadata removed and may still find that they did not contain additional useful data.
106.    Which of the following properly lists the order of volatility from least to most volatile?

        1. Printouts, swap files, CPU cache, RAM
        2. Hard drives, USB media, DVDs, CD-RWs
        3. DVDs, hard drives, virtual memory, caches
        4. RAM, swap files, SSDs, printouts

        Answer:

        C. The order of volatility for media from least to most volatile is often listed as backups and printouts; then disk drives like hard drives and SSDs; then virtual memory; and finally CPU cache, registers, and RAM. Artifacts stored in each of these locations can be associated with the level of volatility of that storage mechanism. For example, routing tables will typically be stored in RAM, making them highly volatile. Data stored on a rewritable media is always considered more volatile than media stored on a write-only media.
107.    While conducting a forensic review of a system involved in a data breach, Alex discovers a number of Microsoft Word files including files with filenames like `critical_data.docx` and `sales_estimates_2023.docx`. When he attempts to review the files using a text editor for any useful information, he finds only unreadable data. What has occurred?

        1. Microsoft Word files are stored in ZIP format.
        2. Microsoft Word files are encrypted.
        3. Microsoft Word files can be opened only by Microsoft Word.
        4. The user has used antiforensic techniques to scramble the data.

        Answer:

        A. Modern Microsoft Office files are actually stored in a ZIP format. Alex will need to open them using a utility that can unzip them before he can manually review their contents. He may want to use a dedicated Microsoft Office forensics tool or a forensics suite with built-in support for Office documents.
108.    Lukas believes that one of his users has attempted to use built-in Windows commands to probe servers on the network he is responsible for. How can he recover the command history for that user if the system has been rebooted since the reconnaissance has occurred?

        1. Check the Bash history.
        2. Open a command prompt window and press F7.
        3. Manually open the command history from the user's profile directory.
        4. The Windows command prompt does not store command history.

        Answer:

        D. Once a command prompt window has been closed on a Windows system, the command history is erased. If Lukas could catch the user with an open command prompt, he could press F7 and see the command history.
109.    Angela is conducting an incident response exercise and needs to assess the economic impact on her organization of a $500,000 expense related to an information security incident. How should she categorize this?

        1. Low impact.
        2. Medium impact.
        3. High impact.
        4. Angela cannot assess the impact with the data given.

        Answer:

        D. Economic impact is calculated on a relative scale, and Angela does not have all of the information she needs. A $500,000 loss may be catastrophic for a small organization and may have a far lower impact on a Fortune 500 company. Other factors like cybersecurity insurance may also limit the economic impact of a cybersecurity incident.
110.    What step follows sanitization of media according to NIST guidelines for secure media handling?

        1. Reuse
        2. Validation
        3. Destruction
        4. Documentation

        Answer:

        B. The NIST guidelines require validation after clearing, purging, or destroying media to ensure that the action that was taken is effective. This is an important step since improperly applying the sanitization process and leaving data partially or even fully intact can lead to a data breach.
111.    Latisha wants to create a documented chain of custody for the systems that she is handling as part of a forensic investigation. Which of the following will provide her with evidence that systems were not tampered with while she is not working with them?

        1. A chain of custody log
        2. Tamper-proof seals
        3. System logs
        4. None of the above

        Answer:

        B. Tamper-proof seals are used when it is necessary to prove that devices, systems, or spaces were not accessed. They often include holographic logos that help to ensure that tampering is both visible and cannot be easily hidden by replacing the sticker. A chain of custody log works only if personnel actively use it, and system logs will not show physical access. If Latisha has strong concerns, she may also want to ensure that the room or space is physically secured and monitored using a camera system.
112.    Matt's incident response team has collected log information and is working on identifying attackers using that information. What two stages of the NIST incident response process is his team working in?

        1. Preparation and containment, eradication, and recovery
        2. Preparation and post-incident activity
        3. Detection and analysis, and containment, eradication, and recovery
        4. Containment, eradication, and recovery and post-incident activity

        Answer:

        C. Collecting and analyzing logs most often occurs in the detection and analysis phase, whereas connecting attacks back to attackers is typically handled in the containment, eradication, and recovery phase of the NIST incident response process.
113.    Raj discovers that the forensic image he has attempted to create has failed. What is the most likely reason for this failure?

        1. Data was modified.
        2. The source disk is encrypted.
        3. The destination disk has bad sectors.
        4. The data cannot be copied in RAW format.

        Answer:

        C. If Raj has ensured that his destination media is large enough to contain the image, then a failure to copy is most likely because of bad media. Modification of the source data will result in a hash mismatch, encrypted drives can be imaged successfully despite being encrypted (the imager doesn't care!), and copying in RAW format is simply a bit-by-bit copy and will not cause a failure.
114.    Liam notices the following entries in his Squert web console (a web console for Sguil IDS data). What should he do next to determine what occurred?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf015.jpg)

        1. Review SSH logs.
        2. Disable SSH and then investigate further.
        3. Disconnect the server from the Internet and then investigate.
        4. Immediately change his password.

        Answer:

        A. Failed SSH logins are common, either because of a user who has mistyped their password or because of scans and random connection attempts. Liam should review his SSH logs to see what may have occurred.
115.    Which of the following activities is not part of the containment and restoration process?

        1. Minimizing loss
        2. Identifying the attacker
        3. Limiting service disruption
        4. Rebuilding compromised systems

        Answer:

        B. Identifying the attacker is typically handled either during the identification stage or as part of the post-incident activities. The IR process typically focuses on capturing data and allowing later analysis to ensure that services are restored.
116.    Samantha has recently taken a new position as the first staff security analyst that her employer has ever had. During her first week, she discovers that there is no information security policy and that the IT staff do not know what to do during a security incident. Samantha plans to start up a CSIRT to handle incident response. What type of documentation should she provide to describe specific procedures that the CSIRT will use during events like malware infections and server compromise?

        1. An incident response policy
        2. An operations manual
        3. An incident response program
        4. A playbook

        Answer:

        D. Playbooks describe detailed procedures that help to ensure that organizations and individuals take the right actions during the stress of an incident. Operations guides typically cover normal operational procedures, while an incident response policy describes the high-level organizational direction and authority for incident response. An incident response program might generate a policy and a playbook but would not include the detailed instructions itself.
117.    What is space between the last sector containing logical data and the end of the cluster called?

        1. Unallocated space
        2. Ephemeral space
        3. Slack space
        4. Unformatted space

        Answer:

        C. Slack space is the space left between the end of a file and the end of a cluster. This space is left open, but attackers can hide data there, and forensic analysts can recover data from this space if larger files were previously stored in the cluster and the space was not overwritten prior to reuse.
118.    Jack is preparing to take a currently running PC back to his forensic lab for analysis. As Jack considers his forensic process, one of his peers recommends that he simply unplug the power cable rather than doing a software-based shutdown. Why might Jack choose to follow this advice?

        1. It will create a crash log, providing useful memory forensic information.
        2. It will prevent shutdown scripts from running.
        3. It will create a memory dump, providing useful forensic information.
        4. It will cause memory-resident malware to be captured, allowing analysis.

        Answer:

        B. If the system contains any shutdown scripts or if there are temporary files that would be deleted at shutdown, simply pulling the power cable will leave these files in place for forensic analysis. Pulling the cord will not create a memory or crash dump, and memory-resident malware will be lost at power-off.
119.    Rick wants to validate his recovery efforts and intends to scan a web server he is responsible for with a scanning tool. What tool should he use to get the most useful information about system vulnerabilities?

        1. Wapiti
        2. Nmap
        3. OpenVAS
        4. ZAP

        Answer:

        C. Of the tools listed, only OpenVAS is a full-system vulnerability scanner. Wapiti is a web application scanner, ZAP is an attack proxy used for testing web applications, and Nmap is a port scanner.
120.    What is the key goal of the containment stage of an incident response process?

        1. To limit leaks to the press or customers
        2. To limit further damage from occurring
        3. To prevent data exfiltration
        4. To restore systems to normal operation

        Answer:

        B. The containment stage of incident response is aimed at limiting damage and preventing any further damage from occurring. This may help stop data exfiltration, but the broader goal is to prevent all types of damage, including further exploits or compromises.
121.    What level of forensic data extraction will most likely be possible and reasonable for a corporate forensic examiner who deals with modern phones that provide filesystem encryption?

        1. Level 1: Manual extraction
        2. Level 2: Logical extraction
        3. Level 3: JTAG or HEX dumping
        4. Level 4: Chip extraction

        Answer:

        B. Logical copies of data and volumes from an unlocked or decrypted device is the most likely mobile forensic scenario in many cases. Most forensic examiners do not have access to chip-level forensic capabilities that physically remove flash memory from the circuit board, and JTAG-level acquisition may involve invasive acquisition techniques like directly connecting to chips on a circuit board.
122.    Wang believes that a Windows system he is responsible for is compromised and wants to monitor traffic to and from it. Which of the following is not a typical capture option in circumstances like these?

        1. A packet capture tool installed on the system
        2. A packet capture tool on another system on the same network
        3. Packet capture at the network edge
        4. Packet capture at the network core

        Answer:

        A. Wang knows that installing additional software on Windows system to capture traffic can interfere with forensic efforts or warn attackers that they are being observed. Using packet capture from another location on the network is the more common option in this scenario.
123.    Carol has discovered an attack that appears to be following the process flow shown here. What type of attack should she identify this as?

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf016.jpg)

        1. Phishing
        2. Zero-day exploit
        3. Whaling
        4. Advanced persistent threat

        Refer to the image shown here for questions 124–126.

        ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c03uf017.jpg)

        Answer:

        D. The process flow that Carol has discovered is typically used by an advanced persistent threat (APT). Phishing would focus on gaining credentials, whaling is similar but focused on important individuals, and a zero-day exploit leverages a newly discovered vulnerability before there is a patch or general awareness of the issue.
124.    During an e-discovery process, Carol reviews the request from opposing counsel and builds a list of all the individuals identified. She then contacts the IT staff who support each person to request a list of their IT assets. What phase of the EDRM flow is she in?

        1. Information governance
        2. Identification
        3. Preservation
        4. Collection

        Answer:

        B. She is in the identification phase of the Electronic Discovery Reference Model (EDRM), which involves identifying systems and data before they are collected and preserved.
125.    During the preservation phase of her work, Carol discovers that information requested as part of the discovery request has been deleted as part of a regularly scheduled data cleanup as required by her organization's policies. What should Carol do?

        1. Conduct a forensic recovery of the data.
        2. Create synthetic data to replace the missing data.
        3. Report the issue to counsel.
        4. Purge any other data related to the request based on the same policy.

        Answer:

        C. Carol should notify counsel and provide information about the policy and schedule that resulted in the data being removed. This will allow counsel to choose what steps to take next.
126.    In what phase should Carol expect to spend the most person-hours?

        1. Identification
        2. Collection and preservation
        3. Processing, review, and analysis
        4. Production

        Answer:

        C. With most e-discovery cases, reviewing the large volumes of data to ensure that only needed data is presented and that all necessary data is made available takes up the most staff time. Many organizations with larger e-discovery needs either dedicated staff or outsourced efforts like this.
127.    The incident response kit that Cassandra is building is based around a powerful laptop so that she can perform onsite drive acquisitions and analysis. If she expects to need to acquire data from SATA, SSD, and flash drives, what item should she include in her kit?

        1. A write blocker
        2. A USB hard drive
        3. A multi-interface drive adapter
        4. A USB-C cable

        Answer:

        C. Cassandra should ensure that she has at least one USB multi-interface drive adapter that can connect to all common storage drive types. If she were performing forensic analysis, she would also want to use a hardware or software write blocker to ensure that she retains forensic integrity of the acquisition. A USB-C cable and a USB hard drive are commonly found in forensic and incident response toolkits, but neither will help Cassandra connect to bare drives.
128.    Which of the following items is not typically found in corporate forensic kits?

        1. Write blockers
        2. Crime scene tape
        3. Label makers
        4. Decryption tools

        Answer:

        B. Crime scene tape isn't a typical part of a forensic kit if you aren't a law enforcement forensic analyst or officer. Some businesses may use seals or other indicators to discourage interference with investigations. Write blockers, label makers, and decryption tools are all commonly found in forensic kits used by both commercial and law enforcement staff.
129.    What incident response tool should Kai build prior to an incident to ensure that staff can reach critical responders when needed?

        1. A triage triangle
        2. A call list
        3. A call rotation
        4. A responsibility matrix

        Answer:

        B. A call list provides a list of the personnel who should or can be contacted during an incident or response scenario. Sometimes called an escalation list, they typically include the names of the staff members who should be called if there is no response. A rotation list or call rotation is used to distribute workload among a team, typically by placing a specific person on-call for a set time frame. This may help decide who is on the call list at any given point in time. A triage triangle is made up for this question, and responsibility matrices are sometimes created to explain who is responsible for what system or application but aren't directly used for emergency contact lists.
130.    Greg finds a series of log entries in his web server logs showing long strings `"AAAAAAAAAAAAAAAAAAAAAAA"`, followed by strings of characters. What type of attack has he most likely discovered?

        1. A SQL injection attack
        2. A denial-of-service attack
        3. A buffer overflow attack
        4. A PHP string-ring attack

        Answer:

        C. Overflowing a memory location by placing a string longer than the program expects into a variable is a form of buffer overflow attack. Attackers may choose to use a string of the same letters to make the overflow easier to spot when testing the exploit.
131.    During a security incident, Joanna makes a series of changes to production systems to contain the damage. What type of change should she file in her organization's change control process when the response effort is concluding?

        1. Routine change
        2. Priority change
        3. Emergency change
        4. Pre-approved change

        Answer:

        C. This is an example of an emergency change because the change was made without any advance approval. It was necessary to meet urgent security requirements, and Joanna should follow up as soon as possible by filing an emergency change notice.
132.    Which one of the following incident response test types provides an interactive exercise for the entire team but does not run the risk of disrupting normal business activity?

        1. Full interruption test
        2. Checklist review
        3. Management review
        4. Tabletop exercise

        Answer:

        D. Tabletop exercises allow testing of the incident response process without disrupting normal business activity. This is a good approach that gathers the team together to walk through an incident scenario. Full interruption tests are disruptive to the business and would not be appropriate in this case. Checklist reviews and management reviews do not provide the requested level of interaction with the team.
133.    Which of the following cloud service environments is likely to provide the best available information for forensic analysis?

        1. SaaS
        2. IaaS
        3. PaaS
        4. IDaaS

        Answer:

        B. Generally speaking, analysts may obtain more forensic information when their organization has greater control over the underlying cloud resources. Infrastructure as a service (IaaS) environments provide the greatest level of control and, therefore, typically provide access to the most detailed information.
134.    Ken is helping his organization prepare for future incident response efforts and would like to ensure that they conduct regular training exercises. Which one of the following exercises could he use to remind incident responders of their responsibilities with the least impact on other organizational priorities?

        1. Checklist review
        2. Structured walk-through
        3. Capture the flag
        4. Tabletop exercise

        Answer:

        A. Any of these exercises may be used to help remind incident responders of their responsibilities. Checklist reviews have the least impact on the organization because they may be done asynchronously by individual employees. The other training/exercise types listed here would require a more substantial commitment of time.
135.    When analyzing network traffic for indicators of compromise, which one of the following service/port pairings would indicate a common protocol running on a nonstandard port?

        1. HTTPS on TCP port 443
        2. RDP on TCP port 3389
        3. SSH on TCP port 1433
        4. HTTP on TCP port 80

        Answer:

        C. All of these are standard port/service pairings, with the exception of SSH, which normally runs on port 22. If this is discovered frequently during attacks, analysts may want to generate a new IoC to better recognize future attacks.
136.    Camilla is participating in the eradication and recovery stage of an incident response process. Which one of the following activities would not normally occur during this phase?

        1. Vulnerability mitigation
        2. Restoration of permissions
        3. Verification of logging/communication to security monitoring
        4. Analysis of drive capacity consumption

        Answer:

        D. Vulnerability mitigation, restoration of permissions, and the verification of logging and communication to security monitoring are all activities that normally occur during the eradication and recovery phase of incident response. The analysis of drive capacity consumption is the assessment of an indicator of compromise (IoC), which occurs during the detection and analysis phase of incident response.
137.    What type of exercise actually activates an organization's incident response plan but has the lowest likelihood of disrupting normal activities?

        1. Checklist review
        2. Tabletop exercise
        3. Full interruption test
        4. Parallel test

        Answer:

        D. Parallel tests and full interruption tests involve the activation of incident response procedures, while checklist reviews and tabletop exercises do not. Full interruption tests are more risky than parallel tests because they involve stopping normal operations. Therefore, parallel tests have a lower likelihood of disrupting normal activities.
138.    Which one of the following events is _least_ likely to trigger the review of an organization's information security program?

        1. Security incident
        2. Changes in compliance obligations
        3. Changes in team members
        4. Changes in business processes

        Answer:

        C. Changes in team members may cause someone to initiate a review, but it is more likely that a review would be initiated based on changes in the processes protected by the security program, control requirements (such as compliance obligations), or a control failure (such as a security incident).
139.    The Open Source Security Testing Methodology Manual (OSS TMM) is focused on testing in three major areas. Which one of the following is not one of those areas?

        1. Physical locations
        2. Communications
        3. Web servers
        4. Human interactions

        Answer:

        C. The Open Source Security Testing Methodology Manual (OSS TMM), published by the Institute for Security and Open Methodologies provides guidance on testing the security of physical locations, human interactions, and communications. While web servers may fall under the general category of communications, they are not one of the specific testing objectives of OSS TMM.
140.    Kevin is conducting an assessment of a web application using the OWASP Testing Guide. He is searching for XSS vulnerabilities in the application and would like to use an approach that balances the time required to conduct the testing and the effectiveness of the test. Which approach would be most appropriate?

        1. Use an automated testing tool.
        2. Conduct a penetration test.
        3. Test each input field manually.
        4. Interview the software developers.

        Answer:

        A. This question is challenging because all of the answers are useful techniques when evaluating the security of a web application. However, we are looking for the answer that best balances the time required to conduct the test and the thoroughness of the results. Using an automated testing tool can quickly check all of the input fields in an application. Manual testing may produce more vulnerabilities than an automated test, but it is very time-intensive, as is a penetration test. Interviewing software developers may result in some useful information, but it will not provide detailed results helpful in finding XSS vulnerabilities.
141.    What is the minimum interval at which an organization should conduct business continuity plan refresher training for those with specific business continuity roles?

        1. Weekly
        2. Monthly
        3. Semiannually
        4. Annually

        Answer:

        D. Individuals with specific business continuity roles should receive training on at least an annual basis. While it is always preferable to offer more frequent training, annual training is sufficient to meet the requirements of most organizations.
142.    Which one of the following programs has the primary goal of ensuring that an organization is able to maintain normal operations during a disaster or other disruption?

        1. Disaster recovery
        2. Incident response
        3. Risk management
        4. Business continuity

        Answer:

        D. The goal of the business continuity program is to ensure that the organization is able to maintain normal operations even during an unexpected event. When an incident strikes, business continuity controls may protect the business' core functions from disruption.

        The goal of the disaster recovery program is to help the organization quickly recover normal operations if they are disrupted. An incident may cause service disruptions that would trigger the disaster recovery plan.

        Both the business continuity and disaster recovery programs may interact with the incident response program, but the incident response program is not directly responsible for maintaining normal operations. The same is true for risk management programs, which are focused on identifying and addressing all risks to the organization.
143.    Which one of the following programs has the primary goal of helping the organization quickly recover normal operations if they are disrupted?

        1. Disaster recovery
        2. Incident response
        3. Risk management
        4. Business continuity

        Answer:

        A. The goal of the disaster recovery program is to help the organization quickly recover normal operations if they are disrupted. An incident may cause service disruptions that would trigger the disaster recovery plan.

        The goal of the business continuity program is to ensure that the organization is able to maintain normal operations even during an unexpected event. When an incident strikes, business continuity controls may protect the business' core functions from disruption.

        Both the business continuity and disaster recovery programs may interact with the incident response program, but the incident response program is not directly responsible for recovering normal operations. The same is true for risk management programs, which are focused on identifying and addressing all risks to the organization.
144.    During what phase of the incident response process would an organization implement defenses designed to reduce the likelihood of a security incident?

        1. Preparation
        2. Detection and analysis
        3. Containment, eradication, and recovery
        4. Post-incident activity

        Answer:

        A. Organizations should build solid, defense-in-depth approaches to cybersecurity during the preparation phase of the incident response process. The controls built during this phase serve to reduce the likelihood and impact of future incidents.
145.    After wrapping up an incident response investigation, Chris is attempting to determine what went wrong so that he can implement new security controls that will prevent similar incidents in the future. What term best describes his work?

        1. Lessons learned review
        2. Post-incident activity
        3. Incident management
        4. Root-cause analysis

        Answer:

        D. This question is tricky because many of these answers are partially correct. Root-cause analysis is the correct answer because it is the most specific term that describes Chris' work. The root-cause analysis is designed to figure out _why_ an incident occurred. This is conducted as part of a lessons learned review, which is part of post-incident activity, which is part of incident management. However, all three of those terms are less specific, so they do not best describe the activity.
146.    What common criticism is leveled at the Cyber Kill Chain?

        1. Not all threats are aimed at a kill.
        2. It is too detailed.
        3. It includes actions outside the defended network.
        4. It focuses too much on insider threats.

        Answer:

        C. The Cyber Kill Chain includes actions outside the defended network, which many defenders cannot take action on, resulting in one of the common criticisms of the model. Other criticisms include the focus on a traditional perimeter and on antimalware-based techniques, as well as a lack of focus on insider threats.
147.    Tamara is a cybersecurity analyst for a private business that is suffering a security breach. She believes the attackers have compromised a database containing sensitive information. Which one of the following activities should be Tamara's first priority?

        1. Identifying the source of the attack
        2. Eradication
        3. Containment
        4. Recovery

        Answer:

        C. Tamara's first priority should be containing the attack. This will prevent it from spreading to other systems and also potentially stop the exfiltration of sensitive information. Only after containing the attack should Tamara move on to eradication and recovery activities. Identifying the source of the attack should be a low priority.
148.    Robert is finishing a draft of a proposed incident response policy for his organization. Who would be the most appropriate person to sign the policy?

        1. CEO
        2. Director of security
        3. CIO
        4. CSIRT leader

        Answer:

        A. The incident response policy provides the CSIRT with the authority needed to do their job. Therefore, it should be approved by the highest possible level of authority within the organization, preferably the CEO.
149.    Which one of the following is not an objective of the containment, eradication, and recovery phase of incident response?

        1. Detect an incident in progress.
        2. Implement a containment strategy.
        3. Identify the attackers.
        4. Eradicate the effects of the incident.

        Answer:

        A. Detection of a potential incident occurs during the detection and analysis phase of incident response. The other activities listed are all objectives of the containment, eradication, and recovery phase.
150.    Which one of the following is not a phase of the threat lifecycle addressed in the MITRE ATT\&CK model?

        1. Domination
        2. Exfiltration
        3. Execution
        4. Privilege escalation

        Answer:

        A. MITRE provides the ATT\&CK, or Adversarial Tactics, Techniques, and Common Knowledge, knowledge base of adversary tactics and techniques. The ATT\&CK matrices include detailed descriptions, definitions, and examples for the complete threat life cycle, from initial access through execution, persistence, privilege escalation, and exfiltration. Domination is not one of the phases.
