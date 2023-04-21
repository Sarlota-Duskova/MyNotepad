# Well-known Ports & Protocols

### File Transfer Protocol (FTP)

* Transmit files
* TCP/IP connections
* Client-server protocol
* Log on or anonymous login
* Operates over port 21 using TCP, but port 20 is sometimes used as well

#### FTP Channels

* Command channel - pass the instruction
* Data channel - for moving a files

#### FTP Modes

* Active - two-way communication, client will request something on the server, then client start listening if responses from the server comes
  * Client is often behind a firewall, so the firewall might be blocking responses from the server
* Passive - from the client to the server, client really just tells the server to listen
  * Passive mode using port 21

#### Establishing FTP Connection

* Command-line FTP
* Web browsers
* FTP client - GUI

#### FTP Features

* Transfer large files
* Improve workflow
* Resume transfers
* Schedule transfers
* Recover data

### Secure Shell (SSH)

* Secure access
* Automated file transfers
* Remote commands
* Network infrastructure management

#### Establishing an SSH

* SSH Client
* Command prompt
  * Uses port 22

#### SSH Commands

* scp
  * Program used for copying files, secured version of RCP (Remote Copy Program)
* sftp
  * Secured version of FTP (File Transfer Protocol)

#### SSH Encryption

* Symmetrical
* Asymmetrical (public and private key)
* Hashing

### Secure File Transfer Protocol (SFTP)

* Secure file transfer protocol
* Runs over SSH
* Supports SSH functionality
* Designed for increased web security
* Use TCP port 22

#### Using SFTP

* Command line
* GUI

#### FTPS&#x20;

* Requires complicated configuration
* Prone to problems
* Requires x.509
* Risk of file corruption
* Cannot be used as a file system
* Requires additional installation and patching

### Telnet Application Protocol

* One of the earliest remote login protocols
* Provides terminal session to remote host
* Established via TCP protocol and port 23
* Device-dependent presentation of information
* Cane be used to manage applications without GUI
* Affordable and accessible

#### Telnet uses&#x20;

* Database access
* Application server program interaction
* Network server and device administration

#### Telnet commands

* telnet hostname
* telnet ip-address port number

### Simple Mail Transfer Protocol (SMTP)

* Standard protocol for sending emails
* Simplifies communication between email servers
* In home environment sending emails with SMTP and when I received email back it is POP3
* In corporate environment it's only SMTP Protocol which is used, all mails remains on the mail servers I just use a program to access the server to see my email
* Use port 25 and TCP as its transport protocol
* Default port 25 is by default not secured
* Using secured port 465/587, more would be seen 587

#### SMTP Phases

* Handshake
* Message transfer
* Connection close

### Domain Name System (DNS)

* Translates domain names to IP addresses
* Eliminates need to memorize IP addresses
* It's up in the Application layer
* Uses port 53&#x20;
* Uses the UDP protocol

#### DNS Servers

www.myfavoritewebsite.com

* DNS recursor
* Root nameserver
* TLD (Top Level Domain) nameserver - starts at .com

**Recursive DNS Resolver**

* Beginning of query
* Responds to recursive request
* Tracks down DNS record

**Authoritative DNS Server**

* End of query
* Holds and is responsible for DNS resource records

#### DNS Queries

* Recursive - I ask a question and I get an answer
* Iterative - it has to iterate or if you will, reiterate several times
* Non-recursive - asking your server for a name for which it is the authoritative server

#### DNS Caching

* Instance where I will see a non-recursive query
* Browser - its not authoritative, but it remember from last time
* Operating system level - can cache that value as well

### Dynamic Host Configuration Protocol (DHCP)

* Facilitates efficient communications between endpoints on a network
* Assigns IP address, subnet mask, default gateway address and DNS address
* Simplifies network IP address management

#### Benefits

* Accurate IP configuration - assign IP configuration to all of the clients
* Reduced IP conflicts
* Automated IP address administration
* Effective change management

#### Risks

* DHCP in its default configuration is not particularly secure so there can be **Unauthorized servers**
* **Unauthorized clients** - any device that has physical access to the network could receive an IP address configuration from a DHCP server
* **IP address depletion** - run out of IP addresses

#### Components

* DHCP server - routers could also be a DHCP server
* DHCP client - receives the IP address configuration from the server
* IP address pool - only the IP address, but then each pool is assigned those other options such as the default gateway, the subnet mask, the DNS server or any other service
* Subnet - serviced by the server, it can be configured to service more than one subnet
* Lease - duration for which that configuration is valid (around week)
* DHCP relay - DHCP process itself relies on broadcasts

### Trivial File Transfer Protocol (TFTP)

* Simple file transfer protocol
* Uses UDP
* Reads and writes files to or from a remote host
* Port 69

#### TFTP Common uses

* Booting network - computers doesnt boot from local storage - this is known as a post-execution environment boot (PXE)
  * The system requests its boot information (boot files) from a network server
