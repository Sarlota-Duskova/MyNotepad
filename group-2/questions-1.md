# Questions

1.  Which of the following technologies associated with the Internet of Things (IoT) is often used to identify pets using embedded chips?

    1. Z-wave
    2. Bluetooth
    3. NFC
    4. RFID

    Answer:

    D. Radio-frequency identification (RFID) uses tags containing data, frequently embedded in pets, which can be read using electromagnetic fields. Z-wave is a short-range wireless technology, frequently used for home automation. Bluetooth is a short-range wireless protocol, frequently used for computer peripherals and Personal Area Networks (PANs). Near-field communication (NFC) provides wireless communication over ranges of 4 cm or less, and it is often used for payment systems.
2.  Which of the following is typically _not_ an example of the Internet of Things (IoT)?

    1. A key fob that unlocks your car
    2. A smartphone home automation app
    3. A remotely monitored cardiac pacemaker
    4. A seismic early warning system

    Answer:

    A. A key fob that unlocks your car is typically a short-range radio or infrared device that does not use the Internet for its communications. Each of the other examples describes a device with an IP address that uses the Internet to communicate with a controller or monitoring station.
3.  A Wireless Access Point (WAP) enables computers equipped with wireless network interface adapters to function in which of the following topologies?

    1. Star
    2. Ad hoc
    3. Bus
    4. Infrastructure

    Answer:

    D. A WAP is a device with a wireless transceiver that also connects to a standard cabled network. Wireless computers communicate with the WAP, which forwards their transmissions over the network cable. This is called an infrastructure topology. A star or bus network requires the computers to be physically connected to the network cable, and an ad hoc topology is one in which wireless computers communicate directly with one another.
4.  Ralph has been hired by a company to redesign its Local Area Network (LAN). Right now, it has a single 100 Mbps Ethernet LAN with 40 users and 2 shared servers, all connected through 3 hubs. The users on the network must be able to share files with one another and also access the shared servers. The users are complaining that the network is too slow. Management states that cost is a factor that must be considered. Which of the following upgrade scenarios should Ralph recommend in this situation?

    1. Split the network into smaller segments with dedicated hubs as opposed to shared hubs.
    2. Split the network into two routed LANs with 20 users each.
    3. Replace the hubs with switches to define separate collision domains and filter unnecessary traffic from each segment.
    4. Replace the hubs with a layer 3 switch and define two Virtual LANs (VLANs) with 20 users each.

    Answer:

    C. The best choice is to replace the hubs with switches, since the network is relatively small, and cost is an issue. On the existing network, all users share the same 100 Mbps communication channel, and each computer must take turns transmitting. By replacing the hubs with switches, you provide each computer with a dedicated 100 Mbps connection to the switch, while reducing unnecessary traffic and collisions on the network. There is no such thing as a dedicated hub. Splitting the network into two routed LANs is not the best solution, because all users must share information on a constant basis. Also, cost is a factor, and routers are more expensive than switches. Replacing the hubs with a layer 3 switch and defining two VLANs with 20 users each is not a reasonable solution, because layer 3 switches are very expensive.
5.  Which of the following devices can split a single network into two collision domains while maintaining a single broadcast domain?

    1. Hub
    2. Bridge
    3. Switch
    4. Router
    5. Repeater

    Answer:

    B. A bridge can split a single network into two collision domains, because it forwards only the packets that are destined for the other side of the bridge. The bridge forwards all broadcast packets, so it maintains a single broadcast domain. A hub maintains a single collision domain and a single broadcast domain. A switch creates a separate collision domain for each port, and a single broadcast domain for the entire network. A router creates two collision domains, but it does not forward broadcasts, so there are two broadcast domains as well. A repeater is a physical layer device that amplifies signals; it does not affect collision domains.
6.  Which two of the following functions is the multifunction device on a home or small office network known as a broadband router least likely to provide? (Choose two.)

    1. Wireless Access Point (WAP)
    2. Switch
    3. Proxy server
    4. DHCP server
    5. VPN headend

    Answer:

    C, E. Broadband routers generally do not function as proxy servers, which are application layer devices used to regulate access to the Internet. They are also typically not Virtual Private Network (VPN) headends, which enable multiple remote VPN clients to connect to the network. Many broadband routers are also WAPs, enabling users to construct a LAN without a complicated and expensive cable installation. Many broadband routers have switched ports for connections to wired devices, such as printers and computers. Most broadband routers use DHCP to assign IP addresses to devices on the private network.
7.  Which of the following devices run exclusively at the physical layer of the Open Systems Interconnection (OSI) model? (Choose all that apply.)

    1. Routers
    2. Hubs
    3. Repeaters
    4. Switches

    Answer:

    B, C. A repeater is a physical layer device that amplifies the signals entering it and transmits them again. A hub is a physical layer device that propagates incoming signals out through all of its ports. Switches and routers have physical layer elements but are primarily data link and network layer devices, respectively.
8.  Which of the following is the true definition of the term _modem_?

    1. A device that connects a computer to the Public Switched Telephone Network (PSTN)
    2. A device that connects a Local Area Network (LAN) to the Internet
    3. A device that converts analog signals to digital signals and back again
    4. A device that connects a Local Area Network (LAN) to a Wide Area Network (WAN)

    Answer:

    C. A modem (modulator/demodulator) is any device that converts analog signals to digital signals and digital signals back to analog signals. The digital device does not have to be a computer, and the analog device does not have to be the PSTN. There are many devices that are incorrectly referred to as modems, such as devices that connect a digital LAN to a digital WAN or all-digital devices that connect computers to the Internet.
9.  Which of the following devices is used to physically connect computers in the same Virtual Local Area Network (VLAN)?

    1. A bridge
    2. A hub
    3. A switch
    4. A router

    Answer:

    C. Replacing routers with switches turns an internetwork into a single large subnet, and VLANs exist as logical elements on top of the switching fabric. Although VLANs are the functional equivalent of network layer subnets, the systems in a single VLAN are still connected by switches, not routers. Bridges connect network segments at the data link layer and selectively forward traffic between the segments. However, bridges do not provide a dedicated connection between two systems like a switch does, and they do not make it possible to convert a large, routed internetwork into a single switched network. Therefore, they have no role in implementing VLANs. Hubs are physical layer devices that propagate all incoming traffic out through all of their ports. Replacing the routers on an internetwork with hubs would create a single shared network with huge amounts of traffic and collisions. Hubs, therefore, do not connect the computers in a VLAN.
10. Which of the following best describes the function of a firewall?

    1. A device located between two networks that enables administrators to restrict incoming and outgoing traffic
    2. A device that connects two networks together, forwarding traffic between them as needed
    3. A device that enables Internet network clients with private IP addresses to access the Internet
    4. A device that caches Internet data for subsequent use by internal network clients

    Answer:

    A. A firewall is a filter that can prevent dangerous traffic originating on one network from passing through to another network. A device that connects two networks together and forwards traffic between them is a router, not a firewall. A device that enables Internet network clients with private IP addresses to access the Internet is a description of a NAT router or a proxy server, not a firewall. A device that caches Internet data is a proxy server or caching engine, not a firewall.
11. Which of the following terms is used to describe the method by which a firewall examines the port numbers in transport layer protocol headers?

    1. IP address filtering
    2. Service-dependent filtering
    3. Deep Packet Inspection (DPI)
    4. Next-Generation Firewall (NGFW)

    Answer:

    B. Service-dependent filtering blocks traffic based on the port numbers specified in the transport layer header fields. Because port numbers represent specific applications, you can use them to prevent traffic generated by these applications from reaching a network. IP address filtering operates at the network layer. DPI scans the contents of packets, rather than their headers. NGFW defines a device with advanced protection capabilities; port number scanning is a basic firewall function.
12. Which of the following devices can also be described as a multiport repeater?

    1. Hub
    2. Bridge
    3. Switch
    4. Router

    Answer:

    A. A repeater is a physical layer device that regenerates incoming signals and retransmits them. A hub is a type of repeater that receives data through any one of its multiple ports and retransmits the data out through all of its other ports. Bridges and switches are data link layer devices, and routers are network layer devices. None of these three can be described as multiport repeaters.
13. Which of the following bridging types has never been used on Ethernet Local Area Networks (LANs)?

    1. Store and forward
    2. Transparent
    3. Source route
    4. Multiport

    Answer:

    C. Source route bridging was a technique used on Token Ring (and not Ethernet) networks, in which a Routing Information Field (RIF) in the packet header identified the network segments the packet should follow to reach its destination. Store and forward, transparent, and multiport bridges have all been used on Ethernet networks.
14. Which of the following physical network devices can conceivably be implemented as software in a computer's operating system? (Choose all that apply.)

    1. Hub
    2. Switch
    3. Router
    4. Firewall

    Answer:

    C, D. Most operating systems are capable of functioning as routers or firewalls. To route traffic, the system must have two network connections. A software firewall can be part of a computer's routing functionality, or it can be a stand-alone firewall that protects only the local system. Computers cannot function as hubs or switches, because multiple ports would be required, and standard network adapters do not implement those functions.
15. Which of the following criteria does a firewall capable of service-dependent filtering use to block traffic?

    1. Hardware addresses
    2. Protocol identifiers
    3. IP addresses
    4. Port numbers

    Answer:

    D. Service-dependent filtering blocks traffic based on the port numbers specified in the transport layer header fields. Because port numbers represent specific applications, you can use them to prevent traffic generated by these applications from reaching a network. IP address filtering enables you to limit network access to specific computers; it is not service dependent. Filtering based on hardware addresses provides the same basic functionality as IP address filtering, but it is more difficult to spoof hardware addresses than IP addresses. Filtering by protocol identifier enables you to block all traffic using TCP or UDP; it is not service dependent.
16. Ralph is a freelance network consultant installing a three-node small business network. The computers are all in the same room and use wired Ethernet to connect to the switched ports of a multifunction device. The device also functions as a Network Address Translation (NAT) router for a cable modem connection to the Internet. NAT provides a measure of security, but Ralph wants to be sure that the network is protected from unauthorized Internet traffic and attacks against open ports. Which of the following solutions would enable Ralph to accomplish this goal with the minimum cost to the client?

    1. Install a hardware firewall between the multifunction device and the cable modem.
    2. Install an Intrusion Prevention System (IPS) between the multifunction device and the cable modem.
    3. Install a personal firewall on each of the computers.
    4. Connect an Intrusion Detection System (IDS) to one of the switched ports in the multifunction device.
    5. Use a port scanner to monitor the traffic entering the open ports on the computers.

    Answer:

    C. A personal firewall is an inexpensive way to protect an individual computer from Internet incursions. Installing a hardware firewall is a complex and expensive solution, not suitable for a small network. An IPS is a relatively expensive solution, suitable for larger networks. An IDS is also expensive, and connecting it to a switched port would not enable it to protect the other computers on the network. A port scanner is a device that performs scans on demand. It does not continuously monitor ports, and it does nothing to protect them.
17. Which of the following statements about hubs and switches are true? (Choose all that apply.)

    1. Hubs operate at the physical layer, whereas switches operate at the network layer.
    2. All of the devices connected to a hub are part of a single collision domain, whereas each device connected to a switch has its own collision domain.
    3. There are switches available with network layer functionality, but there are no hubs with that capability.
    4. Switches create a separate broadcast domain for each connected device, whereas hubs create a single broadcast domain for all of the connected devices.

    Answer:

    B, C. Hubs operate at the physical layer and switches at the data link layer. Hubs and switches both create a single broadcast domain for all of the connected devices. Switches create a separate collision domain for each connected device, whereas hubs create a single collision domain. There are switches (but not hubs) with network layer (layer 3) functionality.
18. Which of the following problems is the Spanning Tree Protocol (STP) intended to prevent? (Choose all that apply.)

    1. Broadcast storms
    2. Late collisions
    3. Bridging loops
    4. Crosstalk

    Answer:

    A, C. STP disables redundant links between switches that can allow packets to circulate endlessly around the network. This is called a bridging loop. As a result of a bridging loop, the network can be flooded with broadcast traffic, which is called a broadcast storm. STP does nothing to prevent late collisions, which is an Ethernet timing problem, or crosstalk, which is a cabling fault.
19. Which of the following devices perform essentially the same function? (Choose two.)

    1. Hubs
    2. Bridges
    3. Switches
    4. Routers

    Answer:

    B, C. A switch is essentially a multiport bridge. Both switches and bridges process incoming packets by scanning their data link layer hardware addresses and forwarding the packets out the port connected to the destination system. The primary difference between them is that switches have many ports, whereas bridges have only two. Hubs and routers are physical layer and network layer devices, respectively, and perform different functions.
20. Which of the following is not one of the five functional levels associated with a distributed control system such as Supervisory Control and Data Acquisition (SCADA) systems?

    1. Field level
    2. Remote access
    3. Direct control
    4. Plant supervisory
    5. Production control
    6. Production scheduling

    Answer:

    B. The five functional levels in a distributed control system such as SCADA are field level, direct control, plant supervisory, production control, and production scheduling. Remote access is not one of the levels.
21. Which of the following switch types immediately forwards frames after looking at only the destination address?

    1. Cut-through
    2. Source route
    3. Store-and-forward
    4. Destination

    Answer:

    A. Cut-through switches are fast, because they look at only the first six bytes (the destination Media Access Control, or MAC, address) when forwarding a frame. They do not perform a cyclical redundancy check (CRC) on the entire frame's contents prior to forwarding it out a port leading to the destination. Source route is a bridging technique in which the source host, not the switch, determines the path a frame will take through a network to reach a destination. Store-and-forward switches take in the entire frame and verify its contents by performing a CRC calculation before forwarding it. There is no switch called a destination switch.
22. Which of the following does a switch use to forward incoming packets out through the correct ports?

    1. IP addresses
    2. MAC addresses
    3. DNS names
    4. MTU values

    Answer:

    B. Switches use Media Access Control (MAC) addresses to identify the ports associated with specific hosts. The switch reads the destination MAC address from each incoming packet and forwards it out through the port associated with that address. Switches are data link layer devices, so they do not use IP addresses or DNS names to forward packets. The Maximum Transmission Unit (MTU) value specifies the maximum size of data link layer frames; the switch does not use it to forward packets.
23. Which of the following statements about the Spanning Tree Protocol (STP) is not true?

    1. STP operates at the data link layer of the OSI model.
    2. STP is implemented in switches.
    3. STP prevents traffic from circulating endlessly around a network.
    4. STP compiles a database containing the IP addresses of connected devices.

    Answer:

    D. STP operates at the data link layer of the OSI model, so it works with hardware addresses, not IP addresses. Switches use STP to prevent redundant links from causing traffic loops on the network.
24. Small Office Home Office (SOHO) networks typically use a multifunction connectivity device that can perform all but which one of the following functions?

    1. DHCP
    2. DNS
    3. Switch
    4. Router
    5. Hub
    6. NAT router
    7. Access Point (AP)

    Answer:

    E. SOHO multifunction devices typically function as routers connecting the local network to an Internet Service Provider (ISP), switches providing wired connections to host devices, Dynamic Host Configuration Protocol (DHCP) servers assigning IP addresses, Domain Name System (DNS) servers resolving names into IP addresses, Network Address Translation (NAT) routers providing hosts with private IP addresses access to the Internet, and APs providing wireless devices with access to the network. They do not function as hubs.
