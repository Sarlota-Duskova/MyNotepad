# Exam 1

1.  Which of the following are the layers in the standard three-tier datacenter architecture? (Choose all that apply.)

    1. Core
    2. Intermediate
    3. Distribution
    4. Access

    Answer:

    A, C, D. The three-tier hierarchical architecture for datacenters consists of core, distribution, and access layers. The access layer in a datacenter contains servers, the distribution layer contains redundant switch connections, and the core layer provides high-speed transport between the switches. There is no intermediate layer in the architecture.
2.  You are a new hire at Adatum Corp., and this is your first day on the job. You are setting up your workstation, but you are unsure whether you are permitted to install your favorite software on the company's computer. The Human Resources server has a large library of employee documents. Which of the following is a document that you might want to consult to determine whether personal software is allowed?

    1. SLA
    2. AUP
    3. NDA
    4. BYOD

    Answer:

    B. An Acceptable Use Policy (AUP) specifies whether and how employees can use company-owned hardware and software resources. AUPs typically specify what personal work employees can perform while on the job, what hardware and software they can install, and what levels of privacy they are permitted when using company equipment. This is the document that will most likely include the information you seek. A Service Level Agreement (SLA) is a contract between a provider and a subscriber. A Non-Disclosure Agreement (NDA) specifies what company information employees are permitted to discuss outside the company. Bring Your Own Device (BYOD) is a policy that specifies how employees can connect their personal devices to the company network.
3.  You are working the help desk when a user calls and reports that she is unable to connect to the Internet. Which of the following steps would you be least likely to perform first when troubleshooting the problem?

    1. Check the configuration of the router connecting the Local Area Network (LAN) to the Internet.
    2. Ask the user if she can access resources on the local network.
    3. Check to see if anyone else is experiencing the same problem.
    4. Check the user's job title to see if she is an important person in the company.

    Answer:

    A. There are many possible causes for the problem that are more likely than a router configuration error, so this is not something you should check first. Asking if the user can access the local network attempts to isolate the problem. If she cannot, the problem could be in her computer; if she can, then the problem lies somewhere in the Internet access infrastructure. If other users are experiencing the problem, then the issue should receive a higher priority, and you will know for sure that the problem does not lie in the user's computer. While the user's job title might not be the first thing you check, it is a political reality that higher ranking users get preferential treatment.
4.  Which of the following is not a means of preventing unauthorized individuals from entering a sensitive location, such as a datacenter?

    1. Key fobs
    2. Motion detection
    3. Biometric scans
    4. Identification badges

    Answer:

    B. Biometric scans, identification badges, and key fobs are all mechanisms that are designed to distinguish authorized from unauthorized personnel. Motion detection cannot make this distinction and is therefore not a means of preventing unauthorized access.
5.  You are an IT consultant who has been contracted to install new computers on a client's Gigabit Ethernet network. You want the performance of the new computers to be as good as it can be, so you configure their network adapters to run at the full speed of 1 Gbps and to use full-duplex communication. You test the computers after installing them, and they function well. However, once the computers are in service, you begin getting complaints from the client of extremely poor network performance on the new machines. You return to the site that evening and run some `ping` tests, but you do not detect any problem. You call in a colleague to perform a packet analysis, and she detects large numbers of packet collisions, late collisions, Cyclic Redundancy Check (CRC) errors, and runt frames. Which of the following could be the cause of the problem?

    1. Damaged cables
    2. Transmit/Receive (TX/RX) reversal
    3. Duplex mismatch
    4. Incorrect cable type

    Answer:

    C. The problem is most likely the result of a duplex mismatch. There should be no collisions on a full-duplex network, so the problem is clearly related to the duplexing of the communications. A twisted-pair Ethernet adapter, running in its original half-duplex mode, detects collisions by looking for data on both the transmit and receive pins at the same time. In full-duplex mode, however, data is supposed to be transmitted and received at the same time. When one side of a connection is configured to use full duplex, as the new computers are, and the other end is configured to use half duplex (as the network switches must be), the full-duplex communications on the one side look like collisions to the half-duplex side. The half-duplex adapter transmits a jam signal as a result of each collision, which causes the full-duplex side to receive an incomplete frame. Both sides then start to retransmit frames in a continuing cycle, causing network performance to diminish alarmingly. The `ping` tests do not detect a problem, because `ping` transmits only a small amount of data in one direction at a time. All of the other options would likely cause the `ping` tests to fail. The solution to the problem is to configure the new computers to autonegotiate their speed and duplex modes.
6.  Which of the following is a wireless topology that does not require the use of an access point?

    1. Star
    2. Ad hoc
    3. Bus
    4. Infrastructure

    Answer:

    B. An ad hoc topology (also known as an independent basic service set) is one in which wireless computers communicate directly with one another without the need for an access point. A Wireless Access Point (WAP) is a device with a wireless transceiver that also connects to a standard cabled network. Wireless computers communicate with the access point, which forwards their transmissions over the network cable. This is called an infrastructure topology. Star and bus topologies are not used by wireless networks; they require the computers to be physically connected to the network cable.
7.  You want to create a network in which computers from different departments are assigned to separate Virtual Local Area Networks (VLANs). You also want to be able to forward traffic between the VLANs so that each computer is capable of accessing any other computer. Which of the following will enable you to perform all these functions with a single device?

    1. Load balancer
    2. Virtual router
    3. Multilayer switch
    4. Broadband router

    Answer:

    C. A multilayer switch is a network connectivity device that functions at both layer 2 and layer 3 of the Open Systems Interconnection (OSI) model. At layer 2, the data link layer, the device functions like a normal switch, providing an individual collision domain to each connected node and enabling you to create multiple VLANs. At layer 3, the network layer, the device also provides routing capabilities by forwarding packets between the VLANs. Virtual routers, load balancers, and broadband routers are strictly layer 3 devices that can route traffic but cannot create VLANs.
8.  Which of the following are standard terms used in data loss prevention to describe specific data states? (Choose all that apply.)

    1. Data on-line
    2. Data at-rest
    3. Data in-motion
    4. Data in-use

    Answer:

    B, C, D. _Data at-rest_ is a data loss prevention term that describes data that is currently in storage while not in use. _Data in-motion_ is the term used to describe network traffic. _Data-in-use_ describes endpoint actions. _Data on-line_ is not one of the standard data loss prevention terms.
9.  Temporal Key Integrity Protocol (TKIP) is an encryption protocol that was introduced in the IEEE 802.11 wireless network standards to replace another protocol that was found to be easily penetrated. Which of the following 802.11 wireless security protocols uses TKIP for encryption?

    1. AES
    2. WEP
    3. WPA
    4. WPA2

    Answer:

    C. WiFi Protected Access (WPA) is the wireless security protocol that was designed to replace the increasingly vulnerable Wired Equivalent Privacy (WEP) protocol. WPA added an encryption protocol called Temporal Key Integrity Protocol (TKIP) that was more difficult to penetrate. However, over time, TKIP too became vulnerable, and WPA2 was introduced, which replaced TKIP with the Advanced Encryption Standard protocol (CCMP-AES).
10. You have been asked by your supervisor in the IT department to test some newly installed cable runs. She hands you the tool shown in the following figure. What is the function of the tool and how do you use it?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c06uf001_0.jpg" alt="" height="801" width="834"><figcaption></figcaption></figure>

    1. When you place the tool at one end of a wire, it generates a tone that can be detected at the other end.
    2. When you touch the end of the tool to a copper cable, you can detect and measure the electrical current flowing through it.
    3. When you connect the tool to the end of a fiber-optic cable, you can measure the length of the cable run.
    4. When you attach the tool to the end of a twisted-pair cable, it tests for crosstalk and other performance characteristics.

    Answer:

    A. The device shown in the figure is a tone generator and locator, which you can use to test twisted-pair wiring and detect certain basic wiring faults. By connecting the tone generator to each wire in turn and locating the tone at the other end, you can determine whether each wire is attached to the appropriate pin in the connector. This tool is not capable of performing any of the tasks described in the other options.
11. A multifactor authentication system consists of at least two different identifying criteria, typically falling into two of the following categories: something you have, something you do, something you know, and something you are. Which of the following authentication factors is an example of something you have?

    1. A password
    2. A fingerprint
    3. A smartcard
    4. A finger gesture

    Answer:

    C. The term _something you have_ refers to a physical possession that identifies a user, such as a smartcard. This type of authentication is nearly always used as part of a multifactor authentication procedure because it is possible for a smartcard or other physical possession to be lost or stolen. A fingerprint would be considered something you are, a password is something you know, and a finger gesture is something you do.
12. Which of the following are port numbers used for Structured Query Language (SQL) communications? (Choose all that apply.)

    1. 1433
    2. 3389
    3. 1521
    4. 3306

    Answer:

    A, C, D. Port number 1433 is used by SQL Server; port 1521 is used by SQLnet, and port 3306 is used by MySQL. The port number 3389 is used by the Remote Desktop Protocol (RDP) and is not involved in SQL communications.
13. At a garage sale, you purchase some 802.11a wireless network adapter cards for desktop computers at a very low price. Your plan is to use them to expand your 802.11g home network. After installing one of the adapters in a computer, you attempt to connect to the network, but you cannot see the Service Set Identifier (SSID) in the list of available networks. You try installing a different adapter, thinking the first one might be broken, but the second one does not work either. What can you do to resolve the problem and connect the computer to your network?

    1. Configure the access point to use the 5 GHz frequency.
    2. Move the computer closer to the access point.
    3. Manually enter the SSID in the computer's wireless network client software.
    4. Nothing. 802.11a equipment cannot connect to an 802.11g network.

    Answer:

    D. Wireless Local Area Network (WLAN) equipment built to the 802.11a standard can only use the 5 GHz frequency band. However, an 802.11g access point can only use the 2.4 GHz frequency band. Therefore, the network adapters cannot be made to connect to your access point by any means.
