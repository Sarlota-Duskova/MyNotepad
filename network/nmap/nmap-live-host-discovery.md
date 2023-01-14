# Nmap Live Host Discovery

**Discover live hosts:**

* **ARP scan:** This scan uses ARP requests to discover live hosts
* **ICMP scan:** This scan uses ICMP requests to identify live hosts
* **TCP/UDP ping scan:** This scan sends packets to TCP ports and UDP ports to determine live hosts.
* Add `-sn` if you are only interested in host discovery without port-scanning.

### Nmap Host Discovery Using ARP

1. When a privileged user tries to scan targets on a local network (Ethernet), Nmap uses ARP requests. A privileged user is `root` or a user who belongs to `sudoers` and can run `sudo`.
2. When a privileged user tries to scan targets outside the local network, Nmap uses ICMP echo requests, TCP ACK (Acknowledge) to port 80, TCP SYN (Synchronize) to port 443, and ICMP timestamp request.
3. When an unprivileged user tries to scan targets outside the local network, Nmap resorts to a TCP 3-way handshake by sending SYN packets to ports 80 and 443.

* The ARP query only works if the target is on the same subnet as yourself, i.e., on the same Ethernet/WiFi.

**Nmap using ARP for host discovery without any port scanning:** `nmap -PR -sn MACHINE_IP/24`

### Nmap Host Discovery Using ICMP

* (ICMP Type 8/Echo) requests
* (ICMP Type 0) ping reply
* To use ICMP echo request to discover live hosts, add the option `-PE`.
* The `-PP` option tells Nmap to use ICMP timestamp requests.
* ICMP address mask requests `-PM`.

### Nmap Host Discovery Using TCP and UDP

#### TCP SYN Ping

* We can send a packet with the SYN (Synchronize) flag set to a TCP port, 80 by default, and wait for a response.
* An open port should reply with a SYN/ACK (Acknowledge).
* A closed port would result in an RST (Reset).
* `PS21-25` will target ports 21, 22, 23, 24, and 25.

#### TCP ACK Ping

* Must be running Nmap as a privileged user to be able to accomplish this.
* An unprivileged user, Nmap will attempt a 3-way handshake.
* `-PA`

#### UDP Ping

* If we send a UDP packet to a closed UDP port, we expect to get an ICMP port unreachable packet; this indicates that the target system is up and available.
* `-PU` for UDP ping.

#### Masscan

* `-p` can be followed by a port number, list, or range.

#### Reverse-DNS Lookup

* A specific DNS server `-dns-servers DNS_SERVER`
* The option `-R` to query the DNS server even for offline hosts.

| Option |              Purpose             |
| :----: | :------------------------------: |
|   -n   |           no DNS lookup          |
|   -R   | reverse-DNS lookup for all hosts |
|   -sn  |        host discovery only       |



The Nmap option `-sn` disables port scanning, leaving the discovery phase enabled, which makes Nmap perform a **ping sweep**. Depending on the privileges, Nmap by default uses different techniques to achieve this task: sending a `TCP SYN` packet to port `443`, `TCP ACK` packet to port `80` and ICMP echo and timestamp requests if executed as a privileged user, or a `SYN` packets to port `80` and `443` via the `connect() syscall` if executed by users who can't send raw packets. **ARP/Neighbor Discovery** is also enabled when scanning local Ethernet networks as privileged users. MAC addresses and vendors are identified from the ARP requests sent during the ARP/Neighbor Discovery phase.