25. Which of the following is the correct term for the process by which the Spanning Tree Protocol (STP) on a switch evaluates the paths through the network and places each port in the forwarding or blocking state?

    1. Assimilation
    2. Convergence
    3. Tree-building
    4. Listening

    Answer:

    B. The process by which STP populates its database with information about each port in a switch and designates the ports as forwarding or blocking is called convergence. Assimilation, tree-building, and listening are not terms for STP path evaluation.
26. A multilayer switch typically functions at which layers of the OSI reference model? (Choose two.)

    1. Data link
    2. Network
    3. Transport
    4. Application

    Answer:

    A, B. All switches operate at the data link layer of the OSI model, but multilayer switches usually also function as routers, which are network layer devices. They are not usually transport or application layer devices.
27. Which of the following is something that only a firewall capable of stateful packet inspection can do?

    1. Filter traffic-based port numbers
    2. Block traffic destined for specific IP addresses
    3. Scan transport layer header fields for evidence of SYN floods
    4. Block all TCP traffic from entering a network

    Answer:

    C. A firewall that supports stateful packet inspection examines other network and transport layer header fields, looking for patterns that indicate damaging behaviors, such as IP spoofing, SYN floods, and teardrop attacks. Port number filtering is the most commonly used form of packet filtering; it is not the same as stateful packet inspection. Blocking traffic based on IP addresses prevents specific systems from accessing a network; stateful packet inspection is a much more complicated operation. Packet filtering based on protocol identifiers enables you to block TCP traffic; this is not stateful packet inspection.
28. In local area networking, which of the following is not a type of bridge?

    1. Store and forward
    2. Routing
    3. Transparent
    4. Multiport

    Answer:

    B. Bridges are data link layer (layer 2) devices. Routing is a network layer (layer 3) function, so it is not a type of bridge. A store-and-forward, or simple, bridge examines each packet and decides whether to forward it to the connected network. A transparent bridge compiles a database of forwarding information, based on the packets it has processed previously. A multiport bridge provides connections to multiple networks; a switch is a type of multiport bridge.
29. Which of the following are methods typically used by Intrusion Detection Systems (IDSs) to analyze incoming network traffic? (Choose all that apply.)

    1. Anomaly-based detection
    2. Behavior-based detection
    3. Signature-based detection
    4. Statistic-based detection

    Answer:

    A, C. IDSs can use anomaly-based detection to identify deviations from a known baseline of trustworthiness, or signature-based detection to locate specific malicious byte or instruction sequences. Behavior-based and statistic-based detection are not typical IDS methods.
30. Virtual Local Area Networks (VLANs) create the administrative boundaries on a switched network that are otherwise provided by which of the following devices?

    1. Hubs
    2. Routers
    3. Firewalls
    4. Bridges

    Answer:

    B. Connecting subnets with routers at the network layer maintains the data link layer administrative boundaries that prevent broadcast transmissions from being propagated throughout the entire internetwork. Switching eliminates those data link layer boundaries, and administrators can use VLANs to simulate them. Because hubs propagate all of the traffic they receive out through all of their ports indiscriminately, they create no administrative boundaries. Firewalls are filtering devices that protect networks against malicious traffic; their functions are not related to VLANs. Switches are essentially multiport bridges that forward incoming traffic only to the device for which it is destined. Therefore, bridges are more closely related to eliminating administrative boundaries than to establishing them.
31. Which of the following devices can you use to connect two multimode fiber-optic Ethernet networks in different buildings 2000 meters apart using a single-mode fiber-optic cable segment running at the same speed, while maintaining a single collision domain?

    1. Bridge
    2. Switch
    3. Router
    4. Media converter

    Answer:

    D. A simple media converter is a physical layer device that can connect different types of network media together, as long as they have the same speed and duplex settings. Because the converter simply retransmits the signals, the single-collision domain is maintained. Bridges and switches are data link layer devices that create multiple-collision domains. Routers are network layer devices that create separate collision and broadcast domains.
32. Which of the following is another term for a multiport bridge?

    1. Router
    2. Switch
    3. Hub
    4. Gateway

    Answer:

    B. A switch is a data link layer device that essentially performs the function of a bridge for each device connected to one of its ports. It can therefore be described as a multiport bridge. Routers, hubs, and gateways are devices that operate at the network, physical, and application layers, respectively, so they cannot be described as bridges.
33. Which of the following devices enables two computers to communicate when they are using different protocols at each layer of the Open Systems Interconnection (OSI) reference model?

    1. A router
    2. A switch
    3. A hub
    4. A gateway

    Answer:

    D. A gateway enables two devices using different protocols to communicate by performing translation and conversion services for them. Routers, hubs, and switches all require the same protocol at some of the OSI model layers.
34. Review the following figure. How many collision domains and broadcast domains exist in the network diagram?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c02uf001_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. There are three collision domains and three broadcast domains.
    2. There is one collision domain and three broadcast domains.
    3. There is one broadcast domain and three collision domains.
    4. There are no collision domains and only one broadcast domain.
    5. There are nine collision domains and three broadcast domains.

    Answer:

    A. Each port on a router defines a separate collision domain. Hubs forward all traffic to all of the connected nodes, so each network segment is a single-collision domain. Routers do not forward broadcasts, so each network segment is also a separate broadcast domain.
35. Which of the following statements about switches and routers are true? (Choose all that apply.)

    1. Routers operate at the network layer, whereas switches operate at the data link layer.
    2. All of the devices connected to a switch are part of a single broadcast domain, whereas the networks connected to a router form separate broadcast domains.
    3. Routers can communicate with each other and share information, but switches cannot.
    4. Switches forward packets based on their hardware addresses, whereas routers forward packets based on their IP addresses.

    Answer:

    A, B, D. Routers are network layer devices that do not forward broadcast messages, so they create separate broadcast domains for each network. Switches do forward broadcasts, forming a single broadcast domain. Routers and switches can communicate using dedicated protocols. As data link layer devices, switches read only hardware addresses from packet frames; routers forward traffic based on the IP addresses in packets' IP headers.
36. Ralph is installing an Ethernet Local Area Network (LAN) for a small business with two offices on opposite sides of a courtyard. Ralph plans to run a multimode fiber-optic cable across the courtyard, but the budget is limited, and he cannot use fiber for the whole network. Therefore, he installs Unshielded Twisted Pair (UTP) cable in the two offices, which have 10 and 12 workstations, respectively. Which of the following devices should Ralph use to join the two UTP installations together into one LAN using the fiber-optic run across the courtyard, while keeping the cost to a minimum?

    1. Media converters
    2. Hubs
    3. Switches
    4. Routers

    Answer:

    A. Media converters will enable Ralph to join the multimode fiber-optic run to the UTP at both sides of the courtyard while maintaining a single network at minimum cost. Inexpensive small-business hubs and switches cannot join different media together. Routers can join different media, but they are more expensive, and they would separate the installation into three separate networks.
37. Five computers are connected to the same switch, but only four are able to communicate with each other. Assuming that all of the hardware is functioning properly, which of the following could be a reason for the fifth computer's communication problem?

    1. The switch has the fifth computer connected to a Virtual Local Area Network (VLAN) that's different from that of the other four.
    2. The network is experiencing a switching loop.
    3. The fifth computer is experiencing an MTU black hole, whereas the other four computers are not.
    4. There is a virtual router between the fifth computer and the other four.

    Answer:

    A. If the fifth computer is in a different VLAN from the other four, it would be unable to communicate with them. A switching loop would affect communication between all of the computers, not just the fifth one. An MTU black hole is a condition in which a system is unable to complete the Path MTU Discovery process, due to an intervening firewall. Because these five computers are all on the same LAN, they all have the same MTU, and Path MTU Discovery is not necessary. A virtual router would enable switched computers on different subnets to communicate with each other; it would not prevent them from communicating.
38. Which of the following types of systems are frequently used to collect information from Intrusion Detection Systems (IDSs)?

    1. SIEM
    2. NGFW
    3. RADIUS
    4. VoIP

    Answer:

    A. Security Information and Event Management (SIEM) systems can function as a central clearinghouse for information gathered by IDSs and other security processes. Next-Generation Firewall (NGFW), Remote Authentication Dial-In User Service (RADIUS), and Voice over IP (VoIP) are not systems that collect IDS information.
39. Which of the following network devices are “dumb”—that is, purely electrical devices with no electronic intelligence?

    1. Hubs
    2. Switches
    3. Routers
    4. Bridges

    Answer:

    A. Hubs are network devices that simply receive signals through one port, electrically enhance them, and transmit them out through another port. Routers, switches, and bridges are capable of reading the signals and processing them, which classifies them as intelligent.
40. Which of the following explains why splitting a large, switched Ethernet LAN into two LANs by adding a router can help to alleviate traffic congestion and improve performance? (Choose all that apply.)

    1. Adding a router reduces the amount of broadcast traffic on each of the two LANs.
    2. Adding a router reduces the amount of unicast traffic on each of the two LANs.
    3. Adding a router diverts traffic to an alternate path through the network.
    4. Adding a router prevents computers on one LAN from communicating with computers on another LAN.

    Answer:

    A, B. Adding a router splits the Ethernet LAN into two LANs, creating two separate broadcast domains. Each computer, therefore, has a smaller number of broadcast messages to process. Because the network is split by the router, the amount of unicast traffic on each subnet is reduced.
41. A small business office currently has a 100Base-TX Ethernet network with a single 8-port hub. All of the hub ports are populated, and the business owner wants to expand the network further. However, the hub does not have an uplink port. The owner has purchased a new hub, also with eight ports, which does have an uplink port, but he does not know how to connect them together. What must the owner do to install the new hub on the network?

    1. Use a standard patch cable to connect a standard port on the existing hub to a standard port on the new hub.
    2. Use a standard patch cable to connect a standard port on the existing hub to the uplink port on the new hub.
    3. Purchase a crossover cable and use it to connect a standard port on the existing hub to the uplink port on the new hub.
    4. Purchase a second new hub with an uplink port to replace the old one and use a standard patch cable to connect the two uplink ports together.

    Answer:

    B. Standard hub ports have a crossover circuit, which ensures that the transmit signals at one end of the connection arrive at the receive pins at the other end. The uplink port in a hub bypasses the crossover circuit, so that two connected hubs do not have crossover circuits that cancel each other out. A connection between a standard port and an uplink port, using a standard cable, results in a single crossover, which is correct wiring. Each of the other solutions results in either two crossovers or no crossovers, which is incorrect.
42. Which of the following tasks can you perform to split a large, switched Local Area Network (LAN) into multiple broadcast domains? (Choose all that apply.)

    1. Replace one or more switches with hubs.
    2. Install a firewall to filter broadcast traffic.
    3. Enable the Spanning Tree Protocol (STP) on the switches.
    4. Create Virtual Local Area Networks (VLANs) in the switches.
    5. Install routers on the network.

    Answer:

    D, E. By default, a switched LAN consists of a single broadcast domain. To create multiple broadcast domains, you can install routers to split the installation into two or more networks, because routers do not forward broadcasts. The other possibility is to create VLANs in the switches. Each VLAN is a separate broadcast domain. All of the other options would have no effect on the number of broadcast domains on the network.
43. Which of the following statements about bridges and switches is true?

    1. Bridges and switches are network layer devices that use logical addressing to forward frames.
    2. Bridges and switches are data link layer devices that use Media Access Control (MAC) addresses to forward frames.
    3. Bridges and switches build their internal tables based on destination addresses and forward packets based on source addresses.
    4. Bridges and switches must support the network layer protocol implemented on the Local Area Network (LAN).
    5. Each port on a bridge or switch defines a separate broadcast domain.

    Answer:

    B. Bridges and switches are data link layer devices that forward frames based on the destination MAC address contained in the frame. They operate in promiscuous mode, listening and processing all frames on each segment, and they build forwarding tables with this information. Forwarding tables are built based on source MAC addresses. Bridges are protocol independent; they are not involved with the upper layer protocols being carried on the LAN. Broadcast domains are defined by network layer devices, not data link layer devices.
44. Which of the following is a correct term describing the function of a switch?

    1. Layer 2 router
    2. Ethernet hub
    3. Multiport bridge
    4. Layer 3 repeater

    Answer:

    C. A switch is best described as a multiport bridge, because it reads the hardware addresses of incoming packets and forwards them out through the port for the destination node. Although a switch does function at layer 2 of the OSI model (the data link layer), it is not a router, which connects networks together at layer 3 (the network layer). Hubs and repeaters are physical layer (layer 1) devices that are not capable of performing the functions of a switch.
45. Which of the following are available as Internet of Things (IoT) devices?

    1. Refrigerators
    2. Doorbells
    3. Thermostats
    4. Speakers
    5. All of the above

    Answer:

    E. The IoT consists of devices that are ordinarily passive, but which have been made intelligent by configuring them to participate on an IP network. All of the devices listed are available as “smart” devices that enable remote users to interact with them over the Internet.
46. Which of the following is the primary reason why replacing hubs with switches on an Ethernet Local Area Network (LAN) improves its performance?

    1. Switches forward packets faster than hubs.
    2. Switches do not forward broadcast transmissions.
    3. Switches reduce the number of collisions on the network.
    4. Switches read the IP addresses of packets, not the hardware addresses.

    Answer:

    C. The main reason why switches improve the efficiency of an Ethernet LAN is that they create a separate collision domain for each switched port, eliminating most collisions. Collisions result in packets having to be retransmitted, so fewer collisions means fewer retransmissions, which improves performance. Switches do not forward packets faster than hubs. Switches do forward broadcast transmissions. Switches do read hardware addresses, not IP addresses.
47. Which of the following is a correct definition of a collision domain?

    1. A group of Local Area Networks (LANs), connected by routers, that enables any node to transmit to any other node
    2. A group of computers connected so that a broadcast transmission by any one device reaches all of the other devices
    3. A group of devices connected by cable segments that are longer than the maximum length stated in the physical layer specification
    4. A group of devices connected so that when two devices transmit at exactly the same time, a data collision occurs

    Answer:

    D. A collision domain is a LAN with a shared network medium, so that two devices transmitting at the same time generate a signal quality error, also known as a collision. Ethernet LANs connected by hubs create a shared medium, whereas switched networks create a separate collision domain for each connected node. Routers create separate collision domains. A group of computers able to receive broadcasts is the definition of a broadcast domain, not a collision domain. Overlong cables can precipitate collisions but do not define a collision domain.
48. Which of the following terms are used to describe the device used to place calls on a Voice over Internet Protocol (VoIP) installation? (Choose all that apply.)

    1. Terminal
    2. Gateway
    3. Endpoint
    4. PBX

    Answer:

    A, C. VoIP uses the terms _terminal_ and _endpoint_ to refer to the device with which users make calls, including computers and telephone handsets. A VoIP gateway is the device that provides the conduit between an IP network and the Public Switched Telephone Network (PSTN). A VoIP private branch exchange (PBX) is a device that switches calls between endpoints on the local IP network and provides access to external Internet lines.
49. Which of the following statements about hubs is not true?

    1. Hubs are data link layer devices that connect network devices in a star or ring topology.
    2. Hubs amplify and repeat signals received through one port out all other ports regardless of the destination.
    3. Hubs are physical layer devices that connect network devices in a star topology.
    4. Hubs provide internal crossover circuits and use uplink ports to form a hierarchical star.

    Answer:

    A. Hubs are physical layer devices that amplify and repeat signals out all ports except the one through which the data was received, regardless of the destination. Hubs are used to physically connect end systems to a star topology. Hubs typically provide an internal crossover circuit connection. Uplink ports are used to extend the distance of a star network, forming a hierarchical star.
