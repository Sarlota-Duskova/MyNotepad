# Ethernet Switching & Wireless Standards

## Data Virtual Local Area Network

### VLAN Virtual Local Area Network

* Logical grouping of devices

**Benefits:**

* Cost-effective solution
* Reduces administrative overhead

&#x20;**VLAN Characteristics**

* Increase the number of broadcast domains
* Reduce security risks
* Improve performance
* Design more flexible networks
* Change network configurations easily

**LAN Topology**

<figure><img src="../../.gitbook/assets/lan.jpg" alt=""><figcaption></figcaption></figure>

**VLAN Configuration**

<figure><img src="../../.gitbook/assets/vlan.jpg" alt=""><figcaption></figcaption></figure>

**VLAN Membership**

* Static
* Dynamic

**VLAN Connections**

* Access link - computer to switch
* Trunk link - switch to switch

**Trunk Tagging**

* Identifies VLAN membership across multiple switches

<figure><img src="../../.gitbook/assets/trunk_tagging.jpg" alt=""><figcaption></figcaption></figure>

## Voice VLAN Configurations

* Allocated for VoIP systems

<figure><img src="../../.gitbook/assets/voicevlan.jpg" alt=""><figcaption></figcaption></figure>

**Benefits**

* Ensures VoIP devices are not impeded
* Prioritizes voice services
* Simplifies network configuration

**Voice VLAN Modes**

* Normal mode
* Security mode

## Ethernet Switching Port Configuration

### Duplex Communication

* Traffic can travel in both directions

**Full-duplex communication**

* Send and receive at the same time

**Half-duplex communication**

* Send or receive

<figure><img src="../../.gitbook/assets/duplex.jpg" alt=""><figcaption></figcaption></figure>

### Link Aggregation Control Protocol (LACP)

* Combine the bandwidth of multiple physical ports into a single logical port
* Increased reliability
* Physical resource allocation
* Improved bandwidth
* Cost-effective

### Port Aggregation Protocol (PAgP)

* Three configuration
  * Auto (passive)
  * Desirable (active)
  * On

### Flow Control

* Reduces packet loss

### Port Mirroring

* Used for diagnosing errors

### Port Security

* Prevents unknown devices from forwarding packets

### Jumbo Frames

<figure><img src="../../.gitbook/assets/jumbo.jpg" alt=""><figcaption></figcaption></figure>

### Ethernet Interfaces

* MDI (Medium Dependent Interface)
* MDIX (Crossover)
* Auto-MDI/MDIX

## Media Access Control Address Tables

### MAC Addresses

* A media access control (MAC) address is 48-bit long, represented by 12 hexadecimal characters, and coded into the network interface upon manufacture
* Example MAC address: 00:AA:19:9A:58:B4

<figure><img src="../../.gitbook/assets/mac.jpg" alt=""><figcaption></figcaption></figure>

OUI (Organizationally Unique Identifier) - allocated to a particular vendor or manufacturer by the IEEE (Institute of Electrical and Electronics Engineers)

**MAC Address Operation**

* Resides in the Data Link 2 layer&#x20;
  * LLC Sublayer (Logical Link Control)
  * MAC Sublayer

## Power over Ethernet

* Enables network cables to carry electrical power

**Common Devices:**

* VoIP phones
* Wireless devices
* IP cameras

**Benefits**

* Cost savings
* Reliability
* Scalability
* Flexibility

**Limitations**

* Power delivery rates
* Transmission distance
* Device compatibility

**Distances**

* 100 to 1000+ meters thats just the data
* The power can actually go a lot father than that

**Specifications**

* PoE - Voice over IP phone, some kind of a sensor or a meter or a Wireless Access Point
* PoE+ - Required for camera that also moves
* PoE++ - would be for a devices that really do draw a lot of power, such as a complex video conferencing system or various other building management devices

Only main difference here is the amount of power that is going to be required for the device and/or what the specifications call for.

## Spanning Tree Protocol (STP)

* Protocol used to prevent switching/ bringing loops
* Works at the data link layer where switches and bridges operate

**Looping**

* Ethernet frames circulating the network without reaching their destination

**Looping example:**

<figure><img src="../../.gitbook/assets/looping.jpg" alt=""><figcaption></figcaption></figure>

