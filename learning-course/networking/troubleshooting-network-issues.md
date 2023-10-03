# Troubleshooting Network Issues

## Protocol Analyzers and Packet Sniffers

### Packet Sniffers

* Intercept and log network traffic
* Wired
* Wireless
* Software applications
* Hardware appliances

#### Examples of the information that can be ascertained from packet sniffers:

* Communications between parties
* Captures cleartext passwords
* Identifies websites visited
* Classification of traffic
* Applications being used

### Diagnostic Testing

* Monitor activity
* Troubleshoot network

### Identifying Threats

* Identify protocols
* Detect vulnerabilities

## Network Port Scanning

### Port Scanning

* Identify open ports
* Application and service communication

### Ethical Hacking

* Identify holes
* Secure network

### Hacking

* Identify vulnerabilities
* Access network

### Vanilla Technique

* All 65 536 ports
* Basic port scan
* Connect requests
* Logged by firewalls

### SYN Scan

* Half-open scan
* Wait for SYN-ACK response
* Doesn't respond
* Not logged
* Sender learns if port is open or closed

### FIN Scan

* Unsolicited FIN flag (finish)
* &#x20;Reveal state of port

### Xmas Scan

* Set of flags
* Based on system response

### FTP Bounce Scan

* FTP server disguises sender location
* Sender undetected

### Sweep Scan

* Identify active devices
* Ping port on multiple devices

## Wi-Fi Analysis Tools and Techniques

### Wi-Fi Analyzer

* Software
* Dedicated hardware
* Scan Wi-Fi usage
* Map site
* Identify interference

### Wi-Fi Analyzer Statistics

* Supported speeds
* Lost packets/retry rates
* Device information
* Inventory
* Hardware

## Bandwidth Speed Testing

### Bandwidth

* Multiple factors affect bandwidth
* Troubleshoot with bandwidth speed tester

### Factors Affecting Bandwidth

* Distance
* Wiring
* Network devices
* Time of day

### Online Speed Testers

* Different tools
* Browser

### Bandwidth Speed Tester - Ping

* Single destination
* Time, packet loss

### Bandwidth Speed Tester

* Download
* Upload

## Common Network Software Tools

### iperf

* Used to measure maximum bandwidth performance (TCP/UDP)

### NetFlow

* Is a protocol that was designed by Cisco to capture and analyze network traffic to gain more insight into the type and the volume of traffic in your network
* Collectors
* Analyzers

#### TFTP (Trivial File Transfer Protocol)

* Simple protocol for transferring files between network devices

### Terminal Emulator

#### Telnet and SSH

* Enables a host computer to access another computer
* Connections can be made using
  * Command line interface
  * Graphical interface

### IP Scanning

* Identify IP address space statistics
* Gain insight

### IP Scanning Benefits

* Troubleshooting
* Monitoring
* Auditing
* Managing

## Common Command Line Tools

### Command Line Tools - Ping (Packet Internet Groper)

* Between hosts
* ICMP (Internet Control Message Protocol) as its transport protocol and quite simply determines the status of a connection to a remote host
* Loopback (localhost = 127.0.0.1)

### ipconfig

* Identify network configuration
* Display TCP/IP address information
* All, release, renew parameters

### tracert

* Packet path
* Source to destination

### pathping

* Latency and loss
* Echo requests
* Problem identification
* Multiple parameters

### nslookup

* Diagnose DNS by returning the IP address that matches the host name that you supply or vice versa
* Identify DNS server
* Verify address by record type
* Reverse name lookups

### arp

* Display
* Manage ARP cache information
* Add
* Remove

Recall that arp resolves an IP address to a MAC address

### netstat

* Connection status
* Routing tables
* Protocol and port status

### route

* Configure routing table
* Add, delete, change

## Common Linux Commands

### ifconfig

* Assign
* Configure
* Display

### tcpdump

* TCP/IP packets
* Save for analysis
* .pcap format
* View with tcpdump or open source tools

### iptables

* Manage tables of IPv4 packet filter rules
* Setup, maintain, inspect
* Built-in or user-defined chains

### nmap

* Security
* Exploration
* Auditing
* Monitoring

### dig

* DNS nameservers
* Host addresses
* Server roles
* Similar to nslookup
* Other information

## Wireless Specifications and Limitations

### Wireless Speed and Distance Limitations

* One of the most common problems
* Wireless signals can only travel a certain range
* Performance can be impacted by
  * Walls/corners
  * Materials
  * Other radio interference
  * Signals from other devices

2.4 GHz can travel farther and is better at penetrating obstacles

5.0 GHz is faster and less prone to interference

### Wi-Fi Router Position

* Re-positioning a router in a different location can potentially result in greater performance

### Router Firmware

* Security
* Performance
* Stability

### Received Signal Strength Indicator (RSSI)

* Measurement used to detect strength of signal between device and router

### Effective Isotropic Radiated Power (EIRP)

* Measurement of antenna power

### Reflection

* Wireless signals can bounce off certain surface types

### Absorption

* Common reaction when wireless signals meet different materials
  * Wood
  * Concrete
* Affects overall signal strength

### Other issues

