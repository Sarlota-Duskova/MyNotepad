# Questions

1.  You are installing a fiber-optic cable between two buildings. To install the cable, you must run it through a conduit between the buildings, and access to the conduit is not easy. Before you run the cable, you want to ensure that it's working properly. Which tool should you use?

    1. Cable tester
    2. Multimeter
    3. Loopback plug
    4. Tone generator and probe

    Answer:

    A. Cable testers are indispensable tools for any network technician. Usually you would use a cable tester before you install a cable to make sure it works. Of course, you can test them after they've been run as well. Multimeters are used to test power supplies and wall outlets. Loopback plugs are used to test network interface cards, and tone generators and probes are used to locate a wire among other wires.
2.  Which TCP/IP protocol, designed to download email, allows for multiple clients to be simultaneously connected to the same mailbox?

    1. SMTP
    2. POP3
    3. IMAP
    4. SMB

    Answer:

    C. Internet Message Access Protocol (IMAP) is a secure protocol designed to download email. It has several advantages over the older Post Office Protocol 3 (POP3). First, IMAP4 works in connected and disconnected modes. Second, it lets you store the email on the server, as opposed to POP3, which requires you to download it. Third, IMAP4 allows multiple clients to be simultaneously connected to the same inbox. Simple Mail Transfer Protocol (SMTP) is used for sending mail, and Server Message Block (SMB) is used in sharing files across a network.
