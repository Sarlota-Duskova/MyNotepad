# Exam 2

1.  Which of the following are technologies typically used for Personal Area Networks (PANs)? (Choose all that apply.)

    1. RFID
    2. Z-Wave
    3. ISDN
    4. NFC
    5. Bluetooth

    Answer:

    B, D, E. Bluetooth, Z-Wave, and near-field communication (NFC) are all short-range wireless technologies that are capable of providing communications between PAN devices. The other options are not suitable for PAN communications. Radio-frequency identification (RFID) uses tags containing data, frequently embedded in pets, which can be read using electromagnetic fields. Integrated Services Digital Network (ISDN) is a wide area networking technology that uses the telephone infrastructure to provide a high-speed dial-up service.
2.  Review the following figure. How many collision domains and broadcast domains are there in the network diagram?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c07uf001_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. There are three collision domains and one broadcast domain.
    2. There is one collision domain and one broadcast domain.
    3. There are three collision domains and three broadcast domains.
    4. There are seven collision domains and three broadcast domains.
    5. There are nine collision domains and three broadcast domains.

    Answer:

    E. Each port on a router defines a separate network segment. Because routers do not forward broadcast transmissions, each of the three segments forms a separate broadcast domain. Hubs forward all traffic to all of the connected nodes, so the network segment with the hub forms a single collision domain. Switches forward traffic only to the destination node, so each workstation connected to one of the switches forms a separate collision domain. The switch-to-router links count for two more collision domains. There are six switched workstations, plus the hub segment and the two switch-to-router links, for a total of nine collision domains.
3.  Which of the following types of network devices can provide authentication services for multiple remote access servers using the device's own account database?

    1. NAS
    2. IDS
    3. NGFW
    4. RADIUS

    Answer:

    D. A. Remote Authentication Dial-In User Service (RADIUS) server can provide authentication, authorization, and accounting services for remote access servers. Intrusion Detection Systems (IDSs), Next-Generation Firewalls (NGFWs), and Network Attached Storage (NAS) devices do not provide this type of authentication services.
4.  You are designing the network for your company's new branch office, and you need a device on which administrators can create Virtual Local Area Networks (VLANs) and that will forward traffic between them. Which of the following types of devices can do this?

    1. Virtual router
    2. Multilayer switch
    3. Broadband router
    4. Load balancer

    Answer:

    B. A multilayer switch is a network connectivity device that functions at both the data link layer (layer 2) and the network layer (layer 3) of the Open Systems Interconnection (OSI) reference model. At layer 2, the device functions like a normal switch, creating an individual collision domain for each connected node and enabling administrators to create multiple VLANs. At layer 3, the device also provides routing capabilities by forwarding packets between the VLANs. Virtual routers, load balancers, and broadband routers are strictly layer 3 devices that can route traffic but cannot create VLANs.
5.  You are setting up a new network for which you have been given the IPv4 network address 10.61.0.0/19. You want to calculate the number of hosts you can create on each subnet. How many bits are allocated to the host identifier in an IPv4 address on this network?

    1. 5
    2. 8
    3. 13
    4. 21

    Answer:

    C. The value after the slash in a Classless Inter-Domain Routing (CIDR) address specifies the number of bits in the network identifier. An IP address has 32 bits, so if 19 bits are allocated to the network identifier, 13 bits are left for the host identifier.
6.  The protocols that are responsible for the delivery of data packets to their final destinations on an internetwork operate at which layer of the Open Systems Interconnection (OSI) reference model?

    1. Application
    2. Session
    3. Transport
    4. Network
    5. Data link

    Answer:

    D. On a TCP/IP network, the Internet Protocol (IP) at the network layer is the protocol responsible for the delivery of data to its final destination, using IP addresses that can be routed through an internetwork. Data link layer protocols are only concerned with communication between devices on a Local Area Network (LAN) or between two points connected by a Wide Area Network (WAN). The transport, session, and application layers are not involved in the actual delivery of data over the network.
7.  Originally, Storage Area Networks (SANs) were dedicated solely to storage-based traffic. A Local Area Network (LAN) was also required for other types of traffic. Today, however, it is possible for SAN and LAN traffic to coexist on a single network medium. Which of the following SAN protocols are capable of sharing a network medium with standard LAN traffic? (Choose all that apply.)

    1. InfiniBand
    2. Fibre Channel
    3. iSCSI
    4. FCoE

    Answer:

    C, D. The iSCSI protocol runs on a standard IP network, and the Fibre Channel over Ethernet (FCoE) variant runs on a standard Ethernet network. Both of these protocols can share a network with LAN traffic, although the use of a Quality of Service (QoS) mechanism is usually recommended. The original Fibre Channel implementation and InfiniBand both require a dedicated network medium that does not support LAN traffic.
8.  Which of the following application layer protocols do not include a program that enables a user to log on to a remote network device and execute commands using a character-based interface? (Choose all that apply.)

    1. Telnet
    2. Simple Mail Transfer Protocol (SMTP)
    3. File Transfer Protocol (FTP)
    4. Domain Name System (DNS)

    Answer:

    B, D. SMTP and DNS are both application layer protocols, but neither one includes a character-based program. Both Telnet and FTP are protocols that include command-line client applications, with Telnet providing terminal emulation and FTP file transfer functionality.
9.  Many network diagrams use Cisco symbols to illustrate the locations of and relationships between network components. Cisco symbols are standardized pictographs that illustrate the basic function of a network component. In a network diagram that uses Cisco symbols, what component does the symbol in the figure represent?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c07uf002_0.jpg" alt="" height="322" width="368"><figcaption></figcaption></figure>

    1. A hub
    2. A switch
    3. A router
    4. A gateway

    Answer:

    B. The Cisco symbol shown in the figure is used in network diagrams to represent a switch, as symbolized by the multiple arrows pointing outward. This symbol is not used to represent a hub, a router, or a gateway.
10. You are planning an automated operating system deployment for 100 new Windows workstations your company has received. You intend to configure the workstations to boot using Preboot Execution Environment (PXE), during which time the system will obtain an IP address from a Dynamic Host Configuration Protocol (DHCP) server and then download a boot image file from a Trivial File Transfer Protocol (TFTP) server. Which of the following well-known ports must you open on the firewall separating the workstations from the servers? (Choose all that apply.)

    1. 64
    2. 65
    3. 66
    4. 67
    5. 68
    6. 69

    Answer:

    D, E, F. DHCP servers use well-known port numbers 67 and 68. TFTP uses port number 69. Neither protocol uses port 64, 65, or 66.
11. Your department is experiencing frequent delays as users wait for images to render using their outdated graphics software package. As a result, you submitted a change request for a new software product at the monthly meeting of the company's change management team. Now that the change request has been approved, it is time to implement the change. Which of the following administrative tasks will most likely be the change management team's responsibility during the implementation process? (Choose all that apply.)

    1. Notifying users
    2. Documenting all modifications made
    3. Authorizing downtime
    4. Designating a maintenance window

    Answer:

    C, D. The change management team is usually not responsible for tasks directly involved in the implementation of the changes they approve. Therefore, they would not be the ones to notify users exactly when the change will take place or document the procedure afterward. They would, however, be responsible for providing a maintenance window, during which the change must occur, and authorizing any downtime that would be needed.
12. You are installing a new server that is equipped with two power supplies. The server's firmware enables you to set the mode in which the power supplies will be used. In which of the following modes must the dual power supplies be running for the system to be fault tolerant?

    1. Individual mode
    2. Combined mode
    3. Redundant mode
    4. Hot backup mode

    Answer:

    C. A server with dual power supplies can run in one of two modes: redundant or combined. In redundant mode, each of the power supplies is capable of providing 100 percent of the power needed by the server. Therefore, the server can continue to run if one power supply fails, making it fault tolerant. In combined mode, both power supplies are needed to provide the server's needs, so a failure of one power supply will bring the server down. Individual mode and hot backup mode are not terms used for this purpose.
