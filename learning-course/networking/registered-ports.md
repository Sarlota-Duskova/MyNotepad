# Registered Ports

### Structured Query Language (SQL) Server

* using port 1443

#### Relational Database Management System (RDBMS)

* Basic for all modern database systems
* Usestables to store database objects
* Tables use fields to maintain specific information
* Individual entries are known as records

#### SQL Actions

* Execute queries -to retrieve records
* Insert recocrds
* Update records
* Delete records
* Set permissions

#### Database engine

* Relational engine - maintains the connectivity or the relationships between tables (example: customer and order)
* Storage engine

#### SQL Server Operating System (SQLOS)

* Provides operating system services&#x20;

#### SQL Server Services and Tools

* Data managemenet
* Business intelligence (BI)
* Use port 1433

### SQLnet Configurations

* Runs over TCP port 1521
* Oracle's networking software

#### Benefits

* Scalability
* Protocol support
* Media and topology support
* Network transparency
* Heterogeneous networking

#### Configurations

* Client configuration
* Server configuration

Configuration Files:

* sqlnet.ora - basic configuration details like tracing and/or encryption
* tnsnames.ora - configuration file that defines the database addresses for establishing the connections
* ldap.ora - configuration file that sets lightweight directory access protocol properties
* listener.ora - configure the database listeners (accept the incoming requests)
* cman.ora - connection manager settings which is the text file containing the overall settings for the SQLnet connection

### MySQL Database Service

* Database management system
  * Open source SQL database management system
  * Supported by Oracle corporation
* TCP port 3306
* MySQL databases are relational (multiple tables that are all connected to each other, they all have that interrelated data)

#### Compability

* Client/server systems
* Embedded systems - it's portable such mobile app

#### Security

* Secure privilege and password systems
* Encrypted password traffic

#### Scalability

* Large database support
* 64 index per table limitation

#### Clients and tools

* mysqldump
* mysqladmin
* MySQL workbench

#### Client connections

* Any platform&#x20;
  * TCP/IP sockets
* Windows
  * Named pipes
* Unix systems
  * Unix domain socket files

### Remote Desktop Protocol (RDP)

* Remote management - refers to an administrator who needs to establish a connection to a server that is physically distant and perform administrative tasks
* Remote access - refer to an administrator  who needs to perform some kind of administrative task on a system that is physically distant

#### Versions

* Windows
* Apple macOS
* Open source

#### RDP Ports

* TCP port 3389
* UDP port 3389

#### RDP Protocol

* Establishes dedicated network channels for exchanging information
  * Using port 3389
  * Via TCP/IP
* All data is encrypted during RDP session

#### Properties

* TLS support
* Bandwidth reduction
* Smart card authentication
* Printer redirection
* 128-bit encryption

#### Advantages

* Security
* Low costs
* Flexibility

#### Disadvantages

* Requires administrators with knowledge of technology
* Possible bottlenecks - if hundreds of users all trying to use RDP to get to the single instance on the server at the same time  this can cause a bit of a slowdown in the performance
* Requires reliable internet connections
* Possibility of downtime

### Session Initiation Protocol (SIP)

* Video
* Voice
* Messaging

#### Session attributes

* User capabilities
* Session setup
* Session management
* User availability
* User location

#### Operation

* Similar to HTTP and SMTP

#### Requests

* Invite
* Bye
* Update - make change such as a user joining a session or user leaving
* Ack - confirm that a user has responded to a request
* Cancel - which would stop any pending request

### Common IP Protocol Types

#### Transmission Control Protocol (TCP)

* Used for data transmission

#### User Datagram Protocol (UDP)

* Ideal for time-sensitive transmissions - such as streaming a video

#### Internet Control Message Protocol (ICMP)

* Network layer protocol - operates at the network layer of the OSI model
* Used as a supporting protocol in the overall TCP/IP suite of protocols
* Acts as an error message standard and provides feedback on communications

#### Generic Routing Encapsulation (GRE)

* Tunneling protocol developed by Cisco Systems
* Encapsulates various network layer protocols
* Tunnels are designed to be completely stateless

#### IP Security (IPsec)

* Authentication
* Integrity
* Confidentiality

#### Security&#x20;

* Encapsulating Security Payload (ESP)
* Authentication Header (AH) - establishment of the identity&#x20;

### Packet Switched Networks&#x20;

#### Connection-oriented Protocol

* Used by endpoint devices to transmit data
* Referred to as a reliable service network
* Transmission Control Protocol (TCP)

#### Benefits&#x20;

* Less error prone
* More reliable
* Data arrives in same order

#### Connectionless Protocols

* Communication sent between two network endpoints without any prior arrangement
  * Device will send message prior to ensuring device on other end is ready to receive
  * Certain protocols allow for error correction
    * Retransmission can be requested if necessary

### Test