**Advantages**

* Simple to use
* Wide support
* Redundancy
* Proven technology
* Familiar

**Disadvantages**

* I/O limitations
* Widespread failure



STP is being replaced through different architectures in data centers and the use of features such as Link Aggregation Protocol

## CSMA/CD Media Access Control Methods

* Carrier sense multiple access/collision detection

**Collision Detection (CD)**

* Regulates communication

**CSMA/CD Components**

* Carrier sense (CS)
* Medium access (MA)
* Collision detection (CD)

**CSMA/CD Process**

<figure><img src="../../.gitbook/assets/csmad.jpg" alt=""><figcaption></figcaption></figure>

**Protocols**

* CSMA/CD
* CSMA/CA (Collision avoidance)

## Address Resolution Protocol (ARP)

* Resolves IP address to MAC (Media Access Control) address
* Works between layers 2 and 3
  * MAC address = Layer 2
  * IP address = Layer 3

**Advantages of ARP**

* End node discovery
* Easily identify MAC addresses

**Disadvantages of ARP**

* Prone to malicious activity

**ARP Attacks**

* Man-in-the-middle attacks
* Denial-of-service attacks
* Session hijacking

## Neighbor Discovery Protocol (NDP)

* Used in conjuction with IPv6
* Responsible for the resolution of IPv6 addresses into valid MAC addresses
* Addresses are stored in neighbor cache

**Neighbor Cache**

* Devices using NDP manage their own neighbor cache

**NDP Cache Components**

* Destination cache
* Default router list
* Prefix cache

**NDP Additional Functionality**

* Detecting duplicate addresses
* Verifying host relevance
* Router and prefix detection
* Determining transmission parameters
* Redirect options

## 802.11 Standards and Technologies

In February of 1980 => 802

**IEEE 802.11**

* Transmission speed of 1-2 Mbps over 2.4 GHz frequency&#x20;

**IEEE 802.11a**

* Speeds of up to 54 Mbps over 5 GHz frequency

**IEEE 802.11b**

* 11 Mbps
* Backward compatible with 802.11
* 2.4 GHz

**IEEE 802.11g**

* 54 Mbps
* 2.4 GHz

**IEEE 802.11ac**

* Speeds from 433 Mbps to 1.3 Gbps

**IEEE 802.11ax**

* WiFi 6
* Next generation standard in WiFi technology
* Referred to also as AX WiFi
* Greater speeds and stability
* Up to 14 Gbps

## Wireless Frequencies and Ranges

**WiFi Frequencies**

### **2.4 GHz**

**Speed**

* Maximum speed of 450 to 600 Mbps

**Range**

* 150 feet indoors and 300 feet outdoors

**Considerations**

**Pros**

* Larger coverage area
* Better penetrating objects
  * Concrete
    * Wood

**Cons**

* Lower data rates
* Prone to interference
* Can become overcrowded

### **5 GHz**

**Speed**

* Maximum speed of 1300 Mbps

**Channels**

* Multiple non-overlapping channels

**Benefits**

* Higher speeds
* Clearer signal
* Not as susceptible to interference

**Disadvantages**

* Shorter range
* Compatibility

## Common Wi-Fi Channels

### WiFi Channels

* 2.4 GHz = 11 WiFi channels
* 5 GHz = 45 WiFi channels

### Channel Designations

#### WiFi Channels

* USA = channels 1-11
* Europe = channels 1-13
* Japan = 1-14

<figure><img src="../../.gitbook/assets/wifi (1).jpg" alt=""><figcaption></figcaption></figure>

* Each channel spans a range of 22 MHz on the entire spectrum

#### Channel Width

Channel width affects these values:

* Speed
* Volume of data

#### Channel Configuration

* Automatic
* Manual

## Wireless Channel Bonding

### Channel Bonding

* Common in IEEE 802.11
* Used to combine different channels
* Increases throughput

<figure><img src="../../.gitbook/assets/channel.jpg" alt=""><figcaption></figcaption></figure>

#### Channel Bonding Popularity

* Introduced with 802.11n
* Provides additional functionality and increased throughput

#### 2.4 GHz Frequency Band

**3 non-overlapping channels**

