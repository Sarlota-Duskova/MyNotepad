# Nmap Basic Port Scans

|  Port Scan Type  |      Example Command      |
| :--------------: | :-----------------------: |
| TCP Connect Scan |    nmap -sT MACHINE\_IP   |
|   TCP SYN Scan   | sudo nmap -sS MACHINE\_IP |
|   UDP Scan sudo  |    nmap -sU MACHINE\_IP   |

|         Option        |                  Purpose                 |
| :-------------------: | :--------------------------------------: |
|          -p-          |                 all ports                |
|        -p1-1023       |           scan ports 1 to 1023           |
|           -F          |           100 most common ports          |
|           -r          |      scan ports in consecutive order     |
|        -T<0-5>        | -T0 being the slowest and T5 the fastest |
|     --max-rate 50     |          rate <= 50 packets/sec          |
|     --min-rate 15     |          rate >= 15 packets/sec          |
| --min-parallelism 100 |      at least 100 probes in parallel     |

#### Nmap considers the following six states:

**1. Open:** indicates that a service is listening on the specified port.

**2. Closed:** indicates that no service is listening on the specified port, although the port is accessible. By accessible, we mean that it is reachable and is not blocked by a firewall or other security appliances/programs.

**3. Filtered:** means that Nmap cannot determine if the port is open or closed because the port is not accessible. This state is usually due to a firewall preventing Nmap from reaching that port. Nmap’s packets may be blocked from reaching the port; alternatively, the responses are blocked from reaching Nmap’s host.

**4. Unfiltered:** means that Nmap cannot determine if the port is open or closed, although the port is accessible. This state is encountered when using an ACK scan -sA.

**5. Open|Filtered:** This means that Nmap cannot determine whether the port is open or filtered.

**6. Closed|Filtered:** This means that Nmap cannot decide whether a port is closed or filtered.

### TCP connect port scan

* The TCP header is the first 24 bytes of a TCP segment.

**The TCP header flags are:** **URG:** Urgent flag indicates that the urgent pointer filed is significant. The urgent pointer indicates that the incoming data is urgent, and that a TCP segment with the URG flag set is processed immediately without consideration of having to wait on previously sent TCP segments. **ACK:** Acknowledgement flag indicates that the acknowledgement number is significant. It is used to acknowledge the receipt of a TCP segment.

**PSH:** Push flag asking TCP to pass the data to the application promptly.

**RST:** Reset flag is used to reset the connection. Another device, such as a firewall, might send it to tear a TCP connection. This flag is also used when data is sent to a host and there is no service on the receiving end to answer.

**SYN:** Synchronize flag is used to initiate a TCP 3-way handshake and synchronize sequence numbers with the other host. The sequence number should be set randomly during TCP connection establishment.

**FIN:** The sender has no more data to send.

* The client sends a TCP packet with SYN flag set.
* The server responds with SYN/ACK if the port is open.
* The client completes the 3-way handshake by sending an ACK.
* Run TCP connect scan using `-sT`.
* If you are not a privileged user (root or sudoer), a TCP connect scan is the only possible option to discover open TCP ports.
* The `-F` option enable fast mode and decrease the number of scanned ports from 1000 to 100 most common ports.
* The `-r` option can also be added to scan the ports in consecutive order instead of random order. This option is useful when testing whether ports open in a consistent manner, for instance, when a target boots up.

### TCP SYN port scan

* SYN scan it **requires a privileged (root or sudoer) user** to run it.
* SYN scan **does not need to complete the TCP 3-way handshake**.
* TCP connect scan `-sT` traffic. Any open TCP port will require Nmap to complete the TCP 3-way handshake before closing the connection.
* `-sS` **does not need to complete the TCP 3-way handshake**; instead, Nmap sends an RST packet once a SYN/ACK packet is received.

### UDP port scan

* If a UDP packet is sent to a closed port, an ICMP port unreachable error (type 3, code 3) is returned.
* UDP scan using the `-sU` option.

### Fine-Tuning Scope

**Port scan:**

* Scan of all ports by using `-p-`, which will scan all 65535 ports.
* Port list `-p22,80,443` will scan ports 22, 80 and 443.
* Port range: `-p1-1023` will scan all ports between 1 and 1023.
* The most common 100 ports use `-F`.
* Using `--top-ports 10` will check the ten most common ports.

**Timing:**

* Control the scan timing using `-T<0-5>`.
* `-T0` is the slowest (paranoid)
* `-T5` is the fastest. **Templates:**
* paranoid (0)
* sneaky (1)
* polite (2)
* normal (3)
* aggressive (4)
* insane (5)

**Intrusion Detection System (IDS)** is a system that detects unauthorised network and system intrusions.

* Examples include detecting unauthorised devices connected to the local network and unauthorised users accessing a system or modifying a file.

**Avoid IDS alerts:**

* `-T0` scans one port at a time and waits 5 minutes between sending each probe.
* If you don’t specify any timing, Nmap uses normal `-T3`.
* `-T5` is the most aggressive in terms of speed; however, this can affect the accuracy of the scan results due to the increased likelihood of packet loss.
* `-T4` is often used during CTFs and when learning to scan on practice targets.
* `-T1` is often used during real engagements where stealth is more important.

**Control the packet rate**

* `--min-rate <number>`
* `--max-rate <number>`

**Control probing parallelization**

* `--min-parallelism <numprobes>`
* `--max-parallelism <numprobes>`
