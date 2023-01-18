# IP Address

### 1.1 IP address, netmask, routing

IPv4 is 32-bit\
IPv6 is 128-bit

**Example:**

IP address is 192.168.1.204\
Subnet mask is 255.255.255.0\
We have every time reserved two addresses:\
\- Network address: 192.168.1.0\
\- Default Gateway: 192.168.1.1 - it will be a router\
\- Broadcast address: 192.168.1.255

**Public IP address:**

Show public address:

`nslookup myip.opendns.com resolver1.opendns.com`

**Private IP address:**

The range of private IPs:

&#x20;class A 10.0.0.0 to 10.255.255.255

&#x20;class B 172.16.0.0 to 172.31.255.255

&#x20;class C 192.168.0.0 to 192.168.255.255



They are mathematically produced and allocated by the Internet Assigned Numbers Authority (IANA), a division of the Internet Corporation for Assigned Names and Numbers (ICANN).

* When you are at home, that network will probably be your Internet Service Provider (ISP). At work, it will be your company network.
* Your IP address is assigned to your device by your ISP.
* Your internet activity goes through the ISP, and they route it back to you, using your IP address. Since they are giving you access to the internet, it is their role to assign an IP address to your device.
* **Static IP addresses** In contrast to dynamic IP addresses, static addresses remain consistent. Once the network assigns an IP address, it remains the same. Most individuals and businesses do not need a static IP address, but for businesses that plan to host their own server, it is crucial to have one.
* **Dynamic IP addresses** Dynamic IP addresses change automatically and regularly. ISPs buy a large pool of IP addresses and assign them automatically to their customers.

**Attacking the network** DDoS attack (distributed denial-of-service).

#### Netmask

Netmask provides the available number range of IP addresses From Class A to Class C, and specifies a mask to divide these networks into sub-networks (subnets).

* 255.0.0.0 for Class A with an 8-bit netmask
* 255.255.0.0 for Class B with a 16-bit netmask
* 255.255.255.0 for Class A with a 24-bit netmask

**Class A**

* **0---** : If the first bit of an IPv4 address is “0”, this means that the address is part of class A. This means that any address from **0.0.0.0** to **127.255.255.255** is in class A.

**Class B**

* **10--** : Class B includes any address from **128.0.0.0** to **191.255.255.255**. This represents the addresses that have a “1” for their first bit, but don’t have a “1” for their second bit.

**Class C** **110-** : Class C is defined as the addresses ranging from **192.0.0.0** to **223.255.255.255**. This represents all of the addresses with a “1” for their first two bits, but without a “1” for their third bit.

**Class D** **1110** : This class includes addresses that have “111” as their first three bits, but a “0” for the next bit. This address range includes addresses from **224.0.0.0** to **239.255.255.255**.

**Class E** **1111** : This class defines addresses between **240.0.0.0** and **255.255.255.255**. Any address that begins with four “1” bits is included in this class.

#### Routing

Network routing is the process of selecting a path across one or more networks. The principles of routing can apply to any type of network, from telephone networks to public transportation. In packet-switching networks, such as the Internet, routing selects the paths for Internet Protocol (IP) packets to travel from their origin to their destination. These Internet routing decisions are made by specialized pieces of network hardware called routers.

**Routing protocols**

* IP (The Internet Protocol)
* BGP (The Border Gateway Protocol)
* OSPF (The Open Shortest Path First)
* RIP (The Routing Information Protocol)

### 1.2 CIDR notations /16,/24,/32

**Classless Inter-Domain Routing**

IP address is made up of four sections called octets

192.168.1.1/24 192.168.1 = network .1 = host /24 = subnet mask

subnet mask 255.255.255.0 is 32-bit 11111111.11111111.11111111.00000000 11111111.11111111.11111111 = network .00000000 = host

Example: 192.168.60.50/20 the suffix "/20" indicates the subnet mask 255.255.240.0

\| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 | 11111111.11111111.11110000.00000000 11110000 this contain | 128 | 64 | 32 | 16 | so it is 128+64+32+16=240 => 255.255.240.0

Network ID: 192.168.48.0 => 48 xxxxxxxx.xxxxxxxx.00111100.xxxxxxxx 11111111.11111111.11110000.00000000 xxxxxxxx.xxxxxxxx.00110000.xxxxxxxx so this 00110000 is 32+16 = 48

Broadcast ID: 192.168.63.255 11111111.11111111.11110000.00000000 the last 1 is for 16 so 48+16-1 = 63

Usable IPs: 192.168.48.1 - 192.168.63.254

### 1.3 Practical part:

#### 1.3.1 For the specified IP range, list all the IP addresses it contains (10.2.32.0/22)

xxxxxxxxx.xxxxxxxxx.00100000.xxxxxxxxx 11111111.11111111.11111100.00000000 xxxxxxxxx.xxxxxxxxx.00100000.xxxxxxxxx

Network ID: 10.2.32.0 Broadcast ID: 10.2.35.255 (32+4-1=35) Usable IPs: 10.2.32.1 - 10.2.35.254

nmap -sn 10.2.32-35.1-254 or nmap -sn 10.2.32.0/22