* OS network installs - when doing bulk operating system network installs (when you need to push out an OS image to many different computers)
* Device firmware upgrades
* Back up and retrieval of device configuration
* Downloading executables

#### How it works

* RRQ/WRQ (Read Request/ Write Request) request sent
* **ACK** (Acknowledgement) if it was a write request or **DATA packet response** if it was a read request
  * TFTP is an application layer protocol, it's way up at layer seven, ACK is built in to the programming of the application
* Numbered data packets sent
* Numbered ACK packet response - the client will also send ACK of those received numbered packets

#### Security

* No encryption
* No server authentication function
* Limit access to content

### HyperText Transfer Protocol (HTTP)

* For resource fetching
* Foundation of web-based data exchange
* Communication via messages vs. data streams
* Sent over TCP or TLS-encrypted TCP connection
* Port 80

#### Uses

* Caching
* Relaxing constraints - a browser will typically enforce strict separation between websites
* Authentication
* Proxy and tunneling - can have a web server whose IP address is in fact shielded from client systems and they are going through a proxy system to get that content
* Sessions

#### Process

* Open TCP connection
* Send HTTP message
* Read response
* Close or reuse

#### HTTP messages

* Requests
  * HTTP method
  * Path/URL
  * HTTP protocol version
  * Headers
  * Body
* Responses
  * HTTP protocol version
  * Status code
  * Status message
  * Headers
  * Body

### Post Office Protocol v3

* Used by local email software clients to retrieve emails from a remote mail server
* Supported by virtually every email client
* Simple to configure, operate and maintain
* Works on port 110 which is not secured
* Works on port 995  it is secured with SSL

#### How it works

* Client connects to POP3 server
* Authentication
* Message retrieval
* Download and after that delete it from server (some clients allow to store it on server, but only for amount of time)

#### Advantages

* Messages are downloaded and can be read offline
* Attachments open quickly
* Requires less server storage space
* Controllable capacity and size
* Easy to configure and use

#### Drawbacks

* No access from other machines
* Difficulty exporting
* Risk of data corruption and loss
* Risk of viruses or attacks

### Network Time Protocol (NTP)

* Used to sync computer clock times in a network
* Fault-tolerant
* Scalable
* Port 123 (UDP)

#### Purpose

* Accurate time  across all of the systems in your environment

#### Features

* Access highly precise atomic and GPS clocks
* Synchronize via primary time servers
* Uses UTC (Universal Coordinated Time)

### Internet Message Access Protocol (IMAP)

* Used for accessing email on a remote server from a local client
* Directly manage emails on the email server
* Emails only downloaded once opened and have the option to leave a message on the server if want
* Uses unsecured port 143 or secured using SSL operates over port 993

#### Advantages

* Access anywhere
* No download delays
* Increased efficiency and control
* Use offline

#### Challenges

* Requires connection
* Uses storage space
* No automatic deletion

| IMAP                                                  | POP3                                                              |
| ----------------------------------------------------- | ----------------------------------------------------------------- |
| Emails synchronized between computer and email server | Emails are retrieved from your computer and deleted by the server |
| Can create folders on the server                      | Can only access on your computer                                  |
| Can access worldwide from multiple devices            | Once deleted, you no longer have access                           |
|                                                       | Cannot create folders                                             |

### Simple Network Management Protocol (SNMP)

* Enables different devices on a network to share information
* Facilitates communication between devices with different hardware and software
* Identifies connected devices
* Used to monitor network conditions and performance

#### Limitations

* Restricted to SNMP compatible devices
* SNMP must be enabled on the device

#### Components

* SNMP manager - system that is responsible for performing the overall management of the environment, makes requests of an agent and the agent resides on a device that would typically be thought of as the client
* SNMP agent - gathers the information from the client and responds to that query
* MIB (Management Information Base) - all of the components about which the agent would be aware, when the manager issues a query to the agent, agent goes through MIB and says what is it
* SNMP device - it could be everything client or switch or router it's any device

#### SNMP Traps

Could be a notification

* Polled traps - represent the management device quite literally
* Autonomous traps - as an alert if something fails and it immediately informs the manager without waiting for the poll

#### SNMP Ports

* Port UDP 161 - used by SNMP manager when polling
* Port UDP 162 - used when agent sends information to the manager via an SNMP trap

### Lightweight Directory Access Protocol (LDAP)

* Maintain and organize distributed directory information
* Manage and access information exchange over IP network

#### How LDAP works

* Connect with server - port 389
* Client and server exchange data&#x20;

#### Benefits

* Unique entries
* Allows multiple independent directories
* Extensible
* Runs directly over TCP/IP and SSL
* Based on existing technologies
* Automated, open source

#### Disadvantages

* Requires LDAP compliant servers
* Not as user-friendly

#### Components

* Attributes
* Entries
* DIT (Directory Information Tree)

### HyperText Transfer Protocol Secure (HTTPS)

* Secure version of HTTP
* Runs over the SSL protocol (Secure Sockets Layer) - provides encryption for increased security when transferring data over an unsecured network
* Web browsers typically have a visual indicator of HTTPS
* Operates over port 443