50. Which of the following statements about routers are true? (Choose all that apply.)

    1. Routers are network layer devices that use IP addresses to forward frames.
    2. Routers are data link layer devices that use Media Access Control (MAC) addresses to forward frames.
    3. Routers build their internal tables based on destination MAC addresses and forward frames based on source MAC addresses.
    4. Routers must support the network layer protocol implemented on the Local Area Network (LAN).
    5. Each port on a router defines a separate broadcast domain.

    Answer:

    A, D, E. Routers are network layer devices that use IP addresses to forward frames, not MAC addresses. Routers are protocol dependent. They must support the network layer protocol being routed. As a network layer device, a router defines networks (or LANs) that represent a separate broadcast domain. Routers do not build their routing tables or forward frames using MAC addresses.
51. Which of the following hub types are supported by the 100Base-TX physical layer specification? (Choose all that apply.)

    1. Class I
    2. Class II
    3. Class III
    4. Class IV

    Answer:

    A, B. The 100Base-TX specification specifies two hub types: Class I and II. Class I hubs perform signal translation; Class II hubs do not. A network can have only one Class I hub per collision domain; a network can have two Class II hubs per collision domain. The other options do not exist.
52. Which of the following statements about routers is not true?

    1. Routers can connect two or more networks with dissimilar data link layer protocols and media.
    2. Routers can connect two or more networks with the same data link layer protocols and media.
    3. Routers store and maintain route information in a local text file.
    4. Servers with multiple network interfaces can be configured to function as software routers.
    5. Routers can learn and populate their routing tables through static and dynamic routing.

    Answer:

    C. Routers store and maintain route information in a routing table that is stored in memory, not in a local text file. All of the other statements about routers are true.
53. The network administrator for a small business is installing a computer to function as a firewall protecting their internetwork from Internet intrusion. At which of the following locations should the administrator install the firewall system?

    1. Anywhere on the private internetwork, as long as the Internet is accessible
    2. Between the Internet access router and the Internet Service Provider's (ISP's) network
    3. At the ISP's network site
    4. Between the Internet access router and the rest of the private internetwork

    Answer:

    D. The firewall is a conduit between the private network and the ISP's network (which provides access to the Internet), through which all traffic must pass. This ensures that the firewall has the opportunity to examine every packet that passes between the private network and the Internet and filter out those that are not authorized. If the firewall was located in the midst of the private internetwork, it would be possible for Internet computers to bypass the firewall and communicate directly with the private systems. Placing the firewall on the far side of the router would put it on the ISP's network, causing it to filter all of the ISP's traffic and not just that destined for the private network. Installing the firewall at the ISP's site would have the same effect as installing it on the far side of the router at the private network site.
54. What must you do to configure a firewall to admit File Transfer Protocol (FTP) traffic to the internal network using its default port settings? (Choose all that apply.)

    1. Open port 20
    2. Open port 21
    3. Open port 22
    4. Open port 23
    5. Open port 24

    Answer:

    A, B. The FTP protocol uses two well-known ports: 20 and 21. A firewall must have both of these ports open to admit FTP traffic. FTP does not require ports 22, 23, or 24.
55. Proxy servers operate at which layer of the OSI reference model?

    1. Data link
    2. Network
    3. Transport
    4. Application

    Answer:

    D. A proxy server is an application layer service, because it receives Internet service requests from client computers, reads the application layer protocol data in each request, and then generates its own request for the same service and transmits it to the Internet server the client specifies. Only an application layer service can read and process the application layer data in network packets. A proxy server cannot be a data link layer device, because it can provide Internet access to an entire internetwork, while the data link layer is concerned with communications on a single subnet. Proxy servers cannot be network layer devices, because the network layer handles all internetwork packets indiscriminately and is unaware of what application generated the data carried inside the packets. The transport layer is not involved in processing application data, so proxy servers cannot be said to function at the transport layer.
56. Which of the following is a feature that is not found in a traditional firewall product, but which might be found in a Next-Generation Firewall (NGFW)?

    1. Stateful packet inspection
    2. Deep Packet Inspection (DPI)
    3. Network Address Translation (NAT)
    4. Virtual Private Network (VPN) support

    Answer:

    B. DPI is a firewall technique that examines the data carried in packets and not just the protocol headers. While traditional firewalls typically do not support DPI, NGFWs often do. Stateful packet inspection, NAT, and VPN support are all features that are commonly supported by traditional firewall products.
57. Which of the following statements about content filtering in firewalls is true?

    1. Content filters examine the source IP addresses of packets to locate potential threats.
    2. Content filters enable switches to direct packets out through the correct port.
    3. Content filters examine the data carried within packets for potentially objectionable materials.
    4. Content filters use frequently updated signatures to locate packets containing malware.

    Answer:

    C. Content filters are a firewall feature that examines the data inside packets, rather than their origin, to locate objectionable material. They do not scan IP addresses, nor do they detect typical types of malware. Content filters are not implemented in switches.
58. Which of the following is not one of the criteria typically used by load balancers to direct incoming traffic to one of a group of servers?

    1. Which server has the lightest load
    2. Which server has the fastest response time
    3. Which server is next in an even rotation
    4. Which server has the fastest processor

    Answer:

    D. In most cases, a load balancing router works by processing incoming traffic based on rules set by the administrator. The rules can distribute traffic among a group of servers using various criteria, such as each server's current load or response time, or which server is next in a given rotation. Load balancers typically do not use the hardware configuration of the servers to direct traffic since this is a factor that does not change.
59. Which of the following devices enables you to use a standard analog telephone to place calls using the Internet instead of the Public Switched Telephone Network (PSTN)?

    1. Proxy server
    2. VPN headend
    3. VoIP gateway
    4. UTM appliance

    Answer:

    C. A VoIP gateway is a device that provides a conduit between an IP network and the Public Switched Telephone Network (PSTN). The gateway enables standard telephones connected to the PSTN to place calls using VoIP services on the Internet. A proxy server is an application layer device that provides web browsers and other client programs to access the Internet. A Virtual Private Network (VPN) headend enables multiple client systems to access a network from remote locations. A unified threat management (UTM) appliance typically performs VPN, firewall, and antivirus functions.
60. Which of the following devices enable users on private networks to access the Internet by substituting a registered IP address for their private addresses? (Choose all that apply.)

    1. NAT router
    2. RADIUS server
    3. Proxy server
    4. UTM appliance

    Answer:

    A, C. Network Address Translation (NAT) is a network layer device that converts the private IP addresses of all of a client's transmissions to registered IP address. NAT therefore works for all applications. A proxy server is an application layer device that performs the same type of conversion, but only for specific applications. A Remote Authentication Dial-In User Service (RADIUS) server can provide Authentication, Authorization, Accounting, Auditing (AAAA) services for remote access servers. It does not convert IP addresses. A unified threat management (UTM) appliance typically performs VPN, firewall, and antivirus functions. It too does not convert IP addresses.
61. HVAC systems can use the Internet of Things (IoT) to monitor which of the following? (Choose all that apply.)

    1. Temperature
    2. Pressure
    3. Humidity
    4. Printers
    5. Occupancy
    6. Cameras
    7. Door locks

    Answer:

    A, B, C, E. HVAC sensors can measure temperatures and humidity in climate-controlled areas, such as datacenters; atmospheric pressure in devices like boilers and compressors; and occupancy, to control conditions based on the presence of people. Printers, cameras, door locks, and other physical access control devices are not part of an HVAC system.
62. A VPN headend is an advanced type of which of the following devices?

    1. Switch
    2. Router
    3. Gateway
    4. Bridge

    Answer:

    B. A Virtual Private Network (VPN) headend is a type of router that enables multiple client systems to access a network from remote locations. Because the device provides an interface between networks, it is considered to be a type of router, not a switch, a gateway, or a bridge.
63. Which of the following technologies is typically associated with virtual PBX services?

    1. Quality of Service (QoS)
    2. Voice over IP
    3. CARP
    4. Round-robin DNS

    Answer:

    B. A virtual PBX is an arrangement in which a telephone company provides the PBX services to a customer but maintains the actual hardware at their own facility. The recent emphasis on cloud computing has led to a number of hosted PBX solutions that use Voice over IP (VoIP) to provide services to customers. QoS is a technique for prioritizing traffic by tagging packets based on their content. It is not a virtual PBX technique. The Cache Array Routing Protocol (CARP) enables proxy servers to exchange information; it does not provide virtual PBX services. In round-robin DNS, a DNS server contains multiple resource records for the same server name, each with a different IP address representing one of the computers running the server application. When a client resolves the server name, the DNS server accesses each of the resource records in turn so that each address theoretically receives the same number of visitors. This is not a virtual PBX technology.
64. Ralph, the administrator of a 500-node private internetwork, is devising a plan to connect the network to the Internet. The primary objective of the project is to provide all of the network users with access to web and email services while keeping the client computers safe from unauthorized users on the Internet. The secondary objectives of the project are to avoid having to manually configure IP addresses on each one of the client computers individually and to provide a means of monitoring and regulating the users’ access to the Internet. Ralph submits a proposal calling for the use of private IP addresses on the client computers and a series of proxy servers with public, registered IP addresses, connected to the Internet using multiple T-1 lines. Which of the following statements about Ralph's proposed Internet access solution is true?

    1. The proposal fails to satisfy both the primary and secondary objectives.
    2. The proposal satisfies the primary objective but neither of the secondary objectives.
    3. The proposal satisfies the primary objective and one of the secondary objectives.
    4. The proposal satisfies the primary objective and both of the secondary objectives.

    Answer:

    C. Proxy servers provide network users with access to Internet services, and the unregistered IP addresses on the client computers protect them from unauthorized access by users on the Internet, which satisfies the first objective. The proxy servers also make it possible for network administrators to regulate users' access to the Internet, which satisfies one of the two secondary objectives. However, the proxy servers cannot assign IP addresses to the client computers, and the plan makes no mention of DHCP or another automatic TCP/IP configuration mechanism. Therefore, the plan does not satisfy the other secondary objective.
65. Which of the following protocols can be used by wireless controllers to communicate with the Access Points (APs) on a Wireless Local Area Network (WLAN)? Choose all that apply.

    1. CAPWAP
    2. LWAPP
    3. LDAP
    4. PPTP

    Answer:

    A, B. The Control and Provisioning of Wireless Access Points (CAPWAP) protocol and the Lightweight Access Point Protocol (LWAPP) are both protocols that enable wireless controllers to manage and control Access Points (APs). Lightweight Directory Access Protocol (LDAP) is used by directory services, and Point-to-Point Tunneling Protocol (PPTP) is used for virtual private networking.
66. Which of the following devices enables administrators of enterprise wireless networks to manage multiple Access Points (APs) from a central location?

    1. Hypervisor
    2. Wireless controller
    3. Wireless endpoint
    4. Demarcation point

    Answer:

    B. In many enterprise wireless networks, the Access Points (APs) do not run a full operating system and are called thin or lightweight APs. The network also has a device called a wireless controller that performs some of the required tasks and manages the APs. A wireless endpoint is another term for a computer or other device that is a client on the wireless network. Hypervisors and demarcation points have nothing to do with wireless networking. A hypervisor creates and manages Virtual Machines (VMs) on a host server, and a demarcation point is the interface between a private network and an outside telecommunications service.
67. Which of the following devices can administrators use to create multiple Virtual Local Area Networks (VLANs) and forward traffic between them?

    1. Multilayer switch
    2. Virtual router
    3. Load balancer
    4. Broadband router

    Answer:

    A. A multilayer switch is a network connectivity device that functions at both layer 2 and layer 3 of the OSI model. At layer 2, the device functions like a normal switch, providing individual collision domains to each connected node and enabling administrators to create multiple VLANs. At layer 3, the device also provides routing capabilities by forwarding packets between the VLANs. Virtual routers, load balancers, and broadband routers are strictly layer 3 devices that can route traffic but cannot create VLANs.
68. Which of the following is not a mechanism for distributing incoming network traffic among multiple servers?

    1. Load balancer
    2. Round-robin DNS
    3. NLB cluster
    4. VPN headend

    Answer:

    D. A Virtual Private Network (VPN) headend is a type of router that enables multiple client systems to access a network from remote locations. It does not distribute traffic among servers. A load balancer is a type of router that forwards traffic with a single IP address to multiple servers in turn. Round-robin DNS is a technique in which a DNS server resolves a name into several IP addresses, each in turn. A Network Load Balancing (NLB) cluster is a group of servers, all running the same application, that distribute incoming traffic among themselves.
69. A load balancer is a type of which of the following devices?

    1. Switch
    2. Router
    3. Gateway
    4. Firewall

    Answer:

    B. A load balancer is a type of router that forwards traffic with a single IP address to multiple servers in turn. In most cases, a load balancing router works by processing incoming traffic based on rules set by the administrator. Because a load balancer works with IP addresses, it is a network layer device. Load balancers are not switches, gateways, or firewalls.
70. Which of the following devices expands on the capabilities of the traditional firewall by adding features like Deep Packet Inspection (DPI) and an Intrusion Prevention System (IPS)?

    1. RADIUS server
    2. CSU/DSU
    3. NGFW
    4. Proxy server

    Answer:

    C. Next-Generation Firewalls (NGFWs) expand on the packet filtering capabilities of traditional firewalls by adding features such as DPI and IPSs, as well as inspection of encrypted traffic and antivirus scanning. Remote Authentication Dial-In User Service (RADIUS) servers can provide centralized Authentication, Authorization, Accounting, Auditing (AAAA) services. A CSU/DSU is a device that provides a router on a private network with access to a leased line. A proxy server is an application layer service that receives Internet service requests from client computers, reads the application layer protocol data in each request, and then generates its own request for the same service and transmits it to the Internet server the client specifies.
71. Which of the following is a device that switches calls between endpoints on the local IP network and provides access to external Internet lines?

    1. VoIP PBX
    2. VoIP gateway
    3. VoIP endpoint
    4. Multilayer switch

    Answer:

    A. A private branch exchange (PBX) switches internal calls and provides access to external lines. A VoIP PBX performs the same tasks as a traditional PBX. A VoIP gateway is the device that provides the conduit between an IP network and the Public Switched Telephone Network (PSTN). A VoIP endpoint is a device that makes use of the VoIP system, such as a computer or handset. A multilayer switch is a data networking device that includes both switching and routing capabilities.
72. Which of the following statements about Internet access through a proxy server accounts for the security against outside intrusion that a proxy provides?

    1. The proxy server uses a public IP address, and the client computers use private addresses.
    2. The proxy server uses a private IP address, and the client computers use public addresses.
    3. Both the proxy server and the client computers use private IP addresses.
    4. Both the proxy server and the client computers use public IP addresses.

    Answer:

    A. Because the client computers use private IP addresses, they are invisible to the Internet, so users outside the private network cannot see or access them. The proxy server has a public IP address so it can participate in service transactions with Internet servers. If the proxy server used a private IP address, it would not be able to access the Internet directly. If the clients used public IP addresses, they would be visible to the Internet and vulnerable to intrusion.