* Total width of approximately 70 MHz (channels 1 through 11)
* Only a single bounded pair of 40 MHz can be configured (channels 1 and 6)
* Only a single non-overlapping channels would remain (channel 11)

#### 5 GHz Frequency Band

**25 non-overlapping channels**

* Total width of over 500 MHz
* Many more bonded pairs can be configures
  * Up to 160 MHz in 802.11 ac
  * Very high throughput

## Service Set Identifier (SSID)

* Used to uniquely name a wireless local area network (WLAN)

#### Basic Service Set (BSS)

* Used to form one logical WLAN segment

#### Extended Service Set (ESS)

* One or more interconnected Basic Service Sets (BSS)
  * One Access Point
  * One Station

#### WiFi Roaming

<figure><img src="../../.gitbook/assets/wifi_2.jpg" alt=""><figcaption></figcaption></figure>

#### Independent Basic Service Set (Ad Hoc)

* Simplest IEEE 802.11 network

#### Difference between Infrastructure mode and Ad Hoc mode:

**Infrastructure mode:**

* Much more common
* Wireless router that provides connectivity to all devices and also provides you access to the Internet
* All of the devices, when communicating go through that wireless router

**Ad-Hoc mode:**

* Allows do both
* Devices can go through the central router, but they are also allowed to set up direct connections with each other

## Wireless Antenna Types

#### Antennas

* Used to transmit or receive radio
* Converts electric power into radio waves
* Can be tiny in size to very large structures

#### Omni-directional Antennas

* Transmit and receive with equal efficiency in all directions
* Signals emanate in a sphere
* Examples include radio transmission towers, cell phone antennas, Wi-Fi routers

**Advantages:**

* Easy to install
* Mounted virtually anywhere and in any direction

**Disadvantages**

* Typically have a shorter range due to the signal being spread so broadly
* Inefficient

#### Directional Antennas

* Designed to have a narrow directional signal
  * By design, these types of antennas work more effectively in some directions compared to others

**Advantages:**

* Improved transmission
* Improved reception of communications
* Reduced interference

**Disadvantages:**

* Decreased effective beam width

#### Directional Antenna Types

* Semi-directional - represent half of the circle
* Bi-directional - 45 degree front and also behind me

#### Yagi-Uda Antennas

* Arrangemenets of perpendicular and parallel elements
* Highly directional antenna
* Used for fixed point-to-point systems

#### Parabolic Dish Antennas

* Use a parabola to focus incoming signals to a point
* Common in satellite communications and other long-range, directional applications

## Wireless Encryption Solutions (WEP)

* Older encryption algorithm
* Secures data across a wireless network
* WEP key
  * Sequence of hexadecimal characters
  * Characters must match on all devices communicating on a wireless network

**Advantages:**

* Interoperability
* Useful when connecting older devices

**Disadvantages:**

* Can be cracked
* Changing the key can be tedious

#### Wi-Fi Protected Access (WPA)

* Developed by Wi-Fi Alliance
  * Designed to replace WEP
  * Adopted in 2003
* Stronger encryption
* Data integrity
  * Verify data has not been tampered with or altered

**Advantages:**

* Stronger encryption than WEP
* Uses Temporal Key Integrity Protocol (TKIP)
* Dynamic key changes if necessary

**Disadvantages:**

* Proven to be incompatible with some legacy hardware or older operating systems

#### Wi-Fi Protected Access II (WPA2)

* Provides stronger data protection
* Provides network access control
* Ensures only authorized users can access a wireless network
* Provides government grade security
  * AES encryption algorithm
  * 802.1 x-based authentication
* Editions
  * WPA2-Personal
    * Requires a password
  * WPA2-Enterprise
    * Verifes users through a server

**WPA2 Benefits**

* Compatibility
  * However, older equipment may not support it
* Security
  * More advanced encryption
* TKIP for interoperability with WPA
* Very difficult to crack without network access

#### Temporal Key Integrity Protocol (TKIP)

* Encryption protocol used for wireless LANs
* Improves upon WEP
  * Original WLAN security protocol
* Provides more secure encryption
  * Encryption method in WPA

#### TKIP-RC4

* Suite of algorithms that allows legacy WLAN equipment to upgrade to TKIP
  * Without replacing any hardware
* Uses WEP programming
  * Additional code is "wrapped" at both the beginning and end to modify and encapsulate it
