# OSI Model

### OSI Layer 1 - Physical



### OSI Layer 2 - Data Link

#### Responsibilities

* Physical addressing
* Framing
* Access control
* Flow control
* Error control

#### Logical Link Control (LLC)

* Media access methods
* Connectionless
* Network layer protocols
* Connection-oriented

#### Medium Access Control (MAC)

* MAC address:
  * 12-character hexadecimal value
  * Unique to every network interface

### OSI Layer 3 - Network

#### Functions

* Packet addressing
* Address conversion
* Source-to-destination delivery
* Routing

#### Routing

* Pass data from router to router among the connected networks
* Determine the best path from source to destination
* Independent networks connected to each other

#### Internetworking

* Provides logical connections between different types of networks
* Combine various networks to form a larger network

#### Logical Addressing

* Define addressing scheme
* Combine any number of network

#### Packetizing

* Creates packets upon receiving data from upper layers
* Packets are created by way of encapsulation
* Internet Protocol (IP) applies addresses to each packet

#### Fragmentation

* Dividing larger packets into smaller fragments
  * Fragments can then be easily sent out on physical medium

### OSI Layer 4 - Transport

#### Data Delivery

* User Datagram Protocol (UDP)
* Transmission Control Protocol (TCP)

#### Connectionless Transmission

* Receiver does not acknowledge receipt of packet
* Sending device assumes packet arrived successfully
* Enables faster communication between devices

#### Connection-oriented Transmission

* Establish a connection between the two endpoints before any data is transmitted
* Using TCP

### OSI Layer 5 - Session

* Session protocol
  * Defines parameters for connections
* Manages the transfer of data
  * Who can transfer
  * How long

#### Dialog Control

* Determines which device communicates first and how data will be sent
* Types of dialog control:
  * Simplex - communication occurs in one direction only (one device transmits, while another device receives)
  * Half duplex - traffic can occur in both directions, but only in one direction at a time (one device transmits whole the other receives, then the roles can be reversed so that communication can occur in the opposite direction)&#x20;
  * Full duplex - traffic can be two-way at the same time

#### Protocols

* NetBIOS (Network Basic Input Output System)&#x20;
* DNS (Domain Name Systems)

Both are methods of communication involving name recognition and resolution

* RPC (Remote Procedure Call) is a client-server redirection method whereby requests are generated on clients, but executed on servers
* NFS (Network File System) which allows client systems to access server-based resources, such as folders and files
* Sessions - is responsible for negotiating and maintaining the overall flow of communication during the session

### OSI Layer 6 - Presentation

#### Character code translation

* ASCII
* EBCDIC

#### Data conversion

* Bit order
* CR-LF
* Integer-floating point

### OSI Layer 7 - Application

#### Network Services

* FTP
* DHCP
* DNS
* SMTP
* HTTP

### IP Headers

* IPv4 header = 20 bytes

TCP header size:

* Minimum size of 20 bytes
* Maximum size of 60 bytes
* Defines the port value

UDP header

* Source port of 2 bytes
* Destination port of 2 bytes
* Length od 2 bytes
* Checksum of 2 bytes
* Data (payload) 0-65,507 bytes

### TCP Flags

SYN (Synchronization) - first step of establishing the connection

ACK (Acknowledgement) - acknowledge receipt of that packet

FIN (Finish) - last packet sent by sender&#x20;

RST (Reset) - terminates the connection, when something just isn't correct

PSH (Push) - when buffering needs to be managed or controlled, transport layer might wait for the higher level layers to provide it with more data so that the packet is as full as possible before it's sent

URG (Urgent)

* Data is forwarded immediately
* Notifies receiver to prioritize over other packets
* Receiver is notified once all urgent packets are received

### Fixed and variable payloads

Payloads - data being transmitted

#### Fixed Payload

* Frames become fixed size (size is set)

#### Variable Payload

* A pattern is used to determine frame size

### MTU vs. MSS

#### Maximum Transmission Unit (MTU)

* The largest frame or packet that can be transmitted over a particular type of network
* MTU is specified at Layer 3
* More data can be transmitted
* Enables the use of jumbo frames (can typically be as large as 9000 bytes whereas the standard is usually around 1500)
* Certain routers cannot handle larger packets

**Adjusting MTU Size:**

* For Windows - Netsh command
* For Linux - ifconfig command
* For Mac - change manually using system preferences

#### Maximum Segment Size (MSS)

* Largest amount of data a device can handle
* Data segment and header total size should be less than MTU size

### Test

Which type of traffic management service occurs at the network layer of the OSI Model?

* Routing

Which protocols operate at the application layer of the OSI Model?

* HTTP
* SMTP

Which device or service would not operate at the physical layer of the OSI Model?

* IP Address

If you needed to be certain that your data transmissions are being received, which type of connection and protocol should be used?

* Connection-oriented and TCP

Which command can be used to determine the MTU optimal size?

* Ping

The TCP header specifies which value to ensure that data is processed by the correct application?

* Port

Which TCP flag is used to gracefully terminate a session between two systems?

* FIN

Which type of communication would be analogous to a half duplex transmission?

* Two people using walkie-talkies

A fixed payload typically has which benefits or characteristics?

* They are always the same size
* They can be more efficient than variable payloads

Which common services occur at the presentation layer of the OSI Model?

* Compression
* Encryption

The physical address applied by the data link layer of the OSI Model has which features?

* It is expressed using a 12-character hexadecimal value
* It is a static address that can’t be changed
* It is unique to every network interface

Which statement correctly characterizes the functions of the OSI Model?

* It is a method of describing the functions of a networking system to allow communication