#### HTTPS Keys

* Private key
* Public key

Bank has private keys on their servers that are held only by the bank, bank has to register to be able to obtain a private key, they are essentially investigated by a third party certificate authority, and as long as they pass all of the checks, they are issued their private key, they are the only entity to hold that key

When a client make a connection to their web servers, they receive a public key, client can use that key to protect information, anything encrypted with the public key can only be decrypted with the private key

#### HTTPS Benefits

* Encryption
* Protection
* Verification and validation
* Reliability
* Search engine optimization

#### HTTPS Disadvantages

* Costs - you have to pay for your private key
* Performance - transmitting a lot more data
* Accessibility - sometimes firewalls might block access to a secured site
* Mixed content
* Computing overhead - it takes a lot of memory and lot of processing power to deal with the encryption and the decryption

### Server Message Block (SMB)

* It is used to provide shared access to resources
  * Files
  * Directories
  * Printers
  * Routers
  * Port 139 in Windows environment is quite out of date since Windows 2000 or 445 SMB runs over another protocol called NetBIOS uses TCP uses port 445

#### How SMB works

* Anything that allows you to browse for network resources is an SMB application
  * Both parties establish connection via a standard three way handshake between the client and server and then the TCP protocol itself is used as the data transport

#### SMB Security Considerations

* Supporting earlier versions increases security risk
* SMB 1.0 susceptible to attacks (as DOS attack) it can be disabled

#### SMB Examples

* Samba
* FreeNAS
* ConnectedNAS - paid app for Android

#### SMB benefits

* Easy to use
* Shares both resources and files

#### SMB Challenges

* Best used on LAN-connected hosts only
* Inherent authentication security
* Transfer speed it could be limited

### Syslog Analysis and Monitoring

* Works on many types of devices and applications
* Enables sending data about status, events, diagnostics
* Most devices on your network support Syslog
* Port 514 (UDP)

#### Using Syslog

* Application alerting
* General, harder to predict events

#### Syslog Layers

* Syslog content - information in any kind of event message
* Syslog application - is what actually generates that message, routes it to something like a centralized storage location
* Syslog transport - handles the transmission of an entry from a client device to a Syslog server

#### Syslog server

* Syslog listener
* Database

### SMTP TLS E-mail Security

* Communication partner authentication - want to ensure that messages exchanged between two organization is secured
  * But then any sort of general email that you might send just out to anyone on the Internet would not be secured, because you really arent concerned about it in that particular case
* Provides data integrity
* Provides confidentiality

#### SMTP TLS Characteristics

* Non-proprietary - it is something that anyone can use really
* Not an SMTP extension - it's using SMTP over TLS
* Secures SMTP at transport layer
* Similar to HTTPS

#### SMTP TLS Requirements

* Still need SSL certificates - certificate is simply something that states something about the entity, TLS can still use the certificate just defines the properties of that system
* Specifically confirute and maintenance server to use those certificates and to implement them during communication
* Requires additional resource allocation

#### Security

* Protects transmission of content
* No protection before or after
* Additional security required

#### Risk

* TLS not enforced
* Weaker encryption mechanisms may be used - if one server support 128bit encryption and the other service support 256bit then the lowest cost common denomiator will be used
* Mismatched encryption mechanisms can cause failure - if one server support only 128bit encryption and other one support only 256bit then this can cause a failure

### Secure Lightweight Directory Access Protocol (LDAPS)

* Is not a secure protocol, so it can be combined with or transmitted over SSL to make it secure
* It is only used within the internal organization
* LDAPS uses port 636 and establishes TLS/SSL for client connections
* LDAPS is commonly used in Microsoft environments
* Very compatible with Microsoft's Active Directory
* Requires a certificate from a certification authority (CA)
  * Microsoft or a non-Microsoft CA
* No user interface available for configuring LDAPS

### Secure IMAP (Internet Message Access Protocol) Traffic

* Connect a client to an email server to retrieve email
* Allows two-way communications
* Local client settings can be reflected on the server (create folder structure in local client and that could be implemented on the server as well)
* SSL
  * Encryption protocol for online communications
  * Authentication certificates
  * Encryption algorithm negotiated
  * Secure data transmission

#### How IMAP over SSL works

* The client will initiate the communication with the server at which point the server sends an OK notification indicating service ready
* Client responds
* The server response OK indicating start of negotiation
* Client requests capabilities again
* Exange data

### POP3 SSL Secure E-mail Connections

#### POP3 Implicit SSL Mode&#x20;

* Client will attempt to connect using secure SSL channel
* If server for some reason doesnot support SSL, then the connection will fail

#### POP3 Explicit SSL Mode

* Client will not necessarily assume that SSL is supported
* Client will initially connect using a clear text channel
* Once it determines that the server can support SSL - Issues command to secure the channel

#### Ports

* Secured port 995
* Unsecured port 110

### Test