73. Which of the following statements about proxy servers and NAT servers are true? (Choose all that apply.)

    1. NAT servers and proxy servers can both provide Internet access to clients running any application.
    2. NAT servers and proxy servers both use public IP addresses.
    3. NAT servers and proxy servers both access Internet servers and relay the responses to network clients.
    4. Both NAT servers and proxy servers cache web data for later use.

    Answer:

    B, C. To provide clients with Internet access, a NAT or proxy server must have direct access to the Internet, which requires using a registered, or public, IP address. Both NAT and proxy servers function as the middleman in transactions between the client computers on a private network and Internet servers. The NAT or proxy server transmits the client's service request to the Internet server as though it was its own and, after receiving the reply, relays the response back to the client. Because NAT servers function at the network layer, clients can use any application to access the Internet through the server. Proxy servers, however, operate at the application layer and can provide Internet access only to certain types of client applications. Proxy servers are capable of caching web data for later use, because they are application layer devices that read the application layer protocol data in the message packets they receive. NAT servers are network layer processes that forward packets with no knowledge of the application layer information in their contents.
74. A multilayer switch can operate at which layers of the Open Systems Interconnection (OSI) model? (Choose all that apply.)

    1. Physical
    2. Data link
    3. Network
    4. Transport
    5. Session
    6. Presentation
    7. Application

    Answer:

    B, C, D. A multilayer switch typically operates at the data link, and network layers, assuming the functions of a switch and a router by using Media Access Control (MAC) addresses at the data link layer (layer 2) and IP addresses at the network layer (layer 3) to forward packets to their appropriate destinations. Some switches also function at the transport layer (layer 4) by distinguishing between User Datagram Protocol (UDP) and Transmission Control Protocol (TCP) traffic and using port numbers to forward packets.
75. Which of the following devices can an administrator use to monitor a network for abnormal or malicious traffic?

    1. IDS
    2. UPS
    3. RADIUS
    4. DoS
    5. RAS

    Answer:

    A. Intrusion Detection Systems (IDSs) are designed to monitor network traffic for anomalies and send notifications to administrators. Uninterruptible power supplies (UPSs), Remote Authentication Dial-In User Service (RADIUS) servers, Denial-of-Service (DoS) attacks, and Remote Access Service (RAS) servers all have nothing to do with network monitoring.
76. Which of the following is not a function that is typically provided by a unified threat management (UTM) appliance?

    1. Virtual private networking
    2. Network firewall
    3. Packet forwarding
    4. Antivirus protection

    Answer:

    C. Packet forwarding is a function typically associated with routers and is not a normal function of a UTM appliance. UTM appliances do typically perform VPN, firewall, and antivirus functions.
77. Which of the following features enables an Intrusion Detection System (IDS) to monitor all of the traffic on a switched network?

    1. Stateful packet inspection
    2. Port mirroring
    3. Trunking
    4. Service-dependent filtering

    Answer:

    B. Port mirroring is a feature found in some switches that takes the form of a special port that runs in promiscuous mode. This means that the switch copies all incoming traffic to that port, as well as to the dedicated destination ports. By connecting an IDS or protocol analyzer to this port, an administrator can access all of the network's traffic. Stateful packet inspection is a firewall feature that enables the device to examine network and transport layer header fields, looking for patterns that indicate damaging behaviors, such as IP spoofing, SYN floods, and teardrop attacks. Trunking is a switch feature that enables administrators to create VLANs that span multiple switches. Service-dependent filtering is a firewall feature that blocks traffic based on transport layer port numbers.
78. Which of the following network devices does not employ Access Control Lists (ACLs) to restrict access?

    1. Routers
    2. Hubs
    3. Switches
    4. Wireless Access Points (WAPs)

    Answer:

    B. ACLs restrict access to network devices by filtering usernames, MAC addresses, IP addresses, or other criteria. Routers, switches, and WAPs all use ACLs to control access to them. Hubs are purely physical layer devices that relay electrical or optical signals. They have no way of controlling access to them.
79. Which of the following TCP/IP parameters, configured on an end system, specifies the Internet Protocol (IP) address of a router on the local network that provides access to other networks?

    1. WINS Server Addresses
    2. Default Gateway
    3. DNS Server Addresses
    4. Subnet Gateway

    Answer:

    B. The Default Gateway parameter specifies the address of the local router that the end system should use to access other networks. The WINS Server Addresses and DNS Server Addresses parameters are used to resolve names to IP addresses. There is no such parameter as Subnet Gateway.
80. Which of the following routing protocols uses the packet format shown in the figure?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c02uf002_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. RIPv1
    2. RIPv2
    3. OSPF
    4. EIGRP
    5. BGP

    Answer:

    A. The figure displays the format for a Routing Information Protocol (RIP) version 1 response packet. The figure does not show the packet format for RIPv2, Open Shortest Path First (OSPF), Enhanced Interior Gateway Routing Protocol (EIGRP), or Border Gateway Protocol (BGP).
81. Which of the following statements about the Enhanced Interior Gateway Routing Protocol (EIGRP) is not true?

    1. EIGRP does not support classless IPv4 addresses.
    2. EIGRP is a hybrid routing protocol.
    3. EIGRP can only transmit incremental routing table updates.
    4. EIGRP shares routes within an autonomous system.

    Answer:

    A. EIGRP can support classless IPv4 addresses. It was designed to replace the Interior Gateway Routing Protocol (IGRP), which could not support classless addresses. All of the other options contain true statements.
82. Which of the following are techniques used in traffic shaping to prevent networks from being overwhelmed by data transmissions? (Choose all that apply.)

    1. Bandwidth throttling
    2. Rate limiting
    3. Broadcast storming
    4. Network Address Translation (NAT)

    Answer:

    A, B. Bandwidth throttling is a traffic shaping technique that prevents specified data streams from transmitting too many packets. Rate limiting is a traffic shaping technique that controls the transmission rate of sending systems. A broadcast storm is a type of network switching loop. NAT is a method by which private networks can share registered IP addresses. Neither of these last two is a traffic shaping technique.
83. Which of the following terms refers to methods by which network traffic is prioritized to prevent applications from suffering faults due to network congestion?

    1. Port forwarding
    2. Dynamic routing
    3. VLANs
    4. QoS

    Answer:

    D. Quality of Service (QoS) is a general term that refers to various mechanisms for prioritizing network traffic so that applications or data streams requiring a certain level of performance are not negatively affected by lower-priority transmissions. Port forwarding is a routing method that redirects traffic intended for one IP address and port number to another. Dynamic routing is a method by which routing tables are automatically updated with new information as the routing fabric of an internetwork changes. Virtual Local Area Networks (VLANs) are a means for partitioning a broadcast domain into discrete units that are functionally equivalent to physical LANs.
84. Which of the following statements about Routing Information Protocol version 1 (RIPv1) is true? (Choose all that apply.)

    1. RIPv1 broadcasts the entire contents of the routing table every 30 seconds.
    2. RIPv1 advertises the subnet mask along with the destination network.
    3. RIPv1 broadcasts only the elements in the routing table that have changed every 60 seconds.
    4. RIPv1 does not include the subnet mask in its network advertisements.

    Answer:

    A, D. Routers that are running the RIPv1 routing protocol broadcast their entire routing tables every 30 seconds, regardless of whether there has been a change in the network. RIPv1 does not include the subnet mask in its updates, so it does not support subnetting.
85. Which of the following mechanisms for prioritizing network traffic uses a 6-bit classification identifier in the Internet Protocol (IP) header?

    1. Diffserv
    2. CoS
    3. Traffic shaping
    4. QoS
    5. Administrative distance

    Answer:

    A. Differentiated services (Diffserv) is a mechanism that provides Quality of Service (QoS) on a network by classifying traffic types using a 6-bit value in the differentiated services (DS) field of the IP header. Class of Service (CoS) is a similar mechanism that operates at the data link layer by adding a 3-bit Priority Code Point (PCP) value to the Ethernet frame. Traffic shaping is a means of prioritizing network traffic that typically works by delaying packets at the application layer. Quality of Service (QoS) is an umbrella term that encompasses a variety of network traffic prioritization mechanisms. Administrative distance is a value that routers use to select the most efficient route to a destination.
86. Which of the following statements about static routing are true? (Choose all that apply.)

    1. Static routes are manually configured routes that administrators must add, modify, or delete when a change in the network occurs.
    2. Static routes are automatically added to the routing table by routing protocols when a new network path becomes available.
    3. Static routes adapt to changes in the network infrastructure automatically.
    4. Static routes are a recommended solution for large internetworks with redundant paths to each destination network.
    5. Static routes are a recommended solution for small internetworks with a single path to each destination network.

    Answer:

    A, E. Administrators must manually add, modify, or delete static routes when a change in a network occurs. For this reason, static routes are not recommended for use in large internetworks where there are multiple paths to each destination network. Static routes are not automatically added by routing protocols and do not adapt to changes in a network.
87. Which of the following TCP/IP routing protocols does not include the subnet mask within its route update messages, preventing it from supporting subnetting?

    1. Routing Information Protocol, version 1 (RIPv1)
    2. Routing Information Protocol, version 2 (RIPv2)
    3. Border Gateway Protocol (BGP)
    4. Open Shortest Path First (OSPF)

    Answer:

    A. RIPv1 does not include the subnet mask in its updates. RIPv2 supports subnetting and includes the subnet mask of each network address in its updates. OSPF and BGP both include the subnet mask within their updates.
88. Which of the following terms refers to a routing protocol that does _not_ rely on hop counts to measure the efficiency of routes?

    1. Interior gateway protocol
    2. Edge gateway protocol
    3. Distance vector protocol
    4. Link state protocol

    Answer:

    D. Distance vector protocols rely on hop counts to evaluate the efficiency of routes. Link state protocols use a different type of calculation, usually based on Dijkstra's algorithm. The terms _interior gateway protocol_ and _edge gateway protocol_ do not refer to the method of calculating routing efficiency.
89. What is the maximum number of routes that can be included in a single RIP broadcast packet?

    1. 20
    2. 25
    3. 32
    4. Unlimited

    Answer:

    B. A single RIP broadcast packet can include up to 25 routes. If there are more than 25 routes in the computer's routing table, then RIP must generate additional packets.
90. Which of the following routing protocols can you use on a TCP/IP internetwork with segments running at different speeds, making hop counts an inaccurate measure of route efficiency? (Choose all that apply.)

    1. Enhanced Interior Gateway Routing Protocol (EIGRP)
    2. Routing Information Protocol (RIP)
    3. Open Shortest Path First (OSPF)
    4. Border Gateway Protocol (BGP)

    Answer:

    A, C. OSPF is a link state routing protocol, which means that it does not rely solely on hop counts to measure the relative efficiency of a route. EIGRP is a hybrid protocol that can use link state routing. RIP is a distance vector routing protocol, meaning that it uses hop counts to measure route efficiency. BGP is an exterior gateway protocol that exchanges routing information among autonomous systems using path vectors or distance vectors.
91. Which of the following statements about the Open Shortest Path First (OSPF) routing protocol are true? (Choose all that apply.)

    1. OSPF is an interior gateway protocol.
    2. OSPF is a link state routing protocol.
    3. OSPF does not support Classless Inter-Domain Routing (CIDR).
    4. OSPF shares routes within an autonomous system.

    Answer:

    A, B, D. OSPF does support CIDR. All of the other options contain true statements.
92. What is the term for the process by which dynamic routing protocols update other routers with routing table information?

    1. Convergence
    2. Distance vectoring
    3. Redistribution
    4. Dissemination

    Answer:

    A. Convergence is the term for the process by which routers propagate information from their routing tables to other routers on the network using dynamic routing protocols. Distance vectoring, redistribution, and dissemination do not describe this process.
93. Which of the following TCP/IP routing protocols measures the efficiency of routes by the number of hops between the source and the destination?

    1. Routing Internet Protocol (RIP)
    2. Open Shortest Path First (OSPF)
    3. Border Gateway Protocol (BGP)
    4. Intermediate System to Intermediate System (IS-IS)

    Answer:

    A. RIP is a distance vector protocol, which uses hop counts to measure the efficiency of routes. OSPF, BGP, and IS-IS are all link state protocols, which do not rely on hop counts.
94. Which of the following types of routing protocols route datagrams between autonomous systems?

    1. EGP
    2. RIP
    3. IGP
    4. OSPF

    Answer:

    A. Exterior Gateway Protocol (EGP) routes datagrams between autonomous systems. Interior Gateway Protocol (IGP) routes datagrams within an autonomous system. Routing Information Protocol (RIP) and Open Shortest Path First (OSPF) are examples of interior gateway protocols.
95. Which of the following prevents packets on a TCP/IP internetwork from being transmitted endlessly from router to router?

    1. Open Shortest Path First (OSPF)
    2. Maximum Transmission Unit (MTU)
    3. Administrative distance
    4. Time to Live (TTL)

    Answer:

    D. TTL is a value included in the IPv4 header that specifies the maximum number of hops the packet is allowed on the network. Each router processing the packet reduces the TTL value by one and discards the packet when the value reaches zero. OSPF is a routing protocol. MTU specifies the maximum size of a frame. Administrative distance is a value that routers use to select the most efficient route to a destination.
96. Which of the following command-line tools can you use to create and modify static routes on a Unix or Linux system? (Choose all that apply.)

    1. `route`
    2. `ifconfig`
    3. `traceroute`
    4. `ip`

    Answer:

    A, D. The `route` command was originally created to display a Unix or Linux system's routing table and modify its contents by adding, changing, and deleting static routes. The `ip` command is part of the `iproute2` command-line utility package, which has replaced `route` in many Unix and Linux distributions. Running `ip` with the `route` parameter can manipulate the routing table. The `traceroute` and `ifconfig` tools are not commands for manipulating the routing table.
97. Routers that use the Open Shortest Path First (OSPF) routing protocol calculate the relative costs of routes through the network by exchanging which of the following specifications for each interface with other routers?

    1. Transmission speed
    2. Data link layer protocol
    3. Network medium
    4. IP address

    Answer:

    A. Routers that use OSPF transmit the speed of each network interface with the other OSPF routers in the network. This enables the routers to evaluate the cost of various routes through the network and transmit packets using the route with the smallest cost value. The routers do not need to share information about the data link layer protocols or network media they use or their IP addresses.
98. Which of the following statements about the Border Gateway Protocol (BGP) is not true?

    1. BGP is an exterior gateway protocol.
    2. BGP is a link state routing protocol.
    3. BGP supports Classless Inter-Domain Routing (CIDR).
    4. BGP shares routes among autonomous systems.

    Answer:

    B. BGP is a path vector routing protocol, not a link state routing protocol. All of the other options contain true statements.
99. In an IPv4 routing table, what is the network destination address for the host system's default route?

    1. 0.0.0.0
    2. 127.0.0.0
    3. 127.255.255.255
    4. 255.255.255.255

    Answer:

    A. The default route in an IPv4 routing table always has a destination address of 0.0.0.0. The other destinations are found in a routing table, but they are not the default route destination.
100.    Which of the following routing protocols uses the packet format shown in the figure?

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c02uf003_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

        1. RIPv1
        2. RIPv2
        3. OSPF
        4. EIGRP
        5. BGP

        Answer:

        A. The figure displays the format for a Routing Information Protocol version 2 response packet. The figure does not show the packet format for RIPv1, Open Shortest Path First (OSPF), Enhanced Interior Gateway Routing Protocol (EIGRP), or Border Gateway Protocol (BGP).