14. Parity is a fault tolerance technique used by disk storage arrays in which an additional parity bit is stored for a specified number of data bits. By using the parity information, the storage subsystem can calculate the values of bits that have been lost due to a disk failure, enabling the system to re-create the lost data. Redundant Array of Independent Disks (RAID) is a type of storage array that sometimes uses parity to provide fault tolerance. Which of the following RAID levels provide fault tolerance by using parity data? (Choose all that apply.)

    1. RAID 0
    2. RAID 1
    3. RAID 5
    4. RAID 6
    5. RAID 10

    Answer:

    C, D. RAID is a technology for storing data on multiple hard disk drives, providing fault tolerance, increased performance, or both. The various RAID levels provide different levels of functionality and have different hardware requirements. RAID 5 and RAID 6 both combine disk striping with distributed storage of parity information. RAID 5 enables recovery from a single disk failure. RAID 6 uses redundant parity to enable recovery from a double disk failure. RAID 1 and RAID 10 both use disk mirroring to provide fault tolerance, which does not require parity data. RAID 0 uses data striping only (blocks written to each disk in turn), which does not provide any form of fault tolerance.
15. You are setting up an 802.11n wireless network using the 2.4 GHz frequency band. You plan to install three Wireless Access Points (WAPs). Which of the following channels should you use for your access points to avoid channel overlap that can result in interference? (Choose all that apply.)

    1. 1
    2. 4
    3. 6
    4. 8
    5. 11

    Answer:

    A, C, E. The 2.4 GHz band used by Wireless Local Area Networks (WLANs) consists of channels that are 20 (or 22) MHz wide. However, the channels are only 5 MHz apart, so it is possible for channel overlap to occur between the access points, which can result in interference. Channels 1, 6, and 11 are the only channels that are far enough apart from each other to avoid any overlap with the adjacent channels. Channels 4 and 8 are susceptible to overlap.
16. Your supervisor has asked you to increase the security of the servers on your network. Which of the following procedures can be considered to be server hardening techniques? (Choose all that apply.)

    1. Upgrading server firmware
    2. Disabling unnecessary services
    3. Creating privileged user accounts
    4. Disabling unused TCP and UDP ports

    Answer:

    B, C, D. Disabling services and ports that are not in use is a server hardening technique that reduces the attack surface of a server. Creating privileged user accounts that are only used for tasks that require those privileges reduces the chance that the administrative accounts will be compromised. These, therefore, are all forms of server hardening. Upgrading the UEFI or BIOS firmware on a server typically does not enhance its security, so it cannot be considered a form of server hardening.
17. You are working the IT help desk when a user calls to report that he cannot access the Internet, although he is able to connect to computers on the local network. At the user's workstation, you run the `ipconfig /all` command and examine the output. Which of the options is the most likely explanation for the user's problem, based on the following `ipconfig` results?

    `Windows IP Configuration Host Name . . . . . . . . . . . . : Client12 Primary Dns Suffix . . . . . . . : Node Type . . . . . . . . . . . . : Hybrid IP Routing Enabled. . . . . . . . : No WINS Proxy Enabled. . . . . . . . : No Ethernet adapter Local Area Connection: Connection-specific DNS Suffix . : Description . . . . . . . . . . . : PCIe Family Controller Physical Address. . . . . . . . . : 60-EB-69-93-5E-E5 DHCP Enabled. . . . . . . . . . . : No Autoconfiguration Enabled . . . . : Yes Link-local IPv6 Address . . . . . : fe80::c955:c944:acdd:3fcb%2 IPv4 Address. . . . . . . . . . . : 192.168.23.234 Subnet Mask . . . . . . . . . . . : 255.255.255.0 Lease Obtained. . . . . . . . . . : Monday, October 23, 2017 6:23:47 PM Lease Expires . . . . . . . . . . : Saturday, November 18, 2017 9:49:24 PM Default Gateway . . . . . . . . . : 192.168.216.99 DHCPv6 IAID . . . . . . . . . . . : 241232745 DHCPv6 Client DUID . . . . . . . : 00-01-00-01-18-10-22-0D-60-EB-69-93-5E-E5 DNS Servers . . . . . . . . . . . : 192.168.22.114 NetBIOS over Tcpip. . . . . . . . : Enabled`

    1. DHCP is not enabled.
    2. The Subnet Mask setting is incorrect.
    3. The Default Gateway setting is incorrect.
    4. The DNS Servers setting is located on another network.

    Answer:

    C. The Default Gateway setting should contain the address of a router on the workstation's local network that provides access to other networks, such as the Internet. In this case, therefore, the Default Gateway address should be on the 192.168.23.0 network, but it contains an address on the 192.168.216.0 network, which is not local. Therefore, the user can only access systems on the 192.168.23.0/24 network. The Subnet Mask setting must be correct, or the user would not be able to access any other systems. Unlike the default gateway, the DNS server does not have to be on the workstation's local network, so the address shown can be correct. DHCP does not have to be enabled for the computer to access the Internet.
18. Which of the following are typical examples of the Internet of Things (IoT)? (Choose all that apply.)

    1. A television remote control
    2. A key fob that unlocks your car
    3. A smartphone app for your home thermostat
    4. A remotely monitored cardiac pacemaker
    5. A refrigerator with an internal camera

    Answer:

    C, D, E. A smartphone app that can adjust your thermostat, a remotely monitored cardiac pacemaker, and a camera-equipped refrigerator are all examples of IoT devices because they all have IP addresses and use the Internet to communicate with a controller or monitoring station. Key fobs that unlock cars and TV remote controls are typically short-range radio or infrared devices that do not use the Internet for their communications.
19. When an internal Windows user logs on to an Active Directory domain, which of the following protocols authenticates the user?

    1. Kerberos
    2. WPA2
    3. RADIUS
    4. EAP-TLS

    Answer:

    A. Windows networks that use Active Directory Domain Services (AD DS) authenticate clients using the Kerberos protocol, in part because it never transmits passwords over the network, even in encrypted form. Remote Authentication Dial-In User Service (RADIUS) is an authentication, authorization, and accounting service for remote users connecting to a network. Windows does not use it for internal clients. WiFi Protected Access II (WPA2) is a security protocol used by Wireless Local Area Networks (WLANs). It is not used for AD DS authentication. Extensible Authentication Protocol - Transport Layer Security (EAP-TLS) is a remote authentication protocol that AD DS networks do not use for internal clients.
20. You are installing an ADSL router for your company's new branch office. The router has a switch module containing four Ethernet ports, all of which are assigned to the default VLAN1. When you plug a laptop into one of the Ethernet ports, you can access the Internet with no difficulties. You now need to connect the ADSL router to the company network so that the Wireless Access Points (WAPs) on the network can provide users with Internet access through the ADSL router. However, when you plug the router into a network switch port that is assigned to VLAN4, the switch starts generating “Native VLAN mismatch detected” errors once every minute. Which of the following steps should be part of the solution you implement to stop the error messages from appearing? (Choose all that apply.)

    1. Create a VLAN1 on the network switch.
    2. Configure the network switch port connected to the router to use VLAN1.
    3. Create a VLAN4 on the ADSL router's switch module.
    4. Configure the router port connected to the network switch to use VLAN4.

    Answer:

    C, D. The solution requires you to create a Virtual Local Area Network (VLAN) on the ADSL router that matches the VLAN the network switch port is using. Therefore, you should create a VLAN4 on the router's switch module and assign an Ethernet port to it, which will be the port you use to connect the ADSL router to the network switch. There is no need to create a VLAN1 on the network switch because all switches already have a default VLAN called VLAN1. Modifying the VLAN assignments on the network switch is not a good idea, because it might interfere with the existing VLAN strategy in place.
21. Which of the following steps will not help to prevent war driving attacks from compromising your wireless network? (Choose all that apply.)

    1. Configure your clients and access point to use WEP security.
    2. Configure your clients and access point to use WPA2 security
    3. Configure your access point not to broadcast its SSID.
    4. Configure your access point to use a longer SSID.

    Answer:

    A, D. Changing the length of the Service Set Identifier (SSID) will be no help in preventing a war driving attack. The SSID is just an identifier; its length has no effect on security. Wired Equivalent Privacy (WEP) is a security protocol that has been found to have serious weaknesses that are easily exploitable. It is not a satisfactory way to avoid attacks. On the other hand, configuring the access point not to broadcast its SSID will prevent a war driving attacker with standard equipment from seeing the network. Configuring your equipment to use WiFi Protected Access II (WPA2) security will make it difficult for a war driver who detects your network to connect to it.
22. You have just created a new virtual machine using remote controls provided by a cloud service provider on the Internet. You then install Windows Server on the virtual machine and configure it to function as a web server. Which of the following cloud architectures are you using when you do this? (Choose all that apply.)

    1. IaaS
    2. PaaS
    3. SaaS
    4. Public cloud
    5. Private cloud
    6. Hybrid cloud

    Answer:

    A, D. Infrastructure as a Service (IaaS) provides consumers with processing, storage, and networking resources that they can use to install and run operating systems and other software of their choice. In the public cloud model, one organization functions as the provider, and another organization—in this case, you—consumes the services of the provider. Platform as a Service (PaaS) provides consumers with the ability to install applications of their choice on a server furnished by the provider. Software as a Service (SaaS) provides consumers with access to a specific application running on the provider's servers, but the consumers have no control over the operating system, the servers, or the underlying resources. In a private cloud, the same organization that uses the cloud services is also the sole owner of the infrastructure that provides those services. A hybrid cloud is a combination of public and private infrastructure so that the consumer organization is only a partial owner of the infrastructure.
23. It is your first day working for a consultant that does network cable installations. Your new boss hands you a spool of Category 6 cable, a bag of little clear plastic components, and the tool shown in the following figure. He then tells you to “get started on fives and tens.” What is your new boss expecting you to do?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c06uf002_0.jpg" alt="" height="668" width="834"><figcaption></figcaption></figure>

    1. Pull cable runs
    2. Attach keystone connectors
    3. Install a patch panel
    4. Create patch cables

    Answer:

    D. The plier-like device is a crimper, which cable installers use to attach RJ45 connectors, like those in the bag, to lengths of bulk cable. This is the process of creating patch cables, which are used to connect computers to wall plates and patch panel ports to switches. Your boss is telling you to start making patch cables in five- and ten-foot lengths. You do not use a crimper to attach keystone connectors, and the boss has not given you the tools and components needed to pull cable runs or install a patch panel.
