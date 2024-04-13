# Description

* **1.1 Compare and contrast the Open Systems Interconnection (OSI) model layers and encapsulation concepts.**
  * OSI model
    * Layer 1 – Physical
    * Layer 2 – Data link
    * Layer 3 – Network
    * Layer 4 – Transport
    * Layer 5 – Session
    * Layer 6 – Presentation
    * Layer 7 – Application
  * Data encapsulation and decapsulation within the OSI model context
    * Ethernet header
    * Internet Protocol (IP) header
    * Transmission Control Protocol (TCP)/ User Datagram Protocol (UDP) headers
    * TCP flags
    * Payload
    * Maximum transmission unit (MTU)
* **1.2 Explain the characteristics of network topologies and network types.**
  * Mesh
  * Star/hub-and-spoke
  * Bus
  * Ring
  * Hybrid
  * Network types and characteristics
    * Peer-to-peer
    * Client-server
    * Local area network (LAN)
    * Metropolitan area network (MAN)
    * Wide area network (WAN)
    * Wireless local area network (WLAN)
    * Personal area network (PAN)
    * Campus area network (CAN)
    * Storage area network (SAN)
    * Software-defined wide area network (SDWAN)
    * Multiprotocol label switching (MPLS)
    * Multipoint generic routing encapsulation (mGRE)
  * Service-related entry point
    * Demarcation point
    * Smartjack
  * Virtual network concepts
    * vSwitch
    * Virtual network interface card (vNIC)
    * Network function virtualization (NFV)
    * Hypervisor
  * Provider links
    * Satellite
    * Digital subscriber line (DSL)
    * Cable
    * Leased line
    * Metro-optical
* **1.3 Summarize the types of cables and connectors and explain which is the appropriate type for a solution.**
  * Copper
    * Twisted pair
      * Cat 5
      * Cat 5e
      * Cat 6
      * Cat 6a
      * Cat 7
      * Cat 8
    * Coaxial/RG-6
    * Twinaxial
    * Termination standards
      * TIA/EIA-568A
      * TIA/EIA-568B
  * Fiber
    * Single-mode
    * Multimode
  * Connector types
    * Local connector (LC), straight tip (ST), subscriber connector (SC), mechanical transfer (MT), registered jack (RJ)
      * Angled physical contact (APC)
      * Ultra-physical contact (UPC)
    * RJ11
    * RJ45
    * F-type connector
    * Transceivers/media converters
    * Transceiver type
      * Small form-factor pluggable (SFP)
      * Enhanced form-factor pluggable (SFP+)
    * Quad small form-factor pluggable (QSFP)
    * Enhanced quad small form-factor pluggable (QSFP+)
  * Cable management
    * Patch panel/patch bay
    * Fiber distribution panel
    * Punchdown block
      * 66
      * 110
      * Krone
      * Bix
  * Ethernet standards
    * Copper
      * 10BASE-T
      * 100BASE-TX
      * 1000BASE-T
      * 10GBASE-T
      * 40GBASE-T
    * Fiber
      * 100BASE-FX
      * 100BASE-SX
      * 1000BASE-SX
      * 1000BASE-LX
      * 10GBASE-SR
      * 10GBASE-LR
      * Coarse wavelength division multiplexing (CWDM)
      * Dense wavelength division multiplexing (DWDM)
      * Bidirectional wavelength division multiplexing (WDM)
* **1.4 Given a scenario, configure a subnet and use appropriate IP addressing schemes.**
  * Public vs. private
    * RFC1918
    * Network address translation (NAT)
    * Port address translation (PAT)
  * IPv4 vs. IPv6
    * Automatic Private IP Addressing (APIPA)
    * Extended unique identifier (EUI-64)
    * Multicast
    * Unicast
    * Anycast
    * Broadcast
    * Link local
    * Loopback
    * Default gateway
  * IPv4 subnetting
    * Classless (variable-length subnet mask)
    * Classful
      * A
      * B
      * C
      * D
      * E
    * Classless Inter-Domain Routing (CIDR) notation
  * IPv6 concepts
    * Tunneling
    * Dual stack
    * Shorthand notation
    * Router advertisement
    * Stateless address autoconfiguration (SLAAC)
  * Virtual IP (VIP)
  * Subinterfaces
