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



### OSI Layer 7 - Application























