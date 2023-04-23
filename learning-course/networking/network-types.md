# Network Types

### Mesh Topology

* Unique design
* Each computer connects to all other computers
* Point-to-point (P2P) connection

#### Mesh Topolohy Types

* Partial mesh topology
* Full mesh topology

#### Advantages

* Expand network without user disruption
* Nodes have dedicated links
* Fault identification isolation
* Reduced chance of network failure
* Multiple routes available for communication

#### Disadvantages

* Complex installation
* More space required for dedicated links
* Multiple network interfaces to maintain
* Expensive implementation
* Utilization is low

### Star Topology

* All computers connect using a central node (concentrator)
* Popular on local area networks (LANs)
* Easy and inexpensive installation

#### Advantages

* Only failed nodes are affected
* Easy to modify, configure and troubleshoot
* Fast performance and low network traffic
* Adding, deleting and moving devices is easy

#### Disadvantages

* Concentrator failure brings down the entire network
* Central node can be more expensive
* Heavy network traffic can result
* Concentrator capacity controls performance
* Network can be brought down by damaged devices

### Bus Topology

* A single cable connects all nodes
* Usin T cable
* Linear bus topologz has two endpoints
* Each endpoint has to be terminated

#### Advantages

* Lower cost that other topologies
* Easy and inexpensive installation maket it well suited for LAN networks
* Often used for small, uncomplicated or temporary network installs
* Easy to extend&#x20;

#### Disadvantages

* System may crash from cable fails
* Heavy traffic impacts network performance time
* Heavy traffic causes collisions
* Limited length cables
* Very old technology

### Ring Topology

* Each device communicates with two neighbor devices
* Every computer connects to another computer
* Information is passed from one computer to another
* All messages travel in one direction

#### Advantages

* Easy installation and reconfiguration
* Device addition/ deletion requires moving only two connections
* Equal access to all network computer
* No collisions

#### Disadvantages

* Unidirectional traffic - it never got beyond 10 Mbps
* Entire network can be taken down by a break
* Less popular topology
* Topology signals are always circulating
* Difficult to troubleshoot
* Computer addition or removal can disturb the network
* 20 years old&#x20;

### Hybrid Topology

* Combination of two or more network topologies

#### Advantages

* Ease of error detection and troubleshooting
* Flexible and highly effective
* Scalable

#### Disadvantages

* Complex design
* Costly process

### LAN, MAN and WAN Network Types

* LAN Local Area Network
* MAN Metropolitan Area Network
* WAN Wide Area Network

#### LAN

* Connects devices to allow sharing of data and resources
* Uses private addressing scheme
* Connected by switches
* Very fast data transmission
* Easy design and maintenance

#### MAN

* Covers area larger than LAN, smaller than WAN
* Covers a regional geographic area
* Common organizations
* Designed for high-speed connectivity
* Harder to design and maintain
* Less fault tolerant
* More network congestion
* Costly
* Moderate data transfer rate
* Moderate propagation delay
* Large geographic area
* Supports high speed
* Relatively expensive
* Two types switched WAN and point-to-point WAN
* Challenging to design and maintain
* Slow data rate (1/10 of LAN)
* Propagation delay is a challenge
* Data transmitted by optic wires, microwaves and satellites

#### LAN vs MAN vs WAN

* LANs connect devices within an office or a building
* MANs connect network within a city or between cities
* WANs connect networks within a country or globalyy

### WLAN, PAN and CAN Network Types

WLAN - Wireless Local Area Network

PAN - Personal Area Network

CAN - Campus Area Network

#### WLAN

* Wireless connectivity for devices
* Uses high frequency wadio waves
  * 2,4 GHz
  * 5 GHz
* Generally includes Internet access point
* Allows user movement while staying connected to network

**Access Points**

