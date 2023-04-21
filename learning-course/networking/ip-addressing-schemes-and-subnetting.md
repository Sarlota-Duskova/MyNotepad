# IP Addressing Schemes and Subnetting

### Public vs. Private IP Addresses

#### RFC1918 (1996) Request For Comment

* Category 1 LAN only
* Category 2 LAN + limited outside resources
* Category 3 Internet access

#### TCP/IP version 4 - IPv4  Addresses

Private addresses - use only in LAN environment

* reserved IP addresses
* 10.0.0.0 - 10.255.255.255, 8 network bits used in the 32-bit default subnet mask (255.0.0.0)
* 172.16.0.0 - 172.31.255.255, 16 network bits used in the 32-bit default subnet mask (255.255.0.0)
* 192.168.0.0 - 192.168.255.255, 24 network bits used used in the 32-bit default subnet mask (255.255.255.0)

Public addresses - accessible on the public Internet

* Internet - unique addresses

### NAT vs. PAT

#### NAT (Network Address Translation)

* Map public IP to private IP
* One-to-one or many-to-one

**NAT Types:**

* Static
* Dynamic
* PAT

#### PAT (Port Address Translation)

* Type of NAT, uses ports
* Map private IP to a public IP
* Many-to-one

| NAT                                                   | PAT                                                           |
| ----------------------------------------------------- | ------------------------------------------------------------- |
| Internal local addresses -> internal global addresses | Private unregistered addresses -> public registered addresses |
| No port number requirement                            | Uses port numbers                                             |
| Single host                                           | Multiple hosts (same IP, different port numbers)              |
| Uses IP during translation                            | Uses IP + port numbers                                        |

### IPv4 and IPv6 Addressing

**IPv4**

