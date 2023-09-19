# TCP/IP (Transmission Control Protocol)

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

### three-way handshake

* When you attempt to make a connection, your computer first sends a special request to the remote server indicating that it wants to initialise a connection.
* This request contains something called a SYN (short for synchronise) bit, which essentially makes first contact in starting the connection process.
* The server will then respond with a packet containing the SYN bit, as well as another "acknowledgement" bit, called ACK.
* Finally, your computer will send a packet that contains the ACK bit by itself, confirming that the connection has been setup successfully.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

* The first thing that your computer does is check its local cache to see if it's already got an IP address stored for the website.
* Assuming the address hasn't already been found, your computer will then send a request to what's known as a recursive DNS server.
* These will automatically be known to the router on your network.

Top-Level Domain (TLD) servers are split up into extensions. So, for example, if you were searching for tryhackme.com your request would be redirected to a TLD server that handled .com domains.

Computer have 65535 ports and 1024 are well known.

When is port closed TCP send RST flag (reset).

When a packet is sent to a closed UDP port, the target should respond with an ICMP (Internet Control Message Protocol) (ping) packet containing a message that the port is unreachable.

NULL, FIN and Xmas scans generally used because of firewall evasion.

### Establishing Sequence Numbers

* Each TCP connection requires two sets of sequence numbers
  * One sequence number for messages from the client to the server
  * One sequence number for messages from the server to the client
* Before starting a TCP connection, the client and server must agree on two **initial sequence numbers (ISNs)**
  * The ISNs are different and random for every connection

<figure><img src="../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Sending and Receiving Data

The first byte is byte i = 1, since sequence number x was used for the SYN packet and y for the SYN-ACK packet

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

#### Retransmission

* If a packet is dropped (lost in transit):
  * The recipient will not send an ACK, so the sender will not receive the ACK
  * The sender repeatedly tries to send the packet again until it receives the ACK
* If a packet is received, but the ACK is dropped:
  * The sender tries to send the packet again since it didn’t receive the ACK
  * The recipient ignores the duplicate data and sends the ACK again

#### Ending/Aborting a Connection

* To end a connection, one side sends a packet with the FIN (finish) flag set, which should then be acknowledged
  * This means “I will no longer be sending any more packets, but I will continue to receive packets”
  * Once the other side is no longer sending packets, it sends a packet with the FIN flag set
* To abort a connection, one side sends a packet with the RST (reset) flag set
  * This means “I will no longer be sending nor receiving packets on this connection”
  * RST packets are not acknowledged since they usually mean that something went wrong

### TCP Flags

**ACK**

* Indicator that the user is acknowledging the receipt of something (in the ack number)
* Pretty much always set except the very first packet **SYN**
* Indicator of the beginning of the connection **FIN**
* One way to end the connection
* Requires an acknowledgement
* No longer sending packets, but will continue to receive **RST**
* One way to end a connection
* Does not require an acknowledgement
* No longer sending or receiving packets