* Diffraction
* Scattering

## Wireless Connectivity Considerations

#### Incorrect Antenna Type

* Varios Wi-Fi antennas
  * Each designed for a specific purpose
* Directional antennas
  * Designed to focus on certain areas of coverage
* Omnidirectional antennas
  * Designed for 360-degree coverage

#### Incorrect Antenna Aiming

* Common on legacy access points
  * Diversity antennas
* If improperly aligned, it could be detrimental to performance
* Hidden node
  * Occurs when two clients in opposite directions connect to same access point, but cannot detect each other

#### Channel Utilization

* If utilization is too high, consider another non-overlapping channel

#### Antenna Polarization

* Frequency
* Coverage
* Physical constraints

#### Association

* AP/routers perform association to record each mobile device

#### Wireless Site Survey

* Performed prior to deployment or when troubleshooting

## Common Wireless Connectivity Issues

#### Wi-Fi Interference

* Other Wi-Fi networks in the same range
  * Neighbor's Wi-Fi network
  * Another company Wi-Fi in the same shared building
* Consider using dual-band routers
  * Operate simultaneously
    * 2.4 GHz
    * 5 GHz

#### Channel Assignments

* Incorrect channel assignments
  * Less common with modern devices
    * Auto-detect channel configuration
* If using the 2.4 GHz frequency band
  * Non-overlapping channels
    * Channel 1, 6 and 11

#### Wi-Fi Capacity

* Sharing bandwidth
* 802.11g - 54 Mbps
* 802.11n and 802.11ac - 450 Mbps to 1.3 Gbps
* Lower-end devices
  * May experience other limitations such as RAM and CPU
* Other features use resources on the AP/router
  * MAC filtering
  * Port forwarding
  * Firewall

#### Service Set Identifier (SSID) Issues

* Network name
* Configurable
  * Must match on client and AP
* Misconfigured SSIDs
  * Clients will be unable to connect
  * May connect to wrong network altogether

#### Incorrect Passphrases

**Wired Equivalent Privacy (WEP)**

* Passphrase
  * 40-64 bit encryption
    * 10 hex or 5 ASCII characters
  * 104/128-bit encryption
    * 26 hex or 13 ASCII characters

**WPA/WPA2 Personal**

* Preshared Key
  * 8-63 characters

#### Wireless Connectivity Issues

* Signal loss
* Encryption protocol mismatch
* Coverage issues
* Client disassociation issues
* Captive portal issues

## Wired Network Considerations

#### Crosstalk

* Crosstalk occurs when signals from one wire interfere with signals on another
  * Wires that are exposed or in very close proximity

#### Duplex Mismatch

* Half duplex
* Full duplex

#### Incorrect VLAN Assignment

* 802.1Q trunk
  * Traffic is tagged with the VLAN ID except for the native VLAN
* Untagged traffic will be assigned the wrong VLAN if two switches connected to the trunk have different native VLANs configured
* All trunking switches should be configured for the same native VLAN

#### Bad Ports

* Bad ports on a switch can cause unexpected traffic drops and performance issues
  * If a port is identified as faulty, consider labeling it
    * Prevent any future confusion

#### Interface Configuration Problems

* Poor throughput (e.g. inconsistent)
* No connectivity

#### Bottlenecks

* I/O bus
* CPU/ memory
* Network adapter speed
* Storage

#### Routing Tables

* Determine route data is to be sent

## Default Gateway Issues

* Connect to external network
* Means to leave your own network
* PC with dual adapters
* One interface on each network
* External network
* Default - no other gateway specified

#### Unreachable Default Gateway

* Isolate the problem
* Host - check IP and cables
* Subnet - could be router

## Incorrect Netmask Issues

* 32-bit value
* Network ID
* Host ID

#### Netmask

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

#### Troubleshooting Netmask

* Check devices
* Documentation
* Confirm subnet mask
* Match configuration

#### Troubleshooting Netmask - Tools

* Ipconfig
* Ping

## Duplicate IP or MAC Addresses

* Same IP assigned to two devices
* Disabled
* Lose connectivity
* Same address assigned - when using static IP address
* Statically assigned
* DHCP configuration - setting up range that has been already assigned to some device
* Returning online

#### Static IP Addresses

* Multiple network administrators
* Static IPs don't change
* Additional administrative overhead

#### Troubleshooting Duplicate IP Addresses

* Review documentation
* Ping the address
* Refer to MAC address table
* Packet capturing

#### MAC Addresses

* Hardware address
* 12 hexadecimal characters
* Manufacturer-assigned
* Globaly unique

#### Duplicate MAC Addresses

* Uncommon occurrence
* Vendor-assigned address not used
* Locally administered MAC address

#### ARP Utility

* Discover MAC addresses
* ARP cache
* Troubleshoot problems
* Duplicate IP and MAC

## Resolving Common DNS Issues

#### Troubleshooting DNS

* Domain or host name to IP
* Browsing and e-mail

#### DNS Issues

* Inability to connect
* Browsers report no internet access
* nslookup for internal DNS issues

#### Alternate DNS

* Primary and secondary DNS servers
* Secondary server acts as a stand-by