24. Which of the following well-known ports do you use to configure outgoing mail on a POP3 email client?

    1. 110
    2. 25
    3. 143
    4. 80

    Answer:

    B. The default port for the Post Office Protocol 3 (POP3) is 110, but that is used for incoming mail. Outgoing mail uses the Simple Mail Transfer Protocol (SMTP), which uses the well-known port number 25 by default. Port number 143 is the default port for the Internet Message Access Protocol (IMAP), a different email mailbox protocol that clients never use with POP3. Port number 80 is the default port for the Hypertext Transfer Protocol (HTTP), which is not used by email clients.
25. You are a consultant who has been hired to extend a network by a client that is still running thin Ethernet. Which of the following cable types will you have to bring with you to add thin Ethernet network segments?

    1. RG-8
    2. RG-58
    3. RJ45
    4. RJ11

    Answer:

    B. The cable type used for thin Ethernet segments is a coaxial cable called RG-58. RG-8 coaxial is used exclusively on thick Ethernet segments. RJ45 is a type of connector used in twisted pair cabling for data networks. RJ11 is a connector type used in twisted-pair cabling for telecommunications networks.
26. Which of the following types of cable is never used to connect a workstation to an Ethernet network?

    1. Rollover
    2. Straight-through
    3. Crossover
    4. Plenum
    5. Shielded

    Answer:

    A. A rollover cable is a type of null modem cable, usually flat and light blue in color, with the pinouts reversed on either end, to enable a terminal to communicate with a router or switch through the device's dedicated console port. It cannot connect a workstation to the network. A straight-through cable is the standard network cable used to connect a workstation or other device to an Ethernet network. A crossover cable is designed to connect network adapters to each other directly, creating a two-node network. A plenum cable is a type of cable intended for use within air spaces that has an outer sheath that does not produce toxic fumes when it burns. A shielded cable is intended to protect signals from electromagnetic interference. Both plenum and shielded cables can connect a workstation to a network.
27. Which of the following protocols does Internet Protocol Security (IPSec) use to provide data origin authentication by digitally signing packets before transmitting them over the network?

    1. AH
    2. SSL
    3. ESP
    4. RDP

    Answer:

    A. Authentication Header (AH) is a protocol in the TCP/IP suite that provides digital integrity services, in the form of a digital signature, which ensures that an incoming packet actually originated from its stated source. Encapsulating Security Protocol (ESP) provides encryption services for IPSec. Secure Sockets Layer (SSL) is a security protocol that provides encrypted communications between web browsers and servers. Remote Desktop Protocol (RDP) is a component of Remote Desktop Services, a Windows mechanism that enables a client program to connect to a server and control it remotely.
28. You have constructed a network on which all of the computers are connected to a single switch. You then create Virtual Local Area Networks (VLANs) on the switch, corresponding to the company's departments, and add the switch port for each user workstation and department server to the appropriate VLAN. Later, users report that while they can access their departmental servers and the workstations of other users in the same department, they cannot communicate with any of the other departments. What is the problem, and what must you do to correct it?

    1. There is a faulty VLAN configuration on the switch. You must re-create all of the VLANs and configure each VLAN for routing.
    2. VLANs are limited to data link layer communication only. To enable communication between the VLANs, you must install a router or a layer 3 switch on the network and configure it to route traffic between the VLANs.
    3. The VLANs are using different data link layer protocols. You must configure the VLANs to use the same data link layer protocol in order for them to communicate with each other.
    4. One of the VLANs is configured to filter all of the other VLAN traffic for security purposes. You must change the filter on this one VLAN.

    Answer:

    B. VLANs are virtual layer 2 (data link layer) LANs defined within switches. As with physical LANs, only devices in the same VLAN can communicate with each other until a layer 3 device, such as a router or a layer 3 switch, is added to the network. Re-creating and reconfiguring the VLANs will not correct the problem. Traffic filters are usually implemented on routers, not switches. Once a router is in place, VLANs do not have to use the same data link protocol to communicate with each other.
29. The TCP/IP term socket consists of which of the following elements? (Choose all that apply.)

    1. Port number
    2. MAC address
    3. IP address
    4. Subnet mask

    Answer:

    A, C. The term for an IPv4 address and port number in combination, which identifies an application running on a specific host, is _socket_. A Media Access Control (MAC) address is an address hard-coded into a network adapter. It is not a TCP/IP element. A subnet mask is not needed to identify a host or an application running on it.
30. You are installing a cable modem to provide your home network with access to the internet through your cable television provider. The cable modem is a multifunction device that the cable company says provides everything you need for a home network. Which of the following network functions does a home cable modem typically provide? (Choose all that apply.)

    1. DHCP server
    2. Wireless Access Point
    3. Broadband router
    4. Ethernet switch
    5. Proxy server
    6. RADIUS server

    Answer:

    A, B, C, D. A cable modem must function as a broadband router to provide access to the cable provider's network. Many cable modems are also Wireless Access Points (WAPs), enabling users to construct a Local Area Network (LAN) without a cable installation. Many cable modems have switched Ethernet ports for connections to wired devices, such as printers and computers. Most cable modems use Dynamic Host Configuration Protocol (DHCP) to assign IP addresses to devices on the home network. Cable modems for home use typically do not function as proxy servers or Remote Authentication Dial-In User Service (RADIUS) servers, which are devices generally used on large networks.
31. Which of the following Domain Name System (DNS) resource records is not used for forward name resolution?

    1. PTR
    2. CNAME
    3. AAAA
    4. MX

    Answer:

    A. Like A and AAAA records, which are used for forward name resolution, Pointer (PTR) records contain hostnames and IP addresses. However, PTR records are used only for reverse name resolution—that is, resolving IP addresses into hostnames. A Mail Exchange (MX) record specifies the mail server that the domain should use. Canonical Name (CNAME) records specify aliases for a given hostname. An AAAA resource record maps a hostname to an IPv6 address for name resolution purposes. All of these records except PTR are used for forward name resolution.
32. Which of the following are tasks that can be performed by a protocol analyzer that could provide potential intruders with information about the network? (Choose all that apply.)

    1. A protocol analyzer can decrypt protected information in packets captured from the network.
    2. A protocol analyzer can detect open ports on network systems and launch attacks against them.
    3. A protocol analyzer can display the IP addresses of the systems on the network.
    4. A protocol analyzer can display the application data in packets captured from the network.

    Answer:

    C, D. Protocol analyzers capture packets from the network and interpret their contents, which can include displaying the application layer payload. Depending on the application, the payload can conceivably include confidential information, such as passwords. Protocol analyzers also display the IP addresses of the systems involved in packet transmissions. Although this in itself might not be a great security threat, intruders might use the IP address information to launch other types of attacks. Protocol analyzers cannot decrypt the protected information they find in captured packets. Vulnerability scanners detect open ports and launch attacks against them; protocol analyzers do not do this.
33. Which of the following services are provided by a RADIUS server? (Choose all that apply.)

    1. Attenuation
    2. Authentication
    3. Assistance
    4. Authorization
    5. Accounting

    Answer:

    B, D, E. A Remote Authentication Dial-In User Service (RADIUS) server, also known as an AAA server, provides centralized authentication, authorization, and accounting for other network services. Assistance and attenuation are not functions provided by RADIUS or AAA servers.
34. Some users are having a problem connecting to an application server on their local network. You go to their department and start to troubleshoot the problem by testing connectivity using the ping tool at one of the user workstations. You discover that you can ping the server successfully using its computer name, but pinging the computer's fully qualified domain name (FQDN) fails. As a result of these tests, which of the following can you determine is the most likely source of the problem?

    1. EMI
    2. DHCP
    3. DNS
    4. ACL

    Answer:

    C. Only Domain Name System (DNS) servers perform FQDN resolutions, so that is likely to be the source of the problem. It is possible to successfully ping a device on the local network using its computer name without the use of DNS. Dynamic Host Configuration Protocol (DHCP) cannot be the problem, or you would not be able to ping the server at all. Electromagnetic interference (EMI) would inhibit all network communication, and Access Control Lists (ACLs) are an authorization mechanism that has no effect on `ping` tests.
35. You have been given the job of devising a plan to provide a 500-node private internetwork with access to the Internet. The primary objective of the project is to provide all of the network users with access to web and email services while keeping the client computers safe from unauthorized Internet users. There are two secondary objectives for the project: one is to provide a means of monitoring and regulating the users' Internet activities, and the other is to avoid having to manually configure IP addresses on each one of the client computers. You submit a proposal that calls for the use of private IP addresses on the client computers and a series of proxy servers with public, registered IP addresses, which are connected to the Internet. Which of the following statements about your proposed Internet access solution is true?

    1. The proposal satisfies the primary objective and both of the secondary objectives.
    2. The proposal satisfies the primary objective and one of the secondary objectives.
    3. The proposal satisfies the primary objective but neither of the secondary objectives.
    4. The proposal fails to satisfy both the primary and secondary objectives.

    Answer:

    B. Proxy servers provide network users with access to Internet services, and the unregistered IP addresses on the client computers protect them from unauthorized access by users on the Internet, which satisfies the primary objective. The proxy servers also make it possible for network administrators to monitor and regulate users' access to the Internet, which satisfies one of the two secondary objectives. However, proxy servers are not capable of assigning IP addresses to the client computers, and the proposal makes no mention of a Dynamic Host Configuration Protocol (DHCP) server or any another automatic TCP/IP configuration mechanism. Therefore, the proposal does not satisfy the other secondary objective.
36. Which of the following cloud service models provides the consumer with the least amount of control over the cloud resources?

    1. IaaS
    2. PaaS
    3. SaaS
    4. IaaS, PaaS, and SaaS all provide the same degree of control.

    Answer:

    C. Software as a Service (SaaS) provides the least amount of control. Consumers receive access to a specific application running on the provider's servers, but they have no control over the operating system, the servers, or the underlying resources. The Infrastructure as a Service (IaaS) model provides the consumers with the most control, as the provider furnishes processing, storage, and networking resources that the consumer can use as needed. Platform as a Service (PaaS) provides consumers with the ability to install applications of their choice on a server furnished by the provider, but they have only limited control over the server and no control over the underlying resources.
