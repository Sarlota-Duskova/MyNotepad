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





## Common Wireless Connectivity Issues





## Wired Network Considerations





## Default Gateway Issues





## Incorrect Netmask Issues





## Duplicate IP or MAC Addresses





## Resolving Common DNS Issues







## Expired DHCP Scopes and Rogue DHCP Servers





## Expired IP Addresses and Incorrect System Times





## SSL Certificates and Blocked Ports





## Incorrect Firewall and ACL Settings





## Hardware Failures and Unresponsive Services





## Common Wired Connectivity Issues





## Test

