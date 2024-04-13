# Questions

1.  Which of the following are terms for an area of an enterprise network, separated by firewalls, which contains servers that must be accessible both from the Internet and from the internal network? (Choose all that apply.)

    1. Intranet
    2. DMZ
    3. EGP
    4. Stateless network
    5. Perimeter network
    6. Screened subnet

    Answer:

    B, E, F. Servers that must be accessible both from the internal network and from the Internet are typically located in an area of the enterprise called a screened subnet, a perimeter network, or a demilitarized zone (DMZ). This area is separated from both the Internet and the internal network by firewalls, which prevents unauthorized Internet users from accessing the internal network. Intranet is another term for the internal network. Edge Gateway Protocol (EGP) is a type of routing protocol, and stateless is a type of firewall; neither apply to this definition.
2.  Which of the following authentication protocols do Windows networks use for Active Directory Domain Services (AD DS) authentication of internal clients?

    1. RADIUS
    2. WPA2
    3. Kerberos
    4. EAP-TLS

    Answer:

    C. Windows networks that use AD DS authenticate clients using the Kerberos protocol, in part because it never transmits passwords over the network, even in encrypted form. Remote Authentication Dial-In User Service (RADIUS) is an authentication, authorization, and accounting service for remote users connecting to a network. Windows does not use it for internal clients. WiFi Protected Access 2 (WPA2) is a security protocol used by wireless Local Area Network (LAN networks. It is not used for AD DS authentication. Extensible Authentication Protocol-Transport Layer Security (EAP-TLS) is a remote authentication protocol that AD DS networks do not use for internal clients.
3.  Which of the following are examples of multifactor authentication? (Choose all that apply.)

    1. A system that uses an external RADIUS server for authentication
    2. A system that requires two passwords for authentication
    3. A system that requires a smartcard and a PIN for authentication
    4. A system that requires a password and a retinal scan for authentication

    Answer:

    C, D. Multifactor authentication combines two or more authentication methods and reduces the likelihood that an intruder would be able to successfully impersonate a user during the authentication process. A password and a retinal scan is an example of a multifactor authentication system. A smartcard and a PIN, which is the equivalent of a password, is an example of multifactor authentication because it requires users to supply something they know and something they have. Multifactor authentication refers to the proofs of identity a system requires, not the number of servers used to implement the system. Therefore, the use of a Remote Authentication Dial-In User Service (RADIUS) server is not an example of multifactor authentication. A system that requires two passwords is not an example of multifactor authentication, because an attacker can compromise one password as easily as two. A multifactor authentication system requires two different forms of authentication.
4.  Which of the following protocols can you use to authenticate Windows remote access users with smartcards?

    1. EAP
    2. MS-CHAPv2
    3. CHAP
    4. PAP

    Answer:

    A. The Extensible Authentication Protocol (EAP) is the only Windows remote authentication protocol that supports the use of authentication methods other than passwords, such as smartcards. MS-CHAPv2 is a strong remote access authentication protocol, but it supports password authentication only. Users cannot use smartcards. The Challenge Handshake Authentication Protocol (CHAP) is a relatively weak authentication protocol that does not support the use of smartcards. The Password Authentication Protocol (PAP) supports only cleartext passwords, not smartcards.
5.  Which of the following statements best defines multifactor user authentication?

    1. Verification of a user's identity on all of a network's resources using a single sign-on
    2. Verification of a user's identity using two or more types of credentials
    3. Verification of a user's identity on two devices at once
    4. Verification of a user's membership in two or more security groups

    Answer:

    B. Multifactor authentication combines two or more authentication methods, requiring a user to supply multiple credentials. This reduces the likelihood that an intruder would be able to successfully impersonate a user during the authentication process. The term multifactor does not refer to the number of resources, devices, or groups with which the user is associated.
6.  Which of the following services are methods of tracking a user's activities on a network? (Choose all that apply.)

    1. Authentication
    2. Authorization
    3. Accounting
    4. Auditing

    Answer:

    C, D. Accounting and auditing are both methods of tracking and recording a user's activities on a network, such as when a user logged on and how long they remained connected. Authentication is the confirmation of a user's identity, and authorization defines the type of access granted to authenticated users.
7.  When a user supplies a password to log on to a server, which of the following actions is the user performing?

    1. Authentication
    2. Authorization
    3. Accounting
    4. Auditing

    Answer:

    A. Authentication is the process of confirming a user's identity. Passwords are one of the authentication factors commonly used by network devices. Authorization defines the type of access granted to authenticated users. Accounting and auditing are both methods of tracking and recording a user's activities on a network, such as when a user logged on and how long they remained connected.
8.  When a user swipes a finger across a fingerprint scanner to log on to a laptop computer, which of the following actions is the user performing?

    1. Authentication
    2. Authorization
    3. Accounting
    4. Auditing

    Answer:

    A. Authentication is the process of confirming a user's identity. Fingerprints and other biometric readers are one of the authentication factors commonly used by network devices. Authorization defines the type of access granted to authenticated users. Accounting and auditing are both methods of tracking and recording a user's activities on a network, such as when a user logged on and how long they remained connected.
9.  Which of the following security protocols can authenticate users without transmitting their passwords over the network?

    1. Kerberos
    2. 802.1X
    3. TKIP
    4. LDAP

    Answer:

    A. Kerberos is a security protocol used by Active Directory that employs a system of tickets to authenticate users and other network entities without the need to transmit credentials over the network. IEEE 802.1X does authenticate by transmitting credentials. Temporal Key Integrity Protocol (TKIP) and Lightweight Directory Access Protocol (LDAP) are not authentication protocols.
10. Which of the following statements about authentication auditing are not true?

    1. Auditing can disclose attempts to compromise passwords.
    2. Auditing can detect authentications that occur after hours.
    3. Auditing can identify the guess patterns used by password cracking software.
    4. Auditing can record unsuccessful as well as successful authentications.

    Answer:

    C. Auditing of authentication activities can record both successful and unsuccessful logon attempts. Large numbers of logon failures can indicate attempts to crack passwords. Auditing tracks the time of authentication attempts, sometimes enabling you to detect off-hours logons that indicate an intrusion. Auditing does not record the passwords specified during authentications, so it cannot identify patterns of unsuccessful guesses.
11. When a user swipes a smartcard through a reader to log on to a laptop computer, which of the following actions is the user performing?

    1. Authentication
    2. Authorization
    3. Accounting
    4. Auditing

    Answer:

    A. Authentication is the process of confirming a user's identity. Smartcards are one of the authentication factors commonly used by network devices. Authorization defines the type of access granted to authenticated users. Accounting and auditing are both methods of tracking and recording a user's activities on a network, such as when a user logged on and how long they remained connected.
12. Combining elements like something you know, something you have, and something you are to provide access to a secured network resource is a definition of which of the following types of authentication?

    1. Multifactor
    2. Multisegment
    3. Multimetric
    4. Multifiltered

    Answer:

    A. Multifactor authentication combines two or more authentication methods and reduces the likelihood that an intruder would be able to successfully impersonate a user during the authentication process. A password (something you know) and a retinal scan (something you are) is an example of a multifactor authentication system. A smartcard and a PIN, which is the equivalent of a password, is another example of multifactor authentication because it requires users to supply something they know and something they have. Multisegment, multimetric, and multifiltered are not applicable terms in this context.
13. Which of the following terms describes a system that prevents computers from logging on to a network unless they have the latest updates and antimalware software installed?

    1. NAC
    2. LDAP
    3. RADIUS
    4. TKIP-RC4

    Answer:

    A. Network Access Control (NAC) is a mechanism that defines standards of equipment and configuration that systems must meet before they can connect to the network. Lightweight Directory Access Protocol (LDAP) provides communication between directory service entities. Remote Authentication Dial-In User Service (RADIUS) is an authentication, authorization, and accounting service for remote users connecting to a network. Temporal Key Integrity Protocol (TKIP) with the RC4 cipher is an encryption protocol used on wireless networks running the WiFi Protected Access (WPA) security protocol.
14. Which of the following describes the primary difference between Single Sign-On (SSO) and same sign-on?

    1. SSO enables users to access different resources with one set of credentials, whereas same sign-on requires users to have multiple credential sets.
    2. SSO credentials consist of one username and one password, whereas same sign-on credentials consist of one username and multiple passwords.
    3. SSO requires the user to supply credentials only once, whereas with same sign-on, the user must supply the credentials repeatedly.
    4. SSO requires multifactor authentication, such as a password and a smartcard, whereas same sign-on requires only a password for authentication.

    Answer:

    C. SSO uses one set of credentials and requires the user to supply them only once to gain access to multiple resources. Same sign-on also uses a single set of credentials, with one password, but the user must perform individual logons for each resource. Neither SSO nor same sign-on calls for multifactor authentication.
15. Which of the following is the best description of biometrics?

    1. Something you know
    2. Something you have
    3. Something you are
    4. Something you do

    Answer:

    C. Biometrics is a type of authentication factor that uses a physical characteristic that uniquely identifies an individual, such as a fingerprint or a retinal pattern. Biometrics is therefore best described as something you are, as opposed to something you know, something you have, or something you do.
16. Which of the following authentication factors is an example of something you have?

    1. A fingerprint
    2. A smartcard
    3. A password
    4. A finger gesture

    Answer:

    B. Something you have refers to a physical possession that serves to identify a user, such as a smartcard. This type of authentication is typically used as part of a multifactor authentication procedure because a smartcard or other physical possession can be lost or stolen. A fingerprint would be considered something you are, a password is something you know, and a finger gesture is something you do.
17. Which of the following statements best describes the primary scenario for the use of TACACS+?

    1. TACACS+ was designed to provide authentication, authorization, and accounting services for wireless networks.
    2. TACACS+ was designed to provide authentication, authorization, and accounting services for the Active Directory service.
    3. TACACS+ was designed to provide authentication, authorization, and accounting services for remote dial-up users.
    4. TACACS+ was designed to provide authentication, authorization, and accounting services for network routers and switches.

    Answer:

    D. Terminal Access Controller Access Control System Plus (TACACS+) is a protocol designed to provide Authentication, Authorization, and Accounting (AAA) services for networks with many routers and switches, enabling administrators to access them with a single set of credentials. It was not designed to provide AAA services for wireless networks, Active Directory, or remote dial-in users.
18. The new door lock on your company's datacenter door requires you to supply both a PIN and a thumbprint scan. Which of the following types of authentication factors does the lock use? (Choose all that apply.)

    1. Something you have
    2. Something you know
    3. Something you are
    4. Something you do

    Answer:

    B, C. A PIN, like a password, is something you know, and a thumbprint, or any other biometric factor, is something you are. An example of something you have would be a smartcard, and an example of something you do would be a finger gesture.
19. Your new smartphone enables you to configure the lock screen with a picture of your husband, on which you draw eyes, nose, and a mouth with your finger to unlock the phone. This is an example of which of the following authentication factors?

    1. Something you have
    2. Something you know
    3. Something you are
    4. Something you do

    Answer:

    D. The act of drawing on the screen with your finger is a gesture, which is an example of something you do. A PIN or a password is something you know; a thumbprint, or any other biometric factor, is something you are; and a smartcard is an example of something you have.
20. Which of the following authentication factors is an example of something you do?

    1. A fingerprint
    2. A smartcard
    3. A password
    4. A finger gesture

    Answer:

    D. Something you do refers to a physical action performed by a user, such as a finger gesture, which helps to confirm his or her identity. This type of authentication is often used as part of a multifactor authentication procedure because a gesture or other action can be imitated. A fingerprint would be considered something you are, a password is something you know, and a smartcard is something you have.
21. Which of the following authentication factors is an example of something you know?

    1. A fingerprint
    2. A smartcard
    3. A password
    4. A finger gesture

    Answer:

    C. Something you know refers to information you supply during the authentication process, such as a password or PIN. This is the most common type of authentication factor because it cannot be lost or stolen unless the user violates security policies. A fingerprint would be considered something you are, a finger gesture is something you do, and a smartcard is something you have.
22. Which of the following authentication factors is an example of something you are?

    1. A fingerprint
    2. A smartcard
    3. A password
    4. A finger gesture

    Answer:

    A. Something you are refers to a physical characteristic that uniquely identifies an individual, such as a fingerprint or other form of biometric. This type of authentication is often used as part of a multifactor authentication procedure because a biometric element can conceivably be compromised. A finger gesture would be considered something you do, a password is something you know, and a smartcard is something you have.
23. Which of the following is an implementation of Network Access Control (NAC)?

    1. RADIUS
    2. 802.1X
    3. LDAP
    4. TACACS+

    Answer:

    B. NAC is a set of policies that define security requirements that clients must meet before they are permitted to connect to a network. 802.1X is a basic implementation of NAC. Remote Authentication Dial-In User Service (RADIUS) and Terminal Access Controller Access Control System Plus (TACACS+) are Authentication, Authorization, and Accounting (AAA) services. They are not NAC implementations themselves, although they can play a part in their deployment. Lightweight Directory Access Protocol (LDAP) provides directory service communications.
24. Which of the following is not one of the roles involved in an 802.1X transaction?

    1. Supplicant
    2. Authentication server
    3. Authorizing agent
    4. Authenticator

    Answer:

    C. An 802.1X transaction involves three parties: the supplicant, which is the client attempting to connect to the network; the authenticator, which is a switch or access point to which the supplicant is requesting access; and the authentication server, which is typically a Remote Authentication Dial-In User Service (RADIUS) implementation that verifies the supplicant's identity. There is no party to the transaction called an authorizing agent.
25. In an 802.1X transaction, what is the function of the supplicant?

    1. The supplicant is the service that issues certificates to clients attempting to connect to the network.
    2. The supplicant is the service that verifies the credentials of the client attempting to access the network.
    3. The supplicant is the network device to which the client is attempting to connect.
    4. The supplicant is the client user or computer attempting to connect to the network.

    Answer:

    D. An 802.1X transaction involves three parties: the supplicant, which is the client attempting to connect to the network; the authenticator, which is a switch or access point to which the supplicant is requesting access; and the authentication server, which is typically a Remote Authentication Dial-In User Service (RADIUS) implementation that verifies the supplicant's identity. The supplicant is not involved in issuing certificates.
26. In an 802.1X transaction, what is the function of the authenticator?

    1. The authenticator is the service that issues certificates to clients attempting to connect to the network.
    2. The authenticator is the service that verifies the credentials of the client attempting to access the network.
    3. The authenticator is the network device to which the client is attempting to connect.
    4. The authenticator is the client user or computer attempting to connect to the network.

    Answer:

    C. An 802.1X transaction involves three parties: the supplicant, which is the client attempting to connect to the network; the authenticator, which is a switch or access point to which the supplicant is requesting access; and the authentication server, which is typically a Remote Authentication Dial-In User Service (RADIUS) implementation that verifies the supplicant's identity. The authenticator is not involved in issuing certificates.
27. An 802.1X transaction involves three roles: the supplicant, the authenticator, and the authentication server. Of the three, which role typically takes the form of a RADIUS implementation?

    1. The supplicant
    2. The authenticator
    3. The authentication server
    4. None of the above

    Answer:

    C. The authentication server role is typically performed by a Remote Authentication Dial-In User Service (RADIUS) server. In an 802.1X transaction, the supplicant is the client attempting to connect to the network, the authenticator is a switch or access point to which the supplicant is requesting access, and the authentication server verifies the client's identity.
28. Which of the following are standards that define combined Authentication, Authorization, and Accounting (AAA) services? (Choose all that apply.)

    1. 802.1X
    2. RADIUS
    3. TACACS+
    4. LDAP

    Answer:

    B, C. Remote Authentication Dial-In User Service (RADIUS) and Terminal Access Controller Access Control System Plus (TACACS+) are both services that provide networks with AAA. 802.1X provides only authentication, and Lightweight Directory Access Protocol (LDAP) provides communication between directory service entities.
29. Which of the following standards was originally designed to provide Authentication, Authorization, and Accounting (AAA) services for dial-up network connections?

    1. RADIUS
    2. TACACS+
    3. Kerberos
    4. LDAP

    Answer:

    A. Remote Authentication Dial-In User Service (RADIUS) was originally conceived to provide AAA services for Internet Service Providers (ISPs), which at one time ran networks with hundreds of modems providing dial-up access to subscribers. Terminal Access Controller Access Control System Plus (TACACS+) is a protocol that was designed to provide AAA services for networks with many routers and switches, but not for dial-up connections. Kerberos and Lightweight Directory Access Protocol (LDAP) are not AAA services.
30. Which of the following statements about RADIUS and TACACS+ are correct?

    1. By default, RADIUS uses UDP, and TACACS+ uses TCP.
    2. By default, RADIUS uses TCP, and TACACS+ uses UDP.
    3. By default, both RADIUS and TACACS+ use TCP.
    4. By default, both RADIUS and TACACS+ use UDP.

    Answer:

    A. Remote Authentication Dial-In User Service (RADIUS) uses User Datagram Protocol (UDP) ports 1812 and 1813 or 1645 and 1646 for authentication, whereas Terminal Access Controller Access Control System Plus (TACACS+) uses Transmission Control Protocol (TCP) port 49.
31. Which of the following standards provides Authentication, Authorization, and Accounting (AAA) services for network routers and switches?

    1. RADIUS
    2. TACACS+
    3. Kerberos
    4. LDAP

    Answer:

    B. Terminal Access Controller Access Control System Plus (TACACS+) is a protocol designed to provide AAA services for networks with many routers and switches, enabling administrators to access them with a single set of credentials. Remote Authentication Dial-In User Service (RADIUS) provides AAA services, but not for routers and switches. Kerberos and Lightweight Directory Access Protocol (LDAP) are not AAA services.
32. Which of the following terms refers to the process of determining whether a user is a member of a group that provides access to a particular network resource?

    1. Authentication
    2. Accounting
    3. Authorization
    4. Access control

    Answer:

    C. Authorization is the process of determining what resources a user can access on a network. Typically, this is done by assessing the user's group memberships. Authentication is the process of confirming a user's identity. Accounting is the process of tracking a user's network activity. Access control is the creation of permissions that provide users and groups with specific types of access to a resource.
33. Which of the following terms refers to the process of confirming a user's identity by checking specific credentials?

    1. Authentication
    2. Accounting
    3. Authorization
    4. Access control

    Answer:

    A. Authentication is the process of confirming a user's identity by checking credentials, such as passwords, ID cards, or fingerprints. Authorization is the process of determining what resources a user can access on a network. Accounting is the process of tracking a user's network activity. Access control is the creation of permissions that provide users and groups with specific types of access to a resource.
34. Which of the following terms refers to the process by which a system tracks a user's network activity?

    1. Authentication
    2. Accounting
    3. Authorization
    4. Access control

    Answer:

    B. Accounting is the process of tracking a user's network activity, such as when the user logged on and logged off and what resources the user accessed. Authentication is the process of confirming a user's identity by checking credentials. Authorization is the process of determining what resources a user can access on a network. Access control is the creation of permissions that provide users and groups with specific types of access to a resource.
35. Which of the following statements are true about a public key infrastructure? (Choose all that apply.)

    1. Data encrypted with a user's public key can be decrypted with the user's public key.
    2. Data encrypted with a user's public key can be decrypted with the user's private key.
    3. Data encrypted with a user's private key can be decrypted with the user's private key.
    4. Data encrypted with a user's private key can be decrypted with the user's public key.

    Answer:

    B, D. In a public key infrastructure, data encrypted with a user's public key can only be decrypted with the user's private key, and data encrypted with a user's private key can only be decrypted with the user's public key. This enables the system to provide both message encryption and nonrepudiation. If data encrypted with a user's public key could be decrypted with that same public key, the system would provide no security at all. If data encrypted with a user's private key could be decrypted with that same private key, the user could only send secure messages to him- or herself.
36. Which of the following technologies can maintain an account database that multiple remote access servers can employ to authenticate remote users?

    1. RADIUS
    2. IDS
    3. NGFW
    4. NAS

    Answer:

    A. A Remote Authentication Dial-In User Service (RADIUS) server can provide Authentication, Authorization, and Accounting (AAA) services for remote access servers. Intrusion Detection Systems (IDSs), Next-Generation Firewalls (NGFWs), and Network Attached Storage (NAS) devices do not provide authentication services.
37. Which element of the Confidentiality-Integrity-Availability (CIA) triad prevents unauthorized modification of protected data?

    1. Confidentiality
    2. Integrity
    3. Availability
    4. None of the above

    Answer:

    B. The Integrity element of the CIA triad prevents data from being modified by unauthorized users. Confidentiality is protection against unauthorized viewing of data. Availability provides users with access to the data they need.
38. Which of the following is an example of local authentication?

    1. A system that uses an external RADIUS server for authentication
    2. A system that uses the Kerberos protocol for authentication
    3. A system that authenticates users without network communication
    4. A system that requires a password and a retinal scan for authentication

    Answer:

    C. Systems that use local authentication have user accounts stored on the computer, enabling users to log on without the need for any network communication. Systems that use Remote Authentication Dial-In User Service (RADIUS) or Kerberos for authentication require network communication. A password and a retinal scan is an example of a multifactor authentication system, which might or might not be local.
39. In some cases, network administrators create computers that function as enticing targets for attackers but that do not provide access to any legitimately sensitive services or information. Which of the following is the term used to describe this technique?

    1. DMZ
    2. Honeypot
    3. Root guard
    4. Spoofing

    Answer:

    B. A honeypot is a computer configured to function as bait for attackers, causing them to waste their time penetrating a resource that provides no significant access. A demilitarized zone (DMZ) is the part of a network where administrators locate servers that must be accessible from the Internet. A root guard provides protection to switch ports. Spoofing is an attack technique in which an intruder modifies packets to assume the appearance of another user or computer.
40. Honeypots and honeynets belong to which of the following categories of devices?

    1. Mitigation techniques
    2. Network attacks
    3. Switch port protection types
    4. Firewall filters

    Answer:

    A. A honeypot or honeynet is a type of mitigation technique that takes the form of a computer or network configured to function as bait for attackers, causing them to waste their time penetrating a resource that provides no significant access.
41. Which of the following best describes the process of penetration testing?

    1. Administrators create computers or networks that are alluring targets for intruders.
    2. Administrators attempt to access the network from outside using hacker tools.
    3. An organization hires an outside consultant to evaluate the security conditions on the network.
    4. An organization hires an outside consultant who attempts to compromise the network's security measures.

    Answer:

    D. Penetration testing is when an outside consultant is engaged to attempt an unauthorized access to protected network resources. Testing by an internal administrator familiar with the security barriers would not be a valid test. While having a consultant examine the network's security from within can be useful, this is not a penetration test. Computers or networks that are alluring targets for intruders are called honeypots or honeynets.
42. Which of the following types of servers are typically found in a screened subnet? (Choose all that apply.)

    1. Domain controllers
    2. DHCP servers
    3. Email servers
    4. Web servers

    Answer:

    C, D. A network segment that is separated from the internal network by a firewall and exposed to the Internet is called a screened subnet, a demilitarized zone (DMZ), or a perimeter network. Administrators typically use a screened subnet for servers that must be accessible by outside users, such as web and email servers. For security reasons, domain controllers and Dynamic Host Configuration Protocol (DHCP) servers should be located on internal network segments.
43. Which of the following statements best describes the difference between an exploit and a vulnerability?

    1. An exploit is a potential weakness in software, and a vulnerability is a potential weakness in hardware.
    2. A vulnerability is a potential weakness in a system, and an exploit is a hardware or software element that is designed to take advantage of a vulnerability.
    3. An exploit is a potential weakness in a system, and a vulnerability is a hardware or software element that is designed to take advantage of a vulnerability.
    4. A vulnerability is a potential weakness in software, and an exploit is a potential weakness in hardware.

    Answer:

    B. A vulnerability is a weakness, whether in software or hardware, of which an exploit is designed to take advantage. Neither term is specific to hardware or software.
44. Which of the following abbreviations describes a product that combines real-time monitoring of security events and automated analysis of the event information gathered?

    1. SIEM
    2. SNMP
    3. SEIM
    4. SEM/SIM

    Answer:

    A. Security Information and Event Management (SIEM) is a product that combines two technologies: security event management (SEM) and security information management (SIM). Together, the two provide a combined solution for gathering and analyzing information about a network's security events. Simple Network Management Protocol (SNMP) is a technology that gathers information about managed devices. SEIM and SEM/SIM are not correct abbreviations for Security Information and Event Management.
45. A technician in the IT department at your company was terminated today and had to be escorted from the building. Your supervisor has instructed you to disable all of the technician's accounts, change all network device passwords to which the technician had access, and have the datacenter doors rekeyed. Which of the following terms best describes your supervisor's concern in asking you to do these things?

    1. Social engineering
    2. Internal threats
    3. Logic bombs
    4. War driving
    5. External threats

    Answer:

    B. Your supervisor's concern is that the disgruntled technician might take advantage of his access to devices and facilities to sabotage the network. When an individual takes advantage of information gathered during his or her employment, it is called an internal (or insider) threat. An external threat is one originating from a non-employee. Social engineering is a form of attack in which an innocent user is persuaded by an attacker to provide sensitive information via email or telephone. A logic bomb is a code insert placed into a legitimate software product that triggers a malicious event when specific conditions are met. War driving is an attack method that consists of driving around a neighborhood with a computer, scanning for unprotected wireless networks.
46. Which of the following is the best description of a software product with a zero-day vulnerability?

    1. A product with a vulnerability that has just been addressed by a newly-released fix
    2. A product with a vulnerability that has been addressed by a fix, which nearly all users have applied
    3. A vulnerability in a newly-released product for which no fix has yet been developed
    4. A vulnerability in a product which no attackers have yet discovered or exploited

    Answer:

    C. A zero-day vulnerability is a serious software problem with a potential for exploitation in a newly released software product. The vulnerability has not yet been discovered, addressed, or patched by the software's developer, but it has been discovered by potential attackers. A zero-day vulnerability is one that has not yet been patched or fixed.
47. Ralph is evaluating software products for potential deployment on his company's network. Which of the following types of searches can Ralph use to identify security issues that have been discovered in specific products?

    1. CIA
    2. CVE
    3. SKU
    4. SIEM

    Answer:

    B. The Common Vulnerabilities and Exposures (CVE) database is a resource that assigns identifier numbers to known security issues found in software products. By searching the database, Ralph can learn about the vulnerabilities that have already been found in the products he is evaluating. The Confidentiality - Integrity - Availability (CIA) triad lists important information security concepts, but it does not provide information about specific products. Stock Keeping Units (SKU) are product identifiers that do not involve security issues. Security Information and Event Management (SIEM) is a product that gathers and analyzes information about a network's security events, but it would not help Ralph discover vulnerabilities in the products he is evaluating.
48. Alice's company regularly hires a large number of operators for their phone center. The operators require access to a customer database and an order entry system. Because this is a high-turnover position, Alice has streamlined the on-boarding process by creating a security group with the appropriate permissions needed to access the necessary software. This way, she can simply add each new user to the group, rather than assigning the permissions individually. This is an example of which of the following security concepts?

    1. Least privilege
    2. Zero trust
    3. Role-based access control
    4. Defense in depth

    Answer:

    C. Role-based access control works by assigning permissions to specific jobs or job roles. Each new user can then be associated with a role and receive the necessary permissions automatically. When a user leaves a job, removing them from their role revokes the permissions associated with it. Least privilege, zero trust, and defense in depth are all theoretical security concepts, but they are not descriptive of Alice's practice in this regard.
49. When starting her new position as a network administrator, Alice was given two user accounts. One account is intended for standard user activities, and another has the additional permissions needed for Alice to perform administrative tasks. This is an example of which of the following security concepts?

    1. Zero-day
    2. Multifactor authentication
    3. Least privilege
    4. Defense in depth

    Answer:

    C. Least privilege is the practice of only providing users with the permissions they need to perform their designated tasks and no more. For her standard activities, Alice is given an account that does not have administrative permissions, because she does not need those permissions to perform standard tasks. The administrative account has the additional permissions needed for Alice to perform administrative tasks. The intention is for Alice to use that account only for those administrative tasks. Zero-day is a type of vulnerability; multifactor authentication calls for users to supply two identifying factors; defense in depth refers to the use of multiple security mechanisms to provide additional protection. None of these three options refers to the use of multiple user accounts.
50. Which of the following is a practice that a zero trust architecture is designed to protect against?

    1. Zero-day vulnerabilities
    2. External threats
    3. Deauthentication
    4. Lateral movement

    Answer:

    D. Lateral movement is when a user gains basic access to a network by legitimate means and then uses it to gain unauthorized access to other resources inside the network. A zero trust provides full protection for all sensitive resources, even from users already inside the network. A zero trust architecture does not protect against zero-day vulnerabilities, which are exploits in software; external threats; or deauthentication, which is a type of Denial-of-Service (DoS) attack.
51. Which of the following is not one of the mechanisms often used to implement a defense in depth strategy?

    1. Screened subnets
    2. Network segmentation enforcement
    3. Honeypots
    4. Access control vestibules
    5. Social engineering
    6. Separation of duties

    Answer:

    E. Social engineering is a means for gaining unauthorized access to a network by convincing users to disclose passwords or other sensitive information; it is not part of a defense in depth strategy. Defense in depth can include physical protection, such as access control vestibules; division of resources using network segmentation, separation of duties, or screened subnets; and deceptive lures, such as honeypots.
52. As part of her company's new risk management initiative, Alice has been assigned the task of performing a threat assessment for the firm's data resources. For each potential threat she discovers, which of the following elements should Alice estimate? (Choose all that apply.)

    1. Severity
    2. Mitigation
    3. Likelihood
    4. Posture

    Answer:

    A, C. A threat assessment should estimate the potential severity of a threat, such as the damage that the loss of a specific resource can cause to the organization. The assessment should also estimate the likelihood of a particular threat occurring, as the organization will have to devote more attention to the more likely threats. An assessment of the organization's current posture (or status) with regard to a specific threat and the mitigation techniques used to counter it are both elements that come later in the risk management process, after the threat assessment has been completed.
53. Alice has been assigned the task of examining her department's order entry procedure, to determine whether it meets established cost, quality, and timeliness goals. Which of the following is the best term for this examination?

    1. Vendor assessment
    2. Process assessment
    3. Business assessment
    4. Risk assessment

    Answer:

    B. A process assessment is an examination of an existing procedure to determine its compliance with a specific set of goals that can include cost, quality, and timeliness. A vendor assessment is an examination of the organization's relationship with a specific business partner. Business assessment and risk assessment are more general terms that can include process assessments.
54. A user calls the help desk, complaining that he cannot access any of the data on his computer. A message has also appeared on his screen stating that his data has been encrypted and that it will only be decrypted after he pays $768 in digital currency to an unknown address. Which of the following types of attack has the user experienced?

    1. War driving
    2. Ransomware
    3. Denial-of-Service
    4. ARP poisoning

    Answer:

    B. Ransomware is a type of attack in which a user's access to his or her data is blocked unless a certain amount of money is paid to the attacker. The blockages can vary from simple screen locks to data encryption. War driving is an attack method that consists of driving around a neighborhood with a computer, scanning for unprotected wireless networks. Denial-of-Service (DoS) is a type of attack that overwhelms a computer with traffic, preventing it from functioning properly. Address Resolution Protocol (ARP) poisoning is the deliberate insertion of fraudulent information into the ARP cache stored on computers and switches.
55. Which of the following attack types typically involves modifying network packets while they are in transit? (Choose all that apply.)

    1. Spoofing
    2. Denial-of-Service
    3. On-path
    4. Logic bomb

    Answer:

    A, C. Spoofing is the process of modifying network packets to make them appear as though they are transmitted by or addressed to someone else. One way of doing this is to modify the Media Access Control (MAC) address in the packets to one that is approved by the MAC filter. An on-pass (or man-in-the-middle) attack is one in which an attacker intercepts network traffic, reads the traffic, and can even modify it before sending it on to the destination. Denial-of-Service (DoS) is a type of attack that overwhelms a computer with traffic, preventing it from functioning properly, whereas a logic bomb is a code insert placed into a legitimate software product that triggers a malicious event when specific conditions are met. Neither of these last two involves modifying network packets.
56. Which of the following types of attack involves the modification of a legitimate software product?

    1. Social engineering
    2. War driving
    3. Logic bomb
    4. Evil twin

    Answer:

    C. A logic bomb is a code insert placed into a legitimate software product that triggers a malicious event when specific conditions are met. Social engineering is the practice of obtaining sensitive data by manipulating legitimate users, such as by pretending to be someone with a genuine need for that data. War driving is an attack method that consists of driving around a neighborhood with a computer, scanning for unprotected wireless networks. An evil twin is a fraudulent access point on a wireless network that mimics the Service Set Identifier (SSID) of a legitimate access point, in the hope of luring in users.
57. Which of the following steps can help to prevent war driving attacks from compromising your wireless network? (Choose all that apply.)

    1. Configure your access point to use a longer SSID.
    2. Configure your access point not to broadcast its SSID.
    3. Configure your clients and access point to use WPA2 security.
    4. Configure your clients and access point to use WEP security.

    Answer:

    B, C. Configuring the access point not to broadcast its Service Set Identifier (SSID) will prevent an unsophisticated war driving attacker from seeing the network. Configuring your equipment to use WiFi Protected Access II (WPA2) security will make it difficult for a war driver who detects your network to connect to it. The SSID is just an identifier; its length has no effect on security. Wired Equivalent Privacy (WEP) is a security protocol that has been found to have serious weaknesses.
58. On the fence outside your home, you happen to notice a small sticker that has the Service Set Identifier (SSID) of your wireless network written on it, along with the name of the security protocol your network is using. To which of the following attacks have you been made a victim?

    1. War driving
    2. War chalking
    3. War tagging
    4. War signing

    Answer:

    B. War driving is an attack method that consists of driving around a neighborhood with a computer, scanning for unprotected wireless networks. When a war driver locates a wireless network and marks it for other attackers, it is called war chalking. There are no such attacks as war tagging and war signing.
59. Which of the following is the name for an attack in which an intruder uses a Bluetooth connection to steal information from a wireless device, such as a smart phone?

    1. Bluedogging
    2. Bluesnarfing
    3. Bluesmurfing
    4. Bluejacking

    Answer:

    B. Bluesnarfing is an attack in which an intruder connects to a wireless device using Bluetooth, for the purpose of stealing information. Bluejacking is the process of sending unsolicited messages to a device using Bluetooth. The other options do not exist.
60. Which of the following types of Denial-of-Service (DoS) attack does not involve flooding a server with traffic?

    1. Amplified
    2. Reflective
    3. Distributed
    4. Permanent

    Answer:

    D. Although a DoS attack typically involves traffic flooding, any attack that prevents a server from functioning can be called a DoS attack. A permanent DoS attack is one in which the attacker actually damages the target system and prevents it from functioning. This can be a physical attack that actually damages the hardware, or the attacker can disable the server by altering its software or configuration settings. Flood-based attacks include the Distributed Denial-of-Service (DDoS) attack, one in which the attacker uses hundreds or thousands of computers controlled by malware and called bots or zombies, to send traffic to a single server or website in an attempt to overwhelm it and prevent it from functioning. An amplified DoS attack is one in which the messages sent by the attacker require an extended amount of processing by the target servers, increasing the burden on them more than simpler messages would. A reflective DoS attack is one in which the attacker sends requests containing the target server's IP address to legitimate servers on the Internet, such as Domain Name System (DNS) servers, causing them to send a flood of responses to the target.
61. Which of the following statements best describes the difference between distributed and reflective Denial-of-Service (DoS) attacks?

    1. A distributed DoS attack uses other computers to flood a target server with traffic, whereas a reflective DoS attack causes a server to flood itself with loopback messages.
    2. A distributed DoS attack uses malware-infected computers to flood a target, whereas a reflective DoS attack takes advantage of other servers’ native functions to make them flood a target.
    3. A reflective DoS attack uses malware-infected computers to flood a target, whereas a distributed DoS attack takes advantage of other servers’ native functions to make them flood a target.
    4. A distributed DoS attack floods multiple target computers with traffic, whereas a reflective DoS attack only floods a single target.

    Answer:

    B. Distributed Denial-of-Service (DDoS) attacks use hundreds or thousands of computers that have been infected with malware, called bots or zombies, to flood a target server with traffic in an attempt to overwhelm it and prevent it from functioning. A reflective DoS attack is one in which the attacker sends requests containing the target server's IP address to legitimate servers on the Internet, such as Domain Name System (DNS) servers, causing them to send a flood of responses to the target. Neither attack type causes a computer to flood itself.
62. Which of the following terms refers to a Denial-of-Service (DoS) attack that places more of a burden on the target server than just the flood of incoming traffic?

    1. Amplified
    2. Reflective
    3. Distributed
    4. Permanent

    Answer:

    A. An amplified DoS attack is one in which the messages sent by the attacker require an extended amount of processing by the target servers, increasing the burden on them more than simpler messages would. Reflective and distributed DoS attacks use other computers to flood a target with traffic. A reflective DoS attack is one in which the attacker sends requests containing the target server's IP address to legitimate servers on the Internet, such as Domain Name System (DNS) servers, causing them to send a flood of responses to the target. A Distributed Denial-of-Service (DDoS) attack is one in which the attacker uses a botnet consisting of hundreds or thousands of computers, controlled by malware and called bots or zombies, to send traffic to a single server or website in an attempt to overwhelm it and prevent it from functioning. A permanent DoS attack is one in which the attacker actually damages the target system and prevents it from functioning.
63. Which of the following types of attacks require no additional hardware or software components? (Choose all that apply.)

    1. Brute-force
    2. Social engineering
    3. Denial-of-Service
    4. Phishing

    Answer:

    A, B, C. A brute-force attack is one in which an attacker uses repeated guesses to find a password, an open port, or some other type of sensitive data. A Denial-of-Service (DoS) attack floods a target server with traffic so that it is unable to function normally. While both of these attack types can be mounted using specialized software, they can also be the work of a lone attacker using nothing more than the tools provided on a standard workstation. Social engineering is the practice of obtaining sensitive data by contacting users and pretending to be someone with a legitimate need for that data. It requires nothing more than a telephone or an email client. Phishing is the term for an attack that uses bogus emails or websites designed to infect users with some type of malware.
64. Which of the following attack types are specifically targeted at wireless network clients? (Choose all that apply.)

    1. Logic bomb
    2. Deauthentication
    3. Evil twin
    4. ARP poisoning

    Answer:

    B, C. Deauthentication is a type of Denial-of-Service (DoS) attack in which the attacker targets a wireless client by sending a deauthentication frame that causes the client to be disconnected from the network. The object of the attack is often to compel the client to connect to a rogue access point called an evil twin. An evil twin is a fraudulent access point on a wireless network that mimics the Service Set Identifier (SSID) of a legitimate access point, in the hope of luring in users. A logic bomb is a code insert placed into a legitimate software product that triggers a malicious event when specific conditions are met. Address Resolution Protocol (ARP) poisoning is the deliberate insertion of fraudulent information into the ARP cache stored on computers and switches. Neither of these last two is specifically targeted at wireless clients.
65. Which of the following is an effective method for preventing sensitive data from being compromised through social engineering?

    1. Implement a program of user education and corporate policies.
    2. Install an antivirus software product on all user workstations.
    3. Install a firewall between the internal network and the Internet.
    4. Use Internet Protocol Security (IPSec) to encrypt all network traffic.

    Answer:

    A. Social engineering is the practice of obtaining sensitive data by contacting users and pretending to be someone with a legitimate need for that data. No software or hardware solution can prevent it; the only way is to educate users on the potential dangers and establish policies that inform users what to do when they experience a social engineering attempt. Social engineering is not a virus or other form of malware, so an antivirus product has no effect against it. Social engineering is not implemented in network traffic, so a firewall cannot filter it. Social engineering is not implemented in network traffic, so IPSec cannot protect it.
66. Which of the following terms refer to Denial-of-Service (DoS) attacks that use other computers to flood a target server with traffic? (Choose all that apply.)

    1. Amplified
    2. Reflective
    3. Distributed
    4. Permanent

    Answer:

    B, C. Reflective and distributed DoS attacks use other computers to flood a target with traffic. A reflective DoS attack is one in which the attacker sends requests containing the target server's IP address to legitimate servers on the Internet, such as DNS servers, causing them to send a flood of responses to the target. A Distributed Denial-of-Service (DDoS) attack is one in which the attacker uses hundreds or thousands of computers, controlled by malware and called bots or zombies, to send traffic to a single server or website in an attempt to overwhelm it and prevent it from functioning. An amplified DoS attack is one in which the messages sent by the attacker require an extended amount of processing by the target servers, increasing the burden on them more than simpler messages would. A permanent DoS attack is one in which the attacker actually damages the target system and prevents it from functioning.
67. In which of the following ways is VLAN hopping a potential threat?

    1. VLAN hopping enables an attacker to scramble a switch's patch panel connections.
    2. VLAN hopping enables an attacker to rename the default VLAN on a switch.
    3. VLAN hopping enables an attacker to access different VLANs using 802.1q spoofing.
    4. VLAN hopping enables an attacker to change the native VLAN on a switch.

    Answer:

    C. Virtual Area Network (VLAN) hopping is a method for sending commands to switches to transfer a port from one VLAN to another. This can enable the attacker to connect his or her device to a potentially sensitive VLAN. VLAN hopping does not modify the switch's patch panel connections, only its VLAN assignments. It is not possible to rename a switch's default VLAN. VLAN hopping does not enable an attacker to change a switch's native VLAN.
68. Which of the following tools are needed by an individual performing a war driving attack? (Choose all that apply.)

    1. A stolen credit card number
    2. A wireless-equipped computer or other device
    3. A screwdriver
    4. An automobile or other vehicle
    5. A telephone

    Answer:

    B, D. War driving is an attack method that consists of driving around a neighborhood with a computer, scanning for unprotected wireless networks. It therefore requires nothing more than a vehicle and a wireless-equipped computer. The term _driving_ in war driving refers to driving a vehicle, not a screw; a screwdriver is therefore not required. War driving uses a wireless computer or other device to scan for open networks; a telephone is therefore not required. War driving is a means for locating unprotected networks; it does not require a credit card number, nor does it involve stealing them.
69. Which of the following types of attacks can be used to enable an intruder to access a wireless network despite the protection provided by MAC filtering?

    1. Spoofing
    2. Brute-force
    3. DNS poisoning
    4. War driving

    Answer:

    A. Spoofing is the process of modifying network packets to make them appear as though they are transmitted by or addressed to someone else. One way of doing this is to modify the Media Access Control (MAC) address in the packets to one that is approved by the MAC filter. Brute-force is the method of repeated guessing, which is impractical with MAC addresses. A Domain Name System (DNS) works with IP addresses, not MAC addresses. War driving is the process of looking for unprotected Wireless Access Points (WAPs).
70. Which of the following terms refers to a type of Denial-of-Service (DoS) attack that uses multiple computers to bombard a target server with traffic?

    1. Amplified
    2. Reflective
    3. Distributed
    4. Permanent

    Answer:

    C. A Distributed Denial-of-Service (DDoS) attack is one in which the attacker uses hundreds or thousands of computers, controlled by malware and called bots or zombies, to send traffic to a single server or website in an attempt to overwhelm it and prevent it from functioning. An amplified DoS attack is one in which the messages sent by the attacker require an extended amount of processing by the target servers, increasing the burden on them more than simpler messages would. A reflective DoS attack is one in which the attacker sends requests containing the target server's IP address to legitimate servers on the Internet, such as Domain Name System (DNS) servers, causing them to send a flood of responses to the target. A permanent DoS attack is one in which the attacker actually damages the target system and prevents it from functioning.
71. Which of the following terms refers to a type of Denial-of-Service (DoS) attack that bombards a target server with traffic that requires a large amount of processing?

    1. Amplified
    2. Reflective
    3. Distributed
    4. Permanent

    Answer:

    A. An amplified DoS attack is one in which the messages sent by the attacker require an extended amount of processing by the target servers, increasing the burden on them more than simpler messages would. A reflective DoS attack is one in which the attacker sends requests containing the target server's IP address to legitimate servers on the Internet, such as Domain Name System (DNS) servers, causing them to send a flood of responses to the target. A Distributed Denial-of-Service (DDoS) attack is one in which the attacker uses hundreds or thousands of computers, controlled by malware and called bots or zombies, to send traffic to a single server or website in an attempt to overwhelm it and prevent it from functioning. A permanent DoS attack is one in which the attacker actually damages the target system and prevents it from functioning.
72. Which of the following types of attacks are rarely seen anymore because of changes in device design that were specifically designed to prevent them? (Choose all that apply.)

    1. VLAN hopping
    2. Logic bomb
    3. Phishing
    4. Smurf

    Answer:

    A, D. Smurf attacks rely on routers to forward broadcast traffic. Routers no longer forward broadcast messages, so smurf attacks have been rendered ineffective. In the same way, Virtual Area Network (VLAN) hopping, which is a method for sending commands to switches to transfer a port from one VLAN to another, is rarely seen because switches are now designed to prevent them. A logic bomb is a code insert placed into a legitimate software product that triggers a malicious event when specific conditions are met. Phishing is the term for a bogus email or website designed to infect users with some type of malware. Both of these are still commonly used attack types.
73. Which of the following terms refers to a Denial-of-Service (DoS) attack in which an attacker breaks into a company's datacenter and smashes its servers with a sledgehammer?

    1. Amplified
    2. Reflective
    3. Distributed
    4. Permanent

    Answer:

    D. Although DoS attacks typically involve traffic flooding, any attack that prevents a server from functioning can be called a DoS attack. A permanent DoS attack is one in which the attacker actually damages the target system and prevents it from functioning. This can be a physical attack that damages the hardware, or the attacker can disable the server by altering its software or configuration settings. A Distributed Denial-of-Service (DDoS) attack is one in which the attacker uses hundreds or thousands of computers, controlled by malware and called bots or zombies, to send traffic to a single server or website in an attempt to overwhelm it and prevent it from functioning. An amplified DoS attack is one in which the messages sent by the attacker require an extended amount of processing by the target servers, increasing the burden on them more than simpler messages would. A reflective DoS attack is one in which the attacker sends requests containing the target server's IP address to legitimate servers on the Internet, such as Domain Name System (DNS) servers, causing them to send a flood of responses to the target.
74. Which of the following terms refers to a Denial-of-Service (DoS) attack that involves zombies?

    1. Amplified
    2. Reflective
    3. Distributed
    4. Permanent

    Answer:

    C. Distributed Denial-of-Service (DDoS) attacks use hundreds or thousands of computers that have been infected with malware, called bots or zombies, to flood a target server with traffic, in an attempt to overwhelm it and prevent it from functioning. A reflective DoS attack is one in which the attacker sends requests containing the target server's IP address to legitimate servers on the Internet, such as Domain Name System (DNS) servers, causing them to send a flood of responses to the target. A reflective attack does not require infected computers; it takes advantage of the servers' native functions. An amplified DoS attack is one in which the messages sent by the attacker require an extended amount of processing by the target servers, increasing the burden on them more than simpler messages would. A permanent DoS attack is one in which the attacker actually damages the target system and prevents it from functioning.
75. Which of the following types of attacks can cause a user's attempts to connect to an Internet website to be diverted to an attacker's website instead?

    1. Evil twin
    2. ARP poisoning
    3. Spoofing
    4. DNS poisoning

    Answer:

    D. Domain Name System (DNS) poisoning is a type of attack in which an attacker adds fraudulent information into the cache of a DNS server. Then, when a client attempts to resolve the name of a website or other server, the DNS server supplies the incorrect IP address, causing the client to access the attacker's server instead. An evil twin is a rogue Wireless Access Point (WAP) on a network. Address Resolution Protocol (ARP) poisoning is the deliberate insertion of fraudulent information into the ARP cache stored on computers and switches, which can interfere with the resolution of IP addresses into Media Access Control (MAC) addresses on a local level. Spoofing is the process of modifying network packets to make them appear as though they are transmitted by or addressed to someone else.
76. Which of the following functions can be interfered with by a DNS poisoning attack?

    1. IP address resolution
    2. Name resolution
    3. Password protection
    4. Network switching

    Answer:

    B. Domain Name System (DNS) poisoning is a type of attack in which an attacker adds fraudulent information into the cache of a DNS server. This can interfere with the name resolution process by causing a DNS server to supply the incorrect IP address for a specified name. The process of resolving an IP address into a Media Access Control (MAC) address can be interfered with by Address Resolution (ARP) poisoning. DNS has nothing to do with passwords or switching.
77. In testing the new application he has designed, Ralph has discovered that it contains a weakness that could enable an attacker to gain full administrative access. Which of the following is another term for this weakness?

    1. Exploit
    2. Mitigation
    3. Vulnerability
    4. Honeypot

    Answer:

    C. A vulnerability is a potential weakness in a system that an attacker can use to his or her advantage. An exploit is a hardware or software element that is designed to take advantage of a vulnerability. A mitigation is a form of defense against attacks on system security. A honeypot is a computer configured to function as bait for attackers, causing them to waste their time penetrating a resource that provides no significant access.
78. A senior IT administrator at your company was terminated two weeks ago. Today, Friday, you arrived at the office and found that all of the hosts in the web server farm had had their data deleted. There are no unauthorized entries to the datacenter recorded, but you suspect the terminated administrator is responsible for deleting the data. Which of the following attack types might the administrator have directed at the web server farm?

    1. Social engineering
    2. ARP poisoning
    3. Evil twin
    4. Logic bomb

    Answer:

    D. A logic bomb is a code insert placed into a legitimate software product that triggers a malicious event when specific conditions are met. The terminated administrator might have created code designed to trigger the deletions after the administrator's departure from the company. Social engineering is a form of attack in which an innocent user is persuaded by an attacker to provide sensitive information via email or telephone. The Address Resolution Protocol (ARP) is responsible for resolving IP addresses into Media Access Control (MAC) addresses. ARP poisoning is the deliberate insertion of fraudulent information into the ARP cache stored on computers and switches. An evil twin is a fraudulent access point on a wireless network.
79. Which of the following attack types can be facilitated by ARP poisoning? (Choose all that apply.)

    1. Evil twin
    2. On-path
    3. Session hijacking
    4. Social engineering

    Answer:

    B, C. Address Resolution Protocol (ARP) poisoning is the deliberate insertion of fraudulent information into the ARP cache stored on computers and switches. This can enable an attacker to intercept traffic intended for another system. In an on-path (man-in-the-middle) attack, the attacker can read the intercepted traffic and even modify it before sending it on to the destination. In a session hijacking attack, the attacker can use the intercepted traffic to obtain authentication information, including passwords. An evil twin is a fraudulent access point on a wireless network. Social engineering is a form of attack in which an innocent user is persuaded by an attacker to provide sensitive information via email or telephone.
80. Which of the following statements best describes a type of replay attack?

    1. An intruder reenters a resource previously compromised by another intruder.
    2. An intruder retransmits captured authentication packets to gain access to a secured resource.
    3. An intruder uses the same technique that provided access to other resources to penetrate a new resource.
    4. An intruder accesses a resource that was accidentally left unsecured by an authorized user.

    Answer:

    B. A replay attack is one in which an attacker utilizes the information found in previously captured packets to gain access to a secured resource. In many cases, the captured packets contain authentication data. In this way, the attacker can make use of captured passwords, even when they are encrypted and cannot be displayed. The other options all describe valid attack methodologies, but they are not called replay attacks.
81. Ed receives an email through his personal account, warning him that his checking account has been locked due to excessive activity. To confirm that the activity is fraudulent, the email instructs Ed to click the enclosed hyperlink, log on to his account, and review the list of charges. Ed clicks the link and is taken to a web page that appears to be that of his bank. He then supplies his username and password to log on. Which of the following types of attacks is Ed likely to be experiencing?

    1. Social engineering
    2. Phishing
    3. Logic bomb
    4. Spoofing

    Answer:

    B. This is a classic example of a phishing scam. In all likelihood, the link in the email Ed received has taken him not to the real website of his bank, but rather a duplicate created by an attacker. By supplying his logon credentials, he is in effect giving them to the attacker, who can now gain access to his real bank account. Social engineering is the practice of obtaining sensitive data by contacting users and pretending to be someone with a legitimate need for that data. A logic bomb is a code insert placed into a legitimate software product that triggers a malicious event when specific conditions are met. Spoofing is the process of modifying network packets to make them appear as though they are transmitted by or addressed to someone else.
82. Which of the following attack types are specifically directed at wireless networks? (Choose all that apply.)

    1. Evil twin
    2. Phishing
    3. Deauthentication
    4. War driving

    Answer:

    A, C, D. An evil twin is a fraudulent access point on a wireless network that mimics the Service Set Identifier (SSID) of a legitimate access point, in the hope of luring in users. War driving is an attack method that consists of driving around a neighborhood with a computer, scanning for unprotected wireless networks. Deauthentication is a type of Denial-of-Service (DoS) attack in which the attacker targets a wireless client by sending a deauthentication frame that causes the client to be disconnected from the network. Phishing is an attack type that is targeted at all users, not just wireless ones.
83. Which of the following are not considered to be Denial-of-Service (DoS) attacks? (Choose all that apply.)

    1. An intruder breaks into a company's datacenter and smashes their web servers with a sledgehammer.
    2. An attacker uses the `ping` command with the `-t` parameter to send a continuous stream of large Internet Control Message Protocol (ICMP) packets to a specific server.
    3. An attacker captures the packets transmitted to and from a domain controller to obtain encrypted passwords.
    4. An attacker connects a rogue access point to a company's wireless network, using their Service Set Identifier (SSID) in the hope of attracting their users.

    Answer:

    C, D. A DoS attack is one designed to prevent a target from fulfilling its function. While `ping` floods are a common form of server DoS attacks, physically damaging the server hardware also prevents it from performing its function. Therefore, this too is a type of DoS attack. Capturing packets and rogue access points are not typically described as DoS attacks.
84. In the hacker subculture, which of the following statements best describes a zombie?

    1. A computer that is remotely controllable because it has been infected by malware
    2. A computer that is no longer functioning because it is the target of a Denial-of-Service (DoS) attack
    3. A user that has fallen victim to a phishing attack
    4. A program that attackers use to penetrate passwords using brute-force attacks

    Answer:

    A. A zombie (or bot) is a computer that has been infected by malware—usually some form of Trojan—which an attacker can control remotely, causing the computer to flood a target system with traffic. An attack using multiple zombies is known as a Distributed Denial-of-Service (DDoS) attack. The other options are not examples of zombies.
85. Which of the following statements best describes a ransomware attack?

    1. A website is rendered inaccessible by a Denial-of-Service (DoS) attack until its owner agrees to pay a fee.
    2. A user's access to a specific resource, such as a bank's website, is blocked until the user pays a fee.
    3. A message appears on a user's screen, stating that system is locked and will only be released on payment of a fee.
    4. An application is supplied with limited usability until the user pays a license fee.

    Answer:

    C. Ransomware is a type of attack in which a user's access to his or her computer or data is blocked unless a certain amount of money is paid to the attacker. The blockages can vary from simple screen locks to data encryption.
86. Which of the following types of attacks requires no computer equipment?

    1. Denial-of-Service
    2. Social engineering
    3. Brute-force
    4. Dictionary
    5. Phishing

    Answer:

    B. Social engineering is the practice of obtaining sensitive data by contacting users and pretending to be someone with a legitimate need for that data. No computer equipment is required, and no software or hardware solution can prevent it; the only way is to educate users on the potential dangers and establish policies that inform users what to do when they experience a social engineering attempt. Denial-of-Service (DoS) is a type of attack that overwhelms a computer with traffic, preventing it from functioning properly. A brute-force or dictionary attack is one in which an attacker uses repeated guesses to find a password, an open port, or some other type of sensitive data. Phishing is the term for a bogus email or website designed to infect users with some type of malware.
87. Which of the following best describes a brute-force attack?

    1. An attacker breaking down the door of a datacenter
    2. An attacker cracking a password by trying thousands of guesses
    3. An attacker using zombie computers to flood a server with traffic
    4. An attacker deploying an unauthorized access point on a wireless network

    Answer:

    B. A brute-force attack (also called a dictionary attack) is one in which an attacker uses repeated guesses to find a password, an open port, or some other type of sensitive data. Brute-force does not refer to a physical attack. Flooding a server with traffic created by zombies is a Distributed Denial-of-Service (DDoS) attack. Deploying an unauthorized access point is an evil twin attack.
88. An intruder has deployed a rogue access point on your company's wireless network and is using it to access traffic generated by users who have accidentally connected to it. Which of the following is the name for this type of attack?

    1. Evil twin
    2. War driving
    3. Social networking
    4. Spoofing

    Answer:

    A. An evil twin is a fraudulent access point on a wireless network, which an intruder can use to obtain passwords and other sensitive information transmitted by users. War driving is the term for seeking out open wireless networks. Social engineering is a form of attack in which an innocent user is persuaded by an attacker to provide sensitive information via email or telephone. Spoofing is the process of modifying network packets to make them appear as though they are transmitted by or addressed to someone else.
89. A person identifying herself as Trixie from IT telephones a user called Alice and tells her that there is a problem with her network user account that could cause all her data to be lost. To resolve the problem, Trixie says that she must log on using Alice's account and configure an important setting. All she needs to do this is Alice's account password. This call is, of course, an illicit attempt to learn Alice's password. Which of the following terms describes the type of attack that is currently occurring?

    1. On-path
    2. Spoofing
    3. Social engineering
    4. Evil twin

    Answer:

    C. Social engineering is the term for a type of attack in which a smooth-talking intruder contacts a user and convinces him or her to disclose sensitive information, such as account passwords. An on-path (man-in-the-middle) attack is one in which an attacker intercepts network traffic, reads the traffic, and can even modify it before sending it on to the destination. Spoofing is the process of modifying network packets to make them appear as though they are transmitted by or addressed to someone else. An evil twin is a fraudulent access point on a wireless network.
90. Regularly applying operating system updates and patches to network computers is an important mitigation procedure for which of the following security problems?

    1. Denial-of-Service attacks
    2. Malware
    3. Social engineering
    4. Port security

    Answer:

    B. Operating system updates and patches are frequently released to address newly discovered exploits that make computers vulnerable to malware infestation. Applying updates on a regular basis can help to mitigate the impact of malware. Updates and patches typically cannot mitigate Denial of Service (DoS) attacks, and they have no effect on nontechnical dangers such as social engineering or dangers that apply to switches, such as port security hazards.
91. Which of the following is not a form of social engineering?

    1. Piggybacking
    2. Tailgating
    3. Shoulder surfing
    4. Evil twin
    5. Phishing

    Answer:

    D. The term _social engineering_ refers to various methods that attackers can use to gain access to secured resources by manipulating authorized users, either physically or digitally. An evil twin is a rogue access point deliberately connected to the network for malicious purposes, so it is not a form of social engineering. Piggybacking and tailgating typically refer to the practice of closely following an authorized individual through a physical security barrier, such as a locked door or a guarded entrance. Shoulder surfing is a method of gathering sensitive information by passing behind a user and looking at their monitor. Phishing is a digital form of social engineering in which a user is duped into disclosing sensitive information by a faked email or other communication.
92. Which of the following standards defines a framework for the authentication process, but does not specify the actual authentication mechanism?

    1. WPA
    2. EAP
    3. TKIP
    4. TLS

    Answer:

    B. Extensible Authentication Protocol (EAP) is a framework for the encapsulation of authentication messages. EAP is used on wireless networks and point-to-point connections and supports dozens of different authentication methods. WiFi Protected Access (WPA) is a wireless encryption standard. Temporal Key Integrity Protocol (TKIP) is an encryption algorithm. Transport Layer Security (TLS) is an encryption protocol used for Internet communications.
93. EAP and 802.1X are components that help to provide which of the following areas of wireless network security?

    1. Authentication
    2. Authorization
    3. Encryption
    4. Accounting

    Answer:

    A. Extensible Authentication Protocol (EAP) and 802.1X are both components of an authentication mechanism used on many wireless networks. EAP and 802.1X do not themselves provide authorization, encryption, or accounting services.
94. Which of the following Extended Authentication Protocol (EAP) variants utilize tunneling to provide security for the authentication process? (Choose all that apply.)

    1. PEAP
    2. EAP-FAST
    3. EAP-TLS
    4. EAP-PSK

    Answer:

    A, B. Protected Extended Authentication Protocol (PEAP) encapsulates EAP inside a Transport Layer Security (TLS) tunnel. Flexible Authentication via Secure Tunneling (FAST) also establishes a TLS tunnel to protect user credential transmissions. EAP-TLS uses TLS for encryption, but not for tunneling. EAP-PSK uses a preshared key to provide an authentication process that does not use encryption.
95. A wireless network is configured to allow clients to authenticate only when the signal strength of their connections exceeds a specified level. Which of the following terms best describes this configuration?

    1. Local authentication
    2. Port security
    3. Geofencing
    4. Motion detection

    Answer:

    C. _Geofencing_ is the generic term for a technology that limits access to a network or other resource based on the client's location. In wireless networking, geofencing is intended to prevent unauthorized clients outside the facility from connecting to the network. Local authentication is an application or service that triggers an authentication request to which the user must respond before access is granted. Port security is a method for protecting access to switch ports. Motion detection is a system designed to trigger a notification or alarm when an individual trespasses in a protected area.
96. Which of the following best describes a wireless network that uses geofencing as a security mechanism?

    1. A wireless network that allows clients to authenticate only when the signal strength of their connections exceeds a specified level
    2. A wireless network that requires users to log on to a wired system before they can authenticate on a wireless device
    3. A wireless network that requires users to have an Active Directory account located within the local site
    4. A wireless network that requires users to type in the local Service Set Identifier (SSID) before they can authenticate

    Answer:

    A. Geofencing is a mechanism that is intended to prevent unauthorized clients outside the facility from connecting to the network. The mechanism can take the form of a signal strength or power level requirement, a GPS location requirement, or strategic placement of the antennae for wireless access points. The other options listed are not descriptions of typical geofencing technologies.
97. Which of the following elements associates a public and private key pair to the identity of a specific person or computer?

    1. Exploit
    2. Signature
    3. Certificate
    4. Resource record

    Answer:

    C. As part of a public key infrastructure (PKI), digital certificates are associated with a key pair, consisting of a public key and a private key. The certificate is issued to a person or computer as proof of its identity. A signature does not associate a person or computer with a key pair. An exploit is a hardware or software element that is designed to take advantage of a vulnerability. Resource records are associated with the Domain Name System (DNS).
98. In addition to EAP-TLS, which of the following are also Extensible Authentication Protocol (EAP) variants that use the Transport Layer Security (TLS) protocol? (Choose all that apply.)

    1. PEAP
    2. EAP-PWD
    3. EAP-MD5
    4. EAP-FAST

    Answer:

    A, D. The Protected Extensible Authentication Protocol (PEAP) and EAP Flexible Authentication via Secure Tunneling (EAP-FAST) both use TLS tunneling to secure authentication transmissions. EAP Password (EAP-PWD) and EAP-MP5 do not use TLS for tunneling or any other purpose.
99. Which of the following can be described as wireless network hardening techniques? (Choose all that apply.)

    1. Encryption
    2. Authentication
    3. MAC filtering
    4. Social engineering
    5. Antenna placement

    Answer:

    A, B, C, E. Encryption, authentication, Media Access Control (MAC) filtering, and antenna placement are all techniques for hardening a wireless network against attack. Social engineering is a type of attack in which an intruder contacts a user and convinces him or her to disclose sensitive information, such as account passwords; it is not specifically associated with wireless networks.
100.    Despite having imposed password policies on his network, compelling users to change their passwords frequently, create passwords of a specific length, and use complex passwords, Ralph has had several reports of account penetrations. The victims of the incidents had all apparently shared a “tip” suggesting that users cycle through the names of their children, nephews, nieces, and other relatives when forced to create new passwords, changing letters to numbers as needed. Which of the following actions can Ralph take to remedy the situation without creating a larger problem?

        1. Distribute a list of common passwords that are insecure, such as those based on names, birth dates, etc.
        2. Modify the password policies to force users to change passwords more frequently
        3. Assign the users long passwords consisting of random-generated characters and change them often
        4. Change the password history policy to a value greater than the number of children in any user's family

        Answer:

        A. There are no policies that can prevent users from creating easily guessed passwords. The only action that can help is to educate users on the fact that attackers are frequently able to guess passwords by using information such as familiar names and dates. Forcing more frequent password changes would not compel users to alter their method for choosing passwords, nor would increasing the password history value. Assigning random passwords would address the issue, but user complaints and forgotten passwords would likely create greater problems than it would solve.
101.    Which of the following devices are likely to have default credentials configured into them that attackers might know? (Choose all that apply.)

        1. Wireless access points
        2. Windows servers
        3. Switches
        4. Routers

        Answer:

        A, C, D. Access points, switches, and routers all require authentication to access their administrative interfaces, and most have a standard username and password configured at the factory. The purchaser can modify the default credentials, but many people fail to do so. Windows servers do not have default credentials assigned; the installer is prompted to specify an Administrator password during the setup process.
102.    One of the basic principles of network device hardening is to use secure protocols. Which of the following suggestions comply with this principle? (Choose all that apply.)

        1. Use SSH instead of Telnet.
        2. Use WEP instead of WPA2.
        3. Use TKIP instead of AES.
        4. Use HTTPS instead of HTTP.

        Answer:

        A, D. Secure Shell (SSH) and Telnet are both remote terminal programs, but Telnet passes instructions (including passwords) in cleartext, whereas SSH is encrypted. Hypertext Transfer Protocol Secure (HTTPS) is the encrypted version of Hypertext Transfer Protocol (HTTP). In both of these cases, the suggested substitute is more secure. However, Temporal Key Integrity Protocol (TKIP) provides less secure encryption than Advanced Encryption Standard (AES), and Wired Equivalent Protocol (WEP) is less secure than WiFi Protected Access 2 (WPA2).
103.    On which of the following types of devices should you consider disabling unused ports as a security precaution? (Choose all that apply.)

        1. Hubs
        2. Servers
        3. Switches
        4. Wireless Access Points

        Answer:

        B, C. Servers and switches are both devices on which unused ports can be a security hazard, but they use the term port differently. Servers have application layer ports that permit specific types of service traffic to enter the server. Switches have ports to which administrators can connect computers and other devices. Both can provide attackers with unauthorized access to the device. It is not possible to disable hub ports, and the Wireless Access Points (WAPs) used on enterprise networks typically have only a single port.
104.    For which of the following reasons is disabling the Service Set Identifier (SSID) broadcast of a wireless network to prevent unauthorized access a relatively weak method of device hardening?

        1. Attackers have ways of connecting to the network without the SSID.
        2. Attackers can capture packets transmitted over the network and read the SSID from them.
        3. Every access point's SSID is printed on a label on the back of the device.
        4. Attackers have software that can easily guess a network's SSID

        Answer:

        B. Disabling SSID broadcasts is a way of hiding the presence of a wireless network, but if an intruder knows that a network is there, it is a simple matter to capture packets transmitted by the wireless devices and read the SSID from them. It is not possible to connect to a wireless network without the SSID. SSIDs are set by the administrator of the access point; they are not printed on the device's label. SSIDs can be found relatively easily but guessing them is no easier than guessing a password.
105.    Which of the following cannot be considered to be a server hardening policy?

        1. Disabling unnecessary services
        2. Disabling unused TCP and UDP ports
        3. Upgrading firmware
        4. Creating privileged user accounts

        Answer:

        C. Upgrading the UEFI or BIOS firmware on a server typically does not enhance its security, so it cannot be considered a form of server hardening. Disabling services and ports that are not in use reduces the attack surface of a server, and creating privileged user accounts reduces the chance that privileged accounts will be compromised. Therefore, these are all forms of server hardening.
106.    Which of the following are valid reasons not to disable unused switch ports? (Choose all that apply.)

        1. The datacenter is secured from unauthorized access.
        2. The unused ports are not patched in to wall jacks.
        3. The unused ports are left open to facilitate the on-boarding of new users.
        4. The switch is configured to use a MAC-based access control list.

        Answer:

        A, D. If there is no way for unauthorized people to access the datacenter, then there is no danger of someone plugging a device into a port that is left enabled. If the switch uses an Access Control List (ACL) that specifies the Media Access Control (MAC) addresses of systems permitted to connect to it, then there is no need to disable unused ports. However, disabling the ports is probably far easier than creating and maintaining the ACL. Ports that are not patched in can still be compromised at the switch location. Enabling ports is not difficult, so accommodating new users is not a valid reason for leaving them enabled.
107.    Which of the following Windows password policies includes a provision to prevent users from specifying common passwords?

        1. Maximum password age
        2. Enforce password history
        3. Minimum password length
        4. Passwords must meet complexity requirements

        Answer:

        D. The “Passwords must meet complexity requirements” policy includes a provision that new passwords cannot include the user's account name or full name. If the full name is delimited by spaces or punctuation, the individual words cannot appear in the password either. The other options do not prevent the use of common passwords.
108.    Which of the following is not a method for hardening a Wireless Access Point (WAP)?

        1. Upgrading firmware
        2. Changing default credentials
        3. Generating new Pre-Shared Keys
        4. Deauthentication

        Answer:

        D. Deauthentication is a type of Denial-of-Service (DoS) attack in which the attacker targets a wireless client by sending a deauthentication frame that causes the client to be disconnected from the network. It is therefore not a method for hardening an access point. Upgrading the device's firmware to apply security fixes, changing the default administrative credentials applied at the factory, and frequent Pre-Shared Key (PSK) changes are all means of hardening the security of an access point.
109.    Creating a policy instructing users to avoid passwords that use commonly shared information, such as birth dates and the names of children and pets, is an example of which of the following?

        1. Mitigation techniques
        2. Multifactor authentication
        3. Network hardening
        4. Access control

        Answer:

        C. _Network hardening_ is a term used to describe any method of making it more difficult for intruders to penetrate. In many cases, network hardening techniques are based on education rather than technology. Compelling users to create passwords that are difficult to guess is one example of this. Mitigation techniques are methods for reducing the severity of an attack. Multifactor authentication calls for the use of two different identity confirmation mechanisms, such as a password and a fingerprint. Access control is a technique for creating a list of approved users or systems.
110.    Which of the following are the default administrative user accounts found in Windows and Linux operating systems? (Choose all that apply.)

        1. Administrator
        2. root
        3. admin
        4. Control

        Answer:

        A, B. Administrator is the default administrative user account in Windows, and root is the administrative account in Linux. Control and admin are not privileged user accounts provided with the operating systems.
111.    Which of the following are network segmentation methods that can prevent intruders from gaining full access to a network? (Choose all that apply.)

        1. ACL
        2. VLAN
        3. NAC
        4. DMZ

        Answer:

        B, D. Virtual Local Area Networks (VLANs) can be used to isolate systems on a separate network segment. A demilitarized zone (DMZ), also called a screened subnet or a perimeter network, is a network segment accessible from the Internet and separated from the internal network by a firewall. Both of these are methods for isolating systems to prevent security breaches from spreading beyond their bounds. Access Control Lists (ACLs) and Network Access Control (NAC) are both methods for enhancing network security, but they are not segmentation methods.
112.    Which of the following types of mitigation techniques is not applicable to servers?

        1. Role separation
        2. Applying ACLs
        3. File integrity monitoring
        4. DHCP snooping

        Answer:

        D. Dynamic Host Configuration Protocol (DHCP) snooping is a feature found in some network switches that prevents rogue DHCP servers from assigning IP addresses to clients. It can also detect when DHCP release or decline messages arrive over a port other than the one on which the DHCP transaction originated. The other options are all techniques that are applicable to servers.
113.    Which of the following services are provided by Access Control Lists (ACLs)?

        1. Authentication
        2. Authorization
        3. Accounting
        4. Auditing

        Answer:

        B. ACLs define the type of access granted to authenticated users. This process is known as authorization. Authentication is the confirmation of a user's identity. Accounting and auditing are both methods of tracking and recording a user's activities on a network.
114.    Which of the following terms describes the threat mitigation technique of deploying individual applications and services on virtual servers so that no more than one is endangered at any one time, rather than deploying multiple applications on a single server?

        1. Geofencing
        2. Network segmentation
        3. Role separation
        4. VLAN hopping

        Answer:

        C. Role separation is the practice of creating a different virtual server for each server role or application. In addition to providing other benefits as well, this forces intruders to mount attacks on multiple servers to disable an entire network. Geofencing is a technique for limiting access to a wireless network. Network segmentation describes the process of creating multiple Virtual Local Area Networks (VLANs) or deploying firewalls to isolate part of a network. VLAN hopping is a type of attack in which an intruder sends command messages to a switch to transfer a port from one VLAN to another.
115.    Role separation is a threat mitigation technique that is applied to which of the following types of network components?

        1. Switches
        2. Servers
        3. Routers
        4. Wireless Access Points (WAPs)

        Answer:

        B. Role separation is the practice of creating a different virtual server for each server role or application. In addition to providing other benefits as well, this forces intruders to mount attacks on multiple servers to disable an entire network. Switches, routers, and access points do not use this technique.
116.    A server's firewall is configured using a default policy that does not allow any users remote access to the server unless an administrator creates a rule granting them access. Which of the following terms describes this default policy?

        1. Explicit allow
        2. Explicit deny
        3. Implicit allow
        4. Implicit deny

        Answer:

        D. An implicit deny is a policy that denies access to a resource by default, without a rule defining that denial. Creating a new rule denying access is an explicit deny. If anyone was able to access the server remotely by default, that would be an implicit allow. An explicit allow is a rule granting specific users remote access.
117.    Dynamic ARP Inspection (DAI) is a feature in some network switches that prevents on-path (man-in-the-middle) attacks facilitated by Address Resolution Protocol (ARP) poisoning, the deliberate insertion of fraudulent information into the ARP cache. A switch with DAI inspects incoming ARP packets and rejects those that contain incorrect pairs of IP and Media Access Control (MAC) addresses. Which of the following is the means by which the switch compiles a table of the correct ARP information for comparison with the incoming packets?

        1. DHCP snooping
        2. Secure SNMP
        3. DNS name resolution
        4. NDP

        Answer:

        A. Dynamic Host Configuration Protocol (DHCP) snooping is a process in which the switch examines DHCP traffic to determine the IP addresses that DHCP servers have assigned to specific MAC addresses. DAI detects ARP poisoning attempts by comparing the IP-and-MAC address pairs in ARP packets with those in the DHCP snooping table it has compiled. The switch then discards packets with address pairs that do not match. Secure SNMP Secure Network Protocol (SNP), Domain Name Server (DNS) name resolution, and Neighbor Discovery Protocol (NDP) are not used to implement DAI.
118.    Which of the following statements about DHCP snooping is not true?

        1. DHCP snooping detects rogue DHCP servers.
        2. DHCP snooping is implemented in network switches.
        3. DHCP snooping drops DHCP messages arriving over the incorrect port.
        4. DHCP snooping prevents DNS cache poisoning.

        Answer:

        D. Dynamic Host Configuration Protocol (DHCP) snooping is a feature found in some network switches that prevents rogue DHCP servers from assigning IP addresses to clients. It can also detect when DHCP release or decline messages arrive over a port other than the one on which the DHCP transaction originated. Although DHCP snooping can prevent DHCP clients from being assigned an incorrect IP address, it does not directly prevent the poisoning of Domain Name System (DNS) server caches with erroneous information.
119.    At which layer of the Open Systems Interconnection (OSI) reference model does Dynamic Host Configuration Protocol (DHCP) snooping operate?

        1. Data link
        2. Network
        3. Transport
        4. Application

        Answer:

        A. Although DHCP is an application layer service that uses the User Datagram Protocol (UDP) transport layer protocol to assign network layer IP addresses, DHCP snooping is a data link layer process in which a network switch examines incoming DHCP traffic to determine whether it originates from an authorized server and is arriving over the correct port.
120.    Which of the following types of attacks on a network switch can a flood guard help to prevent?

        1. DNS poisoning
        2. War driving
        3. MAC flooding
        4. Evil twin

        Answer:

        C. By flooding a switch with packets containing many different false Media Access Control (MAC) addresses, an attacker can cause the legitimate entries in the switch's MAC table to be aged out of the device and replaced with bogus entries. When the destinations of incoming packets are not found in the table, the switch broadcasts them throughout the network, where they can be more readily captured and compromised. A flood guard is a mechanism that prevents confirmed MAC addresses in the table from being replaced. A flood guard in a switch cannot protect against Domain Name System (DNS) poisoning, war driving, or evil twin attacks.
121.    Which of the following protocols is a root guard designed to affect?

        1. EAP
        2. STP
        3. LDAP
        4. ARP

        Answer:

        B. A root guard affects the behavior of the Spanning Tree Protocol (STP) by enforcing the selection of root bridge ports on a switched network. Without root guards, there is no way for administrators to enforce the topology of a network with a redundant switching fabric. Root guards do not affect the Extensible Authentication Protocol (EAP), the Lightweight Directory Access Protocol (LDAP), or the Address Resolution Protocol (ARP).
122.    Which of the following mitigation techniques helps organizations maintain compliance to standards such as HIPAA and FISMA?

        1. File integrity monitoring
        2. Role separation
        3. Deauthentication
        4. Tamper detection
        5. Router Advertisement guard

        Answer:

        A. File integrity monitoring (FIM) is a process that typically consists of a comparison of files in their current state to a known baseline copy stored elsewhere. The comparison can be direct, or it could involve the calculation of checksums or other types of file hashes. The object of the comparison is to detect changes in documents, both in content and in sensitive areas, such as credentials, privileges, and security settings, which might indicate the presence of a potential or actual security breach. Role separation applies to the deployment of applications on servers. Deauthentication is a type of wireless network attack. Tamper detection is a term used to describe a physical security measure for hardware. Router Advertisement (RA) guard is a feature found on certain switches that prevents the misuse of RA messages to redirect traffic.
123.    Which of the following functions cannot be implemented using digital signatures?

        1. Integrity
        2. Nonrepudiation
        3. Segmentation
        4. Authentication

        Answer:

        C. Digital signatures can be used for the following functions: authentication, to confirm that data originated from a specific individual; nonrepudiation, to prevent the sender from denying the data's origin; and integrity, to confirm that the data has not been modified in transit. Segmentation is not a function of digital signatures.
124.    When Ralph digitally signs and encrypts a document with his private key, Alice can decrypt the document only by using Ralph's public key. As long as the private key is accepted to be secure, which of the following statements are true? (Choose all that apply.)

        1. Ralph cannot deny having created the document.
        2. No one has altered the document since Ralph sent it.
        3. No one but Ralph can have created the document.
        4. No one but Alice can decrypt and read the document.

        Answer:

        A, B, C. Because only Ralph possesses the private key, only he could have signed and encrypted it. Although it is possible for someone other than Alice to have decrypted the document while it was in transit, using Ralph's public key, that individual could not have modified it and encrypted it again.
125.    When Alice encrypts a document with Ralph's public key, Ralph can decrypt the document only by using his private key. As long as the private key is accepted to be secure, which of the following statements are true? (Choose all that apply.)

        1. Alice cannot deny having created the document.
        2. No one has opened the document since Alice sent it.
        3. No one but Alice can have created the document.
        4. No one but Ralph can decrypt and read the document.

        Answer:

        B, D. Because anyone can obtain Ralph's public key, the document could have been created and encrypted by anyone. However, because only Ralph possesses the private key that can decrypt the document, he can be sure that no one else has opened it while it was in transit.
126.    Which of the following types of patches is most typically applied to a hardware device?

        1. Firmware updates
        2. Driver updates
        3. Feature changes
        4. Vulnerability patches

        Answer:

        A. Firmware is a type of software permanently written to the memory built into a hardware device. A firmware patch overrides the read-only nature of this memory to update the software. Driver updates, feature updates, and vulnerability patches are typically applied to software products, such as applications and operating systems.
127.    Which of the following software releases is a fix designed to address one specific issue?

        1. A patch
        2. An update
        3. An upgrade
        4. A service pack

        Answer:

        A. A patch is a relatively small update that is designed to address a specific issue, often a security exploit or vulnerability. Patches do not add features or new capabilities; they are fixes targeted at a specific area of the software. Updates, upgrades, and service packs are larger packages that might include new features and/or many different fixes.
128.    Unlike individual users, who usually have their operating system patches downloaded and installed automatically, corporate IT departments typically evaluate new patches before deploying them. Which of the following is not a common step in this evaluation process?

        1. Testing
        2. Researching
        3. Rolling back
        4. Backing up

        Answer:

        C. Rolling back, the process of uninstalling a patch to revert to the previous version of the software, is not part of the patch evaluation process. The evaluation process for new patches in a corporate environment usually consists of a research stage, in which you examine the need and purpose for the patch; a testing stage, in which you install the patch on a lab machine; and a backup of the production systems to which you will apply the patch.
129.    Which of the following terms refers to the process of uninstalling a recently released patch to resume using the previous version?

        1. Backslide
        2. Downgrade
        3. Reset
        4. Rollback

        Answer:

        D. _Rollback_ is a term used in change management to describe the process of reversing a change that has been made, to restore the original configuration. In the case of patch management, a rollback is the process of uninstalling a recently installed software update. The terms _backslide_, _downgrade_, and _reset_ are not used to describe this procedure.
130.    How does Media Access Control (MAC) address filtering increase the security of a Wireless Local Area Network (WLAN)?

        1. By preventing access points from broadcasting their presence
        2. By allowing traffic sent to or from specific MAC addresses through the Internet firewall
        3. By substituting registered MAC addresses for unregistered ones in network packets
        4. By permitting only devices with specified MAC addresses to connect to an access point
        5. By isolating specific wireless clients from the rest of the network

        Answer:

        D. MAC address filtering enables administrators to configure an access point to allow only devices with specific addresses to connect; all other traffic is rejected. Access points broadcast their presence using a Service Set Identifier (SSID), not a MAC address. MAC address filtering protects WLANs when implemented in an access point, not a firewall. MAC address filtering does not call for the modification of addresses in network packets. MAC filtering does not isolate clients from the network.
131.    Which of the following is the best description of geofencing?

        1. Something you have
        2. Something you know
        3. Something you do
        4. Somewhere you are

        Answer:

        D. Geofencing is the generic term for a technology that limits access to a network or other resource based on the client's location. It is therefore best described as somewhere you are. A finger gesture would be considered something you do, a password is something you know, and a smartcard is something you have.
132.    MAC filtering is an access control method used by which of the following types of hardware devices?

        1. Wireless Access Point
        2. RADIUS server
        3. Domain controller
        4. Smartcards

        Answer:

        A. Wireless Access Points (WAPs) typically include the ability to maintain an Access Control List (ACL), which specifies the Media Access Control (MAC) addresses of devices that are permitted to connect to the wireless network. The technique is known as MAC address filtering. Remote Authentication Dial-In User Service (RADIUS) servers, domain controllers, and smartcards typically do not include MAC filtering capabilities.
133.    Which of the following technologies utilize Access Control Lists (ACLs) to limit access to network resources? (Choose all that apply.)

        1. NTFS
        2. LDAP
        3. WAP
        4. Kerberos

        Answer:

        A, C. NTFS files and folders all have ACLs, which contain Access Control Entries (ACEs) that specify the users and groups that can access them and the specific permissions they have been granted. Wireless Access Points (WAPs) have ACLs that contain Media Access Control (MAC) addresses of the devices that are permitted to connect to the wireless network. Lightweight Directory Access Protocol (LDAP) and Kerberos are protocols that provide directory service communication and authentication, respectively. Neither one uses ACLs.
134.    Alice is a consultant working in your office, who has been given the Secure Set Identifier (SSID) and the passphrase for the company's main wireless network, but she is unable to connect with her laptop. Which of the following security measures might be preventing her from connecting?

        1. MAC filtering
        2. Disabling SSID broadcast
        3. Geofencing
        4. Using WPA2
        5. Guest network isolation

        Answer:

        A. Media Access Control (MAC) filtering takes the form of an Access Control List (ACL) on the wireless network's access points, listing the MAC addresses of all the devices that are to be permitted to access the network. If the MAC address of Alice's laptop is not included in the ACL, she will be unable to connect to the network. Alice has been given the SSID of the network, so she should be able to connect, even if the access points are not broadcasting the SSID. Geofencing is intended to prevent users outside the office from accessing the network, so this should not be the problem. Alice has been given the passphrase for the network, so she should be able to configure WiFi Protect Access 2 (WPA2) on her laptop. Alice is not using a separate guest network, so this is not preventing her from connecting.
135.    On a wireless network, which of the following best describes an example of a captive portal?

        1. A switch port used to connect to other switches
        2. A web page with which a user must interact before being granted access to a wireless network
        3. A series of two doors through which people must pass before they can enter a secured space
        4. A web page stating that the user's computer has been locked and will only be unlocked after payment of a fee

        Answer:

        B. A captive portal is a web page displayed to a user who is attempting to access a public wireless network. The user typically must supply credentials, provide payment, or accept a user agreement before access is granted. A captive portal does not refer to a switch port, a secured entryway to a room, or a type of extortionate computer attack.
136.    A user attempting to connect to a WiFi hotspot in a coffee shop is taken to a web page that requires her to accept an End User License Agreement (EULA) before access to the network is granted. Which of the following is the term for such an arrangement?

        1. Captive portal
        2. Ransomware
        3. Port security
        4. Root guard

        Answer:

        A. A web page that prompts users for payment, authentication, or acceptance of a EULA is a captive portal. Ransomware is a type of attack that extorts payment. Port security and root guards are methods for protecting access to switch ports.
137.    Which of the following is another term for a switching technique called port isolation?

        1. Frame relay
        2. Private VLAN
        3. Site-to-site VPN
        4. Screened subnet

        Answer:

        B. Port isolation, also known as Private Virtual Local Area Network (VLAN), is a feature in some switches that enables administrators to restrict selected ports to a given uplink, essentially creating a separate, secondary VLAN that is isolated from the switch's default, primary VLAN. Screened subnets (also called perimeter networks or demilitarized zones \[DMZs]), frame relay, and VPNs are not switching techniques.
138.    The Internet of Things (IoT) encompasses a huge number of device types ranging from personal electronics to household appliances to medical equipment to industrial machinery. Many of these devices deal with sensitive information, and many perform critically important tasks. The field of IoT security is still in its infancy; there is no all-encompassing standard defining IoT protection protocols. IoT devices have vastly different security requirements and also vastly different functional capabilities, making it difficult to create a blanket protection mechanism for all of them. Which of the following are potentially viable methods for securing all IoT devices against attack? (Choose all that apply.)

        1. Network segmentation
        2. Network Access Control (NAC)
        3. Security gateways
        4. Firewalls

        Answer:

        B, C. Because many IoT devices are mobile or located in unprotected areas, a firewall is not a viable protection mechanism for all of them, nor is the practice of placing them on separate network segments. Network security mechanisms such as access control policies and centralized gateways providing authentication and authorization could conceivably be incorporated into a general IoT security standard.
139.    Which of the following statements about a switch's default VLAN are true? (Choose all that apply.)

        1. Administrators must create a default VLAN when configuring a new switch.
        2. The default VLAN on a switch cannot be deleted.
        3. The default VLAN on most switches is designated as VLAN 0.
        4. The default VLAN on a switch cannot be renamed.

        Answer:

        B, D. The default Virtual Local Area Network (VLAN) on most switches has the ID VLAN 1, not VLAN 0, and it cannot be renamed or deleted. The default VLAN does not have to be created by the administrator; it is the one to which all ports are assigned in the default configuration.
140.    Control plane policing (CPP or CoPP) is a feature on some routers and switches that limits the rate of traffic on the device's processor, to prevent Denial-of-Service (DoS) and reconnaissance attacks, using which of the following technologies?

        1. IPSec
        2. 802.1X
        3. RA Guard
        4. QoS
        5. VLAN hopping

        Answer:

        D. Control plane policing uses Quality of Service (QoS) policies to block, allow, or impose rate limits on the traffic processed by the router or switch. Internet Protocol Security (IPSec) is a network layer security mechanism that encrypts or authenticates traffic. 802.1X is a network authentication mechanism. Router Advertisement (RA) Guard is a feature found on certain switches that prevents the misuse of RA messages to redirect traffic. Virtual Local Area Network (VLAN) hopping is a method for sending commands to switches to transfer a port from one VLAN to another.
141.    Which of the following technologies enables Virtual Private Network (VPN) clients to connect directly to each other, as well as to the VPN server at the home site?

        1. VPN concentrator
        2. DMVPN
        3. SIP trunk
        4. MPLS
        5. Clientless VPN

        Answer:

        B. VPN typically enables remote clients to connect to a VPN router at a central site, much like the star topology of a Local Area Network (LAN), in which computers are all connected to a central switch. Dynamic Multipoint Virtual Private Network (DMVPN) is a technology that creates a mesh topology between the remote VPN sites, enabling the remote sites to connect directly to each other, rather than to the central VPN server. A VPN concentrator is a type of router that enables multiple client systems to access a network from remote locations. A Session Initiation Protocol (SIP) trunk provides a connection between the private and public domains of a unified communications network. Multiprotocol Label Switching (MPLS) is a data transfer mechanism that assigns labels to individual packets, and then routes the packets based on those labels. Clientless VPN creates an encrypted tunnel to a server using a browser, without the need to install additional client software.
142.    Which of the following Virtual Private Network (VPN) protocols is generally considered to be obsolete?

        1. IPSec
        2. L2TP
        3. PPTP
        4. SSL/TLS

        Answer:

        C. Point-to-Point Tunneling Protocol (PPTP) is considered to be obsolete for VPN use because of several serious security vulnerabilities that have been found in it. IPSec, Layer 2 Tunneling Protocol (L2TP), and Secure Sockets Layer/Transport Layer Security (SSL/TLS) are all still in use.
143.    Which of the following Virtual Private Network (VPN) protocols does not provide encryption within the tunnel?

        1. PPTP
        2. IPSec
        3. L2TP
        4. SSL

        Answer:

        C. Layer 2 Tunneling Protocol (L2TP) is used to create the tunnel forming a VPN connection, but it does not encrypt the traffic passing through the tunnel. To do this, it requires a separate protocol that provides encryption, such as Internet Protocol Security (IPSec). Point-to-Point Tunneling Protocol (PPTP) and Secure Sockets Layer (SSL) are both capable of encrypting tunneled traffic.
144.    Which of the following elements must be identical in both the client and server computers to establish a remote Wide Area Network (WAN) connection? (Choose all that apply.)

        1. The WAN type
        2. The data link layer protocol
        3. The authentication method
        4. The operating system

        Answer:

        A, B, C. Although the computers do not have to use hardware made by the same manufacturer, both must use the same basic type of WAN connection, such as a leased line, a modem and PSTN line, or an Internet connection. Both of the computers must also use the same data link layer protocol, such as PPP, to establish a remote network connection. Most remote network connections use some form of authentication mechanism, even if it is nothing more than the exchange of a username and cleartext password. To establish the remote network connection, both computers must be configured to use the same type of authentication, even if it is no authentication at all. As long as all of the other elements are in place, such as the physical layer connection and the protocols, there is no need for both of the computers involved in a remote network connection to be running the same operating system.
145.    Which of the following is not a protocol that is typically used to secure communication between web servers and web browsers?

        1. SSL
        2. TLS
        3. SSH
        4. DTLS

        Answer:

        C. Secure Shell (SSH) is a character-based tool that enables users to execute commands on remote computers. It does not provide web server/browser security. Secure Sockets Layer (SSL) is a security protocol that provides encrypted communications between web browsers and servers. Transport Layer Security (TLS) is an updated security protocol that is designed to replace SSL. Datagram Transport Layer Security (DTLS) is a security protocol that provides the same basic functions as TLS, but for User Datagram Protocol (UDP) traffic.
146.    Which of the following types of Virtual Private Network (VPN) connection is the best solution for allowing clients limited access to your corporate network?

        1. Host-to-site
        2. Site-to-site
        3. Host-to-host
        4. Extranet

        Answer:

        D. An extranet VPN is designed to provide clients, vendors, and other outside partners with the ability to connect to your corporate network with limited access. A host-to-site VPN is a remote access solution, enabling users to access the corporate network from home or while traveling. A site-to-site VPN enables a branch office to connect to the home office using the Internet rather a more expensive Wide Area Network (WAN) connection. A host-to-host VPN enables two individual users to establish a protected connection to each other.
147.    Which of the following protocols is not used for remote control of computers?

        1. RDP
        2. TFTP
        3. SSH
        4. Telnet

        Answer:

        B. Trivial File Transfer Protocol (TFTP) is typically used to download boot image files to computers performing a Preboot Execution Environment (PXE) startup. It is not used for remote control. Remote Desktop Protocol (RDP) is used by Remote Desktop Services in Windows to provide clients with graphical control over servers at remote locations. Secure Shell (SSH) and Telnet are both character-based tools that enable users to execute commands on remote computers.
148.    Which of the following services is provided by the Remote Desktop Protocol (RDP)?

        1. Thin client computing
        2. Clientless virtual private networking
        3. Encrypted tunneling
        4. Unauthenticated file transfers

        Answer:

        A. RDP is a component of Remote Desktop Services, a Windows mechanism that enables a client program to connect to a server and control it remotely. RDP does not carry actual application data; it just transfers keystrokes, mouse movements, and graphic display information. Because the client program does not participate in the application computing on the server, it is known as a thin client. RDP does not provide clientless virtual private networking, encrypted tunneling, or unauthenticated file transfers.
149.    Which of the following types of Virtual Private Network (VPN) connection is the best solution for connecting a branch office to a corporate headquarters?

        1. Host-to-site
        2. Site-to-site
        3. Host-to-host
        4. Extranet

        Answer:

        B. A site-to-site VPN enables one network to connect to another, enabling users on both networks to access resources on the other one. This is usually a more economical solution for branch office connections than a Wide Area Network (WAN) link. A host-to-site VPN is a remote access solution, enabling users to access the corporate network from home or while traveling. A host-to-host VPN enables two individual users to establish a protected connection to each other. An extranet VPN is designed to provide clients, vendors, and other outside partners with the ability to connect to a corporate network with limited access.
150.    Ralph is a network administrator for a firm that is allowing employees to telecommute for the first time, and he is responsible for designing a remote access solution that will enable users to access network resources, such as company email and databases, securely. All of the remote users have been issued smartcards and will be connecting using Virtual Private Network (VPN) connections on company-supplied laptop computers running Windows 10 and equipped with card readers. The users will be logging on to the company network using their standard Active Directory Domain Services accounts, so it is important for Ralph to design a solution that provides the maximum protection for their passwords, both inside and outside the office. Which of the following authentication protocols should Ralph configure the remote access servers and the laptop computers to use?

        1. Password Authentication Protocol (PAP)
        2. Challenge Handshake Authentication Protocol (CHAP)
        3. Extensible Authentication Protocol (EAP)
        4. Microsoft Challenge Handshake Authentication Protocol (MSCHAPv2)

        Answer:

        C. EAP is the only authentication protocol included with Windows 10 that supports hardware-based authentication, so this is the only viable option. PAP transmits passwords in cleartext and is therefore not a viable option, as is CHAP, because it must store passwords using reversible encryption. MSCHAPv2 provides sufficient password protection but does not support the hardware-based authentication needed for smartcard use.
151.    Which of the following remote access protocols provides users with full graphical control over a Windows computer? (Choose all that apply.)

        1. SSH
        2. RDP
        3. VNC
        4. Telnet

        Answer:

        B, C. Remote Desktop Protocol (RDP) is a component of Remote Desktop Services, a Windows mechanism that enables a client program to connect to a server and control it remotely. RDP does not carry actual application data; it just transfers keystrokes, mouse movements, and graphic display information. Virtual Network Computing (VNC) is a similar desktop sharing system that is platform independent and open source. Secure Shell (SSH) and Telnet are character-based remote control solutions.
152.    Ralph has come upon the term _virtual desktop_, and he is not exactly sure what it means. After performing some Internet searches, he finds multiple definitions. Which of the following is not one of the technologies that uses the term _virtual desktop_?

        1. A three-dimensional realization of a computer display created using a virtual reality hardware device
        2. A computer display with a virtual operating system desktop that is larger than can be displayed on a monitor
        3. A cloud-based Windows 10 deployment that enables users to access their desktops using any remote device
        4. A hardware device that projects a computer desktop on a screen, rather than displaying it on a monitor

        Answer:

        D. The term _virtual desktop_ does not refer to a projection device that can display a computer desktop on a screen. A virtual desktop can be a realization of a computer monitor in a virtual reality environment; a virtualized desktop larger than the monitor, which users can scroll to view all parts of the display; or a cloud-based service provided by Microsoft Azure that provides users with access to their desktops using remote devices.
153.    Which of the following types of traffic are carried by the Remote Desktop Protocol (RDP)? (Choose all that apply.)

        1. Keystrokes
        2. Mouse movements
        3. Display information
        4. Application data

        Answer:

        A, B, C. RDP is a component of Remote Desktop Services, a Windows mechanism that enables a client program to connect to a server and control it remotely. RDP does not carry actual application data; it just transfers keystrokes, mouse movements, and graphic display information.
154.    Which of the following types of traffic are transmitted by Virtual Network Computing (VNC)? (Choose all that apply.)

        1. Keystrokes
        2. Mouse movements
        3. Display information
        4. Application data

        Answer:

        A, B, C. VNC is a graphical desktop sharing system that uses a protocol called Remote Frame Buffer (RFB) to connect a client to a server and control it remotely. VNC does not transmit actual application data; it just transfers keystrokes, mouse movements, and graphic display information.
155.    Which of the following types of traffic are carried by Telnet? (Choose all that apply.)

        1. Keystrokes
        2. Mouse movements
        3. Display information
        4. Application data

        Answer:

        A, C. Telnet is a character-based remote-control protocol and application that is available on virtually all computing platforms. Because it is strictly character based, Telnet clients transmit only keystrokes and receive only character-based display information from the server.
156.    Which of the following describes the primary function of a Remote Desktop Gateway?

        1. Provides multiple users with Remote Desktop client access to one workstation
        2. Provides a single Remote Desktop client with simultaneous access to multiple workstations
        3. Enables remote users outside the network to access network workstations
        4. Enables remote users to access workstations without the need for a Remote Desktop client.

        Answer:

        C. Remote Desktop Gateway is a Windows Server role that enables remote users outside the network to establish a Remote Desktop Protocol (RDP) connection without the need for a Virtual Private Network (VPN) connection. The gateway does not provide multiple Remote Desktop client access to one workstation, Remote Desktop client access to multiple workstations, or access to workstations without a Remote Desktop client.
157.    Which of the following statements about in-band management and out-of-band management are true? (Choose all that apply.)

        1. Out-of-band management tools do not provide access to the remote system's BIOS or UEFI firmware.
        2. Out-of-band management tools enable you to reinstall the operating system on a remote computer.
        3. Telnet, Secure Shell (SSH), and Virtual Network Computing (VNC) are in-band management tools.
        4. To perform out-of-band management on a device, it must have an IP address.

        Answer:

        B, C. Out-of-band management uses a dedicated channel to devices on the network. This means that the device to be managed does not require an IP address. The channel provides access to the BIOS or UEFI firmware and makes it possible to reinstall the operating system on a remote computer. Telnet, SSH, and VNC are not out-of-band management tools.
158.    Which of the following statements best defines out-of-band management?

        1. Out-of-band management is a method for accessing network devices from a remote location.
        2. Out-of-band management is a method for accessing network devices using a direct cable connection.
        3. Out-of-band management is a method for accessing network devices using a connection to the system other than the production network to which the device is connected.
        4. Out-of-band management is a method for accessing network devices using any tool that operates over the production network to which the device is connected.

        Answer:

        C. Out-of-band management refers to the use of an alternative communications channel to a network device. The channel can be a modem connection, a direct cable connection, a wireless or cellular connection, or a dedicated Ethernet connection.
159.    What four components are required for a computer to establish a remote Transmission Control Protocol/Internet Protocol (TCP/IP) connection?

        1. Common protocols
        2. Remote Access Service (RAS)
        3. A physical layer connection
        4. TCP/IP configuration
        5. Point-to-Point Tunneling Protocol (PPTP)
        6. Host and remote software

        Answer:

        A, C, D, F. A computer requires four components to establish a remote connection. First, a physical-layer Wide Area Network (WAN) connection is needed. Second, the two systems must share common protocols from the data link layer and above. Third, if TCP/IP is being used to establish a remote session, then TCP/IP parameters must be configured on the systems. Fourth, host and remote software are needed. The remote client must have software that enables it to establish a remote session, and the server must have software that enables it to receive and grant remote sessions. Microsoft RAS supports both client and server remote access software; however, this is not a required component since other types of software can be used. PPTP is a tunneling protocol and is not a required component for establishing a remote session.
160.    Which of the following statements explains why web browsing over a client-to-site Virtual Private Network (VPN) connection is usually so much slower than browsing locally?

        1. The browser application is running on the VPN server.
        2. The browser is using the remote network's Internet connection.
        3. The VPN tunnel restricts the amount of bandwidth available.
        4. VPN encryption is processor intensive.

        Answer:

        B. When users connect to a remote network using VPN, they become a participant on that network, which includes using the remote network's Internet connection. Therefore, when a user opens a browser, the application passes the user's requests through the VPN tunnel to the remote server, which uses the default gateway and Internet connection at the remote site to connect to the desired address. This is inherently slower than connecting the browser directly to the Internet from the client computer.
161.    In a site-to-site Virtual Private Network (VPN) connection, which of the following combinations of endpoint devices would most likely be involved?

        1. Two workstations
        2. A workstation and a server
        3. A workstation and a VPN concentrator
        4. Two VPN concentrators

        Answer:

        D. A site-to-site VPN connection connects two remote Local Area Networks (LANs) together, enabling users on either network to access the other one. The typical configuration would consist of two VPN concentrators, one at each site, functioning as the endpoints of the connection.
162.    In a client-to-site Virtual Private Network (VPN) connection, which of the following combinations of endpoint devices would most likely be involved?

        1. Two workstations
        2. A workstation and a server
        3. A workstation and a VPN concentrator
        4. Two VPN concentrators

        Answer:

        C. A client-to-site VPN connection connects a single workstation to a remote Local Area Network (LAN), enabling the workstation user to access the remote network's resources. The typical configuration would consist of a standalone workstation and a VPN concentrator at the network site functioning as the endpoints of the connection.
163.    Which of the following are the two most common types of Transport Layer Security/Secure Sockets Layer (TLS/SSL) Virtual Private Network (VPN) connections? (Choose all that apply.)

        1. TLS/SSL client
        2. TLS/SSL portal
        3. TLS/SSL tunnel
        4. TLS/SSL gateway

        Answer:

        B, C. The two most common types of TLS/SSL VPN connection are TLS/SSL portals, which provide users with access to selected remote network resources through a standard website, and TLS/SSL tunnels, which require the client web browser to run an active control, typically using Java or Flash. TLS/SSL client and TLS/SSL gateway are not common TLS/SSL VPN connections.
164.    In a host-to-host Virtual Private Network (VPN) connection, which of the following combinations of endpoint devices would most likely be involved?

        1. Two workstations
        2. A workstation and a server
        3. A workstation and a VPN concentrator
        4. Two VPN concentrators

        Answer:

        A. A host-to-host VPN connection connects two individual workstations at different locations, enabling the users on each workstation to access the other one through a secure tunnel. The typical configuration would consist of two workstations, one at each site, functioning as the endpoints of the connection.
165.    Many managed switches and routers include a console port for administrative access, to which you can connect a laptop and run a terminal program to access the device's interface. Which of the following is the best term for this type of access to the device?

        1. Out-of-band
        2. In-band
        3. Client-to-site
        4. BYOD

        Answer:

        A. The term _out-of-band_ is used to describe any type of management access to a device that does not go through the production network. Plugging a laptop into the console port avoids the network, so it is considered to be an example of out-of-band management. In-band management describes an access method that goes through the production network. Client-to-site is a type of Virtual Private Network (VPN) connection, and Bring Your Own Device (BYOD) is a policy defining whether and how users are permitted to connect their personal devices to the network.
166.    Which of the following statements about running a site-to-site Virtual Private Network (VPN) connection to join two distant Local Area Networks (LANs) together, rather than using a Wide Area Network (WAN) connection, are generally true? (Choose all that apply.)

        1. The VPN is cheaper.
        2. The VPN is slower.
        3. The VPN is less secure.
        4. The VPN is harder to maintain.

        Answer:

        A, B. Because the two endpoints of a VPN are connecting to local Internet Service Providers (ISPs), the ongoing connection costs are typically much less than a long-distance WAN connection. However, in most cases, a VPN is slower because it is affected by Internet bandwidth use and other factors. VPN connections are not inherently less secure than WANs, and they are not necessarily more difficult to maintain.
167.    Which of the following are examples of out-of-band device management? (Choose all that apply.)

        1. Logging on remotely from a network workstation
        2. Plugging a laptop into a console port
        3. Establishing a point-to-point modem connection
        4. Connecting dedicated ports on each device to a separate switch

        Answer:

        B, C, D. Any method of connecting to a router, switch, or other managed device that does not use the production network is considered to be out-of-band management. This includes connecting a computer or terminal directly to the device, using a point-to-point modem connection, or consolidating dedicated ports on all of the devices by connecting them to an isolated switch. Logging on remotely using a workstation on the production network would be considered in-band management.
168.    Which of the following is not an advantage of the Virtual Network Computing (VNC) terminal emulation product over its competitors?

        1. VNC is free.
        2. VNC runs on many operating systems.
        3. VNC runs faster than the competition.
        4. VNC can run through a web browser.

        Answer:

        C. VNC supports many operating systems, can run through a web browser, and is free. However, it is not any faster than the competing products.
169.    Which of the following was the first Transmission Control Protocol/Internet Protocol (TCP/IP) terminal emulation program?

        1. Telnet
        2. SSH
        3. Windows Terminal Services
        4. Virtual Network Computing

        Answer:

        A. Telnet (TELetype NETwork) was the first TCP/IP terminal emulation program, but it is rarely used today because of its limitations. It is character-based only, and it transmits all data as cleartext, which is insecure. Secure Shell (SSH) addresses the security problem, but it too is character-based. Windows Terminal Services and Virtual Network Computing (VNC) were both created to provide graphical terminal emulation.
170.    Which of the following techniques do Virtual Private Networks (VPNs) use to secure the data that they transmit over the Internet? (Choose all that apply.)

        1. Tunneling
        2. Socketing
        3. Message integrity
        4. Authentication

        Answer:

        A, C, D. Tunneling is the process of encapsulating a data packet within another packet. The system then encrypts the entire data packet. Message integrity enables the recipient to detect any data tampering. Authentication ensures that only the intended recipient can access the data. There is no applicable technique called socketing.
171.    Virtual Private Networks (VPNs) use tunneling, which is the process of encapsulating a data packet within another packet for transmission over a network connection, typically using the Internet. The system encrypts the entire encapsulated data packet for protection. Split tunneling is a variation of this method that provides which of the following advantages? (Choose all that apply.)

        1. Conservation of VPN bandwidth
        2. Access to local network devices while connected to the VPN
        3. Additional data integrity protection
        4. Faster data transmission through multiplexing

        Answer:

        B, C. A basic VPN typically uses full tunneling, in which all of the system's network traffic is encapsulated and encrypted for transmission. Split tunneling is a variation of this method in which only part of the system's traffic uses the VPN connection; the rest is transmitted over the network in the normal manner. Administrators can select which applications and devices use the VPN. Split tunneling can conserve Internet bandwidth used by the VPN and provide access to local services without the need for encapsulation. Split tunneling does not provide additional data integrity protection or improved performance through multiplexing.
172.    SSH was created to be an improvement on the Telnet terminal emulation program. In which of the following ways is it an improvement?

        1. SSH is faster than Telnet.
        2. SSH provides graphical terminal emulation.
        3. SSH encrypts passwords and data.
        4. SSH is less expensive than Telnet.

        Answer:

        C. Telnet transmits keystrokes in cleartext, including usernames and passwords. It is therefore insecure. Secure Shell (SSH) improves on the performance of Telnet by encrypting the passwords and other data it transmits over the network. Like Telnet, SSH is free and does not support graphical terminal emulation. SSH is also no faster than Telnet.
173.    Remote Desktop Protocol (RDP) was created for use with which of the following terminal emulation programs?

        1. Windows Terminal Services
        2. Virtual Network Computing (VNC)
        3. Citrix WinFrame
        4. Telnet

        Answer:

        A. RDP is the client/server protocol created for use with Windows Terminal Services, now known as Remote Desktop Services. It is not used with VNC, Citrix products, or Telnet.
174.    Your company has two users who want to telecommute from home. They do not have any hardware or software configured or installed. They need to transfer files to the corporate network over a secure link. Your company has a Virtual Private Network (VPN) concentrator that uses Layer 2 Tunneling Protocol (L2TP) and Internet Protocol Security (IPSec). The users want to implement the fastest available service. Both of the users’ homes are within 10,000 feet of a central office. Which of the following solutions address this scenario? (Choose all that apply.)

        1. Each user should install a modem and VPN client software, and configure it to dial through a local Internet Service Provider (ISP) to connect to the company server using L2TP and IPSec.
        2. Each user should establish a Digital Subscriber Line (DSL) connection by either ordering a new line or using the existing line. Each user then needs to install VPN client software and configure it to connect to the company server using L2TP and IPsec.
        3. Each user should establish a cable television (CATV) connection with a local broadband ISP. Each user then needs to install VPN client software and configure it to connect to the company server using L2TP and IPSec.
        4. Each user should install an Integrated Services Digital Network (ISDN) line in his or her house. Each user then needs to install VPN client software and configure it to dial through a local ISP to connect to the company server using L2TP and IPsec.

        Answer:

        B, C. In this scenario, each user wants the fastest service available to connect to the corporate network over a VPN connection. Of all the services listed here, the only ones that will meet this requirement are DSL and CATV Internet. CATV and DSL Internet connections support high data rates and can be used to connect using a VPN tunnel, so they meet the speed requirement. Each user can use his or her existing CATV connection or use an existing telephone line to install DSL. Once the line is installed, each user needs to install and configure a VPN client on his or her computer and configure it to use L2TP and IPSec. Modem connections are slow—the maximum upstream speed is 33.6 Kbps, and the downstream is 56 Kbps. ISDN's maximum transfer rate for Basic Rate Interface (BRI) is 128 Kbps.
175.    Which of the following is a PPP authentication protocol that enables users to authenticate using smartcards, badge readers, and fingerprint scanners, as well as usernames and passwords?

        1. PPTP
        2. PAP
        3. CHAP
        4. EAP

        Answer:

        D. Extensible Authentication Protocol (EAP) is a shell protocol used with Point-to-Point Protocol (PPP), which enables systems to support various types of authentication mechanisms. The primary advantage of EAP is that it enables a computer to use mechanisms other than passwords for authentication, including public key certificates, smartcards, badge readers, and biometric devices, such as fingerprint scanners. Password Authentication Protocol (PAP) and Challenge Handshake Authentication Protocol (CHAP) support only password authentication. Point-to-Point Tunneling Protocol (PPTP) is a Virtual Private Network (VPN) protocol, not an authentication protocol.
176.    A laptop that is equipped with a fingerprint scanner that authenticates the user is using which of the following types of technology?

        1. Pattern recognition
        2. Hand geometry
        3. Biometrics
        4. Tamper detection

        Answer:

        C. The technology that uses human physical characteristics to authenticate users is called biometrics. Biometric devices can identify users based on fingerprints, retinal pattern, voice prints, and other characteristics.
177.    An IT department receives a shipment of 20 new computers, and Alice has been assigned the task of preparing them for deployment to end users. The first thing she does is affix a metal tag with a bar code on it to each computer. Which of the following terms best describes the function of this procedure?

        1. Asset tracking
        2. Tamper detection
        3. Device hardening
        4. Port security

        Answer:

        A. Bar coding the new computers enables the IT department to record their locations, status, and conditions throughout their life cycle, a process known as asset tracking. Bar codes are not used for tamper detection and device hardening. Port security refers to switches, not computers.
178.    Which of the following types of physical security is most likely to detect an insider threat?

        1. Smartcards
        2. Motion detection
        3. Video surveillance
        4. Biometrics

        Answer:

        C. An insider threat by definition originates with an authorized user. Smartcards, motion detection, and biometrics will only detect the presence of someone who is authorized to enter sensitive areas. Video surveillance, however, can track the activities of anyone, authorized or not.
179.    Which of the following physical security mechanisms can either “fail close” or “fail open”?

        1. Motion detectors
        2. Video cameras
        3. Honeypots
        4. Door locks

        Answer:

        D. The terms _fail close_ and _fail open_ refer to the default position of an electric or electronic door lock when there is a power failure. Security is often a trade-off with safety, and in the event that an emergency occurs, cutting off power, whether secured doors are permanently locked or left permanently open, is a critical factor. These terms do not apply to motion detectors or video cameras. A honeypot is a computer configured to lure potential attackers; it is not a physical security mechanism.
180.    Smart lockers are storage devices that can provide users with access to supplies, deliveries, and other items using various security mechanisms. Which of the following are technologies that smart lockers can use to authenticate users and provide secure access to their contents?

        1. NFC
        2. RFID
        3. Bluetooth
        4. Biometrics
        5. PIN
        6. All of the above

        Answer:

        F. Smart lockers are available with a wide variety of authentication mechanisms, ranging from relatively unsecure PINs, Near Field Communication (NFC), and Bluetooth devices; to high-security biometric scans and radio-frequency identification (RFID) tags.
181.    Which of the following are common types of cameras used for video surveillance of secured network installations? (Choose all that apply.)

        1. IP
        2. LDAP
        3. CCTV
        4. NAC

        Answer:

        A, C. Closed-circuit television cameras are part of a self-contained system in which the cameras feed their signals to dedicated monitors, usually located in a security center. IP cameras are standalone devices that transmit signals to a wireless access point. While CCTV cameras can only be monitored by users in the security center, or another designated location, IP cameras can be monitored by any authorized user with a web browser. Lightweight Directory Access Protocol (LDAP) is a directory services protocol, and Network Access Control (NAC) is a service; neither one is a type of video surveillance device.
182.    Which of the following types of attack can best be prevented by implementing a program of employee education and training?

        1. Social engineering
        2. War driving
        3. Logic bomb
        4. Evil twin

        Answer:

        A. Social engineering is the practice of obtaining sensitive data by manipulating legitimate users, such as by pretending to be someone with a genuine need for that data. Because it is not a technological vulnerability, the only means of preventing this type of attack is to educate and train users to recognize potential threats. War driving is an attack method that consists of driving around a neighborhood with a computer, scanning for unprotected wireless networks. A logic bomb is a code insert placed into a legitimate software product that triggers a malicious event when specific conditions are met. An evil twin is a fraudulent access point on a wireless network that mimics the Service Set Identifier (SSID) of a legitimate access point, in the hope of luring in users.
183.    Which of the following statements describes what it means when the automated lock on the door to a datacenter is configured to fail open?

        1. The door remains in its current state in the event of an emergency.
        2. The door locks in the event of an emergency.
        3. The door unlocks in the event of an emergency.
        4. The door continues to function using battery power in the event of an emergency.

        Answer:

        C. A door that is configured to fail open reverts to its unsecured state—open—when an emergency occurs. This must be a carefully considered decision, as it can be a potential security hazard. However, configuring the door to fail closed is a potential safety hazard in the event of a fire or other disaster.
184.    A high security installation that requires entrants to submit to a retinal scan before the door unlocks is using which of the following types of technology?

        1. Pattern recognition
        2. Hand geometry
        3. Biometrics
        4. Tamper detection

        Answer:

        C. The technology that uses human physical characteristics to authenticate users is called biometrics. Biometric devices can identify users based on fingerprints, retinal pattern, voice prints, and other characteristics.
185.    Which of the following are means of preventing unauthorized individuals from entering a sensitive location, such as a datacenter? (Choose all that apply.)

        1. Biometric scans
        2. Identification badges
        3. Key fobs
        4. Motion detection

        Answer:

        A, B, C. Biometric scans, identification badges, and key fobs are all means of distinguishing authorized from unauthorized personnel. Motion detection cannot make this distinction.
186.    Which of the following security measures can monitor the specific activities of authorized individuals within sensitive areas?

        1. Video surveillance
        2. Identification badges
        3. Key fobs
        4. Motion detection
        5. Locking cabinets

        Answer:

        A. Video surveillance can monitor all activities of users in a sensitive area. With properly placed equipment, event-specific actions, such as commands entered in a computer, can be monitored. Identification badges, key fobs, motion detection, and locking cabinets can indicate the presence of individuals in a sensitive area, but they cannot monitor specific activities.
187.    Which of the following physical security devices can use passive RFIDs to enable an authorized user to enter a secured area? (Choose all that apply.)

        1. Key fob
        2. Keycard lock
        3. Proximity card
        4. Cypher lock
        5. Smart locker

        Answer:

        A, C, E. A radio-frequency identification (RFID) device is a small chip that can be electronically detected by a nearby reader. The chip can contain small amounts of data, such as the authentication credentials needed to grant an individual access to a secured area. Key fobs, proximity cards (prox cards), and smart lockers can use RFIDs to enable users to unlock a door by waving the device near a reader. Keycard locks typically require the card to be inserted into a reader and typically use magnetic strips to store data. Cypher locks rely on data supplied by the user—that is, the combination numbers.
188.    Some key fobs used for authenticated entrance to a secured area have a keypad that requires the user to enter a PIN before the device is activated. Which of the following authentication factors is this device using? (Choose all that apply.)

        1. Something you do
        2. Something you have
        3. Something you are
        4. Something you know

        Answer:

        B, D. Possession of the key fob is something you have, but the key fob could be lost or stolen, so its security is confirmed by entering a PIN, something you know. Unless the user both lost the key fob and shared the PIN, the device remains secure.
189.    Which of the following physical security devices can enable an authorized user to enter a secured area without any physical contact with the device? (Choose all that apply.)

        1. Key fob
        2. Keycard lock
        3. Proximity card
        4. Cypher lock

        Answer:

        A, C. Key fobs and proximity cards (prox cards) often use radio-frequency identification (RFID) devices to enable users to unlock a door by waving the device near a reader. Keycard locks typically use magnetic strips to store data and require the card to be physically inserted into a reader. Cypher locks rely on data manually supplied by the user—that is, the combination numbers.
190.    Video surveillance of sensitive areas, such as datacenters, can aid in the detection of which of the following types of attacks? (Choose all that apply.)

        1. Social engineering
        2. Evil twin
        3. Brute-force
        4. Insider threats

        Answer:

        B, D. Video surveillance can conceivably prevent an evil twin attack, which takes the form of a rogue access point deliberately connected to the network for malicious purposes. Video surveillance can also help to prevent insider threats by monitoring the activities of authorized users. Video surveillance cannot prevent social engineering, which involves nothing more than communicating with people, or brute-force attacks, which are usually performed remotely.
191.    Which of the following statements is true when a biometric authentication procedure results in a false positive?

        1. A user who should be authorized is denied access.
        2. A user who should not be authorized is denied access.
        3. A user who should be authorized is granted access.
        4. A user who should not be authorized is granted access.

        Answer:

        D. When a false positive occurs during a biometric authentication, a user who should not be granted access to the secured device or location is granted access. A false negative is when a user who should be granted access is denied access.
192.    In the datacenter of a company involved with sensitive government data, all servers have crimped metal tags holding the cases closed. All of the hardware racks are locked in clear-fronted cabinets. All cable runs are installed in transparent conduits. These are all examples of which of the following physical security measures?

        1. Tamper detection
        2. Asset tracking
        3. Geofencing
        4. Port security

        Answer:

        A. All of the mechanisms listed are designed to make any attempts to tamper with or physically compromise the hardware devices immediately evident. This is therefore a form of tamper detection. Asset tracking is for locating and identifying hardware. Geofencing is a wireless networking technique for limiting access to a network. Port security refers to network switch ports.
193.    A secured government building that scans the faces of incoming people and compares them to a database of authorized entrants is using which of the following types of technology?

        1. Pattern recognition
        2. Hand geometry
        3. Biometrics
        4. Tamper detection

        Answer:

        C. The technology that uses human physical characteristics to authenticate users is called biometrics. Biometric devices can identify users based on fingerprints, retinal pattern, voice prints, and other characteristics.
194.    Which of the following is not a means of preventing physical security breaches to a network datacenter?

        1. Badges
        2. Locks
        3. Key fobs
        4. Tailgaters

        Answer:

        D. A tailgater is a type of intruder who enters a secure area by closely following an authorized user. Most people are polite enough to hold the door open for the next person without knowing if they are authorized to enter. A tailgater is therefore not an intrusion prevention mechanism. Identification badges, locks, and key fobs are methods of preventing intrusions.
195.    Identification badges, key fobs, and access control vestibules all fall into which of the following categories of security devices?

        1. Physical security
        2. Data security
        3. Asset tracking
        4. Port security

        Answer:

        A. Identification badges, key fobs, and access control vestibules (mantraps) are all physical security mechanisms, in that they prevent unauthorized personnel from entering sensitive areas, such as datacenters. These mechanisms are not used for data file security, asset tracking, or switch port security.
196.    Which of the following are not means of detecting intruders in a network datacenter? (Choose all that apply.)

        1. Motion detection
        2. Video surveillance
        3. Biometrics
        4. Smartcards

        Answer:

        C, D. Biometrics and smartcards are both means of preventing intrusions, whereas motion detection and video surveillance are mechanisms for detecting them.
197.    Which of the following statements describes what it means when the automated lock on the door to a datacenter is configured to fail closed?

        1. The door remains in its current state in the event of an emergency.
        2. The door locks in the event of an emergency.
        3. The door unlocks in the event of an emergency.
        4. The door continues to function using battery power in the event of an emergency.

        Answer:

        B. A door that is configured to fail closed reverts to its secured state—locked—when an emergency occurs. This must be a carefully considered decision, since it can be a potential safety hazard in the event of a fire or other disaster. However, configuring the door to fail open is a potential security hazard.
198.    After an incident in which your company's datacenter was penetrated by an intruder, the management has installed a double doorway at the entrance to the datacenter. The two doors have a small vestibule in between them, and one door must be closed before the other one can open. Which of the following terms describes this arrangement?

        1. Server closet
        2. Mantrap
        3. Controlled entrance
        4. Honeypot

        Answer:

        B. An entrance arrangement in which people must close one door before they can open the next one is called an access control vestibule or mantrap. Security personnel can evaluate potential entrants while they are in the vestibule and detain attempted intruders there.
199.    Ralph's company has purchased new computers to replace some of the older workstations currently in use. Ralph has been assigned the task of preparing the old computers for disposal. They will be sold to a local secondhand dealer. For the dealer to accept the computers, they must have a functional operating system. Company policy also dictates that the computers be permanently wiped of all applications and data before disposal. Which of the following tasks will Ralph have to perform before the computers are sold? (Choose all that apply.)

        1. Reinstall the operating system
        2. Uninstall all applications
        3. Delete all data files
        4. Run a disk wipe utility
        5. Perform a factory reset

        Answer:

        A, D. Deleting files on a hard disk drive leaves them available for retrieval, even though they appear to be gone. A disk wipe utility deletes all of the files on the hard drive and then overwrites the entire disk with zeroes, rendering all files unretrievable. Ralph can then reinstall the operating system to prepare the computer for sale. Performing these two steps eliminates the need to uninstall applications, delete data files manually, or perform a factory reset.
200.    Which of the following is not one of the functions provided by TACACS+?

        1. Authentication
        2. Authorization
        3. Administration
        4. Accounting

        Answer:

        C. Terminal Access Controller Access Control System Plus (TACACS+) is a protocol that was designed to provide AAA services for networks with many routers and switches. AAA stands for Authentication, Authorization, and Accounting, but not administration.