37. The jumbo frame capability is associated with which networking protocol?

    1. Ethernet
    2. Internet Protocol (IP)
    3. Point-to-Point Protocol (PPP)
    4. Transmission Control Protocol (TCP)

    Answer:

    A. Ethernet uses jumbo frames at the data link layer to transfer large amounts of data more efficiently. Ethernet typically restricts frame size to 1,500 bytes, but jumbo frames enable Ethernet systems to create frames up to 9,000 bytes. PPP does not support the use of jumbo frames. Frames are protocol data units associated only with the data link layer, so they do not apply to IP and TCP, which operate at the network and transport layers, respectively.
38. You are working your company's IT help desk, where you are required to follow a specific troubleshooting protocol when handling calls from users. In which of the following troubleshooting steps would you create a trouble ticket?

    1. Establish a theory of probable cause
    2. Verify full system functionality and, if applicable, implement preventive measures
    3. Identify the problem
    4. Test the theory to determine the cause
    5. Document findings, actions, and outcomes
    6. Implement the solution or escalate as necessary
    7. Establish a plan of action to resolve the problem and identify potential effects

    Answer:

    C. The first step in the troubleshooting protocol involves identifying the problem by questioning the user and creating a trouble ticket. You complete the other steps in the troubleshooting protocol after the trouble ticket has been created and prioritized.
39. You are working your company's help desk when a user calls to report that he cannot access any of the data on his computer. He says that a message has appeared on his screen stating that all of his data has been encrypted by the FBI and that it will be decrypted only after he pays $768 in Bitcoin to an unknown address. The user wants to know if he is responsible for making the payment. Which of the following types of attacks has the user experienced?

    1. Denial-of-Service
    2. War driving
    3. Ransomware
    4. ARP poisoning

    Answer:

    C. The user has experienced a ransomware attack. Ransomware is a type of attack in which a user's access to his or her data is blocked unless a certain amount of money is paid to the attacker. The blockages can vary from simple screen locks to data encryption. War driving is an attack method that consists of driving around a neighborhood with a computer scanning for unprotected wireless networks. Denial-of-Service (DoS) is a type of attack that overwhelms a computer with traffic, preventing it from functioning properly. Address Resolution Protocol (ARP) poisoning is the deliberate insertion of fraudulent information into the ARP cache stored on computers and switches.
40. Which of the following Wide Area Network (WAN) services provide unequal amounts of upstream and downstream bandwidth? (Choose all that apply.)

    1. SDSL
    2. CATV
    3. ADSL
    4. FCoE

    Answer:

    B, C. The word _asymmetric_ in Asymmetric Digital Subscriber Line (ADSL) means that the service provides different amounts of bandwidth in each direction. In nearly all cases, asymmetric WAN services provide more downstream bandwidth than upstream. Cable television (CATV) networks are also asymmetrical. The word _symmetric_ in Symmetric Digital Subscriber Line (SDSL) means that the service provides equal amounts of bandwidth in both directions. Fibre Channel over Ethernet (FCoE) is also symmetrical.
41. Network cable runs generally connect office endpoints, such as wall plates, to a central cabling nexus, which is typically where the runs are joined to a backbone network that links them together. Which of the following are terms for such nexuses where network cabling connections are found? (Choose all that apply.)

    1. RDP
    2. IDF
    3. MDF
    4. MTBF

    Answer:

    B, C. A large enterprise network will—at minimum—have demarcation points for telephone services and a connection to an Internet Service Provider's (ISP's) network. In many cases, these services enter the building in the same equipment room that houses the backbone switch, which enables all the devices on the network to access those resources. This room is then called the Main Distribution Frame (MDF). An Intermediate Distribution Frame (IDF) is a place where localized telecommunications equipment, such as the interface between the horizontal cabling and the backbone, is located. For example, an enterprise network housed in a single building might have its MDF in the basement and an IDF on each floor. Mean Time Between Failures (MTBF) and Remote Desktop Protocol (RDP) are not network cabling locations.
42. Your supervisor has asked you to call the cabling contractor your company uses and make an appointment to install some new twisted-pair cable runs. In addition to asking how many cable runs you need pulled, the contractor asks you if you need plenum or PVC. Under which of the following conditions might the local building code require that a data network use plenum cable?

    1. When cable runs exceed the maximum length specified by the physical layer specification
    2. When cables must run through air ducts
    3. When cables run near to devices that generate electromagnetic interference (EMI)
    4. When multiple cables run through the same conduit

    Answer:

    B. A plenum space is an area of a building that provides air circulation as part of its ventilation system, such as a heating or air-conditioning duct. Plenum cables have a sheath made of a fire-retardant material that does not outgas toxic fumes when it burns. When network cables are installed in plenum spaces, many local building codes require that installers use plenum-rated cables conforming to specific standards. Plenum cables provide no benefit when installed near other cables, or EMI sources, or when they exceed specified lengths.
43. Which of the following is not a term for the process of combining the bandwidth of two or more network adapters to increase the overall speed of the connection and provide fault tolerance?

    1. Port aggregation
    2. Link aggregation
    3. Bonding
    4. Clustering
    5. NIC teaming

    Answer:

    D. Clustering refers to the combination of multiple servers—not network adapters—into a single unit to enhance performance and provide fault tolerance. Bonding, link aggregation, port aggregation, and NIC teaming are all terms for the same basic technology, in which the bandwidth of multiple network adapter connections is joined to speed up transmissions. The technology also enables the network communication to continue if one of the adapters fails or is disconnected.
44. You have been asked by the director of the IT department to review the security status of the network device administration procedures currently in use. You know that network device hardening has as one of its first principles the use of secure protocols over insecure ones. Which of the following suggestions are examples of this principle that you should suggest to the director? (Choose all that apply.)

    1. Use WEP instead of WPA2.
    2. Use TKIP instead of AES.
    3. Use HTTPS instead of HTTP.
    4. Use SSH instead of Telnet.

    Answer:

    C, D. Secure Shell (SSH) and Telnet are both remote terminal programs, but Telnet clients pass instructions (including passwords) to the target server in clear text, whereas SSH uses encrypted transmissions. In the same way, Hypertext Transfer Protocol Secure (HTTPS) is the encrypted version of HTTP. In both of these cases, the substitute is more secure and should be suggested to the director. However, Temporal Key Integrity Protocol (TKIP) provides encryption that is less secure than Advanced Encryption Standard (AES), and Wired Equivalent Protocol (WEP) is less secure than WiFi Protected Access II (WPA2).
45. The Simple Network Management Protocol (SNMP) works by processing information gathered from agents installed or embedded in network devices and displaying the information on a central console. Which of the following is the term used for the database in which SNMP agents store information about their properties?

    1. MIB
    2. Trap
    3. Syslog
    4. SIEM

    Answer:

    A. A Management Information Base (MIB) is the database on an SNMP agent in which ASN.1 information about the properties of the managed device is stored. The other three options do not perform this function. A trap is an alert message that SNMP agents send to the network management console when an exceptional event occurs. Syslog is a standard for message logging components. Security Information and Event Management (SIEM) is a combination tool that uses information gathered from logs and network devices to provide a real-time analysis of the network's security condition.
46. When a web browser connects to a web server using an address with the `https://` prefix, the connection is secured using Transmission Control Protocol (TCP) and an encryption protocol. Which of the following are protocols that are typically used to secure communication between web servers and web browsers? (Choose all that apply.)

    1. TLS
    2. SSH
    3. DTLS
    4. SSL

    Answer:

    A, D. Secure Sockets Layer (SSL) is a now-deprecated security protocol that provides encrypted communications between web browsers and servers. Transport Layer Security (TLS) is an updated security protocol that is designed to replace SSL. Datagram Transport Layer Security (DTLS) is a security protocol that provides the same basic functions as TLS but for User Datagram Protocol (UDP) traffic instead of TCP. Secure Shell (SSH) is a character-based tool that enables users to execute commands on remote computers; it does not provide web server/browser security.
47. A screened subnet is a segment that is exposed to the Internet and separated from the internal network by a firewall. Administrators typically use a screened subnet for servers that must be accessible by outside users, such as web and email servers. Which of the following is another term for a screened subnet?

    1. PEAP
    2. DMZ
    3. VLAN
    4. TKIP

    Answer:

    B. Another term for a screened subnet is a DMZ, or demilitarized zone. They are also known as perimeter networks. A Virtual Local Area Network (VLAN) is a logical network segment created within a switch. Protected Extensible Authentication Protocol (PEAP) is an authentication protocol, and Temporal Key Integrity Protocol (TKIP) is an encryption algorithm. These three options are not terms for a screened subnet.
48. Which of the following types of traffic is not exchanged by Remote Desktop clients and servers using the Remote Desktop Protocol (RDP)?

    1. Keystrokes
    2. Mouse movements
    3. Display information
    4. Application data

    Answer:

    D. RDP is a component of Remote Desktop Services, a Windows mechanism that enables a client program to connect to a server and control it remotely. RDP does not carry actual application data; it just transfers keystrokes, mouse movements, and graphic display information.
49. You have been engaged to design a Wireless Local Area Network (WLAN) for a site you have never seen. For that reason, you want the WLAN to be able to support both the 2.4 GHz and 5 GHz frequencies. Which of the following IEEE 802.11 WLAN standards should you look for when you are shopping for equipment that supports both frequencies? (Choose all that apply.)

    1. 802.11a
    2. 802.11b
    3. 802.11g
    4. 802.11n
    5. 802.11ac
    6. 802.11ax

    Answer:

    D, F. Of the options shown, only the 802.11n and 802.11ax standards define WLAN devices that can support both the 2.4 GHz and 5 GHz frequencies. The 802.11a and 802.11ac standards support only 5 GHz, and the 802.11b and 802.11g standards support only 2.4 GHz.
50. Which of the following statements about multitenancy in a public cloud datacenter is not true?

    1. Multitenancy presents a potential security risk because other tenants are utilizing the same hardware.
    2. Multitenancy separates tenants by assigning each one its own virtual machine.
    3. Multitenancy reduces the cost of utilities and other overhead.
    4. Multitenancy introduces the possibility of competition for bandwidth with other tenants.

    Answer:

    B. Multitenancy does not call for tenants to have individual virtual machines. Multitenancy is a software architecture in which multiple tenants share a single instance of an application running in the cloud. Because tenants share a single application, there is a chance that data could be compromised. Because a single application instance is running in the cloud, the operational overhead is reduced compared to the use of individual virtual machines. Tenants share a finite amount of bandwidth, so the possibility exists for competition to occur, such as when one tenant is the target of a Denial-of-Service (DoS) attack.