13. The Domain Name System (DNS) defines a hierarchical name space, locations in which are reflected in fully qualified domain names (FQDNs). Which of the words in the FQDN [`www.paris.mydomain.org`](http://www.paris.mydomain.org/) represents the bottommost layer in the DNS namespace's domain hierarchy?

    1. `www`
    2. `paris`
    3. `mydomain`
    4. `org`

    Answer:

    B. The word `paris` is the name of the bottommost domain in the given FQDN. `paris` is a subdomain within `mydomain`, and `mydomain` is a second-level domain registered by a particular organization. The topmost layer in the DNS hierarchy is represented by `org`, which is a top-level domain. In this FQDN, `www` is not the name of a domain; it is the name of a particular host in the [`paris.mydomain.org`](http://paris.mydomain.org/) domain.
14. The term _datagram_ is typically used by protocols offering connectionless delivery service. Which of the following protocols use(s) the term _datagram_ to describe the data transfer unit it creates? (Choose all that apply.)

    1. TCP
    2. IP
    3. UDP
    4. Ethernet

    Answer:

    B, C. The two main connectionless protocols in the TCP/IP suite are the Internet Protocol (IP) and the User Datagram Protocol (UDP), both of which use the term _datagram_ for their protocol data units. Ethernet uses the term _frame,_ and Transmission Control Protocol (TCP) uses the term _segment_.
15. After using a tape backup solution for years, you have recently started backing up your server to an external hard disk drive. Your backup schedule calls for weekly full backups and daily incremental backups. In the past, performing a restore required multiple jobs, but now only a single job is needed. Why does performing incremental backups to a hard drive, rather than a tape drive, make it possible to restore a server with a single job, rather than multiple jobs?

    1. Because hard drives use a different block size than tape drives
    2. Because hard drives can transfer data faster than tape drives
    3. Because hard drives hold more data than tape drives
    4. Because hard drives are random access devices and tape drives are not

    Answer:

    D. Data is stored on tape drives in a linear fashion. Once you write backup data to a tape, you cannot selectively replace individual files. When you perform a restore job, you have to restore the most recent full backup, followed by incremental backups, which overwrite some of the full backup files with newer ones. Hard disk drives are random access devices, meaning that individual files can be written to and read from any location on the disk. When you perform incremental backup jobs to a hard disk, the software can restore data using any version of each file that is available. Data capacity, transfer speed, and block size are not relevant to the number of jobs required.
16. You have just received notification of a new software release for an application you are running on your servers. The release is intended to address a newly discovered security vulnerability. Which of the following is the correct term for a software release containing a fix designed to address one specific issue?

    1. An upgrade
    2. A patch
    3. A service pack
    4. An update

    Answer:

    B. A patch is a relatively small update that is designed to address a specific issue, often a security exploit or vulnerability. Patches do not add features or new capabilities; they are fixes targeted at a specific area of the operating system. Updates, upgrades, and service packs are larger packages that might include new features and/or many different fixes.
17. Twisted-pair cables consist of multiple pairs of wires within a sheath, with each pair of wires twisted together separately. Which of the following statements best explains the reason for the twists in twisted-pair cabling? (Choose all that apply.)

    1. The twists help to prevent crosstalk in adjacent wire pairs.
    2. The twists make it easier for installers to attach connectors to the cable ends.
    3. The twists extend the cable's bend radius allowance, making it easier to install.
    4. The twists limit the effects of electromagnetic interference (EMI) on the signals carried over the cable.
    5. The twists help to prevent data collisions from occurring.

    Answer:

    A, D. The twisted wire pairs inside twisted-pair cable prevent the signals on the different wires from interfering with each other (which is called crosstalk). The twists also provide resistance to outside EMI. The twists have no effect on collisions. The twists do nothing to facilitate the attachment of connectors. Twists have nothing to do with the bend radius allowance for the cable.
18. The figure shown here lists the processes currently running on a Linux workstation. Which of the following performance monitoring tools, provided in Linux and Unix operating systems, enables you to display information about processes that are currently running on a system?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c07uf003_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. `netstat`
    2. `dig`
    3. `perfmon`
    4. `top`

    Answer:

    D. The `top` utility displays performance information about the currently running processes on a Unix/Linux system. The other options are tools that do not display running processes. `netstat` is a tool that enables you to view active network connections and TCP/IP traffic statistics. It does not measure system performance. The `dig` tool generates Domain Name System (DNS) queries. perfmon is a Windows performance monitoring tool; there no Unix/Linux tool by that name.
19. You are contracting with a provider to obtain email services for the clients on your network, using their existing email servers in the public cloud. You do not need anything from the provider other than email. Which of the following service models will you be using?

    1. PaaS
    2. SaaS
    3. IaaS
    4. All of the above

    Answer:

    B. The Software as a Service (SaaS) model provides consumers with access to a specific application, such as email, running on the provider's servers. Infrastructure as a Service (IaaS) provides the consumers with processing, storage, and networking resources that they can use to install and run operating systems and other software of their choice. Platform as a Service (PaaS) provides consumers with the ability to install applications of their choice on a server installed by the provider.
20. Security Information and Event Management (SIEM) is a combination tool that uses information gathered from logs and network devices to provide a real-time analysis of the network's security condition. Which of the following SIEM processes performs searches for specific criteria, during specific time frames, in logs located on different computers?

    1. Correlation
    2. Retention
    3. Data aggregation
    4. Forensic analysis

    Answer:

    D. In SIEM, forensic analysis is a process of searching logs on multiple computers for specific information based on set criteria and time periods. The other three options specify other SIEM functions. Data aggregation is a process of consolidating log information from multiple sources. Correlation is the process of linking logged events with common attributes together. Retention is the long-term storage of log data.
21. When you start Dynamic Host Configuration Protocol (DHCP) client, it transmits DHCPDISCOVER messages to locate and initiate contact with DHCP servers. Which of the following types of transmissions does the client use for this purpose?

    1. Broadcast
    2. Multicast
    3. Anycast
    4. Unicast

    Answer:

    A. DHCP clients use broadcasts to transmit DHCPDISCOVER messages on the local network. DHCP servers are then required to respond to the broadcasts. DHCP clients cannot use unicast, multicast, or anycast messages to initiate contact with DHCP servers, because the clients have no way of learning the addresses of the DHCP servers.
22. Virtual Private Networks (VPNs) use a technique called tunneling to secure traffic as it passes over a public network, such as the Internet. In some cases, the traffic within the VPN tunnel is also encrypted. Which of the following VPN protocols does not provide encryption within the tunnel?

    1. L2TP
    2. IPsec
    3. PPTP
    4. SSL

    Answer:

    A. Layer 2 Tunneling Protocol (L2TP) is a VPN protocol that creates the tunnel forming a VPN connection, but it does not encrypt the traffic passing through the tunnel. To do this, it requires a separate protocol that provides encryption, such as IPsec. Point-to-Point Tunneling Protocol (PPTP) and Secure Sockets Layer (SSL) are both capable of encrypting traffic in the tunnels they create.
23. You are installing a wireless network in a site that has a great many 2.4 GHz wireless telephones. Which of the following wireless networking technologies can you use, which will never experience interference from the telephones? (Choose all that apply.)

    1. IEEE 802.11b
    2. IEEE 802.11g
    3. IEEE 802.11ac
    4. IEEE 802.11a
    5. IEEE 802.11n

    Answer:

    C, D. IEEE 802.11b, 802.11g, and 802.11n networks all can use the 2.4 GHz frequency band for their transmissions, which can experience interference from a wireless telephone using the same frequency. IEEE 802.11a and IEEE 802.11ac, however, use the 5 GHz band, which will not experience interference from a 2.4 GHz phone.
24. Which of the following is another term for a switch?

    1. Multicast hub
    2. Multiport repeater
    3. Multiport bridge
    4. Multihomed router

    Answer:

    C. A switch is a data link layer device that essentially performs the function of a bridge for each device connected to one of its ports. It can therefore be described as a _multiport bridge_. _Multiport repeater_ is another term for a hub, and _multihomed router_ is a redundancy, as all routers are by definition multihomed—that is, connected to multiple networks. There is no such device as a multicast hub.
25. You are working at a client site with a managed router that includes a console port for administrative access, which you can use to connect a laptop and run a terminal program to access the device's interface. Which of the following is the best term for this type of access to the device?

    1. Client-to-site
    2. In-band
    3. BYOD
    4. Out-of-band

    Answer:

    D. The term _out-of-band_ describes any type of management access to a device that does not go through the production network. Plugging a laptop into the console port avoids the network, so it is considered to be an example of out-of-band management. In-band management describes an access method that does go through the production network. Client-to-site is a type of Virtual Private Network (VPN) connection, and Bring Your Own Device (BYOD) is a policy defining whether and how users are permitted to connect their personal devices to the network.
26. After some incidents of security breaches, you have been asked to draft a revised password policy for the company's users. Which of the following are typical elements of a corporate password policy? (Choose all that apply.)

    1. Frequent password changes
    2. Use of special characters
    3. Minimum password length
    4. Unique passwords

    Answer:

    A, B, C, D. The longer the password, the more difficult it is to guess. Corporate policies typically require passwords of a minimum length. A larger character set also makes a password more difficult to guess, so requiring uppercase, lowercase, numeric, and special characters is common. Changing passwords forces the cracking process to start over, so policies typically require frequent password changes and require users to create unique passwords at each change.
27. You have a laptop that requires you to hold your finger on a scanner pad before you can use it. A device equipped with a fingerprint scanner that authenticates the user is using which of the following types of technology?

    1. Tamper detection
    2. Biometrics
    3. Hand geometry
    4. Pattern recognition

    Answer:

    B. The technology that uses human physical characteristics to authenticate users is called biometrics. Biometric devices can identify users based on fingerprints, retinal patterns, voice prints, and other characteristics.
28. You have been asked to locate the computers on a network which the previous consultant has configured with incorrect IPv6 addresses. Which of the following are not correctly formatted IPv6 addresses? (Choose all that apply.)

    1. fe00::c955:c944:acdd:3fcb
    2. fe00::b491:cf79:p493:23ff
    3. 2001:0:44ef68:23eb:99fe:72bec6:ea5f
    4. 2001:0:49e6:39ff:8cf5:6812:ef56

    Answer:

    B, C, D. Option B contains a _p_, which is a nonhexadecimal digit. Option C contains blocks larger than 16 bits. Option D contains only seven 16-bit blocks (and no double-colon) instead of the eight required for a 128-bit IPv6 address. The address fe00::c955:c944:acdd:3fcb in option A is correctly formatted for IPv6, with the double-colon replacing three blocks of zeroes. Uncompressed, the address would appear as follows: fe00:0000:0000:0000:c955:c944:acdd:3fcb.
29. During a security evaluation by an outside contractor, you are asked whether your company uses a _fail open_ or _fail closed_ policy for the datacenter. You do not know what the contractor means. Which of the following physical security mechanisms can either _fail closed_ or _fail open_?

    1. Door locks
    2. Motion detectors
    3. Honeypots
    4. Video cameras

    Answer:

    A. The terms _fail close_ and _fail open_ refer to the default position of an electric or electronic door lock when there is a power failure. Security is often a trade-off with safety, and in the event that an emergency occurs that results in a power outage, whether secured doors are permanently locked or left permanently open is a critical factor. The terms _fail close_ and _fail open_ do not apply to motion detectors or video cameras. A honeypot is a computer, application, or website configured to lure potential attackers; it is not a physical security mechanism.
30. Your company is concerned about the possibility of insider threats. Which of the following security measures can you use to monitor the specific activities of authorized individuals within sensitive areas?

    1. Identification badges
    2. Motion detection
    3. Video surveillance
    4. Key fobs

    Answer:

    C. Video surveillance can monitor the activities of all users in a sensitive area, authorized or not. With properly placed equipment, even specific actions, such as commands typed into a computer, can be monitored. Identification badges, key fobs, and motion detection can indicate the presence of individuals in a sensitive area, but they cannot monitor specific activities.
31. Ralph is troubleshooting a Windows server, and while doing so, he runs the following command: `ping 127.0.0.1`. The command completes successfully. What has Ralph proven by doing this?

    1. That the computer's network adapter is functioning properly
    2. That the computer's IP address is correct for the network
    3. That the computer's TCP/IP networking stack is loaded and functioning
    4. Nothing

    Answer:

    C. The IP address 127.0.0.1 is a dedicated loopback address that directs outgoing IP traffic directly into the incoming IP traffic buffer. A successful `ping` test using that address indicates that the computer's TCP/IP stack is functioning properly, but the traffic never reaches the network adapter or the network, so the test does not confirm that the adapter is functioning or that the computer has a correct IP address for the network.
32. Which of the following are not examples of multifactor authentication? (Choose all that apply.)

    1. A system that requires a smart card and a PIN for authentication
    2. A system that uses an external RADIUS server for authentication
    3. A system that requires two passwords for authentication
    4. A system that requires a password and a retinal scan for authentication

    Answer:

    B, C. _Multifactor authentication_ combines two or more authentication methods and reduces the likelihood that an intruder would be able to successfully impersonate a user during the authentication process. A password and a retinal scan is an example of a multifactor authentication system. A smartcard and a PIN, which is the equivalent of a password, is an example of multifactor authentication because it requires users to supply something they know and something they have. Multifactor authentication refers to the proofs of identity a system requires, not the number of servers used to implement the system. Therefore, the use of a Remote Authentication Dial-In User Service (RADIUS) server is not an example of multifactor authentication. A system that requires two passwords is not an example of multifactor authentication, because an attacker can compromise one password as easily as two. A multifactor authentication system requires two different forms of authentication.
33. A user calls Ed at the help desk to report that he cannot access the Internet. He can access systems on the local network, however. Ed examines the routing table on the user's workstation and sees the following listing. Which statement explains why the user cannot access the Internet?

    `IPv4 Route Table ========================================================================== Active Routes: Network Destination Netmask Gateway Interface Metric 127.0.0.0 255.0.0.0 On-link 127.0.0.1 331 127.0.0.1 255.255.255.255 On-link 127.0.0.1 331 127.255.255.255 255.255.255.255 On-link 127.0.0.1 331 192.168.2.0 255.255.255.0 On-link 192.168.2.37 281 192.168.2.37 255.255.255.255 On-link 192.168.2.37 281 192.168.2.255 255.255.255.255 On-link 192.168.2.37 281 224.0.0.0 240.0.0.0 On-link 127.0.0.1 331 224.0.0.0 240.0.0.0 On-link 192.168.2.37 281 255.255.255.255 255.255.255.255 On-link 127.0.0.1 331 255.255.255.255 255.255.255.255 On-link 192.168.2.37 281 ========================================================================== Persistent Routes: None`

    1. The routing table does not specify a loopback address.
    2. The routing table does not specify a DNS server address.
    3. The routing table does not specify a default gateway address.
    4. The routing table contains two different routes to the 224.0.0.0 network.

    Answer:

    C. To access the Internet, the workstation's routing table must include a default gateway entry, which would have a Network Destination value of 0.0.0.0. A workstation's routing table does not have to specify the address of a Domain Name System (DNS) server. The loopback (127.0.0.1) and multicast (224.0.0.0) addresses are normal routing table entries that do not affect Internet access.
34. Which of the following statements about single-mode fiber-optic cable are true? (Choose all that apply.)

    1. Multimode cables use an LED light source, while single-mode cables use a laser.
    2. Multimode cables can span longer distances than single-mode cables.
    3. Multimode cables have a smaller core filament than single-mode cables.
    4. Multimode cables have a smaller bend radius than single-mode, making them easier to install.
    5. Multimode fiber-optic cables require a ground, whereas single-mode cables do not.

    Answer:

    A, D. Multimode cables use an LED light source and have a smaller bend radius than single-mode cables. Single-mode cables have a smaller core filament and can span longer distances than multimode cables. Fiber-optic cables are not conductors of electricity, so they do not require a ground.
35. A user swipes a smartcard through the reader connected to a laptop and then types a password to log on to the system. Which of the following actions is the user performing?

    1. Auditing
    2. Accounting
    3. Authorization
    4. Authentication

    Answer:

    D. Authentication is the process of confirming a user's identity. Smartcards and passwords are two of the authentication factors commonly used by network devices. Authorization defines the type of access granted to authenticated users. Accounting and auditing are both methods of tracking and recording a user's activities on a network, such as when a user logged on and how long they remained connected.
36. Which of the following cabling topologies have never been used by standard Ethernet networks? (Choose all that apply.)

    1. Bus
    2. Ring
    3. Star
    4. Mesh

    Answer:

    B, D. Ethernet has never used a ring or mesh topology. The first Ethernet networks used a physical layer implementation commonly known as Thick Ethernet or 10Base5. The network used coaxial cable in a bus topology. Later Ethernet standards use twisted-pair or fiber-optic cables in a star topology.
37. Pulling into your company parking lot at lunchtime, you notice a person without a company parking sticker on his car working at a laptop. You have seen this more than once, and you begin to suspect that unauthorized users are connecting to the company's Wireless Access Point (WAP) and gaining access to the network. Which of the following are steps you can take to prevent this from happening in the future? (Choose all that apply.)

    1. Use Kerberos for authentication
    2. Place the access point in a screened subnet
    3. Disable SSID broadcasting
    4. Implement MAC address filtering

    Answer:

    C, D. Disabling Service Set Identifier (SSID) broadcasting prevents a wireless network from appearing to clients. The clients must specify the SSID to which they want to connect. Media Access Control (MAC) address filtering is a form of Access Control List (ACL) that is maintained in the access point and that contains the addresses of devices that are to be permitted to access the network. Both of these mechanisms make it more difficult for unauthorized devices to connect to the access point. The other two options will not help to prevent unauthorized access. Kerberos is an authentication protocol used by Active Directory, and relocating the access point to a screened subnet (or DMZ) will not resolve the problem.
38. Traffic shaping is a series of techniques that optimize the allocation of network bandwidth. Which of the following are techniques used in traffic shaping to prevent networks from being overwhelmed by data transmissions? (Choose all that apply.)

    1. Broadcast storming
    2. Bandwidth throttling
    3. Network Address Translation (NAT)
    4. Rate limiting

    Answer:

    B, D. Bandwidth throttling is a traffic shaping technique that prevents specified data streams from transmitting too many packets. Rate limiting is a traffic shaping technique that controls the transmission rate of sending systems. A broadcast storm is a type of network switching loop. NAT is a method by which private networks can share registered IP addresses. Neither of these last two is a traffic shaping technique.
39. Multiprotocol switches are devices that perform functions associated with two different layers of the Open Systems Interconnection (OSI) reference model. Which two of the following layers are often associated with network switching? (Choose all that apply.)

    1. Application
    2. Presentation
    3. Session
    4. Transport
    5. Network
    6. Data link
    7. Physical

    Answer:

    E, F. The primary function of a network switch is to process packets based on their Media Access Control (MAC) addresses, which makes it a data link layer device. However, multiprotocol switches are devices that can also perform routing functions based on IP addresses, which operate at the network layer. Switches are not typically associated with the other layers of the OSI model.
40. You are attempting to connect your new laptop to your company's wireless network. The Wireless Access Point (WAP) on the network has a Service Set Identifier (SSID) that is not broadcasted and uses WiFi Protected Access II (WPA2) for security. Which of the following describes what you must do to connect your laptop to the network?

    1. Select the SSID from a list and allow the client to automatically detect the security protocol.
    2. Type the SSID manually and then select WPA2 from the security protocol options provided.
    3. Type the SSID manually and allow the client to automatically detect the security protocol.
    4. Select the SSID from a list and then select WPA2 from the security protocol options provided.

    Answer:

    B. An SSID that is not being broadcasted is not detectable by clients, so you must type it in manually. Security protocols are also not detectable, so you must select the WPA2 protocol from the list of options provided on the laptop.
41. Carrier Sense Multiple Access with Collision Avoidance (CSMA/CA) is a Media Access Control (MAC) mechanism designed to prevent two systems using the same network medium from transmitting at the same time. Which of the following IEEE standards calls for the use of CSMA/CA?

    1. 802.3
    2. 802.1X
    3. 802.11ac
    4. All of the above

    Answer:

    C. The IEEE 802.11ac standard, like all of the Wireless Local Area Network (WLAN) standards in the 802.11 working group, uses CSMA/CA for media access control. The 802.1X standard defines an authentication mechanism and does not require a media access control mechanism. The IEEE 802.3 (Ethernet) standard uses a different mechanism for media access control: Carrier Sense Multiple Access with Collision Detection (CSMA/CD).
42. A large enterprise network will—at a minimum—have demarcation points for telephone services and a connection to an Internet Service Provider's (ISP's) network. In many cases, these services will enter the building in the same equipment room that houses the backbone switch. Which of the following is the term used to describe this wiring nexus?

    1. MTBF
    2. IDF
    3. RDP
    4. MDF

    Answer:

    D. The place containing the demarcation points and the backbone switch is called the Main Distribution Frame (MDF). An Intermediate Distribution Frame (IDF) is the location of localized telecommunications equipment such as the interface between the horizontal cabling and the backbone. Mean Time Between Failures (MTBF) and Remote Desktop Protocol (RDP) are not network wiring locations.
43. You have configured your company's wireless network to enable clients to authenticate only when the signal strength of their connections exceeds a specified level. Which of the following terms best describes the security mechanism provided by this configuration?

    1. Geofencing
    2. Local authentication
    3. Motion detection
    4. Port security

    Answer:

    A. _Geofencing_ is the generic term for a technology that limits access to a network or other resource based on the client's location. In wireless networking, geofencing is intended to prevent unauthorized clients outside the facility from connecting to the network. By allowing only users with strong signals to connect, you help to prevent access to outside users. Local authentication is an application or service that triggers an authentication request to which the user must respond before access is granted. Port security is a method for protecting access to switch ports. Motion detection is a system designed to trigger a notification or alarm when an individual trespasses in a protected area. None of these other options are related to signal strength.
44. Social engineering has become an increasingly serious problem on your company network. Which of the following is an effective method for preventing sensitive data from being compromised through social engineering?

    1. Install a firewall between the internal network and the Internet.
    2. Install an antivirus software product on all user workstations.
    3. Implement a program of user education and corporate policies.
    4. Use IPSec to encrypt all network traffic.

    Answer:

    C. Social engineering is the practice of obtaining sensitive data by contacting users and pretending to be someone with a legitimate need for that data. No software or hardware solution can prevent it; the only way is to educate users of the potential dangers and establish policies that inform users what to do when they experience a social engineering attempt. Social engineering is not a virus or other form of malware, so an antivirus product has no effect against it. Social engineering is not implemented in network traffic, so a firewall cannot filter it, and IPsec cannot protect against it.
45. You have been given a Class B network IP address with which to configure the new network you are designing. Which of the following is the default subnet mask you should use for an IPv4 Class B network?

    1. 255.255.255.255
    2. 255.255.255.0
    3. 255.255.0.0
    4. 255.0.0.0

    Answer:

    C. A Class B address uses the first two octets as the network identifier, which yields a binary subnet mask of 11111111 11111111 00000000 00000000. In decimal form, the subnet mask is 255.255.0.0. The 255.0.0.0 mask is for Class A addresses, and the 255.255.255.0 mask is for Class C addresses. 255.255.255.255 is the broadcast address for the current network.
46. Alice's company has just started working with sensitive government data. To enhance the security of the datacenter, she has implemented some additional security measures. All of the servers now have crimped metal tags holding the cases closed. All of the hardware racks are locked in clear-fronted cabinets. All of the cable runs are installed in transparent conduits. These are all examples of which of the following physical security measures?

    1. Geofencing
    2. Tamper detection
    3. Port security
    4. Asset tracking

    Answer:

    B. All of the mechanisms that Alice has implemented are designed to make any attempts to tamper with or physically compromise the network hardware devices immediately evident. This is therefore a form of tamper detection. Asset tracking is for locating and identifying specific hardware components. Geofencing is a wireless networking technique for limiting access to a network based on signal strength. Port security refers to the protection of network switch ports from unauthorized access.
47. You have just installed a web server for your company, which is configured to host a public Internet site using the registered domain name [`adatum.com`](http://adatum.com/). The server's hostname in the Domain Name System (DNS) is `www`. The web server also has an administrative site, which you want to be able to access remotely. You have configured the administrative site to be encrypted and to use the port number 12354. Which of the following URLs must you use to access the administrative website from the Internet?

    1. [`https://www.adatum.com:12354`](https://www.adatum.com:12354/)
    2. [`http://www.adatum.com`](http://www.adatum.com/)
    3. [`https://www.adatum.com:80`](https://www.adatum.com:80/)
    4. [`http://www.adatum.com:12354`](http://www.adatum.com:12354/)

    Answer:

    A. Because the administrative site is encrypted, you must use the `https://` prefix to access it. Because the administrative site uses the nondefault port number 12354, you must append that number to the server name after a colon.
48. To prevent outside users from accessing your wireless network, you configure the access point not to broadcast the network's Service Set Identifier (SSID). However, you later discover that outsiders are still accessing the network. For which of the following reasons is disabling SSID broadcasts a relatively weak method of device hardening?

    1. Every access point's SSID is printed on a label on the back of the device.
    2. Attackers have software that can easily guess a network's SSID
    3. Attackers can capture packets transmitted over the network and read the SSID from them.
    4. Attackers have ways of connecting to the network without the SSID.

    Answer:

    C. Disabling SSID broadcasts is a way of hiding the presence of a wireless network, but if an intruder knows that a network is there, it is a simple matter to capture packets transmitted by the wireless devices and read the SSID from them. The other options do not explain the weakness of suppressing SSID broadcasts. It is not possible to connect to a wireless network without the SSID. SSIDs are set by the administrator of the access point; they are not printed on the device's label. SSIDs can be found relatively easily, but guessing them is no easier than guessing a password.
49. You are installing a web server farm in your corporate headquarters, which will be used to host websites for the corporation's subsidiaries, located all around the world. In which of the following cloud models does a single organization function as both the provider and the consumer of all cloud services?

    1. Private cloud
    2. Public cloud
    3. Ad hoc cloud
    4. Hybrid cloud

    Answer:

    A. In a private cloud, the same organization that uses the cloud services is also the sole owner of the infrastructure that provides those services. In the public cloud model, one organization functions as the provider, and another organization consumes the services of the provider. A hybrid cloud is a combination of public and private infrastructure so that the consumer organization is only a partial owner of the infrastructure. There is no such thing as an ad hoc cloud model.
50. Your supervisor has recently begun using the terms _on-boarding_ and _off-boarding_. With which of the following types of policies are these terms typically associated?

    1. Incident response
    2. Identity management
    3. Inventory management
    4. Data loss prevention

    Answer:

    B. On-boarding and off-boarding are identity management processes in which users are added or removed from an organization's Identity and Access Management (IAM) system. This grants new users the privileges they need to use the network, modifies their privileges if they change positions, and revokes privileges when they leave the company. On-boarding and off-boarding are not data loss prevention, incident response, or inventory management processes.
51. Virtual Private Networks (VPNs) use a data transmission technique called tunneling, which encapsulates a data packet within another packet for transmission over a network connection, typically using the Internet. The system also encrypts the entire encapsulated data packet for protection. Split tunneling is a variation of this method that provides which of the following advantages? (Choose all that apply.)

    1. Additional data integrity protection
    2. Access to local network devices while connected to the VPN
    3. Faster data transmission through multiplexing
    4. Conservation of VPN bandwidth

    Answer:

    B, D. A standard VPN typically uses full tunneling, in which all of the system's network traffic is encapsulated and encrypted for transmission. Split tunneling is a variation of this method in which only part of the system's traffic uses the VPN connection; the rest is transmitted over the network in the normal manner. Administrators can select which applications and devices use the VPN. Split tunneling can conserve the Internet bandwidth used by the VPN and provide access to local network services without the need for encapsulation. Split tunneling does not provide additional data integrity protection or improved performance through multiplexing.
52. Your supervisor wants you to disable all of the ports on the network's switches that are not in use. You tell her that this is not necessary, and she wants to know why you think so. Which of the following are valid reasons not to disable unused switch ports? (Choose all that apply.)

    1. The unused ports are not patched in to wall jacks.
    2. The datacenter is already secured from unauthorized access.
    3. The switch is configured to use a MAC-based ACL.
    4. Leaving some ports enabled facilitates the on-boarding of new users.

    Answer:

    B, C. If there is no way for unauthorized people to access the datacenter, then there is no danger of someone plugging a device into a port that is left enabled. If the switch uses an Access Control List (ACL) that specifies the Media Access Control (MAC) addresses of systems permitted to connect to it, then there is no need to disable unused ports, because any unknown devices plugged into open ports will not be granted access to the network. The other two options are not valid reasons. Ports that are not patched in can still be compromised at the switch location. Enabling ports is not difficult, so accommodating new users is not a valid reason for leaving them enabled.
53. Despite having imposed password policies on your network that compel users to change their passwords frequently, create passwords of a specific length, and use complex passwords, you have still had several reports of account penetrations. After investigating the incidents, you determine that the victims had all apparently shared a “tip” suggesting that users cycle through the names of their children, nephews, nieces, and other relatives when forced to create new passwords, changing letters to numbers as needed. Which of the following actions can you take to remedy the situation without creating a larger problem?

    1. Modify the password policies to force users to change passwords more frequently.
    2. Change the minimum password age policy to a larger value.
    3. Distribute a list of common passwords that are insecure, such as those based on names, birth dates, etc.
    4. Assign the users long passwords consisting of random-generated characters and change them often.

    Answer:

    C. There are no policies that can prevent users from creating easily guessed passwords. The only action that can help is to educate users that attackers are frequently able to guess passwords by using information such as familiar names and dates. Forcing more frequent password changes would not compel users to alter their method for choosing passwords, nor would increasing the minimum password age value. Assigning random passwords would address the issue, but user complaints and forgotten passwords would likely create greater problems than it would solve.
54. Which of the following network devices can employ Access Control Lists (ACLs) to restrict access? (Choose all that apply.)

    1. Routers
    2. Servers
    3. Switches
    4. Hubs
    5. Wireless Access Points

    Answer:

    A, B, C, E. ACLs restrict access to network devices by filtering user names, Media Access Control (MAC) addresses, IP addresses, or other criteria. Routers, servers, switches, and Wireless Access Points (WAPs) all can use ACLs to control access to them. Hubs are purely physical layer devices that relay electrical or optical signals. They have no access control mechanisms.
55. Which of the following terms is used to describe the threat mitigation technique of deploying individual applications and services on separate virtual servers so that no more than one is endangered at any one time, rather than deploying multiple applications on a single server?

    1. Network segmentation
    2. Geofencing
    3. VLAN hopping
    4. Role separation

    Answer:

    D. Role separation is the practice of creating a different virtual server for each server role or application. In addition to providing other benefits as well, this forces intruders to mount attacks on multiple servers to disable an entire network. Geofencing is a technique for limiting access to a wireless network. Network segmentation describes the process of creating multiple Virtual Local Area Networks (VLANs) or deploying firewalls to isolate part of a network. VLAN hopping is a type of attack in which an intruder sends command messages to a switch to transfer a port from one VLAN to another. None of these last three options refers to virtual machine deployment.
56. Which of the following statements about Dynamic Host Configuration Protocol (DHCP) snooping are true? (Choose all that apply.)

    1. DHCP snooping is implemented in network switches.
    2. DHCP snooping prevents DNS cache poisoning.
    3. DHCP snooping detects rogue DHCP servers.
    4. DHCP snooping drops DHCP messages arriving over the incorrect port.

    Answer:

    A, C, D. DHCP snooping is a feature found in some network switches that prevents rogue DHCP servers from assigning IP addresses to clients. It can also detect when DHCP release or decline messages arrive over a port other than the one on which the DHCP transaction originated. While DHCP snooping can prevent DHCP clients from being assigned an incorrect IP address, it does not directly prevent the poisoning of Dynamic Name System (DNS) server caches with erroneous information.
57. A user reports that she cannot connect to a server on her network. You want to identify the scope of the problem, so you try to reproduce the problem on the user's computer. The problem persists. No other users are reporting the same problem. What is the next logical step that you should perform to identify the affected area?

    1. Examine the server's configuration for the correct settings.
    2. Verify that the local router is forwarding traffic.
    3. Confirm that the switch the client is connected to is functioning.
    4. Perform the same task on another computer connected to the same segment.

    Answer:

    D. In this scenario, only one user is reporting a problem. Therefore, the likeliest next step is to perform the same task on another computer attached to the same segment. If you can perform the task successfully, the problem most likely lies within the user's computer or the connection to the switch. Since no other users are reporting the same problem, the server and switches on the network are probably up and functioning. Checking the router is not necessary since the user and server are on the same network.
58. On a wireless network, which of the following best describes an example of a captive portal?

    1. A web page stating that the data on a user's computer has been locked and will only be unlocked after payment of a fee
    2. A series of two doors with an intervening airlock through which people must pass before they can enter a secured space
    3. A dedicated switch port used to connect to other switches
    4. A web page with which a user must interact before being granted access to a wireless network

    Answer:

    D. A captive portal is a web page displayed to a user attempting to access a public wireless network. The user typically must supply identification, submit credentials, provide payment, or accept an end user agreement before access is granted. A captive portal does not refer to a switch port, a secured entryway to a room, or a type of extortionate computer attack.
59. In the standard troubleshooting methodology, you begin by taking steps to identify the problem. After you have done this, which of the following steps should you perform next?

    1. Verify full system functionality
    2. Establish a theory of probable cause
    3. Establish a plan of action
    4. Implement the solution

    Answer:

    B. After identifying the problem, the next step is to establish a theory for the probable cause of the problem. After that, you can test your theory, establish a plan of action, implement a solution, verify the functionality of the system, and document the entire process.
60. The secured version of the Hypertext Transfer Protocol (HTTPS) uses a different well-known port from the unsecured version (HTTP). Which of the following ports are used by HTTP and HTTPS by default? (Choose all that apply.)

    1. 25
    2. 80
    3. 110
    4. 443

    Answer:

    B, D. The well-known port for HTTPS is 443. The port for unsecured HTTP is 80. Neither of the other options are ports used by HTTP or HTTPS by default. Port 25 is used for the Simple Mail Transfer Protocol (SMTP), and Port 110 is used for the Post Office Protocol (POP3).
61. Which of the following are criteria typically used by load balancers to direct incoming traffic to one server out of a group of servers? (Choose all that apply.)

    1. Fastest response time
    2. Fastest processor
    3. Lightest load
    4. The next in an even rotation

    Answer:

    A, C, D. A load balancing router typically works by processing incoming traffic based on rules set by an administrator. The rules can distribute traffic among a group of servers using various criteria, such as each server's current load or response time or which server is next in a given rotation. Load balancers generally do not use the hardware configuration of the servers to direct traffic, as this is a factor that does not change over time.
62. You are responsible for a network that has a Domain Name System (DNS) server, a proxy server, and an Internet router. A user is reporting that she cannot connect to hosts on her own Local Area Network (LAN) or other internal LANs, and she also cannot access hosts on the Internet. No one else has reported a problem. What is the likeliest location of the issue preventing the user's access to the network?

    1. The router
    2. The DNS server
    3. The proxy server
    4. The user's computer configuration

    Answer:

    D. Since only one user is reporting difficulty, the problem is most likely to be in the user's computer and its configuration. A DNS server, proxy server, or router problem would affect more than one user.
63. Virtual Local Area Network (VLAN) hopping is a type of attack directed at network switches. Which of the following best describes how VLAN hopping is a potential threat?

    1. VLAN hopping enables an attacker to access different VLANs using 802.1q spoofing.
    2. VLAN hopping enables an attacker to scramble a switch's patch panel connections.
    3. VLAN hopping enables an attacker to change the native VLAN on a switch.
    4. VLAN hopping enables an attacker to rename the default VLAN on a switch.

    Answer:

    A. VLAN hopping is a method for sending false commands to switches to transfer a port from one VLAN to another. This can enable the attacker to connect his or her device to a potentially sensitive VLAN. VLAN hopping does not modify the switch's patch panel connections, only its VLAN assignments. It is not possible to rename a switch's default VLAN. VLAN hopping does not enable an attacker to change a switch's native VLAN.
64. You are a first-tier support technician working the IT help desk at your company. In your first hour of duty, you receive four trouble calls. Your job is to prioritize the calls based on their severity. Which of the following should be the problem that receives the lowest priority?

    1. A fatal error that causes a single computer to fail
    2. A problem with a mission-critical backbone router that affects an entire network
    3. A problem with an application server that affects a single Local Area Network (LAN)
    4. A problem with an order entry or customer service call center resource that affects an entire department, with multiple LANs

    Answer:

    A. A problem that affects the entire network should be given highest priority. This includes the issue with the mission-critical backbone router. Problems that affect multiple LANs or an entire department are generally given the next highest priority. A problem that affects a shared application server on a LAN should be given the next highest priority. A problem with a single user's computer should be given the lowest priority, compared to the other problems that have been reported.
65. You are attempting to access a Domain Name System (DNS) server located on the other side of a router, but your attempt fails with an error stating that the destination port UDP 53 is unreachable. Your first step in troubleshooting the problem is to try using the `nslookup` utility to access that specific DNS server. This attempt also fails. Next, you use the `ping` utility with the DNS server's IP address. The `ping` test is successful, indicating that the server is up and running. Which of the following are possible causes of the problem? (Choose all that apply.)

    1. The TCP/IP host settings on your computer are improperly configured.
    2. The router connecting the networks is not running DNS and will not forward this type of datagram.
    3. There is a firewall blocking the DNS server's UDP port 53.
    4. The DNS process on the remote server is not running.
    5. The TCP/IP host settings on the DNS server are improperly configured.

    Answer:

    C, D. One possible cause of the problem is that the DNS process on the remote server is corrupted or not running. Another possible cause is that there is a firewall blocking access to the DNS server's UDP port 53. Both of these would render the port unreachable. The TCP/IP client on the server is operating, as verified by the `ping` utility. This means that the IP host settings on your computer and on the DNS server are both configured properly and functioning. A router does not need to be running DNS to forward datagrams.
66. Which of the following types of switches performs a Cyclic Redundancy Check (CRC) on an entire frame's contents prior to forwarding it out a port leading to the destination system?

    1. Packet filtering
    2. Cut-through
    3. Source route
    4. Store-and-forward

    Answer:

    D. Store-and-forward switches take in the entire frame and verify its contents by performing a CRC calculation before forwarding it. Cut-through switches are faster because they look at only the first 6 bytes (the destination Media Access Control, or MAC, address) when forwarding a frame; they do not perform a CRC on the entire frame. Source route is a bridging technique in which the source host, not the switch, determines the path a frame will take through a network to reach a destination. Packet filtering is a technique used by firewalls. Neither of these is a type of switch.
67. Which of the following attack types is not specifically targeted at wireless network clients?

    1. Logic bomb
    2. Deauthentication
    3. Evil twin
    4. War driving

    Answer:

    A. A logic bomb is a code insert placed into a legitimate software product that triggers a malicious event when specific conditions are met. It can therefore affect both wired and wireless clients. The other options are all attacks directed at wireless networks. Deauthentication is a type of Denial-of-Service (DoS) attack in which the attacker targets a wireless client by sending a deauthentication frame that causes the client to be disconnected from the network. The object of the attack is often to compel the client to connect to a rogue access point called an evil twin. An evil twin is a fraudulent access point on a wireless network that mimics the Service Set Identifier (SSID) of a legitimate access point, in the hope of luring in users. War driving is an attack method that consists of driving around a neighborhood with a computer, scanning for unprotected wireless networks.
68. You are having trouble installing a Wireless Local Area Network (WLAN) using IEEE 802.11b/g equipment in a new office complex. The wireless devices have trouble connecting to the access point, and when they do, they achieve only low speeds. When you use a WiFi analyzer to scan the 2.4 GHz frequency band, you see literally dozens of other networks in the area, spread across all of the available channels. Choose the tasks from the following list that you should perform to enable your wireless devices to connect to the network reliably and at their best possible speeds. (Choose all that apply.)

    1. Configure the access point to suppress SSID broadcasts.
    2. Configure all of the wireless network devices to use the 5 GHz band.
    3. Upgrade all of the network devices to the latest firmware.
    4. Configure all of the network devices to use WPA2 encryption with AES.
    5. Upgrade the access point and all of the wireless client devices to IEEE 802.11n.

    Answer:

    B, E. Upgrading all of the wireless devices to 802.11n will enable them to use the 5 GHz band and evade the interfering traffic generated by the surrounding networks. Configuring the devices to use the 5 GHz band will provide many more channels to choose from and will avoid the interference from the surrounding 2.4 GHz networks. The other options will not resolve the problem. The type of encryption that a wireless network uses has no bearing on the ability of the devices to avoid the interference generated by surrounding networks. Suppressing Service Set Identifier (SSID) broadcasts will not help the devices to connect to the network. Upgrading the firmware on the devices is not likely to have any effect on the connection problems when they are the result of interference from other networks.
69. Which Windows command-line utility produced the output shown here?

    `Interface: 192.168.2.24 --- 0x2 Internet Address Physical Address Type 192.168.2.2 d4-ae-52-bf-c3-2d dynamic 192.168.2.20 00-26-c7-7e-00-e0 dynamic 192.168.2.22 00-90-a9-a2-43-8f dynamic 192.168.2.27 1c-c1-de-ca-1f-12 dynamic 192.168.2.28 30-f7-72-38-e9-1d dynamic 192.168.2.255 ff-ff-ff-ff-ff-ff static 224.0.0.22 01-00-5e-00-00-16 static 224.0.0.251 01-00-5e-00-00-fb static 224.0.0.252 01-00-5e-00-00-fc static 224.0.0.253 01-00-5e-00-00-fd static 239.255.255.250 01-00-5e-7f-ff-fa static 255.255.255.255 ff-ff-ff-ff-ff-ff static`

    1. `arp`
    2. `ping`
    3. `tracert`
    4. `netstat`

    Answer:

    A. Running the `arp` utility with the `-a` parameter on a Windows system displays the contents of the Address Resolution Protocol (ARP) cache, as shown here. The cache contains records of the IP addresses on the network that ARP has resolved into Media Access Control (MAC) addresses. The `ping`, `tracert`, and `netstat` utilities are not capable of producing this output.
70. Your boss is working in the crawlspace under the floor of the datacenter, and he asks you to hand him the pliers. You hand him the tool shown in the following figure, and he throws it back at you. What is the real function of the tool shown in the figure?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c07uf004_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. When you connect the tool to pins in a punchdown block, you can access telephone circuits in order to test them or place telephone calls.
    2. When you attach the tool to one end of a wire, it generates a tone that can be detected at the other end.
    3. To attach a bulk cable end to an RJ45 connector, you use the tool to squeeze the connector closed, forcing the wire ends to contact the connector's pins.
    4. When you attach the tool to a copper cable, you can detect and measure the electrical current flowing through it.

    Answer:

    C. The device shown in the figure is a crimper, which is used to create patch cables by attaching connectors to both ends of a relatively short length of bulk cable. This tool is not capable of placing telephone calls, generating a tone on a wire, or measuring electric current.
71. You are starting work for a contractor that performs telecommunications cable installations. One of the tools in the kit you have been given is in the following figure. What is the name of the tool shown?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c07uf005_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. Crimper
    2. Punchdown tool
    3. Butt set
    4. Tone generator and locator

    Answer:

    B. The device shown in the figure is a punchdown tool, used to connect unshielded twisted-pair cable ends to the keystone connectors used in modular wall plates and patch panels. After lining up the individual wires in the cable with the connector, you use the tool to press each wire into its slot. The tool also cuts the wire sheath to make an electrical contact and trims the end of the wire. The tool shown is not a crimper, a butt set, or a tone generator and locator.
72. You are seeking to upgrade your company's IEEE 802.11b access point to one that provides faster transmission speeds for your newer workstations. Which of the following wireless networking standards are capable of supporting speeds faster than the 11 Mbps of 802.11b but that are still backward compatible with your existing IEEE 802.11b workstations? (Choose all that apply.)

    1. IEEE 802.11
    2. Bluetooth
    3. IEEE 802.11g
    4. IEEE 802.11a
    5. IEEE 802.11n

    Answer:

    C, E. IEEE 802.11g supports transmission speeds up to 54 Mbps, and it is backward compatible with 802.11b equipment. IEEE 802.11n is also backward compatible with 802.11b, and it can run at speeds up to 600 Mbps. Bluetooth is not compatible with any of the IEEE 802.11 standards. IEEE 802.11 cannot run at 54 Mbps, and though 802.11a can, it is not compatible with 802.11b.
73. You are working on your company's screened subnet (also known as a perimeter network), which has five Linux web servers, a Cisco router, a CSU/DSU providing a leased line connection, and a Windows-based firewall on it. While trying to troubleshoot a network communications failure, you type the following command on one of the systems: `traceroute` [`adatum.com`](http://adatum.com/). Which of the following systems might you be working on? (Choose all that apply.)

    1. The Cisco router
    2. One of the Linux web servers
    3. The CSU/DSU console
    4. The Windows-based firewall

    Answer:

    A, B. Both Linux and the Cisco IOS operating systems include the traceroute utility. Windows has its own version of the utility, but it is called `tracert`. The CSU/DSU cannot run a `traceroute` command.
74. Which of the following are network topologies used by IEEE 802.11 Wireless Local Area Networks (WLANs)? (Choose all that apply.)

    1. Bus
    2. Mesh
    3. Ad hoc
    4. Star
    5. Infrastructure

    Answer:

    C, E. WLANs can use the ad hoc topology, in which devices communicate directly with each other, or the infrastructure topology, in which the wireless devices connect to an access point. The bus, star, and mesh topologies are used by wired networks only.
75. You have recently started a new job that enables you to telecommute from home, and you need a Wide Area Network (WAN) connection to the Internet. You will need to access the company network using a Virtual Private Network (VPN) connection to obtain client information, transfer files, and send email through the company servers. Your home is over 30 years old. The existing telephone wiring was not run through a conduit, and it seems to be deteriorating. You have cable television service, and your home is approximately 20,000 feet from the nearest telephone central office. You want to implement the fastest possible remote connection service, but cost is still a factor in the decision. Which WAN technology should you implement?

    1. A standard modem-to-modem connection
    2. A DSL (Digital Subscriber Line) connection
    3. A broadband cable television (CATV) connection
    4. A dedicated leased line (fractional T-1)

    Answer:

    C. In this scenario, the best solution is for you to use the existing CATV service for the Internet connection. CATV offers faster data rates than standard modem-to-modem service and supports VPN connections. A dedicated fractional T-1 line is expensive and is not typically used for remote user connections. Since your telephone lines are not run through conduit and the distance to the central office is more than 18,000 feet, you probably cannot use DSL technology, because it requires good-quality lines and close proximity to a central office.
76. You are working the help desk at a local computer store, and you receive a call from a customer trying to set up a home network using computers running Windows 10 and wired Ethernet equipment. The customer reports that she cannot access the other two computers in the house from her workstation, nor can she access the Internet. You ask her to run the `ipconfig /all` command and read the results to you. She says that her IP address is 192.168.0.2, her subnet mask is 255.255.255.0, and her default gateway is 192.168.0.1. Which of the following is the most likely cause of the customer's problem?

    1. The customer's network address cannot include a zero.
    2. The customer has an incorrect subnet mask.
    3. The customer's network cable is damaged or unplugged.
    4. The customer has an incorrect default gateway address.

    Answer:

    C. The customer's IP address, subnet mask, and default gateway values are appropriate for her home network. There is nothing wrong with having a zero in the network address. Therefore, of the options presented, the only logical choice is that the workstation's network cable is damaged or unplugged.
77. Some networks are designed with a switching fabric that contains redundant paths, for fault tolerance purposes. However, in this type of design, it is possible for packets to circulate endlessly around the network, which is called a switching loop. Which of the following protocols prevents network switching loops from occurring by shutting down redundant links until they are needed?

    1. NAT
    2. RIP
    3. VLAN
    4. STP

    Answer:

    D. The Spanning Tree Protocol (STP) prevents packets from endlessly looping from switch to switch due to redundant links. Creating redundant links is a good preventive measure against switch failure, but packets transmitted over multiple links can circulate from switch to switch infinitely. STP creates a database of switching links and shuts down the redundant ones until they are needed. None of the other three protocols listed can perform this function. Network Address Translation (NAT) is a routing method that enables private networks to share registered IP addresses. Routing Information Protocol (RIP) propagates routing table information to other routers. A Virtual Local Area Network (VLAN) is an organizational tool that operates within switches by creating multiple broadcast domains.
78. You are responsible for an internetwork that consists of four internal Local Area Networks (LANs) with 50 users each. Each internal LAN uses twisted-pair Gigabit Ethernet links that connect the users to a switch. Each of the four switches is connected to a separate router. All four routers connect to the same backbone network, which has a single additional router to connect the company's network to the Internet, using a T-1 Wide Area Network (WAN) link. Today, users on one of the four internal LANs are reporting that when they came in this morning, they could not access the Internet or resources on the other three internal LANs. However, they could access resources on their own LAN with no problems. Which network component is the likeliest source of the problem in this scenario?

    1. The switch on the problem LAN
    2. The Internet router
    3. The router connecting the problem LAN to the backbone
    4. The cable on the backbone network

    Answer:

    C. In this scenario, only the users on one LAN are experiencing problems connecting to the Internet and the other internal LANs. This isolates the problem to a component within that LAN only. Since users can connect successfully to local resources, the problem does not lie within the individual computers, the switch that connects the users to the network, or the backbone network cable. The likeliest problem is therefore in the router connecting the problem LAN to the backbone network. Since users on the other internal LANs are not reporting problems connecting to the Internet, the problem most likely does not involve the Internet router.
79. You are negotiating an agreement with a provider for your company's email service. You have been told to require a 99.99 percent guaranteed rate of service reliability, but the provider is only willing to guarantee 99 percent. Eventually, you and the provider agree on a compromise of 99.9 percent. Which of the following documents will include the negotiated language on this particular point?

    1. AUP
    2. SLA
    3. BYOD
    4. NDA

    Answer:

    B. The agreed upon 99.9 percent guaranteed availability will be part of a Service Level Agreement (SLA), which is a contract between a provider and a subscriber that specifies the percentage of time that the contracted services are available. None of the other three options contain the guaranteed reliability language. Acceptable Use Policies (AUPs) specify whether and how employees can use company-owned hardware and software resources. A Nondisclosure Agreement (NDA) specifies what company information employees are permitted to discuss outside the company. A Bring Your Own Device (BYOD) policy specifies the personal electronics that employees are permitted to use on the company network and documents the procedures for connecting and securing them.
80. Which of the following types of networking devices can split a single network into multiple collision domains while maintaining a single broadcast domain? (Choose all that apply.)

    1. Switch
    2. Bridge
    3. Router
    4. Hub

    Answer:

    A, B. A bridge can split a single network into two collision domains, because it forwards only the packets that are destined for the other side of the bridge. A switch creates a separate collision domain for each port. Both bridges and switches forward all broadcast packets, so they maintain a single broadcast domain for the entire network. A hub maintains a single collision domain and a single broadcast domain. A router creates two collision domains, but it does not forward broadcasts, so it creates two broadcast domains as well.
81. You have just finished installing a web server farm on your company's network, along with a router to create a screened subnet (perimeter network) on which the web servers are located. However, you now cannot access the web servers from your workstation on the internal network. Which of the following is not one of the tasks you will have to complete before you can access the screened subnet from the internal network?

    1. Change MAC addresses
    2. Change IP addresses
    3. Update the DNS records
    4. Change default gateway addresses

    Answer:

    A. Media Access Control (MAC) addresses are hard-coded into network interface adapters and are not easily changeable. There is also no need to change them for this purpose. First, you will have to change IP addresses of the web servers. This is because the computers on the other side of the router, on the screened subnet, must use an IP network address that is different from the internal network's address. Next, you will have to change the default gateway address setting on the internal network computers to the address of the router on the internal network so that traffic can be forwarded to the screened subnet. Finally, you will have to update the resource records on your Domain Name System (DNS) server to reflect the IP address changes.
82. You are testing a twisted-pair cable run using a tone generator and locator. When you apply the tone generator to a particular pin at one end of the cable, you detect a tone on two pins at the other end. Which of the following faults have you discovered?

    1. Split pair
    2. Open
    3. Short
    4. Crosstalk

    Answer:

    C. A short is when a wire is connected to two or more pins at one end of the cable or when the conductors of two or more wires are touching inside the cable. This would cause a tone applied to a single pin at one end to be heard on multiple pins at the other end. The other three options would not cause this to occur. An open circuit would manifest as a failure to detect a tone on a wire, indicating that there is either a break in the wire somewhere inside the cable or a bad connection with the pin in one or both connectors. A split pair is a connection in which two wires are incorrectly mapped in exactly the same way on both ends of the cable. Crosstalk is a type of interference caused by signals on one wire bleeding over to other wires.
83. Your network has been experiencing intermittent service slowdowns and outages ever since the company moved into their new building. You have tried every troubleshooting modality you can think of, but you have not been able to determine the cause. One particular user, perhaps hoping to be the squeaky wheel that gets the grease, has taken to calling you every time he experiences a problem. One day, as you are working in the datacenter, you notice that the user calls every time you hear an additional humming noise. After examining the doors in the hallway, you realize that the racks containing the network switches are located right next to the elevator machinery room. Which of the following conditions is probably causing this intermittent network communication problem?

    1. Bottleneck
    2. EMI
    3. Latency
    4. Crosstalk

    Answer:

    B. Elevator machinery, fluorescent light fixtures, and other electrical devices in an office environment can generate magnetic fields, resulting in electromagnetic interference (EMI). When copper-based cables are located too near to such a device, the magnetic fields can generate an electric current on the cable that interferes with the signals exchanged by network devices. If the network users experience a problem every time the elevator machinery switches on, EMI is a likely cause of the problem. Crosstalk and attenuation can both cause intermittent network communication problems, but they cannot be caused by elevator machinery. Latency describes a generalized delay in network transmissions, not intermittent packet delays.
84. Ralph is installing a pair of redundant servers and must choose whether to run them in an active-active or active-passive configuration. Running the servers in an active-active configuration provides which of the following advantages that the same servers in an active-passive configuration do not? (Choose all that apply.)

    1. Fault tolerance
    2. Load balancing
    3. Data encapsulation
    4. Increased performance

    Answer:

    B, D. In an active-active configuration, servers can balance the incoming client load between them. Because the active servers are all servicing clients, the overall performance of the cluster is increased. Both active-active and active-passive configurations provide fault tolerance. Data encapsulation is not a factor in either configuration.
85. You are starting work at a new company, and on your first day, you ask about wireless access for your laptop. You are given a Service Set Identifier (SSID) and a WiFi Protected Access II (WPA2) passphrase. Later, in the lunchroom, when you try to connect your laptop to the network, you cannot see the SSID you were given in the list of available networks, although you can see other networks. What should you do next to try to resolve the problem?

    1. Move closer to the Wireless Access Point (WAP).
    2. Move away from the microwave in the lunchroom.
    3. Type in the WPA2 passphrase.
    4. Type the SSID in manually.

    Answer:

    D. It is possible that the WAP has been configured to not broadcast the network's SSID as a security measure, so you should first attempt to access it by typing the SSID in manually. You cannot type in the WPA2 passphrase until you are in the process of connecting to the SSID. Moving the laptop closer to the access point or away from possible sources of electromagnetic interference might be solutions to the problem, but they should not be the first thing you try in this case.
86. You are responsible for a Wireless Local Area Network (WLAN) that consists of an 802.11n 2x2 access point and laptop computers with a variety of network adapters. Some of the laptops support 802.11n, most support 802.11g, and a few older models have 802.11b adapters. The WLAN is located in a large office building with many other wireless networks, and you are having trouble finding a channel on the 2.4 GHz band that is not congested with traffic. Scanning the 5 GHz band, you find relatively little traffic, so you reconfigure the access point to use a 5 GHz channel. The result is that some of the laptops are able to connect to the network, whereas others are not. What is the most likely reason for the connection failures, and what must you do to enable all the laptops to connect to the wireless network?

    1. The 802.11b standard does not support communication using the 5 GHz band. You must replace the network adapters in those laptops with newer models for them to connect successfully.
    2. The 5 GHz band does not support automatic channel selection. You must configure each laptop to use the same channel as the access point for all the laptops to connect successfully.
    3. The 5 GHz band does not support Multiple Input, Multiple Output (MIMO) communications, so the 802.11n laptops are unable to connect to the network. You must replace the access point with an 802.11g unit for all the laptops to connect successfully.
    4. The 802.11g and 802.11b standards do not support communication using the 5 GHz band. You must configure the access point to support 2.4 GHz for all the laptops to connect successfully.

    Answer:

    D. The 802.11b and 802.11g standards do not support 5 GHz communications. Configuring the access point to support 2.4 GHz is the only way for the 802.11b and 802.11g computers to connect to the network. The 5 GHz band does support automatic channel selection, so there is no need to configure the channel on each laptop manually. The 5 GHz band does support MIMO, and the 802.11n laptops should be able to connect. The 802.11b standard does support the 2.4 GHz band.
87. In the Domain Name System (DNS), a zone is a contiguous area of the DNS namespace for which authority is delegated to one or more DNS servers. Which of the following DNS resource record types specifies the IP addresses of the authoritative DNS servers for a particular zone?

    1. PTR
    2. SRV
    3. MX
    4. NS

    Answer:

    D. The Name Server (NS) resource record identifies the authoritative servers for a particular DNS zone. Pointer Records (PTRs) are used to resolve IP addresses into hostnames. Mail Exchange (MX) records identify the mail servers for a particular domain. Service Records (SRVs) identify the designated servers for a particular application. None of these other options identify the authoritative servers for a zone.
88. You are experiencing poor performance on your home 802.11n wireless network. You live in a large apartment complex, and when you run a WiFi analyzer, you see many other nearby networks using the often-recommended channels 1, 6, and 11 on the 2.4 GHz frequency. Using the 5 GHz frequency is not an option for your equipment. What should you do to improve the network's performance?

    1. Configure your equipment to use channel 10.
    2. Configure your equipment to use channel 9.
    3. Configure your equipment to use channel 5.
    4. Configure your equipment to use channel 2.

    Answer:

    B. The 2.4 GHz band used by Wireless Local Area Networks (WLANs) consists of channels that are 20 (or 22) MHz wide. However, the channels are only 5 MHz apart, so there is channel overlap that can result in interference. Channels 1, 6, and 11 are the only channels that are far enough apart from each other to avoid any overlap with the adjacent channels. This is why they are often recommended. However, in this scenario, these channels are too crowded with other networks. You should therefore use a channel that is as far as possible from the crowded ones. Channels 2, 5, and 10 are all immediately adjacent to a crowded channel, but channel 9 is at least two channels away from the nearest crowded channel. Therefore, you should configure your equipment to use channel 9.
89. Your company's office building is having a fire inspection, and you are the only person on duty in the datacenter. The inspector from the fire department asks you where they can find documentation about all chemicals and equipment used in the company's datacenter. You lead the inspector to the director's office, but you are not sure what the documents he needs are called. Which of the following document types contains this information?

    1. MSDS
    2. NDA
    3. BYOD
    4. ESD

    Answer:

    A. Material Safety Data Sheets (MSDSs) are documents created by manufacturers of chemical, electrical, and mechanical products that specify the potential risks and dangers associated with them, particularly in regard to flammability and the possibility of toxic outgassing. A properly documented network should have MSDS documents on file for all of the chemical and hardware products used to build and maintain it. MSDSs can be obtained from manufacturers or the Environmental Protection Agency (EPA). Electrostatic discharges (ESDs), Nondisclosure Agreements (NDAs), and Bring Your Own Device (BYOD) policies are not concerned with the dangers inherent in building contents.
90. Which of the following Power over Ethernet (PoE) specifications supplies power to devices using the spare wire pair on a 10Base-T or 100Base-TX twisted-pair network?

    1. 4PPoE
    2. Alternative A
    3. Alternative B
    4. All of the above

    Answer:

    C. The Alternative B PoE variant can use the spare wire pair in a CAT 5 or better 10Base-T or 100Base-TX cable to supply power to connected devices. The Alternative A and 4PPoE variants cannot use the spare wire pair in this manner; they supply power using the wire pairs that carry data at the same time. For Gigabit Ethernet or faster installations, Alternative B is also capable of using the data wire pairs.
91. The iSCSI storage area networking protocol uses clients called initiators and servers called targets. However, on many Storage Area Networks (SANs), there needs to be a way for the initiators to locate the targets. Which of the following technologies do iSCSI initiators use to locate iSCSI targets on the network?

    1. ICMP
    2. DNS
    3. iDNS
    4. iSNS

    Answer:

    D. The Internet Storage Name Service (iSNS) is an application that provides iSCSI initiators with automated discovery of targets located on the network. iSNS can also function as a discovery service for Fibre Channel devices. Internet Control Message Protocol (ICMP) and Domain Name System (DNS) are not capable of registering iSCSI targets. iDNS does not exist.
92. You are deploying an 802.11n wireless network for a client that is asking for the best possible security you can provide without deploying additional servers. When setting up the Wireless Access Point (WAP), you disable Service Set Identifier (SSID) broadcasts, select WiFi Protected Access with Pre-Shared Keys (WPA-PSKs), and configure Media Access Control (MAC) address filtering. Which of the following statements about the security of this arrangement is true?

    1. You should not disable SSID broadcasts since this prevents users from connecting to the network.
    2. The configuration is as secure as you can make it with the specified equipment.
    3. You should use WiFi Protected Access II (WPA2) instead of WPA, since it is more resistant to certain types of attacks.
    4. You should not use MAC address filtering since it exposes MAC addresses to possible attacks.

    Answer:

    C. WPA has been found to be vulnerable, and WPA2 was designed to address those vulnerabilities, so you should use WPA2 instead of WPA. Suppressing SSID broadcasts does not prevent users from connecting to the network, and MAC filtering strengthens security without exposing MAC addresses to undue risk.
93. Which of the following connector types are used with fiber-optic cables? (Choose all that apply.)

    1. DB-9
    2. SC
    3. BNC
    4. ST
    5. MTRJ
    6. RJ11

    Answer:

    B, D, E. Subscriber Connector (SC), Mechanical Transfer - Registered Jack (MT-RJ), and Straight Tip (ST) are all types of fiber-optic connectors. DB-9 is a D-shell connector used for serial ports. Bayonet-Neill-Concelman (BNC) is a type of connector used with coaxial cable. RJ11 is used with twisted-pair cable for telephone connections.
94. Which of the following are available as Internet of Things (IoT) devices?

    1. Refrigerators
    2. Doorbells
    3. Thermostats
    4. Speakers
    5. All of the above

    Answer:

    E. The IoT consists of devices that are ordinarily passive, but which have been made intelligent by installing a network client configuring them to participate on an IP network. All of the devices listed are available as “smart” devices that enable remote users to interact with them over the Internet.
95. You are designing an Ethernet network for your company's newest branch office. Your current task is to decide which Ethernet specification to use for the network, a decision that you know will determine what type of cabling you need to purchase and the topology with which the cable will be installed. Which layers of the Open Systems Interconnection (OSI) reference model apply to the cabling and topology elements of a network?

    1. The application and transport layers
    2. The transport and network layers
    3. The network and data link layers
    4. The data link and physical layers

    Answer:

    D. The physical layer defines the mechanical and electrical characteristics of the cables used to build a network. The data link layer defines specific network (LAN or WAN) topologies and their characteristics. The physical layer specification you will implement is dependent on the data link layer protocol you select. The network, transport, and application layers are not concerned with cables and topologies.
96. You are troubleshooting a workstation that cannot access the network. The workstation is plugged into a wall plate that should provide it with access to a DHCP-equipped network using the 192.168.4.0/24 network address. No one else on that network is reporting a problem. You check that the patch cable is properly plugged into the workstation and the wall plate, which they are, and then run `ipconfig /all` on the workstation and examine the output. Which of the statements could be the explanation for the workstation's problem, based on the following `ipconfig` results?

    `Windows IP Configuration Host Name . . . . . . . . . . . . : Client12 Primary Dns Suffix . . . . . . . : Node Type . . . . . . . . . . . . : Hybrid IP Routing Enabled. . . . . . . . : No WINS Proxy Enabled. . . . . . . . : No Ethernet adapter Local Area Connection: Connection-specific DNS Suffix . : Description . . . . . . . . . . . : PCIe Family Controller Physical Address. . . . . . . . . : 60-EB-69-93-5E-E5 DHCP Enabled. . . . . . . . . . . : Yes Autoconfiguration Enabled . . . . : Yes Link-local IPv6 Address . . . . . : fe80::c955:c944:acdd:3fcb%2 IPv4 Address. . . . . . . . . . . : 169.254.203.42 Subnet Mask . . . . . . . . . . . : 255.255.0.0 Lease Obtained. . . . . . . . . . : Monday, October 23, 2017 6:23:47 PM Lease Expires . . . . . . . . . . : Saturday, November 18, 2017 9:49:24 PM Default Gateway . . . . . . . . . : DHCPv6 IAID . . . . . . . . . . . : 241232745 DHCPv6 Client DUID. . . . . . . . : 00-01-00-01-18-10-22-0D-60-EB-69-93-5E-E5 DNS Servers . . . . . . . . . . . : fec0:0:0:ffff::1%1 fec0:0:0:ffff::2%1 fec0:0:0:ffff::3%1 NetBIOS over Tcpip. . . . . . . . : Enabled`

    1. The DNS server addresses are incorrect.
    2. The Default Gateway address is missing.
    3. The Subnet Mask value is incorrect.
    4. The DHCP scope is exhausted.

    Answer:

    D. The 169.254.203.42 address assigned to the workstation is from the 169.254.0.0/16 network address assigned to Automatic Private IP Addressing (APIPA), a standard for the assignment of IP addresses to Dynamic Host Configuration Protocol (DHCP) clients when they cannot obtain an address from a DHCP server. The workstation's DHCP client is activated, and since no one else is experiencing a problem, you can assume that the DHCP server is functioning. The Subnet Mask value is correct for an APIPA address, and APIPA does not provide Default Gateway or Domain Name System (DNS) server addresses. Therefore, an exhausted DHCP scope is the only one of the explanations provided that could be the cause of the problem.
97. A user calls you at the IT help desk and reports that she is having intermittent problems accessing both local servers and internet websites. Which of the following potential problems can you rule out immediately?

    1. Malfunctioning Domain Name System (DNS) server
    2. Duplicate Media Access Control (MAC) addresses
    3. Duplicate IP addresses
    4. Malfunctioning router

    Answer:

    C. Operating systems detect duplicate IP addresses immediately and display error messages or notifications on the computers involved. Therefore, the user with the problem would have been informed immediately if another system was using her IP address. All of the other options are possible causes of the problem that are more difficult to troubleshoot.
98. You have recently discovered a rogue Dynamic Host Configuration Protocol (DHCP) server on your network. After disabling the rogue server, you now need to terminate all of the rogue IP address leases currently held by DHCP clients on the network and then have them request new leases from the authorized DHCP server. Which of the following commands must you run on each client to do this? (Choose all that apply.)

    1. `ipconfig /dump`
    2. `ipconfig /lease`
    3. `ipconfig /release`
    4. `ipconfig /renew`
    5. `ipconfig /discard`

    Answer:

    C, D. The `ipconfig /release` command terminates the current DHCP address lease. Then, the `ipconfig /renew` command causes the client to begin the process of negotiating a new lease, this time with the authorized DHCP server. `dump`, `lease`, and `discard` are not valid `ipconfig` parameters.
99. Ralph is reading an article about datacenter design, and he is puzzled by references to east-west and north-south traffic. Which of the following statements best describes the difference between east-west and north-south traffic in a datacenter?

    1. East-west is switch-to-switch traffic, while north-south is switch-to-router traffic.
    2. East-west describes traffic between devices at the same layer of the Open Systems Interconnection (OSI) reference model, while north-south describes traffic between OSI model layers.
    3. East-west traffic stays within the datacenter, while north-south traffic does not.
    4. East-west is backbone traffic among switches and routers, while north-south is traffic to end systems, such as servers.

    Answer:

    C. East-west traffic describes traffic flow within the datacenter, while north-south is traffic between devices inside the datacenter and outside devices. The terms east-west and north-south do not pertain to the OSI model layers or to the specific devices used.
100.    Which of the following attack types involves the modification of a legitimate software product?

        1. War driving
        2. Logic bomb
        3. Evil twin
        4. Social engineering

        Answer:

        B. A logic bomb is a code insert placed into a legitimate software product that triggers a malicious event when certain conditions are met, such as when a specific time or date arrives. All of the other options do not involve software products. Social engineering is the practice of obtaining sensitive data by contacting users and pretending to be someone with a legitimate need for that data. War driving is an attack method that consists of driving around a neighborhood with a computer, scanning for unprotected wireless networks. An evil twin is a fraudulent access point on a wireless network that mimics the Service Set Identifier (SSID) of a legitimate access point, in the hope of luring in users.
