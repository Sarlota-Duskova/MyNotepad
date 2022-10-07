# Nmap Advanced Port Scans



|         Port Scan Type         |                    Example Command                   |
| :----------------------------: | :--------------------------------------------------: |
|          TCP Null Scan         |               sudo nmap -sN MACHINE\_IP              |
|          TCP FIN Scan          |               sudo nmap -sF MACHINE\_IP              |
|          TCP Xmas Scan         |               sudo nmap -sX MACHINE\_IP              |
|         TCP Maimon Scan        |               sudo nmap -sM MACHINE\_IP              |
|          TCP ACK Scan          |               sudo nmap -sA MACHINE\_IP              |
|         TCP Window Scan        |               sudo nmap -sW MACHINE\_IP              |
|         Custom TCP Scan        | sudo nmap --scanflags URGACKPSHRSTSYNFIN MACHINE\_IP |
|        Spoofed Source IP       |         sudo nmap -S SPOOFED\_IP MACHINE\_IP         |
|       Spoofed MAC Address      |               --spoof-mac SPOOFED\_MAC               |
|           Decoy Scan           |           nmap -D DECOY\_IP,ME MACHINE\_IP           |
|       Idle (Zombie) Scan       |         sudo nmap -sI ZOMBIE\_IP MACHINE\_IP         |
|  Fragment IP data into 8 bytes |                          -f                          |
| Fragment IP data into 16 bytes |                          -ff                         |

|          Option         |                  Purpose                 |
| :---------------------: | :--------------------------------------: |
| --source-port PORT\_NUM |        specify source port number        |
|    --data-length NUM    | append random data to reach given length |

|  Option  |                Purpose                |
| :------: | :-----------------------------------: |
| --reason | explains how Nmap made its conclusion |
|    -v    |                verbose                |
|    -vv   |              very verbose             |
|    -d    |               debugging               |
|    -dd   |       more details for debugging      |

## TCP Null, FIN, Xmas scan

* Using a flag combination that does not match the SYN packet makes it possible to deceive the firewall and reach the system behind it.
* Stateful firewall will practically block all such crafted packets and render this kind of scan useless.
* **Run as SUDO**

### Null Scan

* All six flag bits are set to zero.
* Using the `-sN` option.
* A lack of reply indicates that the port is open or a firewall is blocking the packet.
* Respond with an RST packet if the port is closed.

### FIN Scan

* The FIN scan sends a TCP packet with the FIN flag set.
* Using the `-sF` option.
* No response will be sent if the TCP port is open.
* Respond with an RST if the port is closed.

### Xmas Scan

* An Xmas scan sets the FIN, PSH, and URG flags simultaneously.
* Using the option `-sX`.
* Respond with an RST if the port is closed.

### Maimon Scan

* The FIN and ACK bits are set.
* The target should send an RST packet as a response.
* Using the `-sM` option.&#x20;

## TCP ACK, Window and Custom Scan

### ACK Scan

* An ACK scan will send a TCP packet with the ACK flag set.
* Using the `-sA` option.
* The target would respond to the ACK with RST.
* TCP packet with the ACK flag set should be sent only in response to a received TCP packet to acknowledge the receipt of some data.
* Would be helpful if there is a **firewall in front of the target**.
* This type of scan is more suitable to **discover firewall rule sets and configuration**.

### Window Scan

* The TCP window scan is almost the same as the ACK scan.
* It examines the TCP Window field of the RST packets returned.
* Using the `-sW` option.
* TCP window scan against a Linux system with no firewall will not provide much information.

### Custom Scan

Set SYN, RST, and FIN simultaneously `--scanflags RSTSYNFIN`

### Spoofing and Decoys

**In brief, scanning with a spoofed IP address is three steps:**

1. Attacker sends a packet with a spoofed source IP address to the target machine.
2. Target machine replies to the spoofed IP address as the destination.
3. Attacker captures the replies to figure out open ports.

`nmap -e NET_INTERFACE -Pn -S SPOOFED_IP 10.10.249.175`

* Specify the network interface using `-e`.
* Disable ping scan `-Pn`.
* The source MAC address using `--spoof-mac SPOOFED_MAC`.
* This address spoofing is only possible if the attacker and the target machine are on the same Ethernet (802.3) network or same WiFi (802.11).

#### Decoy scan

`nmap -D 10.10.0.1,10.10.0.2,ME,RND 10.10.249.175`

* Scan of 10.10.249.175 appear as coming from the IP addresses 10.10.0.1, 10.10.0.2, and then ME (my IP address), RND is assigned randomly

## Fragmented Packets

### Firewall

* A firewall is a piece of software or hardware that permits packets to pass through or blocks them.

### IDS (Intrusion Detection System )

* Inspects network packets for select behavioural patterns or specific content signatures.
* It raises an alert whenever a malicious rule is met.

### Fragmented Packets

* The option `-f` to fragment packets.
* The IP data will be divided into 8 bytes or less.
* Adding another -f (-f -f or -ff) will split the data into 16 byte-fragments instead of 8. -The default value can be change by using the `--mtu`.
* `-ff` (or `-f -f`), the fragmentation of the data will be multiples of 16.
* In other words, the 24 bytes of the TCP header, in this case, would be divided over two IP fragments, the first containing 16 bytes and the second containing 8 bytes of the TCP header.

### Idle/Zombie Scan

* Nmap will make each probe appear as if coming from the idle (zombie) host, then it will check for indicators whether the idle (zombie) host received any response to the spoofed probe.
* This is accomplished by checking the IP identification (IP ID) value in the IP header.
* You can run an idle scan using `nmap -sI ZOMBIE_IP 10.10.249.175`, where `ZOMBIE_IP` is the IP address of the idle host (zombie).

The idle (zombie) scan requires the following three steps to discover whether a port is open:

1. Trigger the idle host to respond so that you can record the current IP ID on the idle host.
2. Send a SYN packet to a TCP port on the target. The packet should be spoofed to appear as if it was coming from the idle host (zombie) IP address.
3. Trigger the idle machine again to respond so that you can compare the new IP ID with the one received earlier.

## Getting more details

* The `--reason` flag gives us the explicit reason why Nmap concluded that the system is up or a particular port is open.
* Using `-v` for verbose output or `-vv` for even more verbosity.
* `-d` for debugging details or `-dd` for even more details.