#### Troubleshooting DNS

* DNS server online?
* Ping DNS server
* Single user?
* Entire subnet?

#### Malware/Attacks

* DNS poisoning
* Other malware

## Expired DHCP Scopes and Rogue DHCP Servers

#### DHCP Scope

* Range of addresses
* Leased to clients
* Complete IP configuration
* Other servers

#### DHCP Scope Properties

* Reservations
* Exclusion ranges
* Lease duration
* Scope name
* Description

#### Common Scope Issues

* DHCP scope not activated
* Lease duration
* Limited scope
* DHCP service stopped
* Client-side misconfiguration

#### Rogue DHCP Server

* Unauthorized DHCP server
* Used to redirect clients
* Clients cannot distinguish the rogue server from a legitimate time

#### Detecting Rogue DHCP Servers

* DHCPLOC utility
* ipconfig/all

#### Mitigating Rogue DHCP Servers

* DHCP snooping
* Intrusion Detection System (IDS)
* Network Monitor
* Active Directory authorizes DHCP servers

## Expired IP Addresses and Incorrect System Times

#### DHCP Lease Time

* Laptops
* Desktops
* Smartphones
* Servers
* Tablets

#### Optimum DHCP Lease Time - Home Network

* More addresses than devices
* Longer lease period

#### Optimum DHCP Lease Time - Public Place

* Many guests
* Shorter lease period

#### Expired IP Addresses

* Address configuration discarded
* Interfere with devices and services
* IP address conflicts

#### Incorrect System Times

* Computer clocks can be inaccurate
* Devices can be manually configured

#### Time Synchronization Is Critical

* Logging
* Managing
* Securing
* Planning
* Debugging

#### Incorrect Time and Network Issues

* Cannot join domain
* Synchronization issues

#### Network Time Protocol

* Synchronize devices
* Universal time servers

## SSL Certificates and Blocked Ports

#### SSL Certificates

* Standard security protocol
* Protects information in transit
* Encryption between bew servers and browsers

#### Common SSL Problems

* Server Name Indication (SNI)
* Missing certificates
* Validity issues
* Client certificates

#### Troubleshooting SSL Issues

* SSL Labs
* Wireshark
* OpenSSL

#### Common SSL Problems

* TLS
* Supported protocols

#### Errors - Certificate Failure

* Missing chain certificates
* Certificate no longer valid
* Verification failed
* Invalid system time

#### Errors

* No shared ciphers
* Unknown protocol (TLS)

#### Blocked Ports

* Endopoints of communication
* Depends on service
* TCP/UDP

#### Blocked Ports - Port Scanners

* Single port
* Range of ports
* Vulnerable ports

## Incorrect Firewall and ACL Settings

#### Firewall Issues

* Misconfiguration
* Lost connectivity

#### Firewall Configuration Issues

* Check network configuration and cabling
* Verify logging
* Verify firewall rules
* Network Address Translation (NAT)
* Before or after security rules
* Check with documentation

#### ACLs - Source and Destination Traffic

* IP addresses
* Zone
* Interface

#### ACL Misconfiguration

* Prevent legitimate access
* Fail to block unauthorized access
* Audit to align configuration and policy

## Hardware Failures and Unresponsive Services

#### Hardware Failure

* Straightforward troubleshooting
* No changes suggest hardware
* Firmware

#### Diagnosing Switches

* Ping switch
* Physically access
* Connectivity
* Status lights

#### Windows Services

* Automatic
* Automatic (delayed)
* Manual
* Disabled

#### Examples of Windoes Services

* Active Directory Service
* Background Intelligent Transfer Service
* DNS Server/client service
* DHCP Server/client service
* Server service
* Remote Desktop Services

#### Configuring Windows Services

* Services console
* PowerShell/Command prompt

#### Troubleshooting Unresponsive Services

* Event Viewer
* Windows Logs > Application
* Windows Logs > System

## Common Wired Connectivity Issues

#### Broadcast Storms

* Capture packets to identify the source of the problem

#### Asymmetric Routing Problems

* Can occur when a network has multiple paths to the Internet

#### Routing Loop

* Can result in serious network problems
* Can occur when data packets are routed through the same routers repeatedly
* Creates an endless circle

#### DHCP Scope Exhaustion

* DHCP IP address pool starts to run out

#### Missing Routes

* Can result in a 'Destination host unreachable' error

#### Optical Link Budget

**Fiber optics**

* Allocation of available optical power
* Considerations
  * Transceiver power
  * Fiber loss
  * Connector loss
  * Patch panel loss

#### Certificate Errors

* E.g. SSL certificate errors

#### Incorrect VLANs

* Typically occurs when users are
  * Moved
  * Configured with new adapters
* Document VLAN arrangement can help prevent issues

#### BYOD Challenges

* Organizations must exert some form of control over devices

## Test

**Which utility would be the best option to use when trying to determine the maximum bandwidth specifications of applications using either the TCP or the UDP transport protocol?**

* iperf

**A packet sniffer might be used in which situations?**

* Identify if weak passwords are being used
* Classifying traffic

**Which statement most accurately characterizes the likelihood of a MAC address conflict in a network?**

*