101.    Which of the following routing protocols has both interior and exterior designations, based on whether it is used for routing within an autonomous system or on the Internet?

        1. RIP
        2. OSPF
        3. EIGRP
        4. BGP

        Answer:

        D. The Border Gateway Protocol (BGP) is a highly scalable protocol used for routing both on private autonomous systems, where it is known as the Internal Border Gateway Protocol (iBGP) and maintains full mesh communication among all of the routers, and on the Internet, where it is known as the External Border Gateway Protocol (eBGP). Routing Information Protocol (RIP), Open Shortest Path First (OSPF), and Enhanced Interior Gateway Routing Protocol (EIGRP) do not have interior and exterior designations.
102.    Which of the following network layer protocols includes a Time to Live (TTL) field? (Choose all that apply.)

        1. IPv4
        2. IPv6
        3. ICMP
        4. IGMP

        Answer:

        A, B. The Internet Protocol (IP) in both of its versions (IPv4 and IPv6) includes a TTL field in its message header that limits the number of times a packet can be routed on a network. Each router processing the packet reduces the TTL value by one until it reaches zero, after which it is discarded. The Internet Control Message Protocol (ICMP) and the Internet Group Management Protocol (IGMP) do not have a TTL field.
103.    Which of the following is not a method of traffic shaping?

        1. Rate limiting
        2. WAN optimization
        3. Bandwidth throttling
        4. Self-limiting

        Answer:

        B. WAN optimization is not a form of traffic shaping, because it compresses data streams and transmits incremental file updates. Traffic shaping uses techniques like rate limiting, bandwidth throttling, and self-limiting to delay the transmission of specific types of data packets to optimize network performance.
104.    An enterprise network has been designed with individual departmental switches because, in most cases, the devices in a specific department exchange network traffic with other devices in the same department. Each of the departmental switches is also connected to a host switch, which enables devices to communicate with other departments. Which of the following terms describes this switching architecture?

        1. Distributed switching
        2. Port forwarding
        3. Traffic shaping
        4. Neighbor discovery
        5. Flow control

        Answer:

        A. Distributed switching describes a hierarchical switching architecture in which remote switches (departmental switches in this case) handle most of the network traffic, with a host switch used only for traffic between the remote locations. Port forwarding is a routing method that redirects traffic intended for one IP address and port number to another. Traffic shaping is a series of techniques that optimize the allocation of network bandwidth. Neighbor discovery is an IPv6 technique used to find addresses of devices and services on the local network. Flow control is a technique for regulating a system's transmission speed.
105.    Review the following figure. Note that each store-and-forward switch has three connected node ports and one port for switch-to-switch connections. All node ports and links are configured for half-duplex communication. The switch-to-switch links are configured for full-duplex communication. Which of the following statements about the switched network is true?

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c02uf004_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

        1. There are nine collision domains, one for each half-duplex connection.
        2. There are 12 collision domains, one for each switch connection.
        3. There are three collision domains, one for each switch-to-switch connection.
        4. There is one collision domain for this network.

        Answer:

        A. All half-duplex port connections on a store-and-forward switch represent a different collision domain. Full-duplex connections are not subject to collisions, so they do not define separate collision domains.
106.    Which of the following could be a valid MAC address for a network interface adapter?

        1. 10.124.25.43
        2. FF:FF:FF:FF:FF:FF
        3. 00:1A:6B:31:9A:4E
        4. 03:AE:16:3H:5B:11
        5. fe80::89a5:9e4d:a9d0:9ed7

        Answer:

        C. A Media Access Control (MAC) address is a 6-byte hexadecimal value, with the bytes separated by colons, as in 00:1A:6B:31:9A:4E. Option A, 10.124.25.43, is all decimals and uses periods; this is an IPv4 address. Option B, FF:FF:FF:FF:FF:FF, is a valid MAC address, but this value is reserved for use as a broadcast address. Option D, 03:AE:16:3H:5B:11, is not a valid hexadecimal address, which should contain only numerals and the letters A to F. Option E, fe80::89a5:9e4d:a9d0:9ed7, is too long for a MAC address; this is a valid IPv6 address.
107.    Which of the following protocols prevents network switching loops from occurring by shutting down redundant links until they are needed?

        1. RIP
        2. STP
        3. VLAN
        4. NAT
        5. ARP

        Answer:

        B. The Spanning Tree Protocol (STP) prevents packets from endlessly looping from switch to switch due to redundant links. Creating redundant links is a good preventive against switch failure, but packets transmitted over multiple links can circulate from switch to switch infinitely. STP creates a database of switching links and shuts down the redundant ones until they are needed. Routing Information Protocol (RIP) propagates routing table information. A Virtual Local Area Network (VLAN) is an organizational tool that operates within switches by creating multiple broadcast domains. Network Address Translation (NAT) is a routing method that enables private networks to share registered IP addresses. Address Resolution Protocol (ARP) is a protocol that discovers a system's MAC address by broadcasting its IPv4 address.
108.    Which of the following cable types can be used to connect an MDI port on a workstation to an Auto-MDI-X port on an Ethernet switch? (Choose all that apply.)

        1. A crossover twisted pair cable
        2. A straight-through twisted pair cable
        3. A coaxial cable
        4. A single-mode fiber optic cable
        5. A multimode fiber optic cable

        Answer:

        A, B. When connecting an MDI port to an Auto-MDI-X port, it is possible to use either a straight-through or a crossover cable because the Auto-MDI-X port can self-adjust to implement the necessary crossover circuit if it is needed. MDI and Auto-MDI-X ports are used only with twisted pair cables, so there is no need for coaxial or fiber optic cables.
109.    Which of the following is a network layer protocol that uses ICMPv6 messages to locate routers, DNS servers, and other nodes on an IPv6 network?

        1. BGP
        2. NDP
        3. OSPF
        4. PoE

        Answer:

        B. The Neighbor Discovery Protocol (NDP) is a network layer protocol that defines five new Internet Control Message Protocol version 6 (ICMPv6) packet types, which enable IPv6 systems to locate resources on the network, such as routers and DNS servers, as well as autoconfigure and detect duplicate IPv6 addresses. Border Gateway Protocol (BGP) is an exterior gateway protocol that is designed to exchange routing information among autonomous systems. Open Shortest Path First (OSPF) is a link state routing protocol that enables routers to exchange routing table information. Power over Ethernet (PoE) is a general term for standards defining mechanisms for power delivery over Ethernet cables, along with data signals.
110.    Which of the following is a protocol that identifies VLANs by inserting a 32-bit field in the Ethernet frame?

        1. IEEE 802.1P
        2. IEEE 802.1Q
        3. IEEE 802.1X
        4. IEEE 802.1AB
        5. IEEE 802.1AX

        Answer:

        B. IEEE 802.1Q is a standard defining a mechanism (called Ethernet trunking by some manufacturers) that identifies the Virtual Local Area Network (VLAN) to which a packet belongs by inserting an extra 32-bit field into its Ethernet frame. IEEE 802.1P is a standard that defines a mechanism for implementing Quality of Service (QoS) at the data link layer by adding a 3-bit field into Ethernet frames. IEEE 802.1X is a standard defining an authentication mechanism called Port-based Network Access Control (PNAC). IEEE 802.1AB is a standard defining the Link Layer Discovery Protocol (LLDP). IEEE 802.1AX is a specification for the Link Aggregation Control Protocol (LACP), which is a mechanism for combining physical ports into a single logical channel.
111.    Each of the following Carrier-Sense Multiple Access with Collision Detection (CSMA/CD) events occurs on an Ethernet network when two stations transmit simultaneously, although not in the order listed. Which of the following events occurs immediately after the collision?

        1. The two stations observe a random backoff interval.
        2. The two stations transmit a jam signal.
        3. The two stations stop transmitting.
        4. The two stations listen to see if the channel is idle.
        5. The two stations begin retransmitting their frames.

        Answer:

        C. Stations on a CSMA/CD network first check the medium to see if it is idle. If they detect an idle medium, they begin transmitting. If two or more devices transmit at the same time, a collision occurs. Immediately after a collision occurs, the two stations involved stop transmitting. After that, they send out a jam signal. Then, the two stations back off for a random interval, and the transmission process begins again.
112.    For the Carrier-Sense Multiple Access with Collision Detection (CSMA/CD) mechanism to function properly on an Ethernet network, host systems must be able to detect when a collision occurs, so they can react to it. Which of the following cabling errors can prevent the collision detection process from functioning properly?

        1. Excessively long cable segments
        2. Incorrect wiring pinouts
        3. Too many systems on a single network
        4. An excessive number of collisions

        Answer:

        A. For CSMA/CD to function properly, a system must detect a packet collision while it is transmitting the packet. If cable segments are too long, the packet might leave the transmitting system before the collision is detected, resulting in a late collision, which cannot be retransmitted. Incorrect pinouts, too many systems, and excessive collisions typically will not prevent the collision detection system from occurring.
113.    When a packet collision between two systems occurs on an Ethernet network, Carrier-Sense Multiple Access with Collision Detection (CSMA/CD) causes the two systems to stop transmitting and generate a jam signal. After sending the jam signal, why do the two systems wait for a randomized backoff interval before retransmitting their packets?

        1. They need time to reassemble the packets.
        2. To prevent another collision from occurring.
        3. They need to rebuffer the packet.
        4. To recalculate the packets’ checksum values.

        Answer:

        B. After transmitting their jam signals, the two systems wait for a randomized interval. This is to prevent them from retransmitting their packets at the same time, resulting in another collision. It is not necessary for the systems to reassemble, rebuffer, or recalculate checksums for their packets.
114.    Which of the following devices is used to physically connect computers in the same VLAN?

        1. A bridge
        2. A hub
        3. A switch
        4. A router

        Answer:

        C. Replacing routers with switches turns an internetwork into a single large subnet, and Virtual Local Area Networks (VLANs) exist as logical elements on top of the switching fabric. Although VLANs are the functional equivalent of network layer subnets, the systems in a single VLAN are still physically connected by switches, not routers. Bridges connect network segments at the data link layer and selectively forward traffic between the segments. However, bridges do not provide a dedicated connection between two systems like a switch does, and they do not make it possible to convert a large, routed internetwork into a single switched network. Therefore, they have no role in implementing VLANs. Hubs are physical layer devices that propagate all incoming traffic out through all of their ports. Replacing the routers on an internetwork with hubs would create a single shared broadcast domain with huge amounts of traffic and many collisions. Hubs, therefore, do not connect the computers in a VLAN.
115.    Which of the following statements is true about an Ethernet network that uses CSMA/CD?

        1. Collisions are a normal occurrence.
        2. Collisions never occur unless there is a network fault.
        3. Collisions cause data to be irretrievably lost.
        4. Collisions are the result of duplicate IP addresses.

        Answer:

        A. Collisions are a normal occurrence on an Ethernet network; they occur when two nodes transmit at exactly the same time. There need not be a network fault for collisions to occur. When collisions occur, the nodes involved retransmit their packets so that no data is lost. Collisions are a phenomenon of data link layer protocols; they have nothing to do with IP addresses, which are network layer constructs.
116.    Which of the following is an abnormal occurrence on an Ethernet network?

        1. Packet retransmissions
        2. Collision detection
        3. Jam signals
        4. Late collisions

        Answer:

        D. Collisions are a normal occurrence on an Ethernet network, but late collisions are not normal. Late collisions occur when two packets collide after one or more finishes transmitting. Packet retransmissions, collision detection, and jam signals are all normal occurrences on an Ethernet network.
117.    VLANs create the administrative boundaries on a switched network that are otherwise provided by which of the following devices?

        1. Hubs
        2. Routers
        3. Domains
        4. Bridges

        Answer:

        B. Connecting subnets with routers at the network layer maintains the data link layer administrative boundaries that prevent broadcast transmissions from being propagated throughout the entire internetwork. Switching eliminates those data link layer boundaries, and administrators can use Virtual Local Area Networks (VLANs) to simulate them. Because hubs propagate all of the traffic they receive out through all of their ports indiscriminately, they create no administrative boundaries. Domains are logical groups of network devices defined by the Domain Name System (DNS). Their functions are not related to VLANs in any way. Switches are essentially multiport bridges that forward incoming traffic only to the device for which it is destined. Therefore, bridges are more closely related to eliminating administrative boundaries than to establishing them.
118.    Which of the following statements about VLANs are true? (Choose all that apply.)

        1. All of the devices in a particular VLAN must be physically connected to the same switch.
        2. A VLAN creates a limited broadcast domain on a switched network.
        3. You must have VLANs on a switched network for communication between computers on different cable segments to occur.
        4. A router is required for communication between VLANs.

        Answer:

        B, D. The computers in a single Virtual Local Area Network (VLAN) can be located anywhere on a switched network, irrespective of the switches' physical configuration. A broadcast message generated by a computer in a VLAN is transmitted to all of the other computers in that VLAN only, just as if the systems were physically located on a separate LAN or subnet. Unicast transmissions between computers on a switched network do not require VLANs, because the switches create what amounts to a direct connection between the two systems. VLANs are needed only for communication processes that require the use of broadcasts, which if transmitted without VLANs, would flood the network. Even though they are a purely logical construction, VLANs function just like physical subnets and require routers for communication between them. Routing capabilities are often integrated into switches to enable communication between VLANs.
119.    Which of the following elements can be used to identify the devices in a particular VLAN? (Choose all that apply.)

        1. Hardware addresses
        2. IP addresses
        3. DNS names
        4. Switch port numbers

        Answer:

        A, D. Every network device has a unique hardware address coded into its network interface adapter, and administrators can use these addresses to select the devices that will be part of a specific Virtual Local Area Network (VLAN). When VLANs are implemented inside the switch, selecting the ports to which specific computers are attached is a simple way to identify the computers in a particular VLAN. IP addresses are layer 3 (network layer) constructs, so they do not apply to layer 2 (data link layer) devices like switches. Although DNS names do uniquely identify computers on a network, DNS is an application layer process and has nothing to do with the switching and routing processes, which occur at the data link and network layers. Therefore, you cannot use DNS names to identify the computers in a VLAN.
120.    Alice has a network that consists of three Virtual LANs (VLANs) defined on all of the network's switches. VLAN 10 is the Sales VLAN, VLAN 20 is the Marketing VLAN, and VLAN 30 is the Accounting VLAN. Users are reporting that they cannot communicate with anyone outside of their own VLANs. What is the problem, and what must Alice do?

        1. The problem is a faulty VLAN configuration on one of the switches. Alice needs to re-create the VLANs and configure each VLAN for routing.
        2. One of the VLANs is configured to filter all other VLAN traffic for security purposes. Alice needs to change the filter on this VLAN.
        3. VLANs are limited to data link layer communication only. To allow communication between VLANs, Alice must add a router or a layer 3 switch to the network and configure it to route traffic between the VLANs.
        4. The VLANs are using different data link layer protocols. VLANs must use the same data link layer protocol in order to communicate.

        Answer:

        C. VLANs are data link layer Local Area Networks (LANs) defined within switches. Only devices (and users) connected to ports belonging to the same VLAN can communicate with each other until a layer 3 device, such as a router or a layer 3 switch, is added to the network. Re-creating and reconfiguring the VLANs will not correct this problem. Traffic filters are usually implemented on routers. VLANs do not have to use the same data link protocol.