x.x.x.x (x = 0-255 it's decimal values)&#x20;

**Benefits of IPv4**

* Ubiquitous
* Easy visualization
* Flexible
* Simple configuration

#### IPv6

* 128-bit addresses
* x:x:x:x:x:x:x:x (x = 16-bit hex)

**Benefits of IPv6:**

* No NAT
* Improved multicasting
* Automatic configuration
* Better routing
* Simplified headers
* Flow labeling - component of quality of service, describing the overall performance of a service
* Authentication and privacy
* Improved administration  - no requires DHCP (Dynamic Host Configuration Protocol) to assign addresses to devices
* No private address collisions

### Automatic Private IP Addressing (APIPA)

* DHCP not present (Dynamic Host Configuration Protocol) is often a server but it could also be a router&#x20;
  * Basic idea is that a pool of addresses will be configured on the server or the router
* Automatic self-IP assignment - APIPA will automatically self-assign an IP address configuration
*

#### How APIPA Works

* No DHCP server found
* IP address assigned using ARP (Address Resolution Protocol)
* Class B 169.254.0.0 to 169.254.255.255 - reserved address
* User notified by DHCP messages

#### Extended Unique Identifier (EUI-64)

* Host can self-assign themselves using 64-bit IPv6 address
* Taken from 48-bit MAC address
* No need for manual configuration/DHCP

MAC address (48-bit)

Organizationally Unique Identifier (OUI) | Network Interface Card (NIC)

\| 00 | B5 | E6 |                                            | D0 | FA | 04 |

Extended Unique Identifier (64-bit)

\| 00 | B5 | E6 | FF | FE | D0 | FA | 04 |

### Unicast, Broadcast, Anycast and Multicast Packets

#### Unicast

* Information between points
* One sender, one receiver
* Primary LAN/internet method
* All LANs support unicast
* Use TCP&#x20;

#### Broadcast

* One endpoint sending to multiple points
* Information sent to all destinations
* Used by most LANs
* All computers will receive the transmission
* Not every system is required to process the transmission

#### Multicast

* One or more points sending to one or more points
* One sender with many receivers
* Can distributed the same information to multiple clients
* Can define a single address that can then be used by multiple clients
* Same packet from the sender is received by those multiple clients
* Multiple clients are using that same receiving address
* Class D IPv4 addresses - use class D when you want to define multicast groups, it will use UDP Protocol

### Link Local Loopback and Default Gateway Addresses

#### Default Gateway

* Allows communication between networks
* Routes traffic
* Relays information between the source and destination networks

#### Default Gateway Options

* Router (it has two interfaces - one for private network and second for public network)
* ISP (Internet Service Provider) - point to point connection, out of date
* Server

#### Loopback Address

* Loops back to local computer
* Home address
* IPv4 = 127.0.0.1
* IPv6 = 0:0:0:0:0:0:0:1 or ::1
* For diagnostic purpose

#### Link-local Address

* Connectivity on local network only
* Not routed
* APIPA addresses
  * IPv4 = 169.254.x.x/16
  * IPv6 = fe80::/64

### Base-2 Conversions and Binary Values

#### IPv4 Classes

| Class   | Address range                | Number of hosts                        |
| ------- | ---------------------------- | -------------------------------------- |
| Class A | 1.0.0.1 to 126.255.255.254   | up to 16 million hosts on 127 networks |
| Class B | 128.1.0.1 to 191.255.255.254 | up to 65,000 hosts on 16,000 networks  |
| Class C | 192.0.1.1 to 223.255.254.254 | up to 254 hosts on 2 million networks  |
| Class D | 224.0.0.0 to 239.255.255.255 | reserved for multicast                 |
| Class E | 240.0.0.0 to 254.255.255.254 | reserved for research                  |

#### Subnetting - IPv4 and Binary

Decimal:

255.255.255.255

Binary

11111111.11111111.11111111.11111111.

\|    1   |  1  |  1  |  1  |  1  | 1 | 1 | 1 |

\| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

128 + 64 + 32 + 16 + 8 + 4 + 2 + 1 = 255

#### Subnet Masks - CIDR (Classless Inter-Domain Routing) Notation

| Bits used for mask | Default mask  | Subnet binary                       | Class |
| ------------------ | ------------- | ----------------------------------- | ----- |
| /8                 | 255.0.0.0     | 11111111.00000000.00000000.00000000 | A     |
| /16                | 255.255.0.0   | 11111111.11111111.00000000.00000000 | B     |
| /24                | 255.255.255.0 | 11111111.11111111.11111111.00000000 | C     |

### Subnetting Fundamentals

2^8 = 256 every time - 2 because reserved 00000000 and 11111111

192.168.0.0 is not used for regular host systems, it is used by the router to indicate that there is no host system, router should ignore the host portion and simply focus on the network portion

* Routers do not connect host systems directly to each other
* They connect network to each other

192.168.0.255 this means every host - this is the broadcast address

* anytime a system needs to send a broadcast packet
* every host on that network will hear it

### Supernetting Strategies

* Changing it by moving a line from right to left, so we are moving from 1 to 0 so from 11111111 to 111111110&#x20;

### IPv6 Addressing Solutions

* Devices use both IPv4 and IPv6 addresses

ae44:0000:dfe6:0000:3bf2:0000:ffe0:0001

can be shortened to:

ae44:0:dfe6:0:3bf2:0:ffe0:1

or

ae44::dfe6:0:3bf2:0:ffe0:1

* Short 0000 to :: only one time within the address

#### Stateless Address Autoconfiguration (SLAAC)

* Stateful and stateless - let the client systems assemble their own addresses or have it managed by DHCP (Dynamic Host Configuration Protocol)
* Autoconfiguration - part of the client, it can determine its own address
* Host can generate its own address
* Local and remote information used
* Prefixes advertised by router
* Address generated from prefix and interface identifier
* Host creates interface identifier
* If no router, link-local address generated

### Layer 3 Subinterfaces

* Virtual interface
* Convert physical info logical

#### How Subinterfaces work

* Connect router to multiple networks
* Route traffic between networks
* Multiple subinterfaces
* Each subinterface has unique IP

#### Using subinterfaces

* VLAN traffic routing
* Configured as if a physical interface

### Virtual IP Addressing

* Single node represents multiple devices
* Virtual IP represents all systems
* Requests are redirected to a real address

#### Using Virtual IP

* DNS points to pool of virtual addresses
* Content gateway distributes addresses based on location
* Failures detected and rectified

### Test

Which address is used as the loopback address in all IPv4 configurations?

* 127.0.0.1

What is the correct range of possible addresses that can be created for the first subnet based on the expression of 192.168.0.1/26?

* 192.168.0.0 – 192.168.0.63

Which statement best characterizes the function of network address translation?

* It maps a private IP address to a public IP address, when you need to communicate with another system on the Internet

Which subnet mask in a class A network will reduce any single subnet to the size of a class C network?

* 255.255.255.0

Which subnet mask will subdivide a class C network into 8 subnets?

* 255.255.255.224
* 128+64+32 = 224

Which subnet mask is required to create a single network from four class C networks?

* 255.255.252.0

Which statement best characterizes the purpose and functionality of a virtual IP address?

* It presents a single IP address to client systems, but it represents multiple IP addresses

If a network configuration is expressed by the value 192.168.0.1/24, which characteristics can be ascertained about the state of this network?

* The network has not been subnetted
* The network is a class C network

What are the benefits of using the IPv6 addressing scheme?

* It provides capability for automatic configuration of IPs
* It provides better routing since the size of routing tables are reduced

By which manner can a subinterface be created?

* By assigning more than one IP address to a single physical network adapter

Which type of transmission would be used for a client system requesting email from its messaging server?

* Unicast

A subnet mask of 255.255.248.0 accommodates approximately how many hosts per subnet?

* 2000
* 255 - 1 - 2 - 4 = 248, 24 - 3 = 21, 32 - 21 = 11, 2^11 - 2 = 2046

An IPv4 address that has been assigned through the APIPA process usually indicates what condition on a network?

* A DHCP server could not be found

What is meant by the fact that the IP protocol is characterized as dual stack?

* It refers to the fact that either version 4 or version 6 can be used to communicate

Which binary value represents the decimal value of 150?

* 10010110