*   **1.5 Explain common ports and protocols, their application, and encrypted alternatives.**

    | **Protocols**                                                            | **Ports** |
    | ------------------------------------------------------------------------ | --------- |
    | File Transfer Protocol (FTP)                                             | 20/21     |
    | Secure Shell (SS)                                                        | 22        |
    | Secure File Transfer Protocol (SFT)                                      | 22        |
    | Telnet                                                                   | 23        |
    | Simple Mail Transfer Protocol (SMTP)                                     | 25        |
    | Domain Name System (DNS)                                                 | 53        |
    | Dynamic Host Configuration Protocol (DHCP)                               | 67/68     |
    | Trivial File Transfer Protocol (TFTP)                                    | 69        |
    | Hypertext Transfer Protocol (HTTP)                                       | 80        |
    | Post Office Protocol v3 (POP3)                                           | 110       |
    | Network Time Protocol (NTP)                                              | 123       |
    | Internet Message Access Protocol (IMAP)                                  | 143       |
    | Simple Network Management Protocol (SNMP)                                | 161/162   |
    | Lightweight Directory Access Protocol (LDAP)                             | 389       |
    | Hypertext Transfer Protocol Secure (HTTPS) \[Secure Sockets Layer (SSL)] | 443       |
    | HTTPS \[Transport Layer Security (TLS)]                                  | 443       |
    | Server Message Block (SMB)                                               | 445       |
    | Syslog                                                                   | 514       |
    | SMTP TLS                                                                 | 587       |
    | Lightweight Directory Access Protocol (over SSL) (LDAPS)                 | 636       |
    | IMAP over SSL                                                            | 993       |
    | POP3 over SSL                                                            | 995       |
    | Structured Query Language (SQL) Server                                   | 1433      |
    | SQLnet                                                                   | 1521      |
    | MySQL                                                                    | 3306      |
    | Remote Desktop Protocol (RDP)                                            | 3389      |
    | Session Initiation Protocol (SIP)                                        | 5060/5061 |

    * IP protocol types
      * Internet Control Message Protocol (ICMP)
      * TCP
      * UDP
      * Generic Routing Encapsulation (GRE)
      * Internet Protocol Security (IPSec)
        * Authentication Header (AH)/Encapsulating Security Payload (ESP)
      * Connectionless vs. connection-oriented
* **1.6 Explain the use and purpose of network services.**
  * DHCP
    * Scope
    * Exclusion ranges
    * Reservation
    * Dynamic assignment
    * Static assignment
    * Lease time
    * Scope options
    * Available leases
    * DHCP relay
    * IP helper/UDP forwarding
  * DNS
    * Record types
      * Address (A)
      * Canonical name (CNAME)
      * Mail exchange (MX)
      * Authentication, authorization, accounting, auditing (AAAA)
    * Start of authority (SOA)
    * Pointer (PTR)
    * Text (TXT)
    * Service (SRV)
    * Name server (NS)
  * Global hierarchy
    * Root DNS servers
    * Internal vs. external
    * Zone transfers
    * Authoritative name servers
    * Time to live (TTL)
    * DNS caching
    * Reverse DNS/reverse lookup/forward lookup
    * Recursive lookup/iterative lookup
  * NTP
    * Stratum
    * Clients
    * Servers
* **1.7 Explain basic corporate and datacenter network architecture.**
  * Three-tiered
    * Core
    * Distribution/aggregation layer
    * Access/edge
  * Software-defined networking
    * Application layer
    * Control layer
    * Infrastructure layer
    * Management plane
  * Spine and leaf
    * Software-defined network
    * Top-of-rack switching
    * Backbone
  * Traffic flows
    * North-South
    * East-West
  * Branch office vs. on-premises datacenter vs. colocation
  * Storage area networks
    * Connection types
      * Fibre Channel over Ethernet (FCoE)
      * Fibre Channel
      * Internet Small Computer Systems Interface (iSCSI)
* **1.8 Summarize cloud concepts and connectivity options.**
  * Deployment models
    * Public
    * Private
    * Hybrid
    * Community
  * Service models
    * Software as a service (SaaS)
    * Infrastructure as a service (IaaS)
    * Platform as a service (PaaS)
    * Desktop as a service (DaaS)
  * Infrastructure as code
    * Automation/orchestration
  * Connectivity options
    * Virtual private network (VPN)
    * Private-direct connection to cloud provider
  * Multitenancy
  * Elasticity
  * Scalability
  * Security implications