121.    The jumbo frame capability is associated with which layer of the Open Systems Interconnection (OSI) model?

        1. Application
        2. Transport
        3. Network
        4. Data link

        Answer:

        D. Ethernet uses jumbo frames at the data link layer to transfer large amounts of data more efficiently. Ethernet typically restricts frame size to 1500 bytes, but jumbo frames enable Ethernet systems to create frames up to 9000 bytes. Frames are protocol data units associated only with the data link layer, so they do not apply to the network, transport, or application layer.
122.    Which of the following technologies would you be less likely to find on the average home or small office network? (Choose all that apply.)

        1. NAT
        2. DHCP
        3. 10GBase-T
        4. VLAN

        Answer:

        C, D. Home and small office networks typically consist of a single subnet and require only a basic switch without the advanced Virtual Local Area Network (VLAN) capabilities that enable administrators to create separate subnets. Most home and small office networks have a Dynamic Host Configuration Protocol (DHCP) server that assigns IP addresses and other TCP/IP configuration settings to clients. The DHCP server can be integrated into a broadband router or another Internet access sharing solution. Most home and small office networks support Network Address Translation (NAT), enabling them to use private IP addresses and still access the Internet. 10GBase-T is the designation for UTP-based 10 Gigabit Ethernet, which is an advanced standard for network interface adapters often found in servers.
123.    Which of the following modifications occur when you configure the native Virtual Local Area Network (VLAN) on your network switches to use 802.1q tagging? (Choose all that apply.)

        1. Double-tagged packets are prevented.
        2. BPDU guards are applied.
        3. Root guards are applied.
        4. Trunk traffic is routed, not switched.

        Answer:

        A, B. To join ports on different switches into one VLAN, you designate a trunk port on each switch for the traffic between switches. Initially, the native VLAN uses the default VLAN1 for trunk traffic, and that traffic is left untagged. Untagged traffic is susceptible to attacks using double-tagged packets. When you configure the native VLAN to use tagging, this makes it impervious to double-tagging. Changing the native VLAN does not create root guards or Bridge Protocol Data Unit (BPDU) guards, and all traffic continues to be switched, not routed.
124.    Which of the following protocols is responsible for inserting the tags into frames that enable switches to forward them to the appropriate Virtual Local Area Network (VLAN)?

        1. IEEE 802.3x
        2. IEEE 802.1X
        3. IEEE 802.1q
        4. IEEE 802.11ac

        Answer:

        C. The IEEE 802.1q protocol is responsible for VLAN tagging, a procedure that enables network switches to support VLANs. Through the insertion of VLAN identifier tags into frames, switches can determine which VLAN each packet is destined for and forward it to the correct ports. IEEE 802.3x is one of the standards for wired Ethernet networks. IEEE 802.1X is a standard that defines a Port-based Network Access Control (PNAC) mechanism used for authentication on wireless and other networks. IEEE 802.11ac is a standard defining the physical and data link layer protocols for wireless networks.
125.    Which of the following best explains how tagging the native Virtual Local Area Network (VLAN) traffic can improve in-band switch management security?

        1. By renaming the default VLAN
        2. By preventing double-tagged packets
        3. By encrypting in-band management traffic
        4. By moving in-band management traffic off the native VLAN

        Answer:

        B. When in-band switch management traffic, such as that generated by a Secure Shell (SSH) connection to a switch, uses the native VLAN, it is untagged by default. This is because the native VLAN is at first the default VLAN1, which is not tagged by the 802.1q protocol, leaving it open to certain types of double-tagging attacks. When you tag the native VLAN traffic, it is rendered immune to double-tagging. The default VLAN cannot be renamed, and SSH traffic is already encrypted by the sending workstation. Changing the native VLAN does not move the management traffic off that VLAN, although many authorities advocate the creation of a separate VLAN dedicated to in-band management traffic.
126.    A switch with auto-medium-dependent interface crossover (MDI-X) ports eliminates the need for which of the following?

        1. 8P8C connectors
        2. Switch-to-switch connections
        3. Straight-through cables
        4. Crossover cables

        Answer:

        D. Ethernet implementations, such as 100Base-TX, which use separate wire pairs for transmitting and receiving data, require a crossover circuit to ensure that the transmit pins on each end of a connection are wired to the receive pins at the other end. This crossover circuit can be implemented in a patch cable—called a crossover cable—or by a switch port. Switches with auto-medium-dependent interface crossover (MDI-X) ports can detect the need for a crossover circuit and implement it automatically in the port. This eliminates the need for crossover cables. Auto-medium-dependent interface crossover (MDI-X) ports do not eliminate the need for 8P8C connectors, connections between switches, or straight-through cables.
127.    Which of the following cable types is needed to connect an MDI port on a workstation to an MDI-X port on an Ethernet switch?

        1. A crossover twisted pair cable
        2. A straight-through twisted pair cable
        3. A coaxial cable
        4. A single-mode fiber optic cable
        5. A multimode fiber optic cable

        Answer:

        B. When connecting an MDI port to an MDI-X port, the necessary crossover circuit is implemented in the MDI-X port. Therefore, the connection needs a straight-through cable, and there is no need for a crossover cable. MDI and MDI-X ports are used only with twisted pair cables, so there is no need for coaxial or fiber optic cables.
128.    Port security on an Ethernet switch is implemented through the use of which of the following methods?

        1. Blacklisted MAC addresses
        2. Whitelisted MAC addresses
        3. Port-by-port MAC address filtering
        4. Spoofed MAC addresses

        Answer:

        C. When implemented in an Ethernet switch, port security uses port-by-port MAC address filtering to allow only one MAC address to access each switch port. Blacklisting blocks the MAC addresses on the list from using all of the ports on the switch. Whitelisting allows the listed MAC addresses to use any port on the switch. MAC address spoofing is a method for defeating port security, blacklists, or whitelists.
129.    Which of the following best explains why networks using Voice over IP (VoIP) often have separate voice and data Virtual Local Area Networks (VLANs)?

        1. To prevent voice and data packet conflicts
        2. To encrypt voice traffic
        3. To encrypt data traffic
        4. To prioritize voice traffic

        Answer:

        D. When transmitting voice traffic on a network along with data traffic, the voice traffic should have priority, to ensure the quality of the stream. Separating data and voice traffic on separate VLANs enables switches to assign voice traffic a higher priority by applying appropriate tags to the voice packets. Separate VLANs are not needed to prevent packet conflicts or to encrypt either voice or data packets.
130.    Which of the following protocols uses a form of flow control called the sliding window technique?

        1. UDP
        2. HTTP
        3. TCP
        4. DNS

        Answer:

        C. The Transmission Control Protocol (TCP) protocol uses a flow control technique in which the receiving system creates a window of a specific size and allows the transmitting system to send packets until that window is full. When the window is full, the sender stops transmitting. The receiver then sends back an acknowledgment packet that specifies the next packet it expects to receive from the sender. The User Datagram Protocol (UDP), Hypertext Transfer Protocol (HTTP), and Domain Name System (DNS) do not use the sliding window technique or any other form of flow control.
131.    Which of the following Power over Ethernet (PoE) specifications supplies power to devices using the spare wire pair on a 10Base-T or 100Base-TX twisted pair network?

        1. Alternative A
        2. Alternative B
        3. 4PPoE
        4. All of the above

        Answer:

        B. The Alternative B PoE variant can use the spare wire pair in a CAT 5 or better 10Base-T or 100Base-TX cable to supply power to connected devices. The Alternative A and 4PPoE variants cannot use the spare wire pair in this manner; they supply power using the wire pairs that carry data at the same time. For Gigabit Ethernet or faster installations, Alternative B is also capable of using the data wire pairs.
132.    Which of the following best describes the process of whitelisting on a wireless network?

        1. Using an Access Control List (ACL) to specify the IP addresses that are permitted to access a wireless network
        2. Using port protection to specify the well-known port numbers of applications that users are permitted to run over a wireless network
        3. Using MAC filtering to create a list of devices that are permitted to access a wireless network
        4. Using an AAA server to create a list of users that are permitted to access a wireless network

        Answer:

        C. Whitelisting is the process of using MAC filtering to specify the hardware addresses of devices that are permitted to access a wireless network. Blacklisting, by contrast, is making a list of addresses that are denied access to the network.
133.    Which of the following features helps to protect network switches from attacks related to the Spanning Tree Protocol (STP)? (Choose all that apply.)

        1. BPDU guard
        2. Root guard
        3. DHCP snooping
        4. Geofencing

        Answer:

        A, B. Bridge Protocol Data Units (BPDUs) are messages that switches running the STP exchange to learn about the available paths through a switched network and the states of other switches. Switches should only receive BPDUs through ports that are connected to other switches. BPDU guard is a feature that prevents BPDU messages from arriving through ports connected to end systems, such as computers, thus preventing an attacker from manipulating the STP topology. A root guard affects the behavior of the STP by enforcing the selection of root bridge ports on a switched network. Without root guards, there is no way for administrators to enforce the topology of a network with a redundant switching fabric.
134.    Which of the following IEEE standards calls for the use of the Carrier-Sense Multiple Access with Collision Avoidance (CSMA/CA) Media Access Control (MAC) mechanism?

        1. 802.11ac
        2. 802.1X
        3. 802.3
        4. All of the above

        Answer:

        A. The IEEE 802.11ac standard, like all of the wireless LAN standards in the 802.11 working group, uses CSMA/CA for MAC. The 802.1X standard defines an authentication mechanism and does not require a MAC mechanism. The IEEE 802.3 (Ethernet) standard uses Carrier-Sense Multiple Access with Collision Detection (CSMA/CD).
135.    Which of the following topologies enables wireless devices to access resources on a wired network?

        1. Ad hoc
        2. Star
        3. Infrastructure
        4. Bus

        Answer:

        C. An infrastructure topology uses a Wireless Access Point (WAP) to connect wireless devices to a wired network. An ad hoc topology connects wireless devices to each other, without connecting to a wired network. The star and bus topologies do not support wireless devices.
136.    Which of the following components are required for two computers to communicate using an IEEE 802.11 wireless LAN in an ad hoc topology?

        1. A router connected to the Internet
        2. A Wireless Access Point (WAP)
        3. An external antenna
        4. None of the above

        Answer:

        D. An ad hoc topology describes wireless computers that communicate directly with each other, without the need for any hardware other than their wireless network adapters. The ad hoc topology therefore does not require a router, an Internet connection, an Access Point (AP), or a special antenna.
137.    Which of the following wireless networking technologies will never experience interference from a 2.4 GHz wireless telephone? (Choose all that apply.)

        1. IEEE 802.11a
        2. IEEE 802.11b
        3. IEEE 802.11g
        4. IEEE 802.11n
        5. IEEE 802.11ac
        6. IEEE 802.11ax

        Answer:

        A, E. IEEE 802.11b, 802.11g, 802.11n, and 802.11ax networks can use the 2.4 GHz frequency band for their transmissions, which can experience interference from a wireless telephone using the same frequency. IEEE 802.11a and IEEE 802.11ac, however, use the 5 GHz band, which will not experience interference from a 2.4 GHz phone.
138.    Which of the following wireless networking standards is capable of supporting speeds of 54 Mbps and is also backward compatible with IEEE 802.11b?

        1. IEEE 802.11a
        2. IEEE 802.11g
        3. IEEE 802.11n
        4. Bluetooth
        5. IEEE 802.11

        Answer:

        B. IEEE 802.11g supports transmission speeds up to 54 Mbps, and it is backward compatible with 802.11b equipment. IEEE 802.11 cannot run at 54 Mbps, and while 802.11a can, it is not compatible with 802.11b. IEEE 802.11n cannot run at 54 Mbps, though it can run at faster speeds. Bluetooth is not compatible with any of the IEEE 802.11 standards.
139.    Which of the following wireless LAN standards include the ability to use Multiple Input, Multiple Output (MIMO) antennae? (Choose all that apply.)

        1. IEEE 802.11a
        2. IEEE 802.11b/g
        3. IEEE 802.11n
        4. IEEE 802.11ac
        5. IEEE 802.11ax

        Answer:

        C, D, E. The IEEE 802.11n, 802.11ac, and 802.11ax standards include MIMO, which enables them to effectively multiplex signals using multiple antennae. This capability was first introduced in the 802.11n standard, so the 802.11a and 802.11b/g standards do not support it.
140.    Which of the following is a cellular communication technology that is virtually obsolete in the United States?

        1. GSM
        2. CDMA
        3. TDMA
        4. LTE

        Answer:

        C. Time Division Multiple Access (TDMA) is a communication technique that splits a frequency into multiple time slots, enabling it to carry multiple data streams. Commonly used in 2G cellular systems, the major U.S. carriers no longer use it in their 3G systems. Code Division Multiple Access (CDMA), Global System for Mobile Communications (GSM), and Long-Term Evolution (LTE) are alternative communications techniques that are currently used by the major U.S. cellular carriers.
141.    Which of the following IEEE wireless LAN standards uses the Direct Sequence Spread Spectrum (DSSS) signal modulation technique?

        1. 802.11a
        2. 802.11b
        3. 802.11g
        4. 802.11n
        5. 802.11ac

        Answer:

        B. The IEEE 802.11b standard calls for DSSS signal modulation. All of the other standards listed call for Orthogonal Frequency-Division Multiplexing (OFDM) encoding.
142.    When designing a wireless LAN installation, which of the following are valid reasons to install a unidirectional antenna in an Access Point (AP), rather than an omnidirectional one? (Choose all that apply.)

        1. The AP will be located against an outside wall.
        2. There are many interior walls between the AP and the most distant workstation.
        3. A unidirectional antenna can be focused to a specific signal pattern width.
        4. All of the above

        Answer:

        D. By placing a unidirectional antenna against an outside wall, you can limit network access to users inside the structure. Unidirectional antennae provide greater signal strength than omnidirectional antennae, enabling their signals to penetrate more interior walls. It is possible to focus a unidirectional antenna to a wider or narrower signal pattern.
143.    How do wireless networking devices conforming to the IEEE 802.11n and 802.11ac standards achieve transmission speeds greater than 72.2 Mbps?

        1. By using direct sequence spread spectrum (DSSS) modulation
        2. By using multiple antennae to transmit several data streams simultaneously
        3. By using frequencies in the 5 GHz band
        4. By sacrificing transmission range for speed

        Answer:

        B. The IEEE 802.11n and 802.11ac standards support a transmission technique called Multiple Input, Multiple Output (MIMO), which combines the bandwidth of multiple data streams to achieve greater throughput. IEEE 802.11n and 802.11ac do use the 5 GHz band, but this in itself does not yield greater transmission speeds. The specified standards do not call for the use of DSSS modulation, nor do they sacrifice range for speed. In fact, 802.11n and 802.11ac networks can achieve greater ranges than the previous technologies.
144.    Which of the following are possible reasons why the 5 GHz frequency tends to perform better than the 2.4 GHz frequency on a wireless LAN? (Choose all that apply.)

        1. The 5 GHz frequency has more channels than the 2.4 GHz frequency.
        2. The 5 GHz frequency supports longer ranges than the 2.4 GHz frequency.
        3. The 5 GHz frequency conflicts with fewer common household devices than the 2.4 GHz frequency.
        4. The 5 GHz frequency transmits at faster speeds than the 2.4 GHz frequency.

        Answer:

        A, C, D. The 5 GHz frequency has 23 channels available in the United States, while the 2.4 GHz frequency has only 11. Many household devices, such as cordless telephones, use the 2.4 GHz frequency band, but relatively few devices use the 5 GHz band. Higher frequencies typically support faster transmission speeds, because with all other conditions equal, they can carry more data in the same amount of time. The 5 GHz frequency typically has a shorter range than 2.4 GHz, because it is less able to penetrate barriers.