51. You have been asked to evaluate the security provided by the cryptographic algorithms in use on your network. Which of the following are not cryptographic algorithms used for file hashing? (Choose all that apply.)

    1. RC4
    2. MD5
    3. AES
    4. SHA

    Answer:

    A, C. Secure Hash Algorithm (SHA) and Message Digest 5 (MD5) are file hashing algorithms used to test data integrity by calculating a hash value before transmitting a file over the network. After the transmission, the receiving system performs the same calculation. If the values match, then the data is intact. RC4 and Advanced Encryption Standard (AES) are both cryptographic algorithms, but they are not used for file hashing.
52. When starting her new position as a network administrator, Alice was given two user accounts. One account is intended for standard user activities, and another has the additional permissions needed for Alice to perform administrative tasks. This is an example of which of the following security concepts?

    1. Zero day
    2. Least privilege
    3. Defense in depth
    4. Multifactor authentication

    Answer:

    B. Least privilege is the practice of only providing users with the permissions they need to perform their designated tasks and no more. For her standard activities, Alice is given an account that does not have administrative permissions because she does not need those permissions to perform standard tasks. The administrative account has the additional permissions needed for Alice to perform administrative tasks. The intention is for Alice to use that account only for those administrative tasks. Zero day is a type of vulnerability; multifactor authentication calls for users to supply two identifying factors; defense in depth refers to the use of multiple security mechanisms to provide additional protection. None of these other three options refers to the use of multiple user accounts.
53. You are in the process of troubleshooting a user's computer that is malfunctioning. Which step of the troubleshooting model involves replacing computer components until you have identified a faulty hardware device?

    1. Establish a plan of action to resolve the problem
    2. Duplicate the problem
    3. Gather information
    4. Verify full system functionality
    5. Test the theory to determine the cause
    6. Document findings, actions, and outcomes
    7. Establish a theory of probable cause

    Answer:

    E. After you have established a theory of probable cause, you can try to test the theory by replacing hardware components one by one until you find the faulty device. All of the other options are steps that come either earlier or later in the troubleshooting process.
54. An insider threat is most likely to be detectable by which of the following types of physical security?

    1. Motion detection
    2. Smartcards
    3. Biometrics
    4. Video surveillance

    Answer:

    D. An insider threat by definition originates with an authorized user. Therefore, smartcards, motion detection, and biometrics will only detect the presence of someone who is authorized to enter sensitive areas. Video surveillance, however, can track the activities of anyone, authorized or not.
55. Which of the following network interface occurrences is considered to be a malfunction on a full-duplex Ethernet network but is not a malfunction on a half-duplex Ethernet network?

    1. Runts
    2. Late collisions
    3. Giants
    4. Collisions

    Answer:

    D. All of these occurrences are malfunctions on a full-duplex Ethernet network, but collisions are normal and expected on a half-duplex network. Runt frames occur when a network interface generates packets that are smaller than the 64-byte minimum allowable length. Giants occur when frames are larger than the 1518-byte maximum allowable length. Late collisions occur when network cables are too long, and frames collide after leaving the sending system.
56. A protocol analyzer is a tool that captures packets from a network and examines their contents. Which of the following Unix/Linux tools is a protocol analyzer?

    1. `nmap`
    2. `tcpdump`
    3. `pathping`
    4. `iptables`

    Answer:

    B. The Unix/Linux `tcpdump` utility is a protocol analyzer. It is a command-line tool that captures network packets and displays their contents. The `iptables`, `nmap`, and `pathping` utilities cannot capture and analyze packets. `iptables` manages Unix/Linux kernel firewall rules, `nmap` is a port scanner, and `pathping` is a Windows route tracing tool.
57. A Storage Area Network (SAN) typically takes the form of a dedicated network used to provide servers with access to hard disk arrays and other storage devices. Which of the following statements about the differences between a SAN and Network Attached Storage (NAS) are true? (Choose all that apply.)

    1. NAS devices typically provide a filesystem, while SAN devices do not.
    2. NAS provides file-level storage access, whereas a SAN provides block-level storage access.
    3. NAS devices typically contain integrated iSCSI targets.
    4. SAN devices have an operating system, whereas NAS devices do not.

    Answer:

    A, B. NAS devices are self-contained file servers that connect directly to a standard IP network. A NAS device provides file-level access to its storage devices, and it includes an operating system and a filesystem. NAS devices are typically not iSCSI targets. SANs provide block-level storage and typically function as iSCSI targets, but they do not include an operating system or filesystem.
58. Your supervisor has just informed you that the CIO has hired an outside consultant to perform penetration testing on the company network. Which of the following best describes what you can expect the consultant to do?

    1. Evaluate the security conditions on the network
    2. Create computers or networks that are alluring targets for intruders
    3. Attempt to compromise the network's security measures
    4. Implement a new companywide security protocol

    Answer:

    C. Penetration testing is a type of network security evaluation in which a client engages an outside consultant who attempts to penetrate the network's security and gain unauthorized access to protected network resources. Testing by an internal administrator familiar with the security barriers would not be a valid test. Although having a consultant examine the network's security from within can be useful, it is not a penetration test. Computers or networks that are alluring targets for intruders are called honeypots or honeynets. Implementation of a new security protocol can only come after the current security situation has been evaluated.
59. Your company is a contractor for the government that regularly works with highly sensitive defense data. To prevent this data from being compromised, the company's datacenter has various special security measures installed. All of the servers have crimped metal tags holding the cases closed. All of the hardware racks are locked in clear-fronted cabinets. All of the cable runs are installed in transparent conduits. These are all examples of which of the following types of physical security measure?

    1. Geofencing
    2. Port security
    3. Tamper detection
    4. Asset tracking

    Answer:

    C. All of the mechanisms listed are designed to make any attempts to tamper with or physically compromise the hardware devices immediately evident. These mechanisms are therefore various forms of tamper detection. Asset tracking is for locating and identifying hardware. Geofencing is a wireless networking technique for limiting access to a network. Port security refers to network switch ports. These options do not apply to the specified mechanisms.
60. Wavelength division multiplexing is a technique for carrying multiple fiber-optic signals on a single network medium. There are several types of this multiplexing technique, including Coarse Wavelength Division Multiplexing (CWDM), Dense Wavelength Division Multiplexing (DWDM), and Bidirectional Wavelength Division Multiplexing (BWDM, or just WDM). Which of the following is one of the ways in which these types of multiplexing differ?

    1. They carry different numbers of channels on a single medium.
    2. They use different wavelength spacings.
    3. They provide different amounts of signal amplification.
    4. They use different forms of amplitude modulation.

    Answer:

    B. The various types of wavelength division multiplexing use different spacing of the wavelengths they carry, which enables them to fit different numbers of channels on a single medium. WDM (or BWDM) carries two wavelengths for bidirectional communication. CWDM can carry up to 16 channels, and DWDM can carry 40 or 80 (depending on the spacing used). Various amplification technologies (including EFDA and Raman) can expand the amounts of usable wavelength in each type.
61. Which of the following protocols use tunneling to establish secured links between TCP/IP systems? (Choose all that apply.)

    1. L2TP
    2. IPSec
    3. MGRE
    4. NAT

    Answer:

    A, B, C. Layer 2 Tunneling Protocol (L2TP), Internet Protocol Security (IPSec), and Multipoint Generic Routing Encapsulation (MGRE) are all protocols that encapsulate packets in an encrypted form within another protocol to secure their contents. Network Address Translation (NAT) enables workstations on private networks to access the Internet by substituting a public IP address in packets generated with private addresses. NAT does not use tunneling.
62. Your supervisor has given you a Class C network IP address and has asked you to create a network with 8 subnets and 30 hosts per subnet. Which of the following subnet masks will you have to use?

    1. 255.255.255.128
    2. 255.255.255.192
    3. 255.255.255.224
    4. 255.255.255.240
    5. 255.255.255.248
    6. 255.255.255.252

    Answer:

    C. To create a network with 8 subnets and 30 hosts per subnet, you must allocate 3 of the 8 bits in the last octet for use as a subnet identifier. This results in a binary value of 11100000 for the last octet in the subnet mask, which converts to a decimal value of 224. Therefore, the correct subnet mask value is 255.255.255.224. Values for the last octet that are lower than 224 would not enable you to create 8 subnets. Values higher than 224 would not enable you to create 30 host addresses.
63. You are a consultant working at a client site. The client has supplied you with the Service Set Identifier (SSID) and the passphrase for the company's wireless network so that you can connect to it with your laptop. However, you are unable to establish a connection. Which of the following security measures might be preventing you from connecting your laptop to the network?

    1. Geofencing
    2. MAC filtering
    3. Using WPA2
    4. Disabling SSID broadcasts

    Answer:

    B. Media Access Control (MAC) filtering takes the form of an Access Control List (ACL) on the wireless network's access points, listing the MAC addresses of all the devices that are permitted to access the network. If the MAC address of your laptop is not included in the ACL, you will be unable to connect to the network. Geofencing is intended to prevent users outside the office from accessing the network. You are inside, so this should not be the problem. You have been given the passphrase for the network, so you should be able to configure the WiFi Protected Access II (WPA2) protocol on your laptop. You have been given the SSID of the network, so you should be able to connect by manually entering it, even if the access points are not broadcasting the SSID.
64. You have just finished installing a new Category 5e cable run for the first time. After attaching keystone connectors to both ends of the cable, you mount the office-side connector to a wall plate and mount the datacenter connector into a patch panel. Then you take a patch cable and connect the patch panel port to an open port in one of the network switches. However, the link pulse LED on the switch port does not light as it is supposed to. What should you do next?

    1. Repull the cable run using Category 6 cable.
    2. Check the cable run for wiring faults.
    3. Make sure the switch port is not disabled.
    4. Plug a computer into the wall plate.

    Answer:

    D. For the link pulse LED on the switch port to light up, there must be an active connection between the switch and a functioning network device at the other end. Plugging a running computer into the wall plate will enable the Ethernet adapters at both ends of the connection to communicate, causing the LED to light. None of the other options will cause the LED to light.