* Station
  * Access points
    * Provide access to the wireless network
    * Function as routers (in airport router itself doesn't need to be a Wi-Fi device, in home  we have Wi-Fi router and it performs both functions - connectivity of all of the devices which really is the switching component, but it also performs the routing to allow us to get to the internet)
  * Clients
    * Can include a variety of devices

#### Personal Area Network (PAN)

* Network specific to an individual in a small office or at home
* Generally includes various devices
* Typically managed from one computer
* Can be accessed by any device
* Modem connected to Internet provides wireless connections

**Functionality:**

* Send documents for printing from another room
* Upload photos from phone to computer
* Stream online entertainment to your TV

#### Campus Area Network (CAN)

* Connects multiple buildings in a larger property
* Common on educational or corporate campuses
* Generally connects to public Internet
* Smaller than MANs and WANs

**Benefits:**

* Usually managed by internal IT team, which results in a high degree of network control
* Easier to apply network security policies than with disconnected networks
* IT team can manage access block insecure devices and enable other safeguards
* Higher speed
* Lower cost

### Peer-to-Peer vs. Client/Server Networks

* All nodes are consider to be equal
* Usually consist of all client systems
* No dedicated servers
* Any system can act as a server or a client

#### Client/Server

* Devices have specific functions
* Client systems make requests to servers
* Servers perform the tasks for the clients
  * Deliver email or a website
  * Centralized storage of files or databases
  * Print

#### Workgroups

* A Microsoft implementation of a peer-to-peer network
* All members are configured with the same Workgroup name
* Simplifies sharing of resources within the workgroup
* No centralized management

#### Domains

* A microsoft implementation of a client/server network
* Dedicated servers manage a single directory of all users and computers
* Client systems join the domain
* Centralized administration and management

### Storage Area Networks (SAN)

* Dedicated, high-speed network
* Allows network access to storage at the block level
* Composed of devices connected with assorted technologies protocols and topologies
* Can span multiple sites
* Storage appears local to host

#### Benefits

* Improved availability for applications
* Enhanced performance
* Increased storage usage and effectiveness
* Important in Business Continuity Managemenet (BCM)
* Addresses enterprise storage needs
* Allows better management of storage
* Enhances disaster recovery
* Can scale to hold thousands of disks

### Multiprotocol Label Switching (MPLS)

* Used to ensure reliable connections for applications in real-time
* Technique, not service
* Expensive
* IP routing can be compared to tracking a package as it passes through multiple destinations on the way to you
* MPLS establishes highly efficient, predetermined routes
* As a packet first enters the network, it gets assigned to a forwarding equivalence class (FEC)
* All network routers have a table that specifies how specific FEC-type packets should be handled
* Allows MPLS to consistently handle the same types of packets
* Packets, like those with voice or video, can be mapped to suitable network routes with low latency
* Labels attach information to packets that is useful to routers

#### Features

* Not bound to an underlying technology
* Designed to improve performance
* Commonly used between branch offices or enterprises requiring real-time applications

#### MPLS Label Components

* Label
* Experimental
* Bottom-of-stack
* Time-to-live

#### Pros

* Scalable and provides good end-user experience
* Reduced network congestion
* Improved bandwidth utilization
* Secure mode of transport
* Not vulnerable to DoS attacks

#### Cons

* Doesn't provide encryption
* More expensive than using public Internet for sending traffic
* Challenging to find a provider who can deliver coverage globally
* Wasn't designed for cloud use

### Multipoint Generic Routing Encapsulation (mGRE)

* A classic GRE tunnel is point-to-point
  * Not easily scalable
* mGRE lets a tunnel have multiple destinations (point-to-multipoint)

### Common Network Provider Links

* Digital Subscriber Line (DSL)
* Cable
* Fiber-optic
* Dial-up

#### DSL

* Among the first widely used broadband services
* Uses existing cooper phone lines
* Download speeds 1 to 500 Mbps
* Upload speeds 384 Kbps to 8 Mbps
* Usually combined with phone service
* Two-wire technology permits broadband internet access without disrupting phone services
* DSL modem connects to devices using local or wireless connections
* Providers often use a combination of DSL, fiber-optic and others

#### Types

* Asymmetric DSL - upload speeds and download speeds were not the same, typically in most home environments all wants more for downloading
* Symmetric DSL - same speed in terms of uploads and downloads

#### Pros

* Speeds suitable for light/moderate file sharing, browsing and backup to the cloud
* Audio and video conferencing capacity
* Fast download speeds

#### Cons

* Not fast enough for heavy cloud backups and file sharing
* Frequent HD streaming and VoIP causes issues
* Can't match upload speeds of fiber or cable&#x20;

#### Cable

* Traditionally uses coaxial cables
* 20-1000 Mbps download speeds&#x20;
* 7-50 Mbps upload speeds
* Usually combined with TV service

#### Cable Pros

* Speeds suitable for moderate browsing, backing up online and sharing files
* VoIP services and HD streaming capacity
* Moderate speeds for uploads
* Fast speeds for download

#### Cable Cons

* Can't reach the same speeds as fiber
* Peak times may result in slower speeds and lag

#### Fiber

* Fast and reliable
* 25 Mbps to 1 Gbps download speeds
* 5 - 880 Mbps upload speeds
* Can be combined with TV and phone service
* Modem or gateway router used to connect office/devices
* Fibers use light beams to transmit data
* Faster and more reliable than DSL and cable
* Upload and download speeds can match

#### Fiber Pros

* Speeds suitable for heavy browsing, backing up online and sharing files
* VoIP services and HD streaming capacity for frequent use
* Superior speeds for uploads and downloads
* Capacity for server hosting and complex cloud services

#### Fiber Cons

* Same areas may have limited availability
* Higher short-term costs
* Reliability and speed can depend on ISP infrastructure

### Other Network Provider Links

#### Satellite

* Provides Internet access in rural and remote areas where landline Internet isn't available&#x20;
* 1-100 Mbps download speeds&#x20;
* 1-4 Mbps upload speeds
* Leased monthly

#### Characteristics&#x20;

* Requires receiver dish
* Data provided by ISPs operating earth-orbiting stations
* Nos as fast as DSL, cable or fiber

#### Satellite Pros

* Available to businesses without access to landline Internet
* Suitable speed for audio/video streaming
* Global access

#### Satellite Cons

* High latency
* Can be impacted by clouds, weather or even tall trees
* Slow upload and download speeds
* Monthly plans are costly

#### Metro-optical

* Metropolitan optical networks
  * Can span distances up to several hundred kilometers
  * Designed to serve large and densely concentrated metropolitan areas
  * Connections are made using Ethernet
  * Network support:
    * Pure Ethernet
    * Ethernet over MPLS
    * Ethernet over DWDM
    * Ethernet over SDH

#### Internet Comparison

| Internet type | Cost     | Speed     | Reliability | Availability |
| ------------- | -------- | --------- | ----------- | ------------ |
| DSL           | Low      | Moderate  | Moderate    | High         |
| Fiber         | Moderate | Very high | High        | Moderate     |
| Cable         | Low      | High      | High        | High         |
| Satellite     | High     | Low       | Low         | Very high    |

### Service-related Entry Points

#### Demarcation point

* Location where connection is made to outside world (WAN provider, ISP)
* Centrally located in a building
* Division between the ISP and your network
* Your equipment is the customer premises equipment (CPE) and the connection is your responsibility from the demarcation point inward

#### Smartjack

* Intelligent device that provides demarcation point
* Contains circuit card in chassis
* Built-in diagnostics options
* Alarm indication capabilities

### vSwitch, vNIC, NFV, and Hypervisor&#x20;

#### Hypervisor

* Separates OS from applications and hardware
* Allows host to run multiple VMs as guests to maximize resource use

#### Benefits

* VMs are separated from each other
* Easily moved or migrated

#### Types

* Type 1 - native or bare metal
* Type 2 - hosted

#### Virtual Switch (vSwitch)

* Application that permits communication between VMs
* Directs communication by checking packets before sending them to a destination
* Embedded in software or is part of server hardware firmware
* Can connect to NIC and is entirely virtual

#### Advantages

* Eases virtual server migration and deployment
* Admins can manage hypervisor-deployed virtual switches
* Easier to roll out new functionality than a physical switch

#### Virtual Network Interface Card (vNIC)

* Used to connect virtual machines, with other nodes
* Responsible for managing network communication
* Every VM can have one or more virtual NICs installed to provide connectivity
* Extra IP addresses can be assigned to a NIC to provide multiple subnet access

#### Network Function Virtualization (NFV)

* Decouples network functions from hardware and runs them on a software platform instead
* Complements using software defines networking for managing networks
* Focuses on network service optimization

#### NFV

* Created to meet service provider need for speeding up new network service deployment

### Test