* RC4 stream encryption is used as its basis
* Data packets are encrypted with a unique encryption key
* TKIP uses four algorithms to increase key strength

#### TKIP-RCE4/AES-CCMP

* Does not address all security issues for WLANs
  * May not be efficient enough for certain data transmissions
    * Government
    * Sensitive corporate
* AES-CCMP
  * Higher level of security
    * Approved for government use
    * May require hardware upgrades

## Common Cellular Technologies

#### GSM

* Global System for Mobile communication (GSM)
* Digital mobile telephony system
* Represents over 90% of all global mobile connections
* Operates at one of two frequencies:
  * 900 MHz
  * 1800 MHz
* Digitizes and compresses data prior to sending down a channel

#### TDMA

* Time Division Multiple Access (TDMA)
* Facilitates multiple users sharing the same media
* Cellular channels are divided into three time slots
* Used by
  * Global System for Mobile Communications (GSM)
  * Digital-Advanced Mobile Phone Service (D-AMPS)
  * Personal Digital Cellular (PDC)

#### CDMA

* Code Division Multiple Access (CDMA)
* Used in second-generation (2G) and third-generation (3G) wireless communications
* Form of multiplexing
* Allows numerous signals on a single transmission channel
* Commonly used 800 MHz and 1.9 GHz

#### LTE (4G)

* Long-term Evolution
* Uses Orthogonal frequency-division multiple access (OFDMA)
* Uses frequency ranges to create separate channels

#### 5G

* Still being developed
* Gbps speeds
* Lower latency (near real-time)
* Perform remote operations
* Specific device support

## MU-MIMO Technology

* Multiple input, multiple output (MIMO)
* Antenna technology for wireless communications
* Sends multiple signals at once and uses an array of antennas
* Antennas at each end of the circuit are combined to help
  * Minimize errors
  * Optimize data speed
* Support
  * 802.11 n
  * 802.11 ac
* Single-session
  * Supports multiple devices in separate sessions
    * Each device must take turns

#### MU-MIMO

* Multi-user multiple input multiple-output (MU-MIMO)
* Enhanced form of MIMO technology
* Simultaneous communication with multiple devices
* Significant performance enhancement
* Devices no longer have to wait for their turn
* 802.11 ac wireless specification
* Increased theoretical maximum wireless speeds ranging from 3.47 Gbps to 6.93 Gbps

## Test

A voice VLAN is typically implemented for which purpose?

* To give voice packets a higher priority than data packets

Which encryption standard can provide managed access through a centralized server?

* WPA2

Which protocol or port configuration option on a switch is typically used for monitoring and diagnostic purposes?

* Port mirroring

Which benefits did the 2.4 GHz frequency offer over 5 GHz?

* Better penetration of obstacles
* Better coverage

Which scenario would most accurately reflect the nature of MU-MIMO in wireless communications?

* Many people on a conference call

Power over Ethernet plus (PoE+) is capable of handling what level of power?

* 30 watts

In the event of a collision on an ethernet network, CSMA/CD specifies that which process or procedure take place?

* Transmitting and receiving devices should retransmit at random intervals

In the 2.4 GHz frequency band, how many bonded pairs could be configured within the entire range?

* 1

Which type of multiple access method is used by LTE (4G)?

* OFDMA

In the 2.4 GHz frequency band, which channels would not overlap with each other?

* 1 and 6
* 6 and 11

The spanning tree protocol addresses which potential issue in a networking environment?

* Switching or bridging loops

VLANs are created and configured in which manner?

* By configuring switch port interfaces

What is the primary characteristic of 802.11 communications that determines if one variety is compatible with another?

* Frequency

Which type of antenna could be envisioned as producing a “slice” of coverage in front of you, and a slice of coverage behind you?

* Bi-directional

The SSID of a wireless network would be best described in which manner?

* The collection of all devices connected to all access points

Which type of resolution or mapping is performed by the Address Resolution Protocol?

* IPv4 addresses to MAC addresses

Which statements accurately describe the nature of a MAC address?

* They operate at the Data-link layer of the OSI model
* They never change
* They are written into the code of the interface

The Neighbor Discovery Protocol would be most accurately described in which manner?

* It is the IPv6 equivalent of the Address Resolution Protocol
