# Physical Security & Network Hardening

## Network Hardening Techniques

### SNMP

* SNMPv1 is inherently insecure, with passwords being passed in plaintext
  * For general monitoring network environment
* SNMPv2 is better, but still has issues
* SNMPv3 was designed explicitly to tackle security issues

### Router Advertisement Guard

* Used to filter router advertisements

### Dynamic ARP Inspection

* Performs validation of Address Resolution Protocol (ARP) packets

### Port Security

* Disable access to unused physical ports
  * Conference rooms
  * Break rooms

### Control Plane Policing

* Protects against denial of service (DoS) and reconnaissance attacks

### Private VLANs

* Primary
* Community
* Isolated

### Default VLAN

* Avoid using default VLAN for network data

### System Services

* Most operating systems contain more enabled services than required by default
* Poses a potential security vulnerability
* Disable all unnecessary services

### DHCP Snooping

<figure><img src="../../.gitbook/assets/dhcp.jpg" alt=""><figcaption></figcaption></figure>

* DHCP snooping can be enabled on switches also like Router Advertisement Guard to prevent clients from accepting DHCP offers from any servers other than those that are authorized

### Patching

* Vulnerabilities are discovered over time
* Patching fixes security and stability problems
* Monitor patch deployment
* Monitor compliance
* Inject patches to OS images
* Ongoing tasks

### Access Control Lists

* Permit
* Deny

## Credentials and Strong Passwords

### Passwords

* Have been proven to be one of the main security vulnerabilities
* People often use simple passwords

### Rules

**Pros:**

* Use combination of characters (uppercase, lowercase and special characters)
* Use longer passwords
* Update passwords on a regular basis
* Use different passwords for different accounts
* Use Multifactor Authentication
* Use password management tools

**Cons:**

* Avoid using personal information (nothing that relates to your family)
* Avoid easily recognizable numbers (address, phone number)
* Avoid using real words
* Avoid writting down password
* Do not save passwords in the browser&#x20;

## Disabling Unused Ports

* Unused ports that are left open can present a security vulnerability
  * Network-based attack
* Ports can be blocked using a firewall
  * Network-based
  * Host-based
    * Windows Firewall

### Windows Firewall

* Used to manage the way your computer communicates on the network
  * Inbound rules
  * Outbound rules
  * Connection security rules
  * Monitoring

### Disabling Unused Ports

* Unused router or switch ports
  * Disable to prevent users from accessing the network (prevent someone from connecting a laptop to any open RJ45 jack on the premises)

### Device Ports - Physical

* Many routers offer the capability to manage physical ports on the device
* Good practice to disable these ports to prevent a rogue user plugging directly into the router device
  * Prevent network access

### Device Ports - Virtual

* Used in TCP and UDP
  * Identify unique end-to-end connections
* Port numbers
  * Each side of connection has its own port number
    * Does not change

## Common Firewall Rules

### Firewall Rule Actions

* Allow
* Deny
* Bypass
* Force Allow
* Log Only

### Firewall Rules Format

* Port
* Source
* Destination
* Protocol
* Permission

### Allow Rules

* Permit/Allow
* Implicitly deny (default position) anything that is not specifically trusted will be blocked

### Firewall Configuration

* Implicit (default actions) - to mistrust any type of traffic that is not explicitly allowed
* Explicit - anything that is explicitly defined will override anything that is implicitly there already

## WPA and WPA2 Wireless Security

### Wired Equivalent Privacy (WEP)

* Older encryption algorithm
* Secures data across a wireless network
* WEP key
  * "Password" for the network
  * Must match on all devices communicating on a wireless network

**Advantages:**

* Interoperability
  * Useful when connecting older devices

**Disadvantages:**

* Can be cracked
* Changing the master key can be tedious

### Wi-Fi Protected Access (WPA)

* Security enhancement over WEP

**Advantages:**

* Stronger encryption than WEP
* Uses Temporal Key Integrity Protocol (TKIP)
* Dynamic key changes if necessary

**Disadvantages:**

* Incompatible with some legacy hardware or older operating systems

### Wi-Fi Protected Access 2 (WPA2)

* Signigicantly more secure than WPA
* Uses Advanced Encryption Standard (AES) for encryption
* Two edition:
  * Personal
  * Enterprise

**Benefits:**

* Compatibility
  * However, older equipment may not support it
* Security
  * More advanced encryption (AES)
* TKIP for interoperability with WPA
* Virtually impossible to crack without network access

## TKIP-RC4 and AES-CCMP Wireless Security





## Wireless Authentication and Authorization





## Geofencing Technology



## Wireless Security Considerations



## IoT Security Considerations



## Virtual Private Networks



## Remote Desktop Protocol





## Secure Shell



## Virtual Network Computing



## Remote Authentication and Authorization





## Out-of-Band Management





## Motion Detection and Video Surveillance





## Asset Tracking and Disposal







## Tamper Detection





## Prevention Techniques





## Test