65. Devices on a TCP/IP network typically use the Address Resolution Protocol (ARP) to locate specific destinations on the local network by resolving IP addresses into Media Access Control (MAC) addresses (also known as hardware addresses). At which layer of the Open Systems Interconnection (OSI) model do these MAC addresses operate?

    1. Physical
    2. Data link
    3. Network
    4. Transport

    Answer:

    B. The Ethernet (or IEEE 802.3) protocol at the data link layer uses MAC addresses to identify computers on the local network. MAC addresses are coded into the firmware of physical network interface adapters by the manufacturer. The physical layer deals with signals and is not involved in addressing. The IP at the network layer has its own addressing system. The transport layer protocols are not involved in addressing.
66. Many network diagrams use Cisco symbols to illustrate the locations of and relationships between network components. Cisco symbols are standardized pictographs that illustrate the basic function of a network component. In a network diagram that uses Cisco symbols, what component does the symbol in the figure represent?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c06uf003.jpg" alt="" height="222" width="224"><figcaption></figcaption></figure>

    1. A hub
    2. A switch
    3. A router
    4. A gateway

    Answer:

    C. The Cisco symbol shown in the figure is used in network diagrams to represent a router, as symbolized by the arrows pointing both in and out. This symbol is not used to represent a hub, a switch, or a gateway.
67. Address Resolution Protocol (ARP) poisoning is the deliberate insertion of fraudulent information into the ARP cache stored on computers and switches. Which of the following types of attack can be facilitated by ARP poisoning? (Choose all that apply.)

    1. Social engineering
    2. Man in the middle
    3. Evil twin
    4. Session hijacking

    Answer:

    B, D. By inserting modified entries into a device's ARP cache, an attacker can cause traffic to be diverted from the correct destination to a system controlled by the attacker. This can enable the attacker to intercept traffic intended for another destination. In a man-in-the-middle attack, the attacker can read the intercepted traffic and even modify it before sending it on to the correct destination. In a session hijacking attack, the attacker can use the intercepted traffic to obtain authentication information, including passwords. Neither of the other two options is facilitated by ARP poisoning. An evil twin is a fraudulent access point on a wireless network. Social engineering is a form of attack in which an innocent user is persuaded by an attacker to provide sensitive information via email or telephone.
68. Recently, your network has been the target of numerous attack attempts. To gather information about the attackers, you have created a server that is designed to function as an enticing target but that does not provide access to any legitimately sensitive services or information. Which of the following is the term used to describe this technique?

    1. Spoofing
    2. DMZ
    3. Root guard
    4. Honeypot

    Answer:

    D. A honeypot is a computer configured to function as bait for attackers, causing them to waste their time penetrating a resource that provides no significant access. This is also a technique that enables the target to gather information about the attackers. A demilitarized zone (DMZ), also known as a screened subnet or perimeter network, is a network segment on which administrators locate servers that must be accessible from the Internet but that are separated from the internal network by a firewall. A root guard provides protection to switch ports. Spoofing is an attack technique in which an intruder modifies packets to assume the appearance of another user or computer.
69. You are a consultant working on a new client's network. The network has been in place for decades, and you have been given a diagram supplied by the original installer. The diagram says that the network computers are connected to a device called a multiport repeater. Which of the following devices can also be described as a multiport repeater?

    1. Hub
    2. Bridge
    3. Switch
    4. Router

    Answer:

    A. A repeater is a physical layer device that regenerates incoming signals and retransmits them. A hub is a type of repeater that receives data through any one of its multiple ports and retransmits the data out through all of its other ports. Bridges and switches are data link layer devices, and routers are network layer devices. None of these three can be described as a multiport repeater.
70. When you run a port scanner on a server, which of the following is the result?

    1. A list of the servers currently running user processes
    2. A list of the computer's hardware ports that are currently in use
    3. A list specifying the numbers of packets transmitted and received by each network adapter on the system
    4. A list of open ports through which the system can be accessed
    5. A list of the IP addresses used by all the devices on the local network

    Answer:

    D. A port scanner examines a system for open ports or endpoints that are accessible from the network using the TCP or UDP protocol, which intruders can conceivably exploit to gain access to the system. Port scanners do not list user processes, hardware ports, numbers of packets, or IP addresses.
71. Your company has a seven-node failover cluster hosting databases on SQL Server. Each server has three network interface adapters installed in it. Two are standard Gigabit Ethernet adapters that provide the nodes with access to each other and clients with access to the cluster. One is a Fibre Channel adapter that provides the cluster nodes with access to a dedicated network that also hosts a large hard disk array. Which of the following terms describe the networks to which the cluster nodes are connected? (Choose all that apply.)

    1. SAN
    2. PAN
    3. WAN
    4. MAN
    5. LAN

    Answer:

    A, E. A Storage Area Network (SAN) is a network that is dedicated to carrying traffic between servers and storage devices. SANs can use specialized network protocols, such as Fibre Channel in this case, or standard Gigabit Ethernet. A Local Area Network (LAN) is a connected group of computers, usually inside a single room or building. In this case, the cluster has one LAN connecting the nodes together and another providing other users with access to the cluster. A Personal Area Network (PAN) provides communication among devices associated with a single person, such as smartphones. A Wide Area Network (WAN) is a network that connects devices or networks at different geographic locations. A Metropolitan Area Network (MAN) is a type of WAN that connects devices within a limited geographic area. The cluster is not connected to a PAN, WAN, or MAN.
72. A Windows user calls you at the help desk and reports that he cannot connect to any hosts on either the local network or a remote network. This is the only report of its kind you have received today. You question the user about the problem and eventually learn that he has made some changes to his workstation's Internet Protocol (IP) settings. What should you do next?

    1. Check the switches in the datacenter to see if they have logged any error messages.
    2. Verify that the routers on the network are functioning.
    3. Run the `ipconfig` command on the user's workstation to view its configuration.
    4. Check the network's Domain Name System (DNS) server to see if it is resolving IP hostnames.

    Answer:

    C. Since only one user is reporting the problem and he has admitted to making changes to his IP configuration, you should start by checking the workstation configuration using the `ipconfig` command. If the routers, the switches, or the DNS server were causing the problem, more than one user would be affected, and there would be additional users calling the help desk.
73. You are a network administrator attempting to use your workstation on the internal network to remotely control a web server called WebServ1 on the perimeter network. However, the remote desktop client software is unable to establish a connection to the server. You can see all the computers on your local network and on the perimeter network. You try using the `ping` utility to test the TCP/IP functionality of WebServ1, and the `ping` test is successful. You then call your colleague on the same internal network and have her try to connect to WebServ1 using the same remote access tool. She connects to WebServ1 successfully. Which of the following could be the cause of the problem you are experiencing?

    1. Blocked TCP/UDP ports on the web server
    2. Name resolution failure
    3. Incorrect firewall settings on your workstation
    4. Unresponsive service on the web server

    Answer:

    C. Because your colleague can connect to WebServ1 successfully, the problem is not an unresponsive service or blocked ports on the server. The problem is not a name resolution failure, because you can successfully ping WebServ1 by name. Therefore, of the options listed, the only possible problem must be that the firewall on your workstation is configured to block the remote desktop client's traffic.
74. The toolkit you were given when you began work for an IT consulting company contained the tool shown in the following figure. What is the function of this tool?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c06uf004_0.jpg" alt="" height="330" width="834"><figcaption></figcaption></figure>

    1. When you touch the end of the tool to a copper cable, you can detect and measure the electrical current flowing through it.
    2. When you place the tool at one end of a wire, it generates a tone that can be detected at the other end.
    3. To connect a bulk cable to a keystone connector, you use the tool to punch each wire down into the correct receptacle on the connector.
    4. When you connect the tool to the end of a fiber-optic cable, you can measure the length of the cable run.

    Answer:

    C. The device shown in the figure is a punchdown tool, which you use to connect unshielded twisted-pair cable ends to the keystone connectors used in modular wall plates and patch panels. After lining up the individual wires in the cable with the connector, you use the tool to press each wire into its slot. The tool also cuts the wire sheath to make an electrical contact and trims the end of the wire. This tool is not capable of performing any of the tasks described in the other options.
75. You are designing a new wireless network based on the IEEE 802.11n standard. The equipment you have selected supports both the 2.4 GHz and 5 GHz frequencies, and you are undecided about which one to use. Which of the following are possible reasons why the 5 GHz frequency tends to perform better than the 2.4 GHz frequency on a Wireless Local Area Network (WLAN)? (Choose all.)

    1. The 5 GHz frequency has more channels than the 2.4 GHz frequency.
    2. The 5 GHz frequency conflicts with fewer common household devices than the 2.4 GHz frequency.
    3. The 5 GHz frequency transmits at faster speeds than the 2.4 GHz frequency.
    4. The 5 GHz frequency supports longer ranges than the 2.4 GHz frequency.

    Answer:

    A, B, C. The 5 GHz frequency has 23 channels available in the United States, whereas the 2.4 GHz frequency has only 11. Many household devices, such as cordless telephones, use the 2.4 GHz frequency band, but relatively few devices use the 5 GHz band. Higher frequencies typically support faster transmission speeds, because with all other conditions equal, they can carry more data in the same amount of time. The 5 GHz frequency typically has a shorter range than 2.4 GHz, because it is less able to penetrate barriers.
76. What is the name of the tool shown in the following figure?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c06uf005_0.jpg" alt="" height="654" width="666"><figcaption></figcaption></figure>

    1. Crimper
    2. Tone generator and locator
    3. Butt set
    4. Punchdown tool

    Answer:

    C. The device shown in the figure is a butt set, a basic tool of telephone installers and line workers. By connecting the clips to pins in a punchdown block, you can access telephone circuits in order to test them or place telephone calls. The device shown is not a crimper, a tone generator and locator, or a punchdown tool.
77. Which of the following server applications uses two well-known port numbers, one for control traffic and one for data traffic?

    1. FTP
    2. SNMP
    3. NTP
    4. HTTP

    Answer:

    A. The File Transfer Protocol (FTP) uses two port numbers. It uses the first, port 21, for a control connection that remains open during the entire client-server session. The second port, 20, is for a data connection that opens only when the protocol is actually transferring a file between the client and the server. Network Time Protocol (NTP), Simple Network Management Protocol (SNMP), and Hypertext Transfer Protocol (HTTP) all use a single port on the server.