3.  You are using your laptop on the company network. In your web browser, you type [`www.google.com`](http://www.google.com/) and press Enter. The computer will not find Google. You open the browser on your phone, and using your cellular connection, you can open Google without a problem. Your laptop finds internal servers and can print without any issues. What is the most likely reason you can't open Google?

    1. DNS server problem
    2. DHCP server problem
    3. Missing subnet mask
    4. Duplicate IP address

    Answer:

    A. The Domain Name System (DNS) server is responsible for resolving hostnames, such as [`www.google.com`](http://www.google.com/), to IP addresses to enable communication. If it's not working properly or you can't connect to it, you won't be able to browse the Internet using friendly website names. Dynamic Host Configuration Protocol (DHCP) is used to assign IP addresses to network clients. The subnet mask might be incorrect, but it wouldn't be missing, and a duplicate IP address would provide an error message stating that.
4.  Which one of the following TCP/IP protocols was designed as a replacement for Telnet?

    1. SMB
    2. SSH
    3. SFTP
    4. FTPS

    Answer:

    B. Secure Shell (SSH) can be used to set up a secure session over port 22 for remote logins or for remotely executing programs and transferring files. Because it's secure, it was originally designed to be a replacement for the unsecure `telnet` command. Server Message Block (SMB), File Transfer Protocol (FTP), and FTP Secure (FTPS) protocols are used for sharing files across a network.
5.  Which of the following network connectivity devices operates at Layer 2 of the OSI model?

    1. Hub
    2. Switch
    3. Cable
    4. Router

    Answer:

    B. A switch operates at layer 2 of the open systems interconnection (OSI) model. Layers of the OSI model are (1) physical, (2) datalink, (3) network, (4) transport, (5) session, (6) presentation, and (7) application. The physical layer encompasses transmission media such as unshielded twisted pair (UTP), shielded twisted pair (STP), fiber optic, and so on. The datalink layer deals with transmitting frames on a LAN, so it includes the network interface card (NIC) and switch. Routers operate on OSI layer 3, because they transmit data between networks. Hubs work on OSI layer 1 because they merely connect devices in the same collision domain without regard to packet header information. The OSI model is not listed as an objective on the CompTIA A+ exam, but understanding it will help you understand network communications.
6.  Which of the following TCP/IP protocols is connection-oriented and attempts to guarantee packet delivery?

    1. IP
    2. TCP
    3. UDP
    4. ICMP

    Answer:

    B. Transmission Control Protocol (TCP) guarantees packet delivery through the use of a virtual circuit and data acknowledgments, and User Datagram Protocol (UDP) does not. Because of this, TCP is often referred to as connection-oriented, whereas UDP is connectionless. Internet Protocol (IP) is used to get packets to their destination across the Internet, and Internet Control Message Protocol (ICMP) is used by connectivity devices to diagnose problems and send messages.
7.  Which TCP/IP protocol allows a user to log into a remote computer and manage files as if they were logged in locally?

    1. FTP
    2. SFTP
    3. SMB
    4. RDP

    Answer:

    D. Remote Desktop Protocol (RDP) is a replacement for the older Telnet protocol, which is not secure. RDP, as its name implies, lets users log into a local machine and use a remote machine almost as if they were sitting at it. RDP uses port 3389. File Transfer Protocol (FTP), Secure File Transfer Protocol (SFTP), also called Secure Shell (SSH) FTP, and Server Message Block (SMB) protocols are all used for sharing files across a network.
8.  Which Wi-Fi standard is the fastest, operating in both the 2.4 and 5 GHz frequencies?

    1. 802.11a
    2. 802.11ac
    3. 802.11ax
    4. 802.11n

    Answer:

    C. 802.11ax (Wi-Fi 6) is considered a replacement for 802.11ac (Wi-Fi 5). 802.11ac operates in the 5 GHz frequency, while 802.11ax can operate between 1 and 7.125 GHz frequencies, encompassing the 2.4 GHz and 5 GHz bands. 802.11ac can send data at over 1 Gbps, while 802.11ax can be several times that. 802.11a was adopted in 1999. It operates at 54 Mbps in the 5 GHz frequency band. 802.11n was adopted in 2008. It operates at 600 Mbps in both the 2.4 GHz and 5 GHz ranges.
9.  Bob has a device that operates at 5 GHz. He is unable to connect his device to a LAN that he hasn't accessed before, although he has verified that he has the correct password. What type of network might pose this problem?

    1. 802.11g
    2. 802.11n
    3. 802.11ac
    4. 802.11ax

    Answer:

    A. If Bob is trying to connect to an 802.11g network, his device will not be able to connect because 802.11g operates on the 2.4 GHz frequency only. 802.11n and 802.11ax both operate on 2.4 GHz and 5 GHz. 802.11ac operates only on the 5 GHz frequency.
10. Which TCP/IP protocol is used to provide shared access to files and printers on the network?

    1. FTP
    2. SSH
    3. SMB
    4. SMTP

    Answer:

    C. Server Message Block (SMB) is a protocol used to provide shared access to files, printers, and other network resources. In a way, it functions a bit like File Transfer Protocol (FTP), only with a few more options, such as the ability to connect to printers and more management commands. Secure Shell (SSH) uses encryption to create a secure contact between two computers, and Simple Mail Transfer Protocol (SMTP) is used for sending email.
11. What port does the Telnet protocol use?

    1. 21
    2. 22
    3. 23
    4. 25

    Answer:

    C. Telnet lets users log into another machine and “see” the remote computer in a window on their screen. Although this vision is text only, users can manage files on that remote machine just as if they were logged in locally. Telnet uses port 23. Telnet has been largely replaced by Secure Shell (SSH), and SSH (over port 22) is more secure than Telnet. Port 21 is used by File Transfer Protocol (FTP), and port 25 is used by Simple Mail Transfer Protocol (SMTP).
12. You have just installed a wireless 802.11ac network for a client. The IT manager is concerned about competitors intercepting the wireless signal from outside the building. Which tool is designed to test how far your wireless signal travels?

    1. Tone generator and probe
    2. Protocol analyzer
    3. Packet sniffer
    4. Wi-Fi analyzer

    Answer:

    D. A wireless locator, or a Wi-Fi analyzer, can be either a handheld hardware device or specialized software that is installed on a laptop, smartphone, or other mobile device and whose purpose is to detect and analyze Wi-Fi signals. It can detect where signals are strong or weak to determine whether there are potential security issues. A tone generator and probe are used for locating a wire. Protocol analyzers and packet sniffers are tools used for capturing and analyzing network traffic.
13. Some of your network users are concerned about submitting confidential information to an online website. What should you tell them?

    1. It's fine, because all Internet traffic is encrypted.
    2. If the website address starts with `TLS://`, it should be OK to submit confidential information to a trusted site.
    3. If the website address starts with `HTTPS://`, it should be OK to submit confidential information to a trusted site.
    4. Don't ever submit confidential information to any online website.

    Answer:

    C. Internet traffic is not encrypted by default. Websites that are secure and encrypt their transmissions will start with `HTTPS://` rather than `HTTP://`. These sites can be trusted to encrypt the data, and their identity is verified.
14. Which TCP/IP Internet layer protocol is responsible for delivering error messages if communication between two computers fails?

    1. ICMP
    2. IP
    3. TCP
    4. UDP

    Answer:

    A. The main Internet layer protocol is Internet Protocol (IP), and it's the workhorse of TCP/IP. Another key protocol at this layer is Internet Control Message Protocol (ICMP), which is responsible for delivering error messages. If you're familiar with the ping utility, you'll know that it utilizes ICMP to send and receive packets. Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) are both communication protocols; TCP guarantees delivery but UDP does not.
15. Which type of IPv6 address identifies a single node on the network?

    1. Multicast
    2. Anycast
    3. Unicast
    4. Localcast

    Answer:

    C. There are three types of addresses in IPv6: unicast, anycast, and multicast. A unicast address identifies a single node on the network. An anycast address refers to one that has been assigned to multiple nodes, and a packet will be delivered to one of them. A multicast address is one that identifies multiple hosts, and a packet will be sent to all of them.
16. What type of network covers large geographical areas and often supports thousands of users, often using lines owned by other entities?

    1. LAN
    2. WAN
    3. PAN
    4. MAN

    Answer:

    B. A wide area network (WAN) covers large geographical areas and often supports thousands of users. A WAN can be for different locations of a single company, or a WAN may connect several different companies together to share information. WAN lines are often leased from a WAN provider. The Internet is considered to be a very large WAN. A local area network (LAN) covers a relatively small area such as a home or business. A personal area network (PAN) is usually used by one person and consists of their computer and its Bluetooth devices. A metropolitan area network (MAN) is similar to a WAN, but the area covered is much smaller, such as a university or a city.
17. Which TCP/IP protocol, developed by Microsoft, uses port 3389 to connect to a remote computer?

    1. RDP
    2. SMB
    3. CIFS
    4. Telnet

    Answer:

    A. Developed by Microsoft, the Remote Desktop Protocol (RDP) allows users to connect to remote computers and run programs on them as if they were sitting at the computer. It uses port 3389. A port is associated with a specific protocol and must be “opened” on a router to allow traffic from the program or protocol to enter the LAN. The combination of an IP address and a port is considered a socket. The IP address gets the data to the right destination, and the port number tells the transmission layer of the OSI model which application the data is to be sent to. Server Message Block (SMB) and Common Internet File System (CIFS) are used in sharing files across a network. Telnet is an unsecure protocol that has been largely replaced by the Secure Shell (SSH) protocol.
18. What port does the SSH protocol use?

    1. 21
    2. 22
    3. 23
    4. 25

    Answer:

    B. Secure Shell (SSH) can be used to set up a secure session for remote logins or for remotely executing programs and transferring files. SSH uses port 22. SSH has largely replaced the insecure Telnet, which uses port 23. Port 21 is used by File Transfer Protocol (FTP), and port 25 is used by Simple Mail Transfer Protocol (SMTP).
19. Which of the following IP addresses is not routable on the Internet?

    1. `10.1.1.1`
    2. `11.1.1.1`
    3. `12.1.1.1`
    4. `13.1.1.1`

    Answer:

    A. Private IP addresses are not routable on the Internet. IPv4 network numbers were arranged in classes, and classes A, B, and C each have their own private range. The private IP address range for Class A networks is `10.0.0.0/8.` The /8 means that the first 8 bits of the subnet mask denote the network number. Expressing a subnet mask this way is known as CIDR (pronounced cider) notation. CIDR stands for classless interdomain routing. While the term CIDR doesn't appear on the objectives for this CompTIA A+ exam, you may still run into it while working in IT.
20. Which network connectivity device does not forward broadcast messages, thereby creating multiple broadcast domains?

    1. Hub
    2. Switch
    3. Bridge
    4. Router

    Answer:

    D. One of the key features of routers is that they break up broadcast domains. Broadcast traffic from one port of the router will not get passed to the other ports, which greatly reduces network traffic. Bridges, hubs, and switches will all forward broadcast packets.
21. What type of address does a router use to get data to its destination?

    1. IP
    2. MAC
    3. Memory
    4. Loopback

    Answer:

    A. Routers are OSI model Layer 3 devices. They keep a chart containing the IP address of the device connected to each port, whether that device is a computer or another router's external address. A media access control (MAC) address is the address of a network interface card (NIC). Memory addresses identify where information is stored, and a loopback address is used to test TCP/IP on the local host. The loopback address for IPv4 is 127.0.0.1, and for IPv6 it is ::1.
22. You have a desktop computer that is behaving erratically on the network. The wired connection will often disconnect without warning. Which tool should you use to troubleshoot the network adapter?

    1. Multimeter
    2. Tone generator and probe
    3. Loopback plug
    4. Cable tester

    Answer:

    C. A loopback plug is for testing the ability of a network adapter to send and receive. The plug gets plugged into the network interface card (NIC), and then a loopback test is performed using troubleshooting software. You can then tell whether the card is working properly. Multimeters are used for testing power supplies and wall outlets, a tone generator and probe help the technician to find a specific wire, and a cable tester checks that an Ethernet wire was configured correctly and that it can make an end-to-end connection.
23. Your company just expanded and is leasing additional space in an adjacent office building. You need to extend the network to the new building. Fortunately, there is a conduit between the two. You estimate that the cable you need to run will be about 300 meters long. What type of cable should you use?

    1. CAT-5e
    2. CAT-7
    3. CAT-8
    4. MMF

    Answer:

    D. Category 5, 6, and 7 UTP cables are limited to 100 meters, while Category 8 is limited to only 100 feet, so none of the UTP cables listed will work. You need fiber, and multimode fiber (MMF) can span distances of 300 meters. MMF is also known as OM1, OM2, OM3, OM4, and OM5. OM stands for optical mode. Specifications for each type of multimode fiber are available in the ISO/IEC 11801 standard.
24. You want to ensure that client computers can download email from external email servers regardless of the protocol their email client uses. Which ports do you open on the firewall to enable this? (Choose two.)

    1. 23
    2. 25
    3. 110
    4. 143

    Answer:

    C, D. Simple Mail Transfer Protocol (SMTP, port 25), Post Office Protocol 3 (POP3, port 110), and Internet Message Access Protocol (IMAP, port 143) are all email protocols. SMTP is for sending email. POP3 and IMAP are for downloading (receiving) email. Port 23 is used by Telnet. Option B is incorrect because the question specifically asks about downloading (not sending) email.
25. You are installing network cabling in a highly secure facility. The cables need to be immune to electronic eavesdropping. What type of cable should you use?

    1. Fiber-optic
    2. UTP
    3. STP
    4. Coaxial

    Answer:

    A. Fiber-optic cabling uses pulses of light instead of electric voltages to transmit data, so it is immune to electrical interference and to wiretapping. UTP, STP, and coaxial are all copper cables, which use electricity to transmit data and so can be subjected to electronic eavesdropping.
26. Which networking device is capable of reading IP addresses and forwarding packets based on the destination IP address?

    1. Hub
    2. Switch
    3. NIC
    4. Router

    Answer:

    D. Routers operate at the Network layer (Layer 3) of the OSI model. Because of this, they make their decisions on what to do with traffic based on logical addresses, such as an Internet Protocol (IP) address. Switches use media access control (MAC) addresses and are OSI Layer 2 devices. Hubs and NICs operate primarily at the physical layer (Layer 1). The OSI model is not listed as an objective on the CompTIA A+ exam, but understanding it will help you understand network communications.
27. Which network device is designed to be a security guard, blocking malicious data from entering your network?

    1. PoE injector
    2. EoP device
    3. Firewall
    4. Router

    Answer:

    C. A firewall is a hardware or software solution that serves as your network's security guard. Firewalls can protect you in two ways: they protect your network resources from hackers lurking in the dark corners of the Internet, and they can simultaneously prevent computers on your network from accessing undesirable content on the Internet or sending out data that they shouldn't. PoE stands for Power over Ethernet, and EoP stands for Ethernet over Power. Neither has to do with protection. While a router may incorporate a firewall, it is not, by itself, a firewall. Routers are responsible for communications with other networks or broadcast domains. A firewall may be a discrete physical network appliance or software incorporated into another device like a router.
28. You are manually configuring TCP/IP hosts on the network. What configuration parameter specifies the internal address of the router that enables Internet access?

    1. Subnet mask
    2. DHCP server
    3. DNS server
    4. Default gateway

    Answer:

    D. The default gateway is the address to the network's router on the LAN side of the router. The router allows the host to communicate with hosts who are not on the local network. The default gateway is also called the router's internal address. The `ipconfig /all` command can be used to see the default gateway address that the local computer is currently configured to use. The router will also have an external address, which is used to communicate with networks outside the LAN. Virtually all modern routers use a process called network address translation (NAT), which will substitute the router's external address for a host's IP address when requesting information from a remote network. The router knows which host requested the information and will pass it on to the correct host when it is received. This is one of the ways that the router protects the local hosts from the outside world.
29. Which of the following devices will be found in a telecommunications room and provides a means to congregate horizontal wiring, terminating each run in a female port?

    1. Patch panel
    2. Multiplexer
    3. Rack U
    4. Demarcation point

    Answer:

    A. A patch panel can be found in a telecommunications room (also called a wiring closet), usually mounted in a networking rack. On the back will be connections to “punch down” wires into. On the front will be a female port, usually an RJ45 type. A multiplexer is a device that aggregates several connections into one. A rack U is simply a measurement of the height of a device mounted into a rack (e.g., my patch panel is 4U). Each U is equal to 1.75 inches. The demarcation point is where responsibility for a network changes from the ISP to its customer.
30. What type of network is most commonly associated with Bluetooth devices such as wireless keyboards, mice, and headphones, and covers a small area?

    1. LAN
    2. WAN
    3. PAN
    4. MAN

    Answer:

    C. A personal area network (PAN) is a small-scale network designed around one person within a limited boundary area. The term generally refers to networks that use Bluetooth technology. A local area network (LAN) covers a larger area such as a house or perhaps one floor of a building and likely uses the Ethernet protocol. A metropolitan area network (MAN) covers a larger area such as a city or university campus, and a wide area network (WAN) covers a very large geographic area such as one connecting distant cities or different countries.
31. When troubleshooting a network connectivity issue, you discover that the local computer has an IPv4 address of `169.254.2.2.` What do you immediately know about this local computer?

    1. It is working fine.
    2. It can't find a DHCP server.
    3. It isn't on the network.
    4. It has an invalid IP address.

    Answer:

    B. The 169.254.0.0/16 range in IPv4 is the automatic private IP addressing (APIPA) range. APIPA comes into play when the host is unable to locate a Dynamic Host Configuration Protocol (DHCP) server, and the network connection is configured to acquire an IP address dynamically. Since the computer is unable to get a dynamic IP address from the DHCP server, the operating system automatically assigns a random IP address in the APIPA range.
32. Which of the following IPv6 addresses is automatically assigned by the host when it boots and is only usable on the broadcast domain that it exists in?

    1. `2000::/3`
    2. `FC00::/7`
    3. `FE80::/10`
    4. `FF00::/8`

    Answer:

    C. An IPv6 address in the `FE80::/10` range is called a link-local address and is similar to an IPv4 automatic private IP addressing (APIPA) address. (The `169.254.0.0/16` range in IPv4 is the APIPA range, used for automatic configuration if the host can't locate a Dynamic Host Configuration Protocol \[DHCP] server.) Link-local addresses are generated by the PC when it boots up. Packets using a link-local address cannot be forwarded by a router.
33. You need to configure a wireless router for an office network. The office manager wants new devices to be able to automatically join the network and announce their presence to other networked devices. Which service should you enable to allow this?

    1. DHCP
    2. NAT
    3. QoS
    4. UPnP

    Answer:

    D. Universal Plug and Play (UPnP) is a standard designed to simplify the process of connecting devices to a network and to enable those devices to automatically announce their presence to other devices on the network. In a truly secure environment, UPnP would be disabled, but it is often left enabled on home networks. Dynamic Host Configuration Protocol (DHCP) automatically assigns an IP address to a device when it is powered on, attached to a network, and configured to obtain an address dynamically. Network address translation (NAT) is a feature of routers used to hide the IP addresses of computers on the local network side of the router from the other networks and computers on the outside of the network. Quality of Service (QoS) can be configured to give desired devices preference over others for using network bandwidth.
34. You are troubleshooting a computer with an IPv6 address that is in the `FE80::/10` range. Which of the following statements are true? (Choose two.)

    1. The computer will not be able to get on the Internet using that IP address.
    2. The computer will be able to get on the Internet using that IP address.
    3. The computer is configured with a link-local unicast address.
    4. The computer is configured with a global unicast address.

    Answer:

    A, C. Addresses in the FE80::/10 range are link-local unicast addresses. A link-local address is assigned to each IPv6 interface but is not routable on the Internet. If this is the only address the host has, it will not be able to get on the Internet.
35. You have set up your web server to function as an FTP server as well. Users on the Internet complain that they are not able to access the server using FTP clients. What port should they be trying to access the server on?

    1. 21
    2. 22
    3. 23
    4. 80

    Answer:

    A. The File Transfer Protocol (FTP) is optimized for downloading files from servers. It uses port 21. Secure Shell (SSH) uses port 22, Telnet uses port 23, and Hypertext Transfer Protocol (HTTP) uses port 80.
36. Which TCP/IP protocol allows you to access data such as employee phone numbers and email addresses that are stored within an information directory?

    1. SNMP
    2. SMTP
    3. CIFS
    4. LDAP

    Answer:

    D. The Lightweight Directory Access Protocol (LDAP) is a directory services protocol based on the X.500 standard. LDAP is designed to access information stored in an information directory typically known as an LDAP directory or LDAP database. This often includes employee phone numbers and email addresses. Simple Network Management Protocol (SNMP) is used in network monitoring, Simple Mail Transfer Protocol (SMTP) is used in sending email, and Common Internet File System (CIFS) is a filesystem for providing shared access between diverse clients.
37. What port is associated with the LDAP protocol?

    1. 22
    2. 139
    3. 389
    4. 3389

    Answer:

    C. Lightweight Directory Access Protocol (LDAP) is designed to access information stored in an information directory typically known as an LDAP directory or LDAP database. LDAP uses port 389. Port 22 is used by Secure Shell (SSH,) 139 is used by NetBIOS, and 3389 is used by the Remote Desktop Protocol (RDP.)
38. You are configuring network hosts with static IP addresses. You have chosen to use a Class B network address. What is the default subnet mask that you should configure on the hosts?

    1. `255.0.0.0`
    2. `255.255.0.0`
    3. `255.255.255.0`
    4. `255.255.255.255`

    Answer:

    B. The default subnet mask for Class B networks is `255.255.0.0`, or written in shorthand, /16. The default subnet mask for Class A networks is `255.0.0.0`, or written in shorthand, /8, and for Class C it is `255.255.255.0`, or written in shorthand, /24. `255.255.255.255` is an IPv4 broadcast address. As a subnet mask it is represented as /32 (in shorthand) in the classless interdomain routing (CIDR) notation.
39. You are installing a new network and working in a telecommunications room. You need to attach several network cables to a 110 block. Which tool should you use to perform this task?

    1. Crimper
    2. Cable stripper
    3. Cable tester
    4. Punchdown tool

    Answer:

    D. If you're working on a larger network installation, you might use a punchdown tool. It's not a testing tool but one that allows you to connect (that is, punch down) the exposed ends of a twisted pair wire into wiring harnesses, such as a 110 block or patch panel. A crimper is used to connect wires to an RJ45 connector, a cable striper removes the outer cover from wires, and a cable tester is used to verify the integrity of a cable.
40. Which of the following Internet connection types offers the fastest download speeds?

    1. Cable
    2. DSL
    3. Fiber-optic
    4. Satellite

    Answer:

    C. Fiber-optic broadband Internet offers fast speeds (often in the 1–2 Gbps range) but is also the most expensive. Cable may have download speeds up to 1 Gbps (typically 10 to 500 Mbps), but upload speeds are typically only around 5 to 50 Mbps, while fiber-optic upload speeds may be in the 1 Gbps range. Digital Subscriber Line (DSL) uses plain old telephone service (POTS) lines and is slow. Satellite networks can be faster than DSL, but still only offer speeds up to about 150 Mbps.
41. Which of the following are public IPv4 addresses? (Choose two.)

    1. `69.252.80.71`
    2. `144.160.155.40`
    3. `172.20.10.11`
    4. `169.254.1.100`

    Answer:

    A, B. IPv4 specifies private (nonroutable) IP address ranges for each class as follows: Class A: 10.0.0.0 to 10.255.255.255, Class B: 172.16.0.0 to 172.31.255.255, and Class C: 192.168.0.0. to 192.168.255.255. Other nonroutable numbers are 127.0.0.1, which is the loopback address, and 169.254.0.0 to 169.254.255.255, which is the automatic private IP addressing (APIPA) range. Class A addresses have a first octet from 0 to 127. Class B's first octet ranges from 128 to 191. Class C's first octet ranges from 192 to 223. Numbers above Class C are reserved.
42. Which TCP/IP protocol uses port 445?

    1. FTP
    2. SSH
    3. SMB
    4. SNMP

    Answer:

    C. Server Message Block (SMB) is a protocol used to provide shared access to files, printers, and other network resources. It originally ran on NetBIOS over UDP using ports 137/138 and over TCP using ports 137 and 139, but it's now part of the TCP/IP stack and uses port 445. Running on NetBIOS allows SMB to facilitate file sharing on a single network, while being part of TCP/IP allows it to facilitate file sharing across the Internet. By itself, SMB is not secure, so it needs other network appliances or software to secure the data being sent over its port(s). File Transfer Protocol (FTP) uses ports 20/21, Secure Shell (SSH) uses port 22, and Simple Network Management Protocol (SNMP) uses ports 161/162.
43. What rendition of SMB was used by Windows servers and NAS servers but is no longer often used?

    1. CIFS
    2. Samba
    3. NFS
    4. SMB3

    Answer:

    A. All of the answer choices are communications protocols for sharing resources. The Common Internet File System (CIFS) is Microsoft's version of Server Message Block (SMB.) Once upon a time CIFS was used extensively for file sharing over a network, but it has since fallen out of favor. While CIFS and SMB both facilitate file sharing, SMB does it better and has other features as well. Samba and Network File System (NFS) facilitate sharing files between clients and servers in Linux distributions. Samba will allow mixed environments with both Windows and Linux machines to share files. NFS will not.
44. For IPv6, which of the following statements are true? (Choose two.)

    1. Each IPv6 interface can have only one address.
    2. Each IPv6 interface is required to have a link-local address.
    3. IPv6 addresses are incompatible with IPv4 networks.
    4. IPv6 does not use broadcasts.

    Answer:

    B, D. Each IPv6 interface can and often does have multiple addresses assigned to it. IPv6 is backward compatible with IPv4 by using tunneling, dual stack, or translation. IPv6 uses multicast addresses in place of broadcast addresses, and a link-local address is established either automatically when a computer boots up or by manually configuring it, but either way the link-local address must be present.
45. Which network connectivity device is seldom used in modern networks, except to extend a network?

    1. Bridge
    2. Hub
    3. Switch
    4. Router

    Answer:

    B. Hubs were once used extensively in Ethernet networks, but they have fallen out of favor because they have a large disadvantage when compared to switches. A hub forms a single collision domain with all of their ports. On a switch, each port is its own collision domain. A switch keeps a table of its ports and the media access control (MAC) address that can be reached from each port. A switch will only forward a packet to a specific port, whereas a hub will forward a packet to all of its ports. The exception is that a broadcast packet will be sent to all switch ports. Switches are faster and more accurate than hubs and are used almost exclusively as the connectivity device within a local area network (LAN.)
46. There is a TCP/IP protocol that should only be used locally because it has virtually no security. It may be used as a part of a preboot execution environment (PXE) or with thin clients booting from a network drive. It uses very little memory and is good for transferring boot files or configuration data between computers on a LAN, and it is connectionless. Which file transfer protocol is this?

    1. FTP
    2. TFTP
    3. FTPS
    4. SMTP

    Answer:

    B. The Trivial File Transfer Protocol (TFTP) is a very simple connectionless protocol. It has little overhead, meaning that it doesn't take much memory to run it. This makes it perfect for booting a thin client across a network. It can be used to transfer the needed boot files to devices that don't have hard drives. It should not be used to transfer files across the Internet because it is not secure. File Transfer Protocol (FTP) is more robust than TFTP. File Transfer Protocol Secure (FTPS) is a secure version of FTP. Simple Mail Transfer Protocol (SMTP) is used to send email messages.
47. Which of the following IPv6 addresses is equivalent to 127.0.0.1 in IPv4?

    1. ::0
    2. ::1
    3. ::127
    4. 2000::/3

    Answer:

    B. 127.0.0.1 is the IPv4 loopback address, used to ping the local network interface. The IPv6 equivalent is ::1.
48. You are asked to perform consulting work for a medium-sized company that is having network connectivity issues. When you examine the patch panel, you notice that none of the dozens of UTP cables are labeled. Which tool can you use to identify which cable goes to which workstation?

    1. Cable tester
    2. Loopback plug
    3. Punchdown tool
    4. Tone generator and probe

    Answer:

    D. If you need to trace a wire in a wall from one location to another, a tone generator and probe is the right tool to use. To use it, attach one end to one end of the cable, such as the end at the computer. Then go to the patch panel with the other end of the probe to locate the cable. These tools are lifesavers when the cables are not properly labeled. A cable tester is used to confirm the integrity of a cable and verity that it is wired correctly. A loopback plug is used to test a network interface card (NIC,) and a punchdown tool is used to terminate wires into a patch panel.
49. Which TCP/IP protocol is responsible for dynamically assigning IP addresses to client computers?

    1. DNS
    2. DHCP
    3. RDP
    4. LDAP

    Answer:

    B. Dynamic Host Configuration Protocol (DHCP) dynamically assigns IP addresses and other IP configuration information to network clients. The Domain Name System (DNS) translates human-readable names to their associated IP addresses, the Remote Desktop Protocol (RDP) allows a user to access a computer remotely as if they were sitting there, and Lightweight Directory Access Protocol (LDAP) is used for retrieving information from a database.
50. Which networking device has multiple ports, each of which is its own collision domain, and examines the header of the incoming packet to determine which port the packet gets sent to?

    1. Hub
    2. Switch
    3. Bridge
    4. Router

    Answer:

    B. Switches provide centralized connectivity for a LAN. Switches examine the header of incoming packets and forward each to only the port whose associated media access control (MAC) address matches the receiving MAC address in the header. Hubs are seldom used now because the entire hub is one collision domain and when a packet is received, the hub sends the packet out to all of its ports indiscriminately. Bridges are used to connect different networks to work as one, and routers are used to forward packets from one network to other networks.
51. Which TCP/IP port will an email client use to push email to its email server?

    1. 23
    2. 25
    3. 110
    4. 143

    Answer:

    B. Email is pushed from clients to servers using the Simple Mail Transfer Protocol (SMTP). SMTP uses port 25. When trying to remember if SMTP is sending or receiving email, think S for Send. Port 23 is used by Telnet, now considered insecure and obsolete. Port 110 is used by POP3 (Post Office Protocol 3), and port 143 is used by IMAP (Internet Mail Access Protocol), both of which are used to retrieve email.
52. A technician is going to set up a Wi-Fi network using standard omnidirectional antennae. Because of the building configuration, transmitting signals for the greatest distance is the technician's primary criterion. Which standard should they choose?

    1. 802.11a
    2. 802.11g
    3. 802.11n
    4. 802.11ac

    Answer:

    C. Of the Wi-Fi standards listed, 802.11n has the longest range by default, at roughly 70 meters indoors and 250 meters outdoors. 802.11ac is newer and faster than 802.11n, but it transmits exclusively in the 5 GHz range, which restricts its functional distance. 802.11a, which is legacy and uses the 5 GHz frequency range, could only send a signal about 30 meters, and 802.11g, which is also legacy but uses the 2.4 GHz frequency range, could only send a signal about 50 meters.
53. You are troubleshooting an intermittently failing Cat 6 network connection. You suspect that there is a short in the connection. Which tool can you use to determine this?

    1. Tone generator and probe
    2. Loopback plug
    3. Cable tester
    4. Crimper

    Answer:

    C. A cable tester typically uses lights to indicate that the cable is working correctly, and if there is a short, then the indicators for two wires would light up at the same time. Cable testers can range from basic ones that are only a few dollars to very sophisticated ones that are hundreds of dollars. Some of the better ones can tell you how many feet from you that the problem in the cable occurs. A tone generator and probe are used to trace a wire or find a specific wire from a group, a loopback plug is used to test a network interface card (NIC), and a crimper attaches a network wire to its terminator, usually an RJ45 plug.
54. What marks the boundary of a IPv4 broadcast domain?

    1. Hub
    2. Switch
    3. Router
    4. Modem

    Answer:

    C. Hubs send every communication they receive out every connected port. Switches will send broadcast packets out every port, but otherwise will send packets to a specific port based on the MAC address. A router will not forward any broadcast packet; therefore a router is the boundary of an IPv4 broadcast domain. A modem (modulator/demodulator) converts signals from one type to another, such as from an analog signal to a digital one.
55. Which TCP/IP protocol gathers and manages network performance information using devices called agents?

    1. SNMP
    2. SMTP
    3. LDAP
    4. SMB

    Answer:

    A. Simple Network Management Protocol (SNMP) gathers and manages network performance information. A management device called an SNMP server can be set up to collect data from these devices (called agents) and ensure that your network is operating properly. SMTP is a mail protocol, LDAP is for accessing database information, and SMB is for file sharing.
56. Which Internet connection type, once popular for home use, offers asymmetrical download and upload speeds and is implemented over common phone lines?

    1. POTS
    2. Cable
    3. DSL
    4. ISDN

    Answer:

    C. Although Digital Subscriber Line (DSL) is being dropped by some providers in favor of fiber-optic lines, it is still a viable Internet connectivity solution in rural areas that fiber has not yet reached. DSL utilizes existing phone lines and provides fairly reliable access while carrying voice and data on the same lines. Most DSL subscriptions are asymmetrical, meaning they offer faster download speeds than upload speeds. POTS stands for Plain Old Telephone Service, an acronym from dial-up days. Cable connectivity is provided by cable TV companies. ISDN is Integrated Services Digital Network, a now obsolete technology that allowed voice and data communication on the same existing telephone lines, similar to DSL.
57. You are installing an 802.11n Wi-Fi network with five wireless access points. The access points are set up so their ranges overlap each other. To avoid communications issues, what principle should you follow when configuring them?

    1. Configure all access points to use the same channel.
    2. Configure all access points to use adjacent channels.
    3. Configure all access points to use nonoverlapping channels.
    4. Channel configuration will not cause communications issues.

    Answer:

    C. When setting up wireless access points, it's good practice to have their ranges overlap to ensure that there is no loss of communication when roaming in the network's area. However, to avoid problems, it's best to set up the access points with nonoverlapping channels; in this way, the overlapping ranges ensure continuous signal coverage while the nonoverlapping channels avoid interference from one WAP to another in the overlapping areas.
58. You need to configure email settings for use with IMAP. Which port will you be configuring?

    1. 25
    2. 80
    3. 110
    4. 143

    Answer:

    D. Internet Mail Access Protocol (IMAP) is used to download mail via port 143. Port 80 is for unsecured web page traffic. Ports 25 and 110 are email ports, but they are associated with SMTP and POP3, respectively.
59. Which of the following technologies will enable you to install networking devices that need power to function, in a location that has no power outlets?

    1. EoP
    2. PoE
    3. WAP
    4. Hub

    Answer:

    B. Power over Ethernet (PoE) enables placement of equipment in areas that otherwise would not be able to accept it. Only four of the eight wires in twisted pair wiring are used for communication. The power is sent over the wires that are not used in communication. If the devices on both ends don't support PoE, then an injector can be used to add power to the line on the way to its destination. Compatibility is important, and there are limits to the amount of power that can be transmitted this way. Ethernet over Power (EoP) is not in the CompTIA A+ objectives, but it uses special devices to send Ethernet communications over existing wiring such as in a household. A wireless access point (WAP) is a device that is used to connect wireless devices to a wired network or to each other. Some WAPs support PoE. A hub is a very simple network connectivity device.
60. You have been asked to install a Wi-Fi network in a building that is approximately 100 meters long and 25 meters wide. Because of cost considerations, you will be using 802.11ac. At a minimum, how many wireless access points will you need?

    1. Two
    2. Three
    3. Four
    4. Six

    Answer:

    B. The 802.11ac standard has an indoor range of approximately 35 meters. At a minimum, you will need three access points. Depending on coverage and indoor interference, such as thick walls, you might need more.
61. What two tools will you need to connect an RJ45 connector to an appropriate cable? (Choose two.)

    1. Punchdown tool
    2. Network tap
    3. Crimper
    4. Cable stripper

    Answer:

    C, D. Punchdown tools are used to connect unshielded twisted pair (UTP) and shielded twisted pair (STP) to a patch panel. A network tap is used to monitor network traffic. The crimper and cable stripper are both needed to add an RJ45 connector to the end of a twisted pair cable. Often both tools are included in one. The stripper removes the outer insulation from the group of wires so that they can be individually inserted into the RJ45 jack. Once the wires are properly inserted, the crimping tool is used to force metal teeth into each wire so that an electrical connection can be made.
62. You are installing network cabling in a drop ceiling of an office space. The ceiling area is used to circulate breathable air. What type of cable must you install?

    1. Coaxial
    2. UTP
    3. Fiber-optic
    4. Plenum

    Answer:

    D. The cable can be any of the three major types, coaxial, twisted pair, or fiber, but it needs to be plenum rated. Normal cables have a PVC coating, which produces a poisonous gas when burned. Plenum-rated cables have a Teflon coating, which is not toxic when burned.
63. You need to install a wireless access point in a drop ceiling where there is no access to a power source. Which technology will allow you to get power to that device?

    1. EoP
    2. PoE
    3. Hub
    4. Repeater/extender

    Answer:

    B. Power over Ethernet (PoE) allows you to power an Ethernet device (such as a switch) through one of the Ethernet ports. For it to work, the access point and the device it plugs into both need to support PoE. Further, both the access point and device need to be compatible with each other. EoP, while not on the current A+ objectives, is a technology that allows the user to transmit Ethernet signals over existing power lines. This can be useful in a place where running Ethernet wires is impossible, but more often Wi-Fi is used in those situations instead. A hub can be used to regenerate a signal, but they also need a power source and are not a wireless access point. A repeater/extender is essentially the same as a hub. It requires power to regenerate a signal and send it on its way.
64. Which of the following IP addresses is not a private address and therefore is routable on the Internet?

    1. `10.1.2.3`
    2. `172.18.31.54`
    3. `172.168.38.155`
    4. `192.168.38.155`

    Answer:

    C. The private IP address ranges are `10.0.0.0/8`, `172.16.0.0/12`, and `192.168.0.0/16`. The address `172.168.38.155` is outside the private IP address range and is a public (routable) address.
65. You are configuring a wireless 802.11ax router. The office manager insists that you configure the router such that traffic from her computer receives higher priority on the network than other users' traffic. Which setting do you need to configure to enable this?

    1. QoS
    2. UPnP
    3. Screened subnet
    4. Port forwarding

    Answer:

    A. By configuring Quality of Service (QoS), an administrator can set different priorities for one or more types of network traffic based on different applications, data flows, or users. UPnP allows devices to identify and connect to other devices on a network. A screened subnet is a secure area established using a router or routers to protect an internal network from traffic coming to a web-facing server. Port forwarding is configured on a router to send specific traffic to a specific device on a network.
66. If you are connecting to a website that encrypts its connection using TLS, what port does that traffic travel on?

    1. 21
    2. 80
    3. 143
    4. 443

    Answer:

    D. To encrypt traffic between a web server and client securely, Hypertext Transfer Protocol Secure (HTTPS) can be used. HTTPS connections are secured using either Secure Sockets Layer (SSL) or Transport Layer Security (TLS). HTTPS uses port 443. Port 21 is used by File Transfer Protocol (FTP), port 80 is used by Hypertext Transfer Protocol (HTTP), and port 143 is used by Internet Mail Access Protocol (IMAP).
67. Your network is currently running a mix of 802.11b and 802.11g devices. At the end of the year, you have extra budget to upgrade some, but not all, of the wireless infrastructure. You want to upgrade to the newest technology possible but still maintain backward compatibility. Which standard should you choose?

    1. 802.11g
    2. 802.11ac
    3. 802.11ax
    4. 802.11r

    Answer:

    C. 802.11b/g transmits in the 2.4 GHz frequency, as does 802.11n, so they are compatible. The newer 802.11ac is a 5 GHz standard and therefore is not backward compatible with 802.11b/g. 802.11ax transmits in both the 2.4 GHz and 5 GHz frequencies, up to 7 GHz. 802.11r is not a standard related to Wi-Fi speed and is not in the A+ exam objectives.
68. What type of network spans multiple buildings or offices, possibly even crossing roads, but is confined to a relatively small geographical area?

    1. LAN
    2. WAN
    3. PAN
    4. MAN

    Answer:

    D. Networks that are larger than a LAN but confined to a relatively small geographical area are metropolitan area networks (MANs). A MAN is generally defined as a network that spans a city or a large campus. LAN stands for local area network. PAN (personal area network) is the smallest of the types of networks, and a WAN is the largest type of network. It could connect faraway cities or even other countries.
69. Which of the following shorthand notations corresponds to the CIDR subnet mask 255.255.224.0?

    1. /19
    2. /20
    3. /21
    4. /22

    Answer:

    A. A subnet mask of 255.255.224.0 has 8 bits in each of the first 2 octets set to on, and it has 3 bits in the third octet on. Therefore, it corresponds to /19 in shorthand. In the binary number system (base two), each bit has two possible values, 0 or 1. Each bit in an octet going from right to left increments by an exponent of two, making the bits of the octets worth the decimal values as follows: | 128 |64 |32 |16 | 8 | 4 | 2 | 1 |. Bits for the subnet mask are always used from left to right, so one bit would be equal to a decimal value of 128. Two bits would be equal to a decimal value of 192 (128 + 64). Three bits would be equal to a decimal value of 224 (128 + 64 + 32), and so on. When all 8 bits of the octet are used for the subnet mask, the equivalent decimal value is 255. For this example, the first 2 octets (8 bits each) are completely on, and in the third octet, only 3 bits are on, making a total of 19 bits in the subnet mask turned on to indicate the network number (8 + 8 + 3 = 19).
70. You are configuring hosts on a network running IPv4. Which elements are required for the computer to connect to the network?

    1. IP address
    2. IP address and subnet mask
    3. IP address, subnet mask, and default gateway
    4. IP address, subnet mask, default gateway, and DNS server address

    Answer:

    B. To communicate on an IPv4 network, a host must be configured with a valid IP address and a subnet mask. A default gateway is needed only if the host will connect to a remote network. DNS servers are optional but useful, because they resolve hostnames to IP addresses.
71. You work at a tech support company and a customer called reporting that they received an error, something about a duplicate IP address. Why are they getting this message? (Choose two.)

    1. All hosts on a network must have a unique IP address.
    2. A PC is manually configured with an IP that is in the DHCP scope.
    3. A PC is manually configured with an IP that is not in the DHCP scope.
    4. None of the PCs have been manually configured.

    Answer:

    A, B. No two nodes on any network, whether IPv4 or IPv6, can have the same IP address because the host portion (or interface ID) of the IP address is what identifies the individual computer on the network. If the network has some machines manually configured, which is generally done with servers, and the remainder of the computers are configured to use Dynamic Host Configuration Protocol (DHCP), you would need to ensure that the manually configured numbers are outside of the DHCP scope (the numbers the DHCP server will automatically assign) but within the bounds of the network. For example, in an IPv4 network, if the network number is 200.100.1.0, the router, which is also acting as a default gateway, might be assigned 200.100.1.1, and numbers from 200.100.1.2 through 200.100.1.20 could be reserved for static configuration on devices that need an IP address that does not change. The DHCP scope would need to _not_ include those numbers. If the network needed an available 180 IP addresses, then 200.100.1.21 to 200.100.1.200 could be safely assigned to the DHCP scope, avoiding any IP address duplication.
72. You're setting up a network for a customer. The network uses a DHCP server, but the customer needs an IP address for their print server that does not change. What are two possible solutions? (Choose two.)

    1. Let the DHCP server assign a number because once assigned, it will not change.
    2. Manually configure the print server to have a static IP address.
    3. Configure a reserved IP address on the DHCP server for the print server.
    4. Static and dynamic IP addresses can't exist on the same network. You'll have to manually configure everything.

    Answer:

    B, C. Certain devices on a network, such as printers and servers, should have an IP address that doesn't change (static) so that the other nodes on the network can always find the device. Option A is incorrect because if the DHCP lease on the IP address expires, the print server would be assigned a different IP address the next time it logs in. A static IP could be configured on the printer server, or the IP address could be configured as reserved on the DHCP server for that print server. Either choice would work. Static and dynamic IP addresses almost always exist on the same network, because each is needed to have a network that runs smoothly.
73. Which obsolete Wi-Fi encryption standard uses a static key, which is commonly 10, 26, or 58 characters long?

    1. WPA3
    2. WPA2
    3. TKIP
    4. WEP

    Answer:

    D. Wired Equivalent Privacy (WEP) was one of the first security standards for wireless devices. It uses a static key; the keys are commonly 10, 26, or 58 hexadecimal characters long. WEP was depreciated in 2004 because it was no longer secure and was replaced temporarily by WPA, which was quickly replaced by WPA2. WPA3 is the current and most secure standard.
74. You've been asked to set up a device that will be monitored using an SNMP agent and manager. What port will the SNMP manager use when polling the agent?

    1. TCP 143
    2. UDP 143
    3. TCP 161
    4. UDP 161

    Answer:

    D. Simple Network Management Protocol (SNMP) uses UDP port 161. User Datagram Protocol (UDP) is considered connectionless, so it does not guarantee delivery of data packets and has a lower network overhead than Transmission Control Protocol (TCP), a connection-oriented protocol, does. Port 143 is used for IMAP.
75. Because of a recent security breach, your IT team shut down several ports on the external firewall. Now, users can't get to websites by using their URLs, but they can get there by using IP addresses. What port(s) does the IT team need to open back up to enable Internet access via URLs?

    1. 20/21
    2. 53
    3. 67/68
    4. 80

    Answer:

    B. Clients are unable to get to the DNS server, which resolves hostnames (or URLs) to IP addresses. DNS uses port 53. Ports 20 and 21 are used for File Transfer Protocol (FTP). Ports 67 and 68 are used by Dynamic Host Configuration Protocol (DHCP). Port 80 is used for Hypertext Transfer Protocol (HTTP), and port 443 is HTTP Secure (HTTPS).
76. All your network hosts are configured to use DHCP. Which IP address would indicate that a host has been unable to locate a DHCP server?

    1. `192.168.1.1`
    2. `10.1.1.1`
    3. `172.16.1.1`
    4. `169.254.1.1`

    Answer:

    D. Automatic Private IP Addressing (APIPA) is a TCP/IP standard used to automatically configure IP-based hosts that are unable to reach a Dynamic Host Configuration Protocol (DHCP) server. APIPA addresses are in the `169.254.0.0/16` range. If you see a computer that has an IP address beginning with 169.254, you know that it has configured itself.
77. You have reason to believe that several network users are actively browsing prohibited content on unsecured sites on the Internet. Which port can you disable on the firewall to immediately stop access to these websites?

    1. 53
    2. 67
    3. 80
    4. 443

    Answer:

    C. Normal (unsecured) websites are accessed on port 80, which is the port that Hypertext Transfer Protocol (HTTP) uses. Shut it down, and no one will be able to access websites, except secure sites that use HTTPS, which is on port 443.
78. Which TCP/IP protocol is designed to help resolve hostnames to IP addresses?

    1. ARP
    2. RARP
    3. DHCP
    4. DNS

    Answer:

    D. The Domain Name System (DNS) is responsible for resolving hostnames to IP addresses. This is used millions of times daily on the Internet; when someone types in a website name, such as [`www.sybex.com`](http://www.sybex.com/), DNS will resolve that to an IP address to enable communication. Address Resolution Protocol (ARP) maps Internet addresses to hardware addresses. Reverse ARP (RAPR) does the opposite, and Dynamic Host Configuration Protocol (DHCP) assigns IP addresses to hosts automatically.
79. You need to install an Internet connection for a forest ranger outlook tower, located far away from electrical lines. Which option would be best for broadband Internet access?

    1. Cable
    2. DSL
    3. Fiber
    4. Satellite

    Answer:

    D. Satellite Internet is not much like any other type of broadband connection. Instead of a cabled connection, it uses a satellite dish to receive data from an orbiting satellite and relay station that is connected to the Internet. Because it requires a clear line of sight between the transmitter and receiver, it can be referred to as “line of sight” wireless. Mobile hotspot (cellular) devices are also an option, but they may not be able to reach the speed of a satellite connection and they depend on a strong cellular signal. For an installation far from civilization (and cell towers), satellite may be the only option. Cable, DSL, and fiber rely on lines that would not run as far as a forest ranger lookout tower.
80. Your customer will be moving their small office to a remote mountain village where there is no cable Internet access. They have heard that there is a wireless option available in the area that is faster than satellite but that requires an antenna and line-of-sight to a tower. What option have they heard about?

    1. Satellite
    2. DSL
    3. WISP
    4. Cellular hotspot

    Answer:

    C. Wireless Internet Service Providers (WISPs) use fixed wireless technology, which requires antennas to send radio waves between your location and a fixed hub on a tower or other tall structure similar to a cellular tower. Download speeds can be up to 1 Gbps. Satellite is an option in very remote areas but has the latency involved with traveling thousands of miles between the connection to the satellite and back again. Digital Subscriber Line (DSL) uses telephone lines to create an Internet connection, but many carriers no longer offer DSL. A cellular hotspot can be used in many remote locations but depends on connection to a cellular tower and is not as fast as satellite.
81. Which TCP/IP host-to-host protocol makes its best effort to deliver data but does not guarantee it?

    1. IP
    2. TCP
    3. UDP
    4. ICMP

    Answer:

    C. The two host-to-host protocols are Transmission Control Protocol (TCP) and User Datagram Protocol (UDP). TCP guarantees packet delivery through the use of a virtual circuit and data acknowledgments, and UDP does not. Because of this, TCP is often referred to as connection-oriented, whereas UDP is connectionless. IP and ICMP are not considered host-to-host protocols.
82. What type of network is typically defined as being contained within a single office or building?

    1. LAN
    2. WAN
    3. PAN
    4. MAN

    Answer:

    A. A local area network (LAN) is often defined as being contained in a single building, office, or home. The types of network based loosely on geography, from smallest to largest are PAN, LAN, MAN, WAN.
83. You are installing a wireless network for a small company. The management wants to have 1 Gbps or better wireless transmission rates. Which of the following standards will allow you to provide this? (Choose two.)

    1. 802.11ac
    2. 802.11ax
    3. 802.11g
    4. 802.11n

    Answer:

    A, B. 802.11a and 802.11g provide throughput that is only 54 Mbps, 802.11n (Wi-Fi 4) provides throughput over 100 Mbps (theoretically up to 300 Mbps), but 802.11ac (Wi-Fi 5) and 802.11ax (Wi-Fi 6) have far surpassed these standards with throughputs, over 1 Gbps and multiple Gbps, respectively.
84. Which of these standards operate in both the 2.4 GHz and 5 GHz frequencies? (Choose two.)

    1. 802.11ac
    2. 802.11ax
    3. 802.11g
    4. 802.11n

    Answer:

    B, D. 802.11ac operates in the 5 GHz frequency only. 802.11g is only 2.4 GHz. 802.11n and 802.11ax operate in both frequencies.
85. What legacy network protocol allows NetBIOS-dependent computer applications to communicate over TCP/IP?

    1. TFTP
    2. HTTPS
    3. NetBT
    4. BGP

    Answer:

    C. NetBIOS over TCP/IP (NetBT) is for older applications still reliant on NetBIOS, the legacy network protocol intended for very small networks. NetBT lets such applications communicate over TCP/IP. Trivial File Transfer Protocol (TFTP) is a basic connectionless protocol that allows file transfer functions without user interaction. Hypertext Transfer Protocol Secure (HTTPS) is a secure connection-oriented protocol that runs over port 443.
86. Which of the following features does not require a managed network switch?

    1. Priority of traffic
    2. VLAN configuration
    3. Direct packets out the proper port
    4. Port mirroring

    Answer:

    C. An unmanaged switch will simply perform the basic task a switch should do: direct network traffic out the correct destination port. Prioritizing traffic, configuring virtual LANs (VLANs), and mirroring ports are all jobs that are done using managed switches.
87. The senior network administrator struggles to configure company network devices spanning several cities. It's a challenge because they are required to be on premises for the network infrastructure of each building. What would be a cost-effective solution?

    1. Employ network administrators at each building.
    2. Go to a flat network.
    3. Train a local sales associate.
    4. Employ a cloud-based network controller.

    Answer:

    D. Migrating network configuration to the cloud would allow the network administrator to perform their duties without requiring travel.
88. What port(s) does DHCP use?

    1. 67/68
    2. 137/139
    3. 80
    4. 445

    Answer:

    A. DHCP uses ports 67/68. Ports 137/139 are for NetBIOS/NetBT. Port 80 is for HTTP, and port 445 is for SMB.
89. What is the maximum distance allowed between a power over Ethernet injector and the Ethernet device running on a 1000BaseT network?

    1. 50 meters
    2. 100 meters
    3. 250 meters
    4. 450 meters

    Answer:

    B. The distance for Power over Ethernet (PoE) is limited by the maximum distance set by the Ethernet cabling: 100 meters (328 feet). The power injector, the device that sources the electrical power to certain wires in the cable, can be as much as 100 meters from the powered device. The injector also needs to have sufficient power to match device needs, and devices must be compatible. PoE devices such as powered switches can provide a few watts or well over 100 watts, depending on the device.
90. Which of the following protocols uses port 137 and 139?

    1. DNS
    2. SMB
    3. NetBT
    4. SSH

    Answer:

    C. NetBT is NetBIOS over TCP/IP, an older protocol for applications that still rely on NetBIOS. It uses ports 137 and 139, and it's still on the CompTIA A+ certification objectives. DNS uses port 53, SMB uses port 445, and SSH uses port 22.
91. When setting up a small office, home office (SOHO) network, how do the end-user devices know what IP address they need to use to connect with the network?

    1. The network switch broadcasts configuration settings.
    2. Devices utilize service location protocol.
    3. The NIC is set with a static address or DHCP-served.
    4. End users configure IP addresses as needed.

    Answer:

    C. The end-user devices are configured to at least request a DHCP-assigned IP address or they are preconfigured with a static IP, gateway, subnet mask, and DNS information.
92. You've been asked to set up a wireless network for a SOHO that will only allow five specific devices to connect. How do you accomplish this?

    1. Disable the router's SSID.
    2. Configure port forwarding.
    3. Set a DHCP scope with only five addresses.
    4. Configure MAC address filtering.

    Answer:

    D. MAC address filtering uses the physical address of a NIC to determine whether or not to allow a device to connect to the router. Disabling the SSID will hide the network from neighbors, but it won't keep them from connecting if they discover the network. Port forwarding redirects requests for a specific port to a specific device on the network. The DHCP scope can be set up to only allow five machines to connect, but it may not be the right five machines.
93. What is the most likely way for a homeowner's IoT devices to connect to their wireless network?

    1. DNS
    2. AD
    3. SSO
    4. DHCP

    Answer:

    D. Unless an Internet of Things (IoT) device possesses an end-user accessible management interface, that device will likely connect at least initially using Dynamic Host Configuration Protocol (DHCP) to obtain an IP address. Domain Name System (DNS) resolves names like [`Wiley.com`](http://wiley.com/) to an IP address. AD is Active Directory, which is a Microsoft client-server security solution, and Single Sign-On (SSO) allows a user to enter their credentials once to access several resources.
94. What type of communication technology is being used at a fast-food restaurant when a customer places their phone next to a device to pay for their purchase?

    1. RFID
    2. NFC
    3. Wi-Fi
    4. HAV

    Answer:

    B. Near-field communication (NFC) requires devices to be within about 10 centimeters of each other to transmit data. In this case, the devices are working in card emulation mode, but NFC can also be used to transmit between two like devices, such as two cell phones, or to read a smart tag. Radio frequency identification (RFID) is another technology that uses radio waves to transfer information. Wi-Fi is 802.11-based wireless networking, and hardware-assisted virtualization (HAV) is virtualization that allows the virtual machine (VM) more direct access to the physical processor's capabilities.
95. What communication technology allows for low-power, passive reading of a small tag or patch on an object that may be a few feet to dozens of feet away?

    1. RFID
    2. NFC
    3. Wi-Fi
    4. RFI

    Answer:

    A. Radio frequency identification (RFID) can be implemented to detect and read a “passive” (no power) tag that is essentially an antenna as it passes within a few feet in range. RFID tags are often used in industry and retail for inventory tracking. The distance for RFID implementation depends on the size and polarization of the antenna, and the frequency and power used, among other features. NFC requires a distance of only a few centimeters. Wi-Fi is 802.11-based wireless networking. Radio frequency interference (RFI) is a nuisance that can disrupt network communications.
96. What type of server provides Internet access to company-provided information such as how to contact a company, products or services for sale, and other information?

    1. FTP server
    2. Proxy server
    3. File server
    4. Web server

    Answer:

    D. A web server consists of hardware and software used to provide information to remote clients via the Internet. The main protocols for web servers are HTTP and HTTPS, but they can use other protocols as well. File Transfer Protocol (FTP) servers are used for downloading files quickly, and while they may have a graphical user interface (GUI), they have much less overhead than a web server. Proxy servers are a security measure between an internal user and the web and are used to monitor and filter information going into or out of a network. File servers are often used on a LAN to provide access to the same files by multiple users.
97. A friend is showing you how they can control their thermostat at home from their cell phone while at work. What type of device do they have at home?

    1. IoT
    2. SQL
    3. DoS
    4. EFS

    Answer:

    A. Internet of Things (IoT) devices allow a multitude of personal and industrial devices to connect and communicate over the Internet. Structured Query Language (SQL) is a method of retrieving information from a database. Denial of service (DoS) is a type of network attack, and Encrypting File System (EFS) allows the user to encrypt individual files, folders, or volumes.
98. What server would function as a central repository of documents and provide network shared file storage for internal users?

    1. FTP server
    2. Proxy server
    3. File server
    4. Web server

    Answer:

    C. The file server is a centralized repository for users, typically company employees. File Transfer Protocol (FTP) servers are used for downloading files quickly, and while they may have a graphical user interface (GUI), they have much less overhead than a web server. Proxy servers are a security measure between an internal user and the web, and they are used to filter information going into or out of a network, whereas web servers may provide information about a company or its products to the general public.
99. You work as a network administrator for a school district. The district is required to provide access to the Internet for students but also required to protect the network and the students from malicious network traffic and inappropriate websites. What type of server do you need to configure?

    1. FTP server
    2. Proxy server
    3. File server
    4. Web server

    Answer:

    B. Proxy servers act as a gateway through which Internet access requests are handled, monitored, and, if need be, filtered. File Transfer Protocol (FTP) servers are used for downloading files quickly, and while they may have a graphical user interface (GUI), they have much less overhead than a web server. File servers are often used on a LAN to provide access to the same files by multiple users, whereas web servers may provide information about a company or its products to the general public.
100.    What type of server can host files for easy access and downloading, similar to how a web server serves web pages?

        1. FTP server
        2. Proxy server
        3. File server
        4. DNS server

        Answer:

        A. The File Transfer Protocol (FTP) server hosts files for easy access, allowing users to browse it and download and upload files. Proxy servers monitor and filter traffic into and out of a network. File servers are a repository of files accessed by multiple users on a network. A DNS server resolves human-readable names such as [`Wiley.com`](http://wiley.com/) to an IP address.
101.    You're a network administrator and just added a device to your network that allows multiple users to access several printers. What have you attached to the network?

        1. Syslog server
        2. DNS server
        3. Print server
        4. Authentication server

        Answer:

        C. A print server can be either a physical device or software configured on a computer. The print server provides centralized availability of print services to authorized users on the network. It accepts print jobs, and the documents are printed according to order of receipt or some configured priority. A syslog server gathers event information from devices on a network, creating a central repository for a network administrator to monitor and respond to events. A DNS server resolves domain names to IP addresses, and an authentication server verifies identity before allowing access to a network.
102.    What server is used to resolve domain names to IP addresses to facilitate web browsing or locating a directory resource on the network?

        1. Syslog server
        2. DNS server
        3. Print server
        4. Authentication server

        Answer:

        B. If a user types [`www.sybex.com`](http://www.sybex.com/) into a web browser, the Domain Name System (DNS) server will resolve the domain name to an IP address. Similarly, DNS servers will resolve a fully qualified domain named (FQDN) network directory resource on the network to make locating that resource possible. Syslog servers provide a repository of events on the network to aid in network management. Print servers provide and manage access to one or more printers by multiple users on a network, and an authentication server verifies identity before granting access to resources on a network.
103.    What server is accessed each time it's necessary to challenge and validate a user's credentials in order for the user to access a network resource?

        1. Syslog server
        2. DNS server
        3. Print server
        4. Authentication server

        Answer:

        D. The authentication server facilitates the challenge/response service for validating someone's credentials. Syslog servers provide a repository of events on the network to aid in network management. DNS servers resolve URLs to IP addresses, and print servers provide and manage access to one or more printers by multiple users on a network.
104.    What service can collect and journal all the system-generated messages produced by servers and network devices?

        1. Syslog server
        2. DNS server
        3. Print server
        4. Authentication server

        Answer:

        A. The syslog server operates with the Syslog protocol, which is used by many different operating systems and devices. These system-generated messages vary from the mundane “System started” to critical alerts. DNS servers resolve domain names to IP addresses. Print servers facilitate and manage printing by multiple users to one or more printers on a network, and authentication servers verify identity before granting access to a resource.
105.    You're configuring your phone to download and upload email. What type of server are you configuring your phone to use?

        1. Web server
        2. Authentication server
        3. Mail server
        4. FTP server

        Answer:

        C. Mail servers are used to send, receive, and sometimes store and manage emails. They operate on ports 25, 110, and 143. Often devices will need to be configured with the name or IP of the server and the proper protocol or port for sending and receiving email. Web servers provide web pages over the Internet. Authentication servers verify identify before allowing access to resources, and FTP servers are used to quickly locate, download, and upload files.
106.    Which of the following are connection-oriented protocols? (Choose two.)

        1. DHCP
        2. TFTP
        3. HTTPS
        4. SSH

        Answer:

        C, D. Connection-oriented protocols work over TCP, which guarantees delivery of packets. This guarantee requires greater resources than UDP, which is connectionless, therefore not requiring that a packet be resent if not received. HTTPS and SSH are connection-oriented protocols, whereas Trivial File Transfer Protocol (TFTP) and DHCP are connectionless protocols.
107.    A company wanting to monitor network traffic or host system behavior to identify suspect activity will install what type of service?

        1. Proxy server
        2. IDS
        3. UTM
        4. ATM

        Answer:

        B. An intrusion detection system (IDS) will monitor and alert you on suspect behavior. The IDS can be a network-based device or host-based, meaning it runs as a process in the background. Proxy servers are used to control traffic into and out of a network. Unified Threat Management (UTM) provides multiple security features on a single appliance. ATM (Asynchronous Transfer Mode) has to do with transferring different types of traffic (i.e., voice and data) over the same communication lines at the same time.
108.    What is the primary difference between an IDS and an IPS?

        1. IDS works both on a host and a network.
        2. IDS will not actively alert on suspect activity.
        3. IPS works in pairs.
        4. IPS will actively react to suspect activity.

        Answer:

        D. The intrusion detection system (IDS) will alert on suspect activity, but it will not react or actively attempt to block the activity. The intrusion prevention system (IPS), however, should attempt to block the activity.
109.    Managing security on your growing network has become difficult, so you ask your peers what they are doing to manage their networks. They recommend a device that will allow you to manage your security in one place. What have they recommended?

        1. IDS
        2. IPS
        3. UTM
        4. UTP

        Answer:

        C. Unified Threat Management (UTM) systems can be hardware networking devices, virtual devices, or an off-premises service. UTM's role is to combine several security features and services into a single device, allowing for easier management and compatibility. IDSs (intrusion detection systems) will only notify an admin if a threat is detected. Intrusion protection systems (IPSs) will detect and respond to security threats. UTP is unshielded twisted pair, a type of network cabling.
110.    A switch is overheating, and the SNMP agent is sending an SNMP trap to an SNMP manager. Which of the following are true? (Choose two.)

        1. It is a managed switch.
        2. It is an unmanaged switch.
        3. It is communicating on port 161.
        4. It is communicating on port 162.

        Answer:

        A, D. A Simple Network Management Protocol (SNMP) trap is unrequested information being sent from an SNMP agent, in this case running on a managed switch. SNMP traps are sent via port 162.
111.    Your cousin is a nature photographer, traveling the country and living in their Class A motorhome. Much of the time their motorhome is parked in a national park, but seldom is Wi-Fi available. Your cousin uploads photos from their camera to a laptop, modifies them, and needs to upload them to their publisher, various magazines, and their website on a regular basis. What is a viable networking option for your cousin?

        1. Satellite
        2. Cellular
        3. WISP
        4. DSL

        Answer:

        B. Cellular is the only type of network connection that allows for the type of mobility that this photographer needs. A cellular hotspot device from a mobile provider would work well. Satellite would require repositioning of the dish on a regular basis and may not work well because of obstructions. WISP requires being within a few miles of a tower and line-of-sight between the antenna and tower, so that wouldn't work well either. DSL requires a stationary phone line.
112.    Based on the drawing, what is the device labeled A?

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c02uf001_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

        1. Switch
        2. Hub
        3. Cable modem
        4. Cable multiplexer

        Answer:

        C. Cable Internet service requires a cable modem to separate the Internet signal from TV channels and to convert the signal into one that your computer can use. A switch is used on a LAN as a central connection point. A hub for networking is an obsolete device that would send any signal it received out of all of its ports. A cable multiplexer connects several signals into one for transmission over a cable, such as input from multiple security cameras.
113.    What is the device in the image used for?

        <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c02uf002_0.jpg" alt="" height="1000" width="754"><figcaption></figcaption></figure>

        1. It multiplexes several signals into one.
        2. It's a network cable tester.
        3. It's for attaching RJ45 connectors to cable.
        4. It's for testing Wi-Fi signal strength.

        Answer:

        B. This device is for testing cables that are terminated with an RJ45 connector.
114.    You are a network administrator. Currently there is no wireless access to the business network, but the company is purchasing tablets so that employees can take their work with them as they move around the facility. What device will you install so that employees will be able to connect to the wired network with wireless devices?

        1. Ethernet router
        2. Proxy server
        3. WAP
        4. NFC hub

        Answer:

        C. You need to add a wireless access point (WAP), which will have an RJ45 port to connect to the company server and Wi-Fi antennas to provide wireless connectivity. An Ethernet router is wired. A proxy server is a security device. NFC, although wireless and using radio waves, is for connecting devices within a few centimeters of each other.
115.    Last weekend you installed and booted several more computers to be ready for Monday morning. Later Monday morning you hear from employees as they come in that they cannot log in. Their desktops don't seem to want to connect. You investigate and find that each faulty workstation has a `169.254.x.x` IP address. What might you look at next?

        1. DHCP scope
        2. LAN connector broken
        3. Windows patch unable to install
        4. Corrupted Registry

        Answer:

        A. With many new systems added and already booted, it is likely that the DHCP scope, which is a valid range of IP addresses that are available to client-based systems on a particular subnet, is now too small for the number of systems requesting IP addresses. Expand the DHCP scope to solve the problem.
116.    What network segmentation technique reduces broadcast domains and provides a layer of security between users on the same network?

        1. VPN
        2. VLAN
        3. UPS
        4. SQL

        Answer:

        B. Virtual LANs, or VLANs, will segment your network into smaller broadcast domains. Multiple VLANs can exist on the same physical switch. Traffic is isolated to only the paths determined by how you have identified VLANs on your managed switches. A VPN (virtual private network) uses tunneling protocols to secure a private connection across a public network. A UPS (uninterruptable power supply) is a battery backup with other features used to maintain power to a device when the main power goes down, and SQL (Structured Query Language) is used to retrieve information from a database.
117.    One of your network users must work remotely from their office on an extremely confidential project. Their team is concerned about security so they call you, the IT department head, to see what can be done. What will you set up between this network user and the company server so that the communications are secure?

        1. VPN
        2. SDN
        3. VLAN
        4. SRAM

        Answer:

        A. A virtual private network (VPN) uses encryption to secure a transmission across a public network. SDN (software-defined networking) is a network architecture designed to make managing a network easier and more flexible. A VLAN separates a LAN into separate broadcast domains and is used for security purposes. SRAM, or static RAM, is often found in processor cache.
118.    Which of the following components is not typically found in a wireless LAN (WLAN)?

        1. WLAN router
        2. WLAN gateway
        3. WLAN server
        4. WLAN client

        Answer:

        C. Wireless LAN (WLAN) networks commonly have three types of nodes: a client, a router, and a gateway. They typically don't include a server and often are of fluid nature, where devices come and go as needed. They may include a printer. A WLAN can be used to connect wireless users to a wired network.
119.    You need to configure dynamic IP addressing on your network to cut down on management time. How will you do this? (Choose two.)

        1. Enable DHCP settings on the router.
        2. Configure each NIC to obtain an IP address automatically.
        3. Configure each NIC to a specific IP address.
        4. Configure each NIC to obtain DNS server addresses automatically.

        Answer:

        A, B. A NIC can be configured either with a specific (static) IP address, or to obtain an IP address from an available Dynamic Host Configuration Protocol (DHCP) server. Many routers have the capability to provide DHCP services. When a device with a properly configured NIC attempts to join a network, a request for an address will be sent to the DHCP server, and the DHCP server will lease an address to that device, if one is available.
120.    Your network admin needs to add a computer to an IPv6 subnet. Which of the following IPv6 addresses is on the same subnet as `2601:0:0:0f:1a:308c:2acb:fee2`?

        1. `2601::of:308c:47:4321`
        2. `2601::0f:ab:cd:123:4a`
        3. `fe80:ab:bc:0f:1a:308c:2abc:fee5`
        4. `2601:0:0:0x::2acb:ac01`

        Answer:

        B. Option B, `2601::0f:ab:cd:123:4a`, and the address in the question both have a subnet of `0f`. IPv6 addresses consist of 128 bits, divided by colons (:) into 8 hextets. Therefore, each hextet represents 16 bits. Leading 0s can be omitted, and in one place in each address, consecutive groups of 0s can be omitted, represented by double colons (::). The last 64 bits (4 hextets) of an IPv6 address are the Interface ID, identifying the unique computer. The first 64 bits are called the prefix. ISPs and very large organizations are assigned /48 prefixes. The next 16-bits (the fourth hextet) are used to define subnets. Option A has a fourth hextet of 0. Option C is a link-local address. Option D is an invalid number because hex numbers only go to letter f.
121.    Dylan is troubleshooting his IPv4 network. The network's subnet mask is `255.255.192.0.` Which of the following IP addresses is _not_ on the same network as the others?

        1. `130.200.65.5`
        2. `130.200.130.1`
        3. `130.200.100.4`
        4. `130.200.125.5`

        Answer:

        B. The third octet's subnet mask of 192 means that the first 2 bits of the octet are used to identify the network number, so the network can be broken down into four subnets using those first 2 bits of the octet. The subnets would be 00000000, 01000000, 10000000, and 11000000. IP addresses within each range would be 0 to 63, 64 to 127, 128 to 191, and 192 to 255. The first and last IP in each range would not be used because they would represent the subnet itself and the broadcast numbers. Options A, C, and D all fall in the second subnet's range. Option B is in the third subnet.
122.    Which of the following is a PoE standard?

        1. 802.3bt
        2. 802.3b
        3. 802.11
        4. 802.11ax

        Answer:

        A. The PoE standards are IEEE 802.3af (PoE), 802.3at (PoE+), and 802.3bt (PoE++). A main difference between the standards is how much power per port can be provided. 802.3af can supply up to 15.4 watts per port, 802.3at can provide up to 30 watts per port, and 802.3bt can provide 60 watts (Type 3) or 100 watts (Type 4). The power that actually reaches the devices is less due to voltage loss over distance. 802.3b is a legacy broadband Ethernet standard. 802.11 and802.11ax are Wi-Fi standards.
123.    Your friend has purchased a PoE device for their home. It is a type 2 device. Which of the following PoE switches will be compatible with this device? (Choose two,)

        1. 802.3af-compliant switch
        2. 802.3at-compliant switch
        3. 802.3bt-compliant switch
        4. 802.11b-compliant switch

        Answer:

        B, C. PoE devices providing power are backward compatible with older devices, meaning that while 802.3bt is rated at 60W for Type 3 and 10W for Type 4, an 802.3bt device will work with an 802.3at (Type 2) device. Option A would not provide enough power for your friend's device. Option D is a Wi-Fi standard, not a PoE standard.
124.    Which of the following is true of an ONT? (Choose two.)

        1. It stands for optical network terminator.
        2. It converts fiber-optic light signals to electrical (Ethernet) signals.
        3. It is user installed.
        4. It requires external power to work properly.

        Answer:

        B, D. ONT (optical network terminal) is installed by a fiber-optic ISP, and it's typically a small box on an outside wall. The terminal is a transducer, converting between copper/electrical signals and fiber-optic/light signals. It does require power, and the terminal may have an indicator light to signal whether it is receiving power.
125.    Which of the following is not a benefit of software-defined networking (SDN)?

        1. Dynamic load balancing
        2. Reduced infrastructure costs
        3. Requires a cloud-based network
        4. Centrally manage physical and virtual routers

        Answer:

        C. Software-defined networking (SDN) has many advantages over traditional networking. It can work with virtual and physical networks using SDN-compatible devices, providing centralized control of the entire network and the ability to reconfigure networks often without having to physically touch a router or switch.
126.    Which type of WISP radio frequency has the advantages of no fees, less expensive equipment, and a wide pool of practical knowledge so help is easier to find?

        1. Licensed
        2. Unlicensed
        3. Limited
        4. Unlimited

        Answer:

        B. Frequencies for wireless Internet service providers (WISPs) can be licensed or unlicensed. (The FCC is the licensing body.) Most WISPs use the unlicensed frequencies because they are free to use.
127.    You are working with your customer, a doctor's office, to develop a network that will allow the doctor's staff to work with their tablet PCs in any room of the office without having to worry about network cabling. What type of network will you establish for the doctor's office?

        1. LAN
        2. VLAN
        3. WLAN
        4. WAN

        Answer:

        C. A wireless LAN (WLAN) would be the best solution for this office. A WLAN is a group of devices in the same location that communicate via radio waves instead of cables. WLANS can have multiple wireless access points (WAPs), preferably overlapping so that users won't experience signal drop. Wi-Fi is a type of WLAN. A LAN is incorrect because it would require disconnecting and reconnecting cables in each room. A VLAN (virtual LAN) is established using security protocols to segregate a network. WAN is incorrect because this is a network in a single office, not geographically distant computers.
128.    Which of the following is a network of storage devices that a server can access as if it were a locally connected drive?

        1. NAS
        2. SAS
        3. SAN
        4. WAN

        Answer:

        C. A storage area network (SAN) is a high-speed network whose purpose is to provide fast access by servers to storage. Network attached storage (NAS) differs from a SAN in that it is not a separate high-speed network but a single storage device attached to a LAN. SAS is statistical analysis software, and WAN is wide area network.
129.    Which of the following is true of a network TAP? (Choose two.)

        1. TAP stands for terminal access point.
        2. It is solely used by hackers to intercept packets.
        3. It is part of a router.
        4. It allows network admins to monitor network traffic.

        Answer:

        A, D. A network terminal access point (TAP) connects to a network in an area of concern and creates a copy of traffic, sending it on to monitoring devices. It can be an integral part of network management. TAPs can be active or passive. Passive TAPs do not require power or management, but active TAPs do.
130.    What software runs on a machine where data files to be accessed are housed and controls access to those files as requested by a client?

        1. CAL
        2. Fileshare server
        3. Fileshare client
        4. SAN

        Answer:

        B. A fileshare server handles requests from fileshare clients for access to data stored on the server. The fileshare server resides on the same machine as the data. A client access license (CAL) is a license allowing one machine to connect to a server, and SAN is a storage area network, both of which are unrelated to the question.
131.    A friend is having some issues with the wireless network in their apartment dropping the connection or running very slowly. What tool can be used to determine the best channel to use?

        1. WAP
        2. Wi-Fi analyzer
        3. Toner probe
        4. Cable tester

        Answer:

        B. A wireless access point (WAP) provides wireless LAN (WLAN) connectivity, but it may not help with the problems on this network. Your friend needs to determine what wireless channel has the least traffic and configure their Wi-Fi to use that channel. For that they need a Wi-Fi analyzer, which can be a separate device or as simple as an app on a smartphone. A toner probe is used to figure out which network cable is connected when they are not labeled, and a cable tester determines if the cable's wires are connected properly.
132.    In the United States, the Federal Communications Commission (FCC) imposes rules that govern radio communications. What is the maximum EIRP (watts) that can be transmitted in the 2.4 GHz band for a point-to-multipoint WISP connection?

        1. 2 watts
        2. 4 watts
        3. 158 watts
        4. 125 mw

        Answer:

        B. Wireless Internet service providers (WISPs) that are operating in the 2.4 GHz band are limited to 4 watts of effective isotropic radiated power (EIRP) for their point-to-multipoint connections. Their point-to-point connections vary between 4 watts and 158 watts for the 2.4 GHz band. The maximum EIRP for the 5 GHz bands is 125 mw. FCC maximums can be found at FCC maximums can be found at [`www.air802.com/fcc-rules-and-regulations.html`](http://www.air802.com/fcc-rules-and-regulations.html).
133.    Using which Wi-Fi channels does not require that your router has Dynamic Frequency Selection (DFS) and Transmit Power Control (TPC) built into the router?

        1. Channels 36 to 48
        2. Channels 52 to 64
        3. Channels 100 to 144
        4. Channels 149-165

        Answer:

        A. Channels 36 to 48 are set aside for domestic use. All channels above that require a router to have DFS and TPC. DFS will automatically switch to a different channel when weather radar and radar system signals are detected. TPC can be used to force clients to lower power so that they won't interfere with nearby users or access points on the same channel. Channel 165 is set aside for industrial, scientific, and medical (ISM) use. In the United States, the FCC and IEEE are the authorities that approve channel uses.
134.    Which broadband network communications technology became more competitive with other types of service when, in 2021, the FCC ruled to include it in the Over-The-Air-Reception Devices Rule (OTARD), which protects the rights of those organizations to place antennas where they are needed?

        1. Fios
        2. Long-range fixed wireless
        3. DSL
        4. Satellite

        Answer:

        B. The FCC's ruling was expanded to include long-range fixed wireless hub or relay antennas and the customer's right to place antennas of certain sizes on their premises, putting WISP providers on a more equal footing with satellite and cellular providers.
135.    What is the host number in an IP address of `192.168.2.200` and a subnet mask of `255.255.255.0`?

        1. `192.168`
        2. `192.168.2`
        3. `2.200`
        4. `200`

        Answer:

        D. When an IP address and subnet mask are converted to the binary numbers that the computer sees, wherever there is a 1 in the subnet mask, that tells the computer that the corresponding bit in the IP address is part of the network number. Wherever there is a 0 in the subnet mask, the corresponding bit in the IP address is part of the host number. The address in the question, `192.168.2.200/24`, is a Class C private address, where, in the subnet mask, the first three octets (24 bits) are all 1s, and the last octet (8 bits) are 0s. So, the first three decimal numbers of the IP address, which is expressed in dotted decimal notation, are the network number, (`192.168.2`) and the last octet (`.200`) is the host (individual computer) address. Network numbers will always go from left to right with no breaks between.
136.    What are the three A's employed by authentication servers?

        1. Authentication, activation, acceptance
        2. Authorization, access, allocation
        3. Accept, access, accounting
        4. Authentication, authorization, accounting

        Answer:

        D. Authentication servers provide the AAA framework for security. Authentication requires that an entity prove who they are before gaining access. Authorization grants the authenticated user access to resources. Accounting tracks user activity.
137.    Which Internet appliance is used to distribute incoming traffic over resources, such as multiple web servers?

        1. Proxy servers
        2. Spam gateways
        3. Load balancers
        4. UTM device

        Answer:

        C. Load balancers do as their name implies. Rather than allow all incoming traffic on a port to go to one server or device, the traffic is distributed among devices. Proxy servers monitor incoming and outgoing packets, filtering them out based on specified criteria. Spam gateways don't allow spam in; rather they are used to filter it out. Unified threat management (UTM) can employ an appliance or be software-driven, or even an outside service that monitors and manages malicious activities against a network.
138.    What type of system, consisting of both hardware and software, is used to control and monitor industrial machines and processes?

        1. SCADA
        2. IrDA
        3. UTM
        4. RADIUS

        Answer:

        A. Supervisory Control and Data Acquisition (SCADA) systems consist of both hardware and software. Hardware is used to gather information, which is sent to a computer running software that analyzes the data and logs events. SCADA can also initiate alarms when specified conditions exist. Infrared Data Association (IrDA) is network communications via infrared light. Unified threat management (UTM) is an appliance, software, or service that combines all malware security in one place. Remote Authentication Dial-In User Service (RADIUS) is a protocol for authentication servers that encrypts transmissions between client and server.
139.    Your friend owns a restaurant and provides free Wi-Fi to their clientele. Lately they have been receiving complaints that the Wi-Fi isn't working. It seems to work for customers already connected but not for people trying to connect. What can be configured on the router to release an IP address and make it available for other users after a couple of hours?

        1. MAC address filtering
        2. Port forwarding
        3. DHCP lease duration
        4. SSID broadcast

        Answer:

        C. A DHCP server will “lease” an IP address to a client for a specified period of time. The default is usually 24 hours. In a SOHO where there are few new users, the lease time could be longer, but in a restaurant where many people come and go each hour, the DHCP scope might not have enough addresses to accommodate that many users. Setting the lease time to a shorter duration will release the IP address and make it available for a new user. MAC address filtering only allows connection from computers with specific MAC addresses and would greatly limit connectivity. Port forwarding sends traffic for a specific port to a specified computer on the network. The SSID is the wireless network name and can be broadcast so that it is easily found, or it can be hidden.
140.    What type of address is known as a DNS AAAA address?

        1. IPv4
        2. IPv6
        3. MAC
        4. Physical

        Answer:

        B. The Domain Name System (DNS) uses two types of records to resolve domain names to IP addresses. Type A records resolve the domain name to IPv4 addresses. Type AAAA records resolve domain names to IPv6 addresses. MAC and Physical addresses are two names for the NIC address.
141.    What type of entry in a DNS record can be used for load balancing of incoming mail?

        1. MX
        2. DX
        3. AAAA
        4. TXT

        Answer:

        A. Multiple Mail Exchanger (MX) records can be set up for a domain that specify different mail servers for load balancing. Direct Connect (DX) is an Amazon Web Services dedicated connection between client and AWS. AAAA signifies an IPv6 address in a DNS record, and TXT DNS records let an administrator specify text in their DNS record. These text records can be used to prevent email spam.
142.    What type of DNS record contains a list of users (IP addresses) that are authorized to send email on behalf of a domain?

        1. DKIM
        2. SPF
        3. DMARC
        4. A

        Answer:

        B. Sender Policy Framework (SPF) is a technique to prevent email address spoofing. It is done using a TXT entry in a domain's DNS service. DomainKeys Identified Mail (DKIM) performs a similar function, but it uses a digital signature. Domain-Based Message Authentication, Reporting, and Conformance (DMARC) uses SPF or DKIM and in addition requires that the sender's domain be the same as the DNS domain name. Domain administrators can specify to quarantine or reject emails that fail DMARC. To use DMARC, a DMARC record must exist in the DNS.
143.    What is the interface ID of the IP address `2001::1a3:f1a:308:833`?

        1. `2001:0:0:0:`
        2. `2001`
        3. `1a3:f1a:308:833`
        4. `833`

        Answer:

        C. This is an IPv6 address. It is 128 bits long, and the last 64 bits are the interface ID, which identifies the individual computer. Since there are eight groups of hex numbers, that means the rightmost four groups are the interface ID. Any leading zeros in an IPv6 address can be omitted, and the :: can be used once in an address to replace consecutive groups of all zeros, so the number in the question fully expanded would be `2001:0000:0000:0000:01a3:0f1a:0308:0833`. The interface ID is therefore `1a3:f1a:308:833`. The leftmost three sections identify the network, and the fourth identifies the subnet. In this example, `2001:0:0` is the site prefix and 0 is the subnet ID. IPv6 addresses do not need a subnet mask like IPv4 addresses do.
144.    What two terms are used to identify an Internet provider that may connect to the Internet using T1 or T3 lines, or fiber optic, for example, and uses point-to-point millimeter-wave or microwave links between its towers for its backbone or to extend its service area, and point-to-multipoint wireless to provide Internet access to its customers?

        1. WISP
        2. ISP
        3. Demarcation point
        4. Long-range fixed wireless

        Answer:

        A, D. For decades now, wireless Internet service providers (WISPs) have been established by groups of individuals or small companies to provide Internet access to areas where it is not profitable for large commercial Internet providers to run, such as very rural areas. They are also called long-range fixed wireless providers. The first one was established in 1992 in the Midwest of the United States. Now there are thousands of them all over the world. In some areas of the world, where there is little or no wired infrastructure, WISPs are the only way that people can get Internet connectivity. A WISP connects to the Internet using either leased lines or microwaves, generally uses point-to-point microwaves between its towers, and uses point-to-multipoint connections between the final tower and users. An ISP is an Internet service provider, and a demarcation point is the place in a customer’s premises where the responsibility for the network changes from the ISP to the customer.
145.    Your friend is again considering the network configuration in their apartment. They've asked you the difference between channels on the 2.4 GHz and 5 GHz networks that are available on their Internet connection. What will you tell them? (Choose two.)

        1. If they are using the 2.4 GHz network, they should choose channel 1, 6, or 11 because they don't overlap each other.
        2. The 5 GHz network channels provide greater bandwidth, so data could be transferred faster, but they may have more interference with their neighbors.
        3. The 5 GHz frequency is considered obsolete, so the 2.4 GHz frequency should be used.
        4. All of the 5 GHz frequencies overlap, so there will be greater interference.

        Answer:

        A, B. Option A is true. Channels 1, 6, and 11 are the only ones that don't overlap in a 2.4 GHz network. Option B is also true. Each channel in a 2.4 GHz network is only about 5 MHz wide, while in a 5 GHz network the minimum is 20 MHz, but it can be configured to use 40 MHz or 80 MHz by combining channels. Option C is false. The 2.4 GHz frequency supports older devices; the 5 GHz frequency is newer. While 2.4 GHz channels overlap with the exception of 1, 6, and 11, 5 GHz channels don't overlap. Your friend needs to choose a frequency and channel that are compatible with their devices, but the router may automatically configure the channel if using the 5 GHz frequency.
146.    Which IEEE Wi-Fi standard is also known as Wi-Fi 6?

        1. 802.11a
        2. 802.11ac
        3. 802.11ax
        4. 802.11n

        Answer:

        C. The Institute of Electrical and Electronics Engineers (IEEE) 802.11ax standard is now known as Wi-Fi 6, and is considered a replacement for 802.11ac (Wi-Fi 5). 802.11n is designated as Wi-Fi 4. Prior IEEE standards (802.11b, 802.11a, and 802.11g) are not designated with official Wi-Fi _X_ nomenclature, but working backward in time, 802.11g would be Wi-Fi 3, 802.11a would be Wi-Fi 2, and 802.11b would be Wi-Fi 1. The CompTIA A+ objectives only ask that you know what Wi-Fi 5 and Wi-Fi 6 are.
