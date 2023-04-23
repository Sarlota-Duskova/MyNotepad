# Network Services & Data Center Architectures

### DNS Namespace Structure

* Internal
* External

They are:

* Third party
* Cloud-hosted DNS
  * Scalability
  * Reliability
  * High availability

#### DNS Hierarchy

* Root-level - it's only "." empty string after that
* Top-level (TLDs)- mycompany.com -> .com is top-level
* Second level - mycompany.com -> .mycompany is second level
* Subdomain (3rd level (sub) domains) - northamerica.mycompany.com -> .northamerica is subdomain
* Host - www.mycompany.com -> www is a host or dc1. - dc1.northamerica.mycompany.com. and the last dot represent root

#### Forward DNS Lookup

* Convert name to IP address
* Common for websites

#### Reverse DNS Lookup

* Opposite of DNS lookup
* Query IP address - A client has an IP address so that's what I'm submitting
* Determines hostname

### DNS SOA Records

#### Start of Authority (SOA) Records

* General parameters for DNS
* Zone contains single SOA record
* Identifies the authoritative server

#### Record Structure

* Class
* Current zone
* Primary master - server itself or the IP address of that system
* Type - SOA
* Contact email
* Serial number
* Refresh time - directs clients to refresh the values to ensure they are correct with respect to the name
* Retry time - tells the client to continue to try for x amount of time before it should consider that server is down
* Expiration time - registration time
* Time to live (TTL) - in given point, it is possible that either the name or the IP address could change

### Common DNS Record Types

#### Name Server Records

* List servers for domain
* Permit other name servers
* More than one name server

#### A Records

* "A" stands for address
* "AAAA" used for IPv6 records

### MX Records

* Mail exchanger record
* Servers configured to accept mail

**MX Parameters:**

* Mail server
* Mail preference

#### SRV Records

* Service records
* Query DNS for locations
* Efficient management and distribution

#### Text (TXT) Record

* Additional information about a named service
* Sender Policy framework (SPF)
* DomainKeys Identified Mail (DKIM)

#### Canonical Name (CNAME)

* Also known as alias records
* Assigns an alternate hostname where an address (A) record already exists

### DHCP IP Addressing Service

#### Dynamic Host Configuration Protocol (DHCP)

* Dynamic IP assignment
* Replaces manual assignment
* IP, gateway, subnet mask, DNS servers

#### DHCP Discover

* Broadcast to locate DHCP server
* If no response, client assigns itself an APIPA (automatic private IPv4 address)

### Network Time Protocol (NTP)

#### NTP Stratum 0

* Most accurate devices
* Atomic, GPS clocks
* Cannot be connected via LAN
* Reference clock
* Synchronization source

#### NTP Stratum 1&#x20;

* Most accurate through network connections
* Synchronized by Stratum 0 reference clock

#### NTP Stratum 2

* Synchronized from Stratum 1 devices through network
* Not as accurate as Stratum 1
* Delays, jitter

#### NTP Stratum 3

* Synchronized from Stratum 2 servers
* Identical algorithm as Stratum 2&#x20;
* Act as server for Stratum 4 devices

### IP Address Management (IPAM)

* IPv4/IPv6 address infrastructure
* DHCP/DNS
* Enhanced IP address management
* All subnets managed by all servers

#### IPAM Multi-server Management (MSM)

* Discover DNS and DHCP across AD forest
* Configuration support of DHCP servers/scopes
* Simultaneous updates across DHCP scopes/servers
* Monitor DHCP scope utilization
* Availability monitoring od DHCP and DNS
* Manual addition or removal of servers

#### IPAM Network Audit

* Query event catalog for changes
* Advanced queries
* Export audit findings
* Resolve configuration problems

#### IPAM Role-based Access Control

* Customize operations and access permissions
* Groups (security, role-based)

### Three-tier Network Architectures

* In larger data centers
* Core switches
* Distribution layer switches
* Access switches

#### Disadvantages

* More intra-DC traffic
* More latency
* Bottlenecks, dropped packets, buffer overruns
* Loops - there are multiple paths, it can end up being directed back to the same place where it came from in the first place

### Software-defined Networking Technology (SDN)

* Network architecture
* Software-controlled
* Hardware-independent

#### Benefits

* Network programmability
* Network abstraction
* Logical centralized intelligence and control
* Openness

### Storage Area Network Solutions (SAN)

* Connect to storage devices via network
* Data blocks
* Fast and resilient

#### Features

* Multipath for any particular block of storage
* High-availability clusters
* High throughput
* Improved performance

#### Fiber Channel (FC) Technologies

* Fiber optic infrastructure
* Fiber Channel Protocol (FCP)

#### Fiber Channel Over Ethernet (FCoE)

* Lossless Ethernet
* Converged infrastructure
* Alternative to Fiber Channel

#### Internet Small Computer Systems Interface (iSCSI)

* SCSI inside TCP/IP
* Target/ initiator
* Block level storage over Ethernet

**Considerations:**

* Manual IP configuration
* Network optimization
* Fast network adapters

**Recommendations:**

* 10Gbps Ethernet
* Fast adapters and switches
* Large data frame transfers

### Spine and Leaf Network Topologies

* When is needed to increase of east-west traffic
* Better capacity
* Better performance
* Scalability

### Colocation Data Centers

* Implemented for data center
* Rent to third parties
* Companies that can't maintain their own
* Multiple servers in one data center
* Company-owned
* May be maintained
* Multiple locations

#### Benefits

* Reduced cost
* Reduced staff
* Geography
* Redundancy
* Scalability
* Easy budgeting

### Test





&#x20;