145.    Alice is attempting to deploy an IEEE 802.11b/g wireless LAN on the fifth floor of a 10-story office building that is surrounded on all sides by other office buildings, all of which seem to be running many wireless LANs. Scanning the 2.4 GHz band, she sees literally dozens of networks, spread across all of the available channels. As a result, her wireless devices have trouble connecting to their Access Point (AP), and when they do, they achieve only low speeds. Which of the following tasks should Alice perform to enable the wireless clients to connect to the network more reliably? (Choose two.)

        1. Upgrade all of the wireless network devices to IEEE 802.11n.
        2. Configure all of the network devices to use WPA2 encryption with AES.
        3. Configure the wireless devices to use the 5 GHz band.
        4. Configure the AP to suppress SSID broadcasts.
        5. Upgrade all of the network devices to the latest firmware.

        Answer:

        A, C. Upgrading the devices to 802.11n will enable them to use the 5 GHz band and evade the traffic generated by the surrounding networks. Configuring the devices to use the 5 GHz band will provide many more channels to choose from and will avoid the interference from the surrounding 2.4 GHz networks. The type of encryption that a wireless network uses has no bearing on the ability of the devices to avoid the interference generated by surrounding networks. Suppressing SSID broadcasts will not help the devices to connect to the network. Upgrading the firmware on the devices is not likely to have any effect on the connection problems when they are the result of interference from other networks.
146.    Which of the following is the fastest speed achievable by a wireless LAN using the currently ratified IEEE 802.11 standards?

        1. 54 Mbps
        2. 600 Mbps
        3. 1.3 Gbps
        4. 2.6 Gbps

        Answer:

        C. The 802.11ac standard defines a wireless LAN running at a speed of up to 1.3 gigabits per second (Gbps). None of the other ratified 802.11 standards call for speeds beyond 600 megabits per second (Mbps). No currently ratified standard enables speeds of 2.6 Gbps.
147.    What is the term for the technology implemented in the IEEE 802.11ac standard that enables a wireless device to transmit multiple frames to multiple clients simultaneously?

        1. MIMO
        2. Channel bonding
        3. CSMA/CA
        4. MU-MIMO

        Answer:

        D. The Multiple Input, Multiple Output (MIMO) technology introduced in the IEEE 802.11n standard enables wireless devices to transmit and receive signals using multiple antennae simultaneously. The Multiuser MIMO (MU-MIMO) variant defined in the 802.11ac standard advances this technique by enabling wireless devices to transmit multiple frames to different users simultaneously, using multiple antennae. Carrier-Sense Multiple Access with Collision Avoidance (CSMA/CA) is a Media Access Control (MAC) mechanism used by all 802.11 networks. Channel bonding is a wireless networking technique that combines channels to increase bandwidth.
148.    On an IEEE 802.11b/g/n wireless network running at 2.4 GHz with multiple Access Points (APs), the traditional best practice is to use channels 1, 6, and 11, with no two adjacent APs configured to use the same channel. Which of the following is the real reason why this is a good plan?

        1. Channels 1, 6, and 11 are the only channels with frequencies that do not overlap.
        2. Channels 1, 6, and 11 have more bandwidth than the other channels.
        3. Channels 1, 6, and 11 have greater ranges than the other channels.
        4. Channels 1, 6, and 11 are the default settings on most wireless devices.

        Answer:

        A. Wireless LAN regulations call for 22 MHz channels in the 2.4 GHz band that are spaced 5 MHz apart, which means that they overlap. Channels 1, 6, and 11 are the only three channels that are distant enough from each other not to overlap. Therefore, they do not interfere with each other. Channels 1, 6, and 11 do not differ from the other channels in their bandwidth or their transmission range. Each wireless device can be set to use only one channel. Therefore, channels 1, 6, and 11 cannot all be the default setting.
149.    Ralph is planning a wireless LAN installation for a warehouse with two offices at either end of the building, approximately 300 feet apart. If he installs a single Access Point (AP) in the center of the warehouse, equidistant from the two offices, which of the following standards should he look for when purchasing hardware so that workstations in both offices will be able to connect to the network at the best possible speed?

        1. IEEE 802.11a
        2. IEEE 802.11g
        3. IEEE 802.11n
        4. IEEE 802.11ac

        Answer:

        C. Wireless networks using equipment based on the IEEE 802.11n standard can span indoor distances of up to 175 feet at speeds up to 600 Mbps. An 802.11ac network can run at faster speeds—up to 1.3 Gbps—but it is limited to approximately 115-foot distances. Networks using 802.11g equipment can span 150 feet, but they run at only a maximum of 54 Mbps. An 802.11a network cannot span more than 75 feet, and it runs at no more than 54 Mbps.
150.    Which of the following terms defines a wireless LAN transmission technique in which devices use multiple antennae to increase transmission speeds?

        1. MIMO
        2. TDMA
        3. PAN
        4. Ant+

        Answer:

        A. Multiple Input, Multiple Output (MIMO) calls for the use of two or more antennae, enabling wireless devices to effectively multiplex signals, thereby increasing their transmission speeds. Time Division Multiple Access (TDMA) is a communication technique that splits a frequency into multiple time slots, enabling it to carry multiple data streams. A Personal Area Network (PAN) provides communication among devices associated with a single person, such as smartphones. Ant+ is a wireless protocol that is typically used to monitor data gathered by sensors, such as those in cardiac pacemakers.
151.    What is the maximum channel width possible using wireless networking equipment based on the ratified IEEE 802.11 regulatory standards?

        1. 20 MHz
        2. 40 MHz
        3. 80 MHz
        4. 160 MHz

        Answer:

        D. Using a technique called channel bonding, the 802.11ac standard defines the combination of up to eight 20 MHz channels, for a total possible channel width of 160 MHz. The 802.11n standard can bond up to two channels, for a 40 MHz width. Earlier standards are limited to a single 20 MHz channel.
152.    Which of the following wireless networking standards are capable of using only the 5 GHz frequency? (Choose all that apply.)

        1. IEEE 802.11a
        2. IEEE 802.11b
        3. IEEE 802.11g
        4. IEEE 802.11n
        5. IEEE 802.11ac

        Answer:

        A, E. The IEEE 802.11a and IEEE 802.11ac standards can use the 5 GHz band only. IEEE 802.11b and IEEE 802.11g can use the 2.4 GHz band only. IEEE 802.11n can use either the 2.4 or 5 GHz band.
153.    Which of the following IEEE wireless LAN standards provides the greatest possible throughput?

        1. 802.11a
        2. 802.11ac
        3. 802.11b
        4. 802.11g
        5. 802.11n

        Answer:

        B. The IEEE 802.11ac standard provides the greatest possible throughput, at up to 1.3 Gbps. The 802.11n standard runs at speeds up to 600 Mbps. The 802.11a and 802.11g standards run at up to 54 Mbps. The 802.11b standard runs at up to 11 Mbps.
154.    Which of the following IEEE 802.11 wireless LAN standards are capable of supporting both the 2.4 GHz and 5 GHz frequencies?

        1. 802.11a
        2. 802.11b
        3. 802.11g
        4. 802.11n
        5. 802.11ac

        Answer:

        D. Only the 802.11n standard defines wireless LAN devices that can support both 2.4 GHz and 5 GHz frequencies. The 802.11a and 802.11ac standards use only 5 GHz, and the 802.11b and 802.11g standards use only 2.4 GHz.
155.    What is the maximum number of transmit and receive antennae supported by the currently ratified IEEE 802.11 wireless LAN standards?

        1. 2
        2. 4
        3. 8
        4. 16

        Answer:

        C. The 802.11ac standard supports Multiple Input, Multiple Output (MIMO) through the use of up to eight antennae on a single device. 802.11n is the only earlier 802.11 standard that supports MIMO, but it can only use a maximum of four antennae.
156.    Which of the following is the term for the network name that you use to connect a client device to an Access Point (AP) on a wireless LAN?

        1. BSS
        2. ESS
        3. SSID
        4. BSSID

        Answer:

        C. The Service Set Identifier (SSID) is the name that you use when connecting to a wireless network. A Basic Service Set (BSS) refers to the wireless network itself, consisting of a single AP and a number of clients. An Extended Service Set (ESS) consists of two or more BSSs, using multiple APs. The Basic Service Set Identifier (BSSID) is the MAC address of the Access Point associated with a BSS.
157.    Which of the following IEEE wireless LAN standards define devices with a maximum aggregate channel width of 20 MHz? (Choose all that apply.)

        1. 802.11a
        2. 802.11g
        3. 802.11n
        4. 802.11ac

        Answer:

        A, B. Devices conforming to the IEEE 802.11a and 802.11g standards can only use a single 20 MHz channel. IEEE 802.n devices can use channel bonding to join two channels together and achieve an aggregate channel width of 40 MHz. IEEE 802.11ac devices can bond up to eight channels, for an aggregate width of 160 MHz.
158.    At which layer of the Open Systems Interconnection (OSI) model do wireless range extenders operate?

        1. Physical
        2. Data link
        3. Network
        4. Transport
        5. Session
        6. Presentation
        7. Application

        Answer:

        A. Wireless range extenders are physical layer devices that receive signals from Wireless Access Points (WAPs) and network adapters and retransmit them, enabling devices to connect that are farther apart than the network would normally support. Because the extenders do not process the packets in any way, but just retransmit the signals, they do not operate at any layer above the physical.
159.    Which of the following wireless security protocols provides the greatest degree of network device hardening?

        1. WEP
        2. WPA
        3. WPA2
        4. EAP

        Answer:

        C. WPA2 is the most secure of the wireless protocols, providing the greatest degree of network device hardening. WiFi Protected Access (WPA) was created to replace the insecure Wired Equivalent Privacy (WEP) protocol, and WPA2 was created to replace the Temporal Key Integrity Protocol (TKIP) used in the first version of WPA with Advanced Encryption Standard (AES). Extensible Authentication Protocol (EAP) is a framework for the encapsulation of authentication messages.
160.    Which of the following encryption protocols was introduced in the WiFi Protected Access (WPA) wireless security standard?

        1. CCMP-AES
        2. TKIP-RC4
        3. EAP-TLS
        4. TACACS+

        Answer:

        B. WPA was created to replace the insecure Wired Equivalent Privacy (WEP) protocol and used Temporal Key Integrity Protocol (TKIP) with the RC4 cipher for encryption. Counter Mode with Cipher Block Chaining Message Authentication Code Protocol (CCMP) with Advanced Encryption Standard (AES) is an encryption protocol that is used with the WiFi Protected Access II (WPA2) security protocol. Extensible Authentication Protocol (EAP) is a framework for the encapsulation of authentication messages. EAP is used on wireless networks and point-to-point connections and supports dozens of different authentication methods, including Transport Layer Security (TLS). It is not the encryption protocol used with WPA. Terminal Access Controller Access Control System Plus (TACACS+) is a protocol designed to provide AAA services for networks with many routers and switches.
161.    TKIP-RC4 is an encryption protocol used with which of the following wireless network security standards?

        1. WEP
        2. WPA
        3. WPA2
        4. EAP

        Answer:

        B. WiFi Protected Access (WPA) was created to replace the insecure Wired Equivalent Privacy (WEP) protocol and used the Temporal Key Integrity Protocol (TKIP) with the RC4 cipher. WPA was replaced by WPA2, which uses Counter Mode with Cipher Block Chaining Message Authentication Code Protocol (CCMP) with Advanced Encryption Standard (AES) for encryption. Extensible Authentication Protocol (EAP) is a framework for the encapsulation of authentication messages.
162.    Which of the following protocols provides wireless networks with the strongest encryption?

        1. AES
        2. TKIP
        3. EAP
        4. 802.1X

        Answer:

        A. WiFi Protected Access (WPA) is a wireless security protocol that was designed to replace the increasingly vulnerable Wired Equivalent Privacy (WEP). WPA added an encryption protocol called Temporal Key Integrity Protocol (TKIP). This too became vulnerable, and WPA2 was introduced, which replaced TKIP with the stronger CCMP-Advanced Encryption Standard (CCMP-AES). Extensible Authentication Protocol and 802.1X do not provide encryption.
163.    When the WiFi Protected Access (WPA) wireless security protocol was released to replace Wired Equivalent Privacy (WEP), it included the Temporal Key Integrity Protocol (TKIP) for encryption. Which of the following is not one of the improvements that WPA and TKIP provide over WEP?

        1. TKIP enlarges the WEP encryption key.
        2. TKIP modifies the encryption key for every packet.
        3. WPA does not require a hardware upgrade for WEP devices.
        4. TKIP eliminates the use of Pre-Shared Keys (PSKs).

        Answer:

        D. TKIP augments the existing WEP encryption key, making it longer, enabling it to be changed for every packet, and enabling WPA to be deployed without replacing network adapter or Access Point (AP) hardware. TKIP does continue to support the use of PSKs.
164.    To connect a wireless client to a Wireless Access Point (WAP) using the WiFi Protected Access II (WPA2) security protocol with a Pre-Shared Key (PSK), which of the following must you supply on both devices?

        1. Base key
        2. Passphrase
        3. Serial number
        4. MAC address

        Answer:

        B. To use the WPA2 protocol with a PSK, the client and the Access Point (AP) must both be configured with the same passphrase. The base key, the serial number, and the MAC address are all components that WPA2 uses to generate the encryption key for each packet.
165.    Upgrading a wireless network from the Wired Equivalent Privacy (WEP) security protocol to WiFi Protected Access (WPA) enables it to use the Temporal Key Integrity Protocol (TKIP) for encryption, which generates a unique key for each packet. Which of the following types of attacks does this capability prevent?

        1. Denial-of-Service (DoS) attacks
        2. Brute-force attacks
        3. Replay attacks
        4. Deauthentication attacks

        Answer:

        C. A replay attack is one in which an attacker utilizes the encryption key found in a previously captured packet to gain access to the network. Because TKIP generates a unique encryption key for every packet, it prevents this type of attack from being successful.
166.    Which of the following wireless security protocols uses CCMP-AES for encryption?

        1. WEP
        2. WPA
        3. WPA2
        4. TKIP

        Answer:

        C. WiFi Protected Access (WPA) is a wireless security protocol that was designed to replace the increasingly vulnerable Wired Equivalent Privacy (WEP). WPA added an encryption protocol called Temporal Key Integrity Protocol (TKIP). This too became vulnerable, and WPA2 was introduced, which replaced TKIP with CCMP-Advanced Encryption Standard (CCMP-AES).
167.    Which of the following was the first wireless LAN security protocol to come into common usage?

        1. WEP
        2. WPA
        3. WPA2
        4. TKIP

        Answer:

        A. Wired Equivalent Privacy (WEP) was the first wireless LAN security protocol to achieve widespread use in commercial products. This protocol was soon found to be vulnerable to attack, and it was replaced by WiFi Protected Access (WPA), which added a stronger encryption protocol called Temporal Key Integrity Protocol (TKIP). This too became vulnerable, and WPA2 was introduced, which replaced TKIP with a different type of encryption, called CCMP-Advanced Encryption Standard (CCMP-AES).