78. You are configuring the computers on a new network, and you have been given the network address 10.26.0.0/13. Which of the following subnet mask values must you use when configuring the computers?

    1. 255.248.0.0
    2. 255.252.0.0
    3. 255.254.0.0
    4. 255.255.248.0
    5. 255.255.252.0
    6. 255.255.254.0

    Answer:

    A. The 13-bit prefix indicated in the network address will result in a mask with 13 ones followed by 19 zeroes. Broken into 8-bit blocks, the binary mask value is as follows:

    11111111 11111000 00000000 00000000

    Converted into decimal values, this results in a subnet mask value of 255.248.0.0.
79. You are testing a twisted-pair cable run using a tone generator and locator. When you apply the tone generator to each of the first seven wires at one end of the cable, you successfully detect a tone on the corresponding pin at the other end. However, when you connect the tone generator to the eighth wire, you fail to detect a tone at the other end. Which of the following fault types have you discovered?

    1. Short circuit
    2. Open circuit
    3. Split pair
    4. Crosstalk

    Answer:

    B. The failure to detect a tone on the eighth wire indicates that there is either a break in the wire somewhere inside the cable or a bad pin connection in one or both connectors. This type of fault is called an open circuit. None of the other three options are faults that manifest as described. A short circuit is when a wire is connected to two or more pins at one end of the cable. A split pair is a connection in which two wires are incorrectly mapped in exactly the same way on both ends of the cable. Crosstalk is a type of interference caused by signals on one wire bleeding over to other wires.
80. Which of the following functions are defined as occurring at the session layer of the Open Systems Interconnection (OSI) model? (Choose all that apply.)

    1. Data encryption
    2. Dialog control
    3. Datagram routing
    4. Dialog separation

    Answer:

    B, D. The session layer is responsible for creating and maintaining a dialog between end systems. This dialog can be a two-way alternate dialog that requires end systems to take turns transmitting, or it can be a two-way simultaneous dialog in which either end system can transmit at will. The session layer functions are called dialog control and dialog separation. Data encryption is performed at the presentation layer, and datagram routing occurs at the network layer.
81. You are working your company's IT help desk, and you have had several calls from users who are reporting problems with their Voice over Internet Protocol (VoIP) and streaming video connections. In each case, the audio or video connection experiences frequent dropouts in sound or video, causing frustrating interruptions. Which of the following terms describes a connectivity problem on a wired network that could cause these symptoms?

    1. Jitter
    2. Latency
    3. Bottleneck
    4. Attenuation

    Answer:

    A. When individual packets in a data stream are delayed, due to network congestion, different routing, or queuing problems, the resulting connectivity problem is called jitter. While this condition might not cause problems for asynchronous applications, real-time communications, such as VoIP or streaming video, can suffer interruptions from which the phenomenon gets its name. Latency describes a generalized delay in network transmissions, not individual packet delays. Attenuation is the weakening of a signal as it travels through a network medium. A bottleneck is a condition in which all traffic is delayed, due to a faulty or inadequate component. None of these three options would account for the problems reported by the users.
82. You are a consultant with a client who wants to have you install a wireless network with the highest throughput currently available. What can you tell your client is the fastest speed achievable by a Wireless Local Area Network (WLAN) using the currently ratified IEEE 802.11 standards?

    1. 54 Mbps
    2. 600 Mbps
    3. 1.3 Gbps
    4. 2.6 Gbps

    Answer:

    C. The 802.11ac standard defines a wireless LAN running at speeds of up to 1.3 gigabits per second (Gbps). None of the other 802.11 standards define networks running at speeds beyond 600 Mbps. There is no currently ratified IEEE 802.11 standard that enables speeds of 2.6 Gbps.
83. A private network uses unregistered IP addresses that are not accessible from the Internet. For computers on the private network to access Internet servers, there must be a device that substitutes registered IP addresses for the unregistered ones. Which of the following devices are capable of performing this kind of IP address substitution? (Choose all that apply.)

    1. RADIUS server
    2. NAT router
    3. UTM appliance
    4. Proxy server

    Answer:

    B, D. Network Address Translation (NAT) is a network layer service, typically integrated into a router, that converts the private IP addresses in all of a client's Internet transmissions to a registered IP address. NAT therefore works for all applications. A proxy server is an application layer device that performs the same type of conversion but only for specific applications. A Remote Authentication Dial-In User Service (RADIUS) server can provide authentication, authorization, and accounting services for remote access servers, but it does not convert IP addresses. A unified threat management (UTM) appliance typically performs Virtual Private Network (VPN), firewall, and antivirus functions. It too does not convert IP addresses.
84. A user calls you at the technical support desk in the computer store where you work. He is installing a home network and is having trouble configuring the IP addresses for his computers. He starts reading off a list of the network addresses he has tried to use. Which of the following are valid IPv4 network addresses that the user can conceivably use to configure his computers? (Choose all that apply.)

    1. 1.1.1.0
    2. 9.34.0.0
    3. 103.256.77.0
    4. 229.6.87.0

    Answer:

    A, B. 1.1.1.0 and 9.34.0.0 are both valid IPv4 network addresses. IPv4 addresses with first byte values from 224 to 239 are Class D addresses, which are reserved for use as multicast addresses. Therefore, the user cannot use 229.6.87.0 for his network. 103.256.77.0 is an invalid address because the value 256 cannot be represented by an 8-bit binary value.
85. Which of the following terms refers to a routing protocol that relies on hop counts to measure the efficiency of routes through an internetwork?

    1. Link state protocol
    2. Distance vector protocol
    3. Edge gateway protocol
    4. Interior gateway protocol

    Answer:

    B. Distance vector protocols rely on hop counts—that is, the number of routers between a source and a destination—to evaluate the efficiency of routes. Link state protocols use a different type of calculation, usually based on Dijkstra's algorithm. The terms _interior gateway protocol_ and _edge gateway protocol_ do not refer to the method of calculating routing efficiency.
86. You have been hired by a client to connect two local area networks together, which are in different buildings 500 meters apart. The cable type you use must support Gigabit Ethernet data rates of 1000 megabits per second (Mbps) and provide a high level of resistance to electromagnetic interference (EMI). Which of the following cable types can you choose to meet the client's needs? (Choose all that apply.)

    1. Single-mode fiber-optic cable
    2. Thin coaxial cable
    3. Multimode fiber-optic cable
    4. Shielded Twisted Pair (STP) cable
    5. Unshielded Twisted Pair (UTP) cable

    Answer:

    A, C. Any type of fiber-optic cable will satisfy the client's requirements. Fiber-optic cable supports the required 1000 Mbps data rate and can connect networks that are 500 meters apart. Fiber-optic cable is also immune to EMI. Although both multimode and single-mode fiber would meet the corporation's general needs, multimode is substantially less expensive than single-mode fiber. Twisted-pair wiring (STP or UTP) meets the data rate, but it does not support connections longer than 100 meters. Thin coaxial cable does not support the data rate or distances longer than 185 meters.
87. You receive a call at the IT help desk from a user who has recently moved to a new office in the company building, down the hall from her old one. Since the move, she has only been able to access the company's wireless network with her laptop intermittently. The network is based on 802.11n equipment, and it is using the 2.4 GHz frequency and the WPA2 security protocol. The user never had a problem in her previous office location. Which of the following could not possibly be the cause of her problem? (Choose all that apply.)

    1. The user's laptop is connecting to the wrong SSID.
    2. The user's laptop is configured to use the 5 GHz frequency.
    3. The user's new office is farther from the access point than her old one.
    4. There are more intervening walls between the user's new office and the access point.
    5. The user's laptop is configured with the wrong WPA2 passphrase.

    Answer:

    C, D. An incorrect frequency, Service Set Identifier (SSID), or WiFi Protected Access II (WPA2) passphrase would prevent the user's laptop from ever connecting to the network, so these cannot be the cause of the problem. Greater distance from the access point or interference from intervening walls can both cause a weakening of wireless signals, which can result in the intermittent connectivity that the user is experiencing.
88. Which of the following statements about static routing are not true? (Choose all that apply.)

    1. Static routes are automatically added to the routing table by routing protocols when a new network path becomes available.
    2. Static routes are manually configured routes that administrators must add, modify, or delete when a change in the network occurs.
    3. Static routes are a recommended solution for large internetworks with redundant paths to each destination network.
    4. Static routes are a recommended solution for small internetworks with a single path to each destination network.
    5. Static routes adapt to changes in the network infrastructure automatically.

    Answer:

    A, C, E. Static routes are not automatically added to the routing table by routing protocols and do not automatically adapt to changes in the network. They are therefore not recommended for large internetworks with redundant paths between networks. Administrators must manually add, modify, or delete static routes when a change in a network occurs. For this reason, static routes are recommended only for use in small networks without multiple paths to each destination.
89. Which layer of the Open Systems Interconnection (OSI) model has its own logical addressing system and is responsible for routing packets from one network to another?

    1. Physical
    2. Data link
    3. Network
    4. Transport
    5. Session
    6. Presentation
    7. Application

    Answer:

    C. Network layer protocols specify logical addresses, such as IP addresses, for end system communication. They also use those addresses to route packets to destinations on other networks. The physical layer defines standards for physical and mechanical characteristics of a network. The data link layer uses Media Access Control (MAC) or hardware addresses, not logical addresses. The transport layer uses port numbers, not logical addresses. Session layer protocols create and maintain a dialog between end systems. Presentation layer protocols are responsible for the formatting, translation, and presentation of information. The application layer provides an entry point for applications to access the protocol stack and prepare information for transmission across a network.