168.    Which of the following did the second version of the WiFi Protected Access (WPA) protocol add to the standard?

        1. CCMP-AES
        2. MIMO
        3. WEP
        4. TKIP

        Answer:

        A. WPA2 adds Counter Mode Cipher Block Chaining Message Authentication Code Protocol - Advanced Encryption Standard (CCMP-AES), a new symmetric key encryption algorithm that strengthens the protocol's security. Multiple-input and multiple-output (MIMO) is a multiplexing technology added to the IEEE 802.11n standard, not to WPA2. Wired Equivalent Protocol (WEP) is the predecessor to WPA; it is not part of WPA2. Temporal Key Integrity Protocol (TKIP) is the encryption algorithm used in the first version of WPA; it was not added in the second version.
169.    You are setting up a wireless LAN in a friend's home, using devices that conform to the IEEE 802.11g standard. You have installed and successfully tested the devices on an open network, and now you are ready to add security. Which of the following protocols should you choose to provide maximum security for the wireless network?

        1. WEP
        2. WPA2
        3. IPsec
        4. TLS
        5. L2TP

        Answer:

        B. WiFi Protected Access 2 (WPA2) will provide the maximum security for the wireless network, in part because it uses long encryption keys that change frequently. Wired Equivalent Privacy (WEP) has a number of vulnerabilities, including short, unchanging encryption keys, that make it less secure than WPA. IPsec is a network layer security standard that does not provide the security needed for IEEE 802.11 wireless networks. Transport Layer Security (TLS) is a protocol that encrypts data exchanged by web servers and clients at the application layer. It does not provide adequate security for wireless LANs. Layer 2 Tunneling Protocol (L2TP) is a virtual private networking protocol; it does not provide adequate security for wireless networks.
170.    CCMP-AES is an encryption protocol used with which of the following wireless network security standards?

        1. WEP
        2. WPA
        3. WPA2
        4. EAP

        Answer:

        C. Counter Mode with Cipher Block Chaining Message Authentication Code Protocol (CCMP) with Advanced Encryption Standard (AES) is an encryption protocol that is used with the WiFi Protected Access II security protocol. WPA was created to replace the insecure Wired Equivalent Privacy (WEP) protocol, and WPA2 was created to replace the Temporal Key Integrity Protocol (TKIP) used in the first version of WPA. Extensible Authentication Protocol (EAP) is a framework for the encapsulation of authentication messages.
171.    Which of the following encryption protocols was introduced in the WiFi Protected Access II (WPA2) wireless security standard?

        1. CCMP-AES
        2. TKIP-RC4
        3. EAP-TLS
        4. TACACS+

        Answer:

        A. Counter Mode with Cipher Block Chaining Message Authentication Code Protocol (CCMP) with Advanced Encryption Standard (AES) is an encryption protocol that is used with the WiFi Protected Access II (WPA2) security protocol. WPA was created to replace the insecure Wired Equivalent Privacy (WEP) protocol, and WPA2 was created to replace the Temporal Key Integrity Protocol (TKIP) used in the first version of WPA. Extensible Authentication Protocol (EAP) is a framework for the encapsulation of authentication messages. EAP is used on wireless networks and point-to-point connections and supports dozens of different authentication methods, including Transport Layer Security (TLS). It is not the encryption protocol used with WPA2. Terminal Access Controller Access Control System Plus (TACACS+) is a protocol designed to provide AAA services for networks with many routers and switches.
172.    Which of the following wireless security protocols can enable network users to authenticate using smartcards?

        1. WEP
        2. WPA2
        3. EAP
        4. AES

        Answer:

        C. Wired Equivalent Protocol (WEP) and WiFi Protected Access II (WPA2) are both wireless security protocols that control access to the network and provide encryption, using protocols like Advanced Encryption Standard (AES). These protocols do not provide authentication services, however. Extensible Authentication Protocol (EAP) is a framework for the encapsulation of authentication messages. Its many variants provide support for the use of smartcards and other authentication factors, such as biometrics, in addition to traditional passwords.
173.    Which of the following forms of the WiFi Protected Access (WPA) and WPA2 protocols require a RADIUS server? (Choose all that apply.)

        1. WPA-Personal
        2. WPA-PSK
        3. WPA-Enterprise
        4. WPA-802.1X

        Answer:

        C, D. WPA-Enterprise, also known as WPA-802.1X, can use the Extensible Authentication Protocol (EAP) to support various types of authentication factors and requires a Remote Authentication Dial-In User Service (RADIUS) server. WPA-Personal, also known as WPA-PSK (Pre-Shared Key), is intended for small networks and does not require RADIUS.
174.    Which of the following forms of the WiFi Protected Access (WPA) and WPA2 protocols call for the use of a Pre-Shared Key (PSK)?

        1. WPA-Personal
        2. WPA-Enterprise
        3. WPA-EAP
        4. WPA-802.1X

        Answer:

        A. WPA-Personal, also known as WPA-PSK, is intended for small networks and requires a PSK. WPA-Enterprise, also known as WPA-802.1X, uses the Extensible Authentication Protocol (EAP) to support various types of authentication factors and requires a Remote Authentication Dial-In User Service (RADIUS) server.
175.    Which of the following stream ciphers does the Temporal Key Integrity Protocol (TKIP) use for encryption on a wireless network?

        1. RC4
        2. AES
        3. CCMP
        4. SHA

        Answer:

        A. TKIP uses the RC4 stream cipher for its encryption. Advanced Encryption Standard (AES) is used with CCMP on version 2 of the WiFi Protected Access (WPA2) security protocol, not version 1 (WPA), which uses TKIP. Secure Hash Algorithm (SHA) is a file hashing algorithm, not used for wireless network encryption.
176.    Which of the following wireless security protocols uses CCMP for encryption?

        1. WEP
        2. WPA
        3. WPA2
        4. 802.1X

        Answer:

        C. CCMP (Counter Mode Cipher Block Chaining Message Authentication Code Protocol), is based on the Advanced Encryption Standard (AES) and is the encryption protocol used with the WiFi Protected Access II (WPA2) security protocol on wireless networks. CCMP is not used with version 1 of the WPA protocol or with Wired Equivalent Privacy. 802.1X is an authentication protocol, not used for encryption.
177.    CCMP is based on which of the following encryption standards?

        1. TKIP
        2. RC4
        3. AES
        4. 802.1X

        Answer:

        C. CCMP (Counter Mode Cipher Block Chaining Message Authentication Code Protocol) is based on the Advanced Encryption Standard (AES) and is the encryption protocol used with the WiFi Protected Access II (WPA2) security protocol on wireless networks. CCMP is not based on the Temporal Key Integrity Protocol (TKIP), which uses RC4 as its stream cipher. 802.1X is an authentication protocol, not used for encryption.
178.    You have installed a new Wireless Access Point (WAP) on your network and configured it to use an SSID that is not broadcasted and WPA2 for security. Which of the following describes what you must do to configure your wireless clients?

        1. Select the SSID from a list and allow the client to automatically detect the security protocol.
        2. Select the SSID from a list and then select WPA2 from the security protocol options provided.
        3. Type the SSID manually and allow the client to automatically detect the security protocol.
        4. Type the SSID manually and then select WPA2 from the security protocol options provided.

        Answer:

        D. An SSID that is not broadcast is not detectable by clients, so you must type it in manually. Security protocols are also not detectable, so you must configure the clients to use the same protocol you selected on the client.
179.    Which of the following wireless LAN security protocols was rendered obsolete after it was found to be extremely easy to penetrate?

        1. WEP
        2. WPA
        3. WPA2
        4. EAP

        Answer:

        A. Wired Equivalent Privacy (WEP) was one of the first commercially available security protocols for wireless LANs, but it was soon found to be easily penetrated and was replaced by WiFi Protected Access (WPA) and then WPA2. Extensible Authentication Protocol (EAP) is a framework for the encapsulation of authentication messages.
180.    Which of the following protocols does the WiFi Protected Access (WPA) security protocol use for encryption?

        1. AES
        2. TKIP
        3. MD5
        4. SHA

        Answer:

        B. WPA uses the Temporal Key Integrity Protocol (TKIP) for encryption. It does not use Advanced Encryption Standard (AES), which eventually replaced TKIP in WPA2. Secure Hash Algorithm (SHA) and Message Digest 5 (MD5) are both file hashing algorithms, not used for wireless network encryption.
181.    Which of the following wireless network security protocols provides open and shared key authentication options?

        1. WPA
        2. WEP
        3. WPA2
        4. EAP

        Answer:

        B. Wired Equivalent Privacy (WEP), which was one of the first commercially successful security protocols for wireless LANs, enabled administrators to choose between open and shared key authentication. The open option enabled clients to connect to the network with an incorrect key. The shared option required the correct key, but it also exposed the key to potential intruders. The correct option is to not use WEP at all, as it was easily penetrated and subsequently replaced by WiFi Protected Access (WPA) and then WPA2. Extensible Authentication Protocol (EAP) is a framework for the encapsulation of authentication messages. None of the other three provides a choice between open and shared key options.
182.    Which of the following wireless security protocols uses TKIP for encryption?

        1. WEP
        2. WPA
        3. WPA2
        4. AES

        Answer:

        B. WiFi Protected Access (WPA) is a wireless security protocol that was designed to replace the increasingly vulnerable Wired Equivalent Privacy (WEP). WPA added an encryption protocol called Temporal Key Integrity Protocol (TKIP). This too became vulnerable, and WPA2 was introduced, which replaced TKIP with an Advanced Encryption Standard protocol (CCMP-AES).
183.    Which of the following is not a factor that weakens the security of the Wired Equivalent Privacy (WEP) protocol used on early IEEE 802.11 wireless LANs?

        1. 40-bit encryption keys
        2. 24-bit initialization vectors
        3. Static shared secrets
        4. Open System Authentication

        Answer:

        D. Open System Authentication enables any user to connect to the wireless network without a password, which actually increases the security of the protocol. This is because most WEP implementations use the same secret key for both authentication and encryption. An intruder that captures the key during the authentication process might therefore penetrate the data encryption system as well. By not using the key for authentication, you reduce the chances of the encryption being compromised. The use of short, 40-bit encryption keys was mandated at the time by U.S. export restrictions. Later protocols used keys at least 128 bits long. The initialization vector (IV) is a randomized value appended to the shared secret to ensure that the cipher never encrypts two packets with the same key. The relatively short IV that WEP uses results in a reasonable probability of key duplication, if an attacker captured a sufficient number of packets. Shared secrets that do not change provide attackers with more time to crack them. The lack of a mechanism to automatically change WEP shared secrets weakened the protocol considerably.
184.    Which of the following encryption ciphers was replaced by CCMP-AES when the WPA2 wireless security protocol was introduced?

        1. EAP
        2. WEP
        3. TKIP
        4. CCMP

        Answer:

        C. WPA2 was introduced when the earlier version of WiFi Protected Access (WPA) was determined to be increasingly vulnerable to attack. WPA used an encryption protocol called Temporal Key Integrity Protocol (TKIP). WPA2 replaced TKIP with an Advanced Encryption Standard (CCMP-AES) protocol.
185.    Which of the following wireless security protocols was substantially weakened by its initialization vector?

        1. WPA
        2. WEP
        3. WPA2
        4. PEAP

        Answer:

        B. Wired Equivalent Privacy (WEP) was one of the first commercially available security protocols for wireless LANs. WEP requires 24 bits of the encryption key for the initialization vector, substantially weakening the encryption. WEP was soon found to be easily penetrated and was replaced by WiFi Protected Access (WPA) and then WPA2. Extensible Authentication Protocol (EAP) is a framework for the encapsulation of authentication messages.
186.    Ralph is installing a wireless LAN that includes three Access Points (APs) to provide coverage for a large building. Which of the following must Ralph do to ensure that users are able to roam without interruption from one AP to another using their portable devices? (Choose all that apply.)

        1. Configure each AP with the same IP address.
        2. Configure each AP with the same security passphrase.
        3. Configure each AP to use the same security protocol.
        4. Configure each AP with the same SSID.

        Answer:

        B, C, D. Roaming from one AP to another without interruption requires that the APs all use the same SSID, the same security protocol, and the same passphrase. The APs will not function properly if they have the same IP address.
187.    Which of the following is the maximum theoretical download speed for a 5G cellular network?

        1. 42 megabits per second
        2. 150 megabits per second
        3. 1 gigabit per second
        4. 10 gigabits per second
        5. 100 gigabits per second

        Answer:

        D. The 5G cellular network specification calls for maximum theoretical download speeds of 10 gigabits per second, although the actual speed realized will be less.
188.    Which of the following statements about 5G cellular networks are true? (Choose all that apply.)

        1. 5G networks can operate on three frequency bands.
        2. 5G networks with the highest speeds also have a more limited range.
        3. 4G devices can connect to 5G networks at reduced speeds.
        4. On a 5G network, the lower frequency bands provide the highest speeds.

        Answer:

        A, B. 5G networks can operate on three frequency bands—low, medium, and high—with the high frequencies having the fastest speeds and reduced range. 4G devices cannot function on 5G networks.
189.    Which of the following IEEE standards describes an implementation of port-based access control for wireless networks?

        1. 802.11ac
        2. 802.11n
        3. 802.1X
        4. 802.3x

        Answer:

        C. IEEE 802.1X is a standard that defines a port-based Network Access Control (PNAC) mechanism used for authentication on wireless and other networks. IEEE 802.11ac and 802.11n are standards defining the physical and data link layer protocols for wireless networks. IEEE 802.3x is one of the standards for wired Ethernet networks.
190.    Unauthorized users are connecting to your Wireless Access Point (WAP) and gaining access to the network. Which of the following are steps you can take to prevent this from happening? (Choose all that apply.)

        1. Disable SSID broadcasting.
        2. Use Kerberos for authentication.
        3. Place the Access Point (AP) in a DMZ.
        4. Implement MAC address filtering.

        Answer:

        A, D. Disabling SSID broadcasting prevents a wireless network from appearing to clients. The clients must specify the SSID to which they want to connect. MAC address filtering is a form of Access Control List (ACL) that is maintained in the AP and contains the addresses of devices that are to be permitted to access the network. Both of these mechanisms make it more difficult for unauthorized devices to connect to the Access Point (AP). Kerberos is an authentication protocol used by Active Directory, and relocating the AP to a DMZ will not resolve the problem.
191.    On a Wireless Access Point (WAP) that uses an Access Control List (ACL) to specify which devices are permitted to connect to the network, which of the following is used to identify the authorized devices?

        1. Usernames
        2. IP addresses
        3. Device names
        4. MAC addresses

        Answer:

        D. WAPs use the layer 2 MAC addresses coded into devices in their ACLs. Usernames, IP addresses, and device names can easily be impersonated.
192.    On a network carrying both voice and data traffic, separate Virtual Local Area Networks (VLANs) enable the voice traffic to be assigned a higher priority than the data traffic. Which of the following are methods for identifying the packets carrying voice traffic, so the switches can assign them to the voice VLAN? (Choose all that apply.)

        1. MAC addresses
        2. VLAN tags
        3. IP addresses
        4. DNS names

        Answer:

        A, B. There are two methods for identifying packets carrying voice traffic: by recognizing the MAC address of the sending system as a voice device, and by recognizing packets that have already been tagged as voice VLAN traffic. It is not possible to identify voice traffic using IP addresses or DNS names.