90. There are several marketing consultants working in your office for the first time, and they have approached you because they are unable to connect to the company's 802.11g wireless network with their laptops. They are selecting the correct Service Set Identifier (SSID) from the Available Networks list, but they still cannot connect, and there are no error messages of any kind. Which of the following tasks should you perform first to try to resolve the problem?

    1. Examine the area where the consultants are working for possible sources of signal interference.
    2. Change the frequency used by the wireless access point from 2.4 GHz to 5 GHz.
    3. Make sure that the consultants' laptops are configured to use the correct wireless security protocol.
    4. Check the network adapters in the laptops for channel overlap.

    Answer:

    C. The use of an incorrect wireless security protocol is a well-known source of errorless connection failures, so checking this will most likely enable you to discover the source of the problem. Channel overlap is a problem that you would check and resolve at the access point, not at the users' workstations. It is not possible to change the frequency on the access point, because the 802.11g standard only supports the 2.4 GHz frequency. Although signal interference could conceivably be the cause for a connection failure, the users can see the network's SSID, so this is not likely to be the problem.
91. You are researching the various types of Storage Area Network (SAN) technologies currently available before making a purchasing recommendation to your IT director. Which of the following are genuine advantages of iSCSI over Fibre Channel? (Choose all that apply.)

    1. iSCSI can share the same network as standard Local Area Network (LAN) traffic; Fibre Channel cannot.
    2. iSCSI is routable, whereas Fibre Channel is not.
    3. iSCSI is less expensive to implement than Fibre Channel.
    4. iSCSI includes its own internal flow control mechanism; Fibre Channel does not.

    Answer:

    A, B, C. iSCSI does not include its own flow control mechanism, so this option is incorrect. It runs over a TCP connection, which is the protocol responsible for flow control. Fibre Channel requires a dedicated network using fiber-optic cable. iSCSI traffic can coexist with standard LAN traffic on a single network, although some type of Quality of Service (QoS) mechanism is frequently recommended. Because it runs on any IP network, iSCSI traffic is routable, and it is far less expensive to implement than Fibre Channel.
92. In which of the following Domain Name System (DNS) transactions does the querying system generate an iterative query? (Choose all that apply.)

    1. A DNS client extracts the server name [`www.adatum.com`](http://www.adatum.com/) from a URL and sends it to its designated DNS server for resolution.
    2. A client's DNS server sends a name resolution request to a root domain server to discover the authoritative server for the `com` top-level domain.
    3. A client's DNS server sends a name resolution request to the `com` top-level domain server to find the authoritative server for the [`adatum.com`](http://adatum.com/) domain.
    4. A client's DNS server, which has been configured to function as a forwarder, sends the server name [`www.adatum.com`](http://www.adatum.com/) from a URL to its Internet Service Provider's (ISP's) DNS server for resolution.
    5. A client's DNS server sends a name resolution request to the [`adatum.com`](http://adatum.com/) domain server to discover the IP address associated with the server name `www` .

    Answer:

    B, C, E. The client's DNS server uses iterative queries when sending name resolution requests to root domain servers and to the authoritative servers for the `com` and [`adatum.com`](http://adatum.com/) domains. In an iterative query, the server replies immediately with the best information it possesses, and the transaction ends. When a client sends a name resolution query to its DNS server, it uses a recursive request so that the server will assume the responsibility for resolving the name. The only other use of recursive requests is in the case of a forwarder, which is configured to pass that responsibility on to another DNS server.
93. A user approaches you as you are passing through his department and reports that he cannot access the Internet. After questioning him, you determine that he can access systems on the local network, however. You examine the routing table on the user's Windows workstation, and you see the problem. Which of the following commands must you run to correct the user's problem, based on the routing table display shown here?

    `IPv4 Route Table =========================================================================== Active Routes: Network Destination Netmask Gateway Interface Metric 127.0.0.0 255.0.0.0 On-link 127.0.0.1 331 127.0.0.1 255.255.255.255 On-link 127.0.0.1 331 127.255.255.255 255.255.255.255 On-link 127.0.0.1 331 192.168.2.0 255.255.255.0 On-link 192.168.2.37 281 192.168.2.37 255.255.255.255 On-link 192.168.2.37 281 192.168.2.255 255.255.255.255 On-link 192.168.2.37 281 224.0.0.0 240.0.0.0 On-link 127.0.0.1 331 224.0.0.0 240.0.0.0 On-link 192.168.2.37 281 255.255.255.255 255.255.255.255 On-link 127.0.0.1 331 255.255.255.255 255.255.255.255 On-link 192.168.2.37 281 =========================================================================== Persistent Routes: None`

    1. `route add 192.168.2.0 MASK 0.0.0.0 192.168.2.37 METRIC 25 IF 192.168.2.99`
    2. `route add 0.0.0.0 MASK 255.255.255.0 192.168.2.99 METRIC 25 IF 192.168.2.37`
    3. `route add 192.168.2.0 MASK 255.255.255.0 192.168.2.99 METRIC 25 IF 192.168.2.37`
    4. `route add 0.0.0.0 MASK 0.0.0.0 192.168.2.99 METRIC 25 IF 192.168.2.37`

    Answer:

    D. To access the Internet, the workstation's routing table must include a default gateway entry. The default gateway is a router on the local network that provides access to other networks, such as the Internet. To manually create a default gateway entry in the routing table, you use the `route add` command with a Network Destination value of 0.0.0.0, a MASK value of 0.0.0.0, and the address of a router on the local network (in this case 192.168.2.99). The entry must also have a METRIC value that is lower than the other entries in the table so that it will be used first.
94. You are heading out to do a cabling job for a client who has coaxial and twisted-pair Ethernet networks at their facility. You want to bring connectors and cables to prepare for any eventuality. Which of the following connector types are typically associated with Ethernet networks? (Choose all that apply.)

    1. N-type
    2. BNC
    3. F-type
    4. RJ45
    5. DB-9

    Answer:

    A, B, D. Thin Ethernet networks use BNC connectors. Thick Ethernet networks use N-type connectors. All Unshielded Twisted Pair (UTP) Ethernet networks use RJ45 connectors. You will not need F-type or DB-9 connectors. F-type connectors are used with coaxial cable but are typically used for cable television installations. DB-9 connectors are commonly used for serial communications ports.
95. When geofencing is used as part of a multifactor authentication system, which of the following best describes geofencing's role?

    1. Somewhere you are
    2. Something you do
    3. Something you have
    4. Something you know

    Answer:

    A. _Geofencing_ is the generic term for a technology that limits access to a network or other resource based on the client's location. It is therefore best described as somewhere you are. A finger gesture would be considered something you do, a password is something you know, and a smartcard is something you have.
96. Some organizations maintain alternative sites that they can use as datacenters should a disaster render the main datacenter unusable. Which of the following types of disaster recovery site can be made operational in the shortest amount of time?

    1. A hot site
    2. A warm site
    3. A cold site
    4. All of the site types require the same amount of preparation time.

    Answer:

    A. Hot, warm, and cold backup sites differ in the hardware and software they have installed. A cold site is just a space at a remote location. The hardware and software must be procured and installed before the network can be restored. It is therefore the least expensive and takes the most time. A warm site has hardware in place, but it still must be installed and configured. A hot site has all of the necessary hardware already installed and configured. A warm site is more expensive than a cold site, and a hot site is the most expensive of all and takes the shortest amount of time to be made operational.
97. Which of the following types of Virtual Private Network (VPN) connection is the best solution for connecting a home user to a corporate network?

    1. Host-to-site
    2. Site-to-site
    3. Host-to-host
    4. Extranet

    Answer:

    A. A host-to-site VPN is a remote access solution, enabling users to access the corporate network from home or while traveling. A site-to-site VPN enables one network to connect to another, enabling users on both networks to access resources on the other one. This is usually a more economical solution for branch office connections than a Wide Area Network (WAN) link. A host-to-host VPN enables two individual users to establish a protected connection to each other. An extranet VPN is designed to provide clients, vendors, and other outside partners with the ability to connect to your corporate network with limited access.
98. Which of the following are valid reasons why the leaf and spine datacenter topology is superior to the standard three-tier topology? (Choose all the apply.)

    1. The leaf and spine topology is less expensive to implement than the three-tier topology.
    2. In a leaf and spine topology, all data flows require the same number of hops.
    3. The leaf and spine arrangement uses a full mesh switching topology.
    4. The leaf and spine topology uses software-defined networking to direct traffic, rather than blocking ports using the spanning tree protocol.

    Answer:

    B, C, D. The leaf and spine topology uses a full mesh topology in its two layers of switches. This is more expensive than the three-tier topology, but it reduces latency by requiring the same number of hops in the path between any two routers. The use of software-defined networking provides adaptive path determination without the use of the Spanning Tree Protocol (STP) for layer 2 port blocking.
99. A baseline is a performance measurement for a device or system, taken under normal operating conditions, which you can use later to quantify any changes that might have taken place. Which of the following Windows applications would you most likely use to create a baseline of system or network performance?

    1. Syslog
    2. Event Viewer
    3. Network Monitor
    4. Performance Monitor

    Answer:

    D. Performance Monitor is a Windows application that can create logs of specific system and network performance statistics over extended periods of time. Such a log created on a new computer can function as a baseline for future troubleshooting. Event Viewer is a Windows application for displaying system log files; it cannot create a performance baseline. Syslog is a log compilation program originally created for Unix systems; it does not create performance baselines. Network Monitor is a protocol analyzer. Although it can capture a traffic sample that can function as a reference for future troubleshooting efforts, this cannot be called a performance baseline.
100.    In most cases, a Denial-of-Service (DoS) attack refers to a deliberate attempt to overwhelm a server with incoming traffic. However, this is not always the case. Which of the following types of DoS attacks does not involve flooding a server with traffic?

        1. Amplified
        2. Distributed
        3. Permanent
        4. Reflective

        Answer:

        C. Although a DoS attack typically involves traffic flooding, any attack that prevents a server from functioning can be called a DoS attack. A permanent DoS attack is one in which the attacker actually damages the target system and prevents it from functioning. This can be a physical attack that actually damages the server hardware, or the attacker can disable the server by altering its software or configuration settings. Flood-based attacks include the Distributed Denial-of-Service (DDoS) attack, in which the attacker uses hundreds or thousands of computers, controlled by malware and called bots or zombies, to send traffic to a single server or website in an attempt to overwhelm it and prevent it from functioning. An amplified DoS attack is one in which the messages sent by the attacker require an extended amount of processing by the target servers, increasing the burden on them more than simpler messages would. A reflective DoS attack is one in which the attacker sends requests containing the target server's IP address to legitimate servers on the Internet, such as DNS servers, causing them to send a flood of responses that overwhelm the target.
