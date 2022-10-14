# Nmap Scans

### Nmap Scans

| **Notes**                                                                                                       | **Wireshark Filters**                                                                                                        |
| --------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Global search.                                                                                                  | <ul><li><code>tcp</code></li></ul><ul><li><code>udp</code></li></ul>                                                         |
| <ul><li>Only SYN flag.</li><li>SYN flag is set. The rest of the bits are not important.</li></ul>               | <ul><li><code>tcp.flags == 2</code></li></ul><ul><li><code>tcp.flags.syn == 1</code></li></ul>                               |
| <ul><li>Only ACK flag.</li><li>ACK flag is set. The rest of the bits are not important.<br></li></ul>           | <ul><li><code>tcp.flags == 16</code></li></ul><ul><li><code>tcp.flags.ack == 1</code></li></ul>                              |
| <ul><li>Only SYN, ACK flags.</li><li>SYN and ACK are set. The rest of the bits are not important.</li></ul>     | <ul><li><code>tcp.flags == 18</code></li></ul><ul><li><code>(tcp.flags.syn == 1) and (tcp.flags.ack == 1)</code></li></ul>   |
| <ul><li>Only RST flag.</li><li>RST flag is set. The rest of the bits are not important.<br></li></ul>           | <p><br></p><ul><li><code>tcp.flags == 4</code></li></ul><ul><li><code>tcp.flags.reset == 1</code></li></ul>                  |
| <ul><li>Only RST, ACK flags.</li><li>RST and ACK are set. The rest of the bits are not important.<br></li></ul> | <ul><li><code>tcp.flags == 20</code></li></ul><ul><li><code>(tcp.flags.reset == 1) and (tcp.flags.ack == 1)</code></li></ul> |
| <ul><li>Only FIN flag</li><li>FIN flag is set. The rest of the bits are not important.</li></ul>                | <ul><li><code>tcp.flags == 1</code></li></ul><ul><li><code>tcp.flags.fin == 1</code></li></ul>                               |

### TCP Connect Scans

* Usually conducted with `nmap -sT` command.

The given filter shows the TCP Connect scan patterns in a capture file.

`tcp.flags.syn==1 and tcp.flags.ack==0 and tcp.window_size > 1024`

### TCP SYN Scan

* Usually conducted with `nmap -sS` command.

The given filter shows the TCP SYN scan patterns in a capture file.

`tcp.flags.syn==1 and tcp.flags.ack==0 and tcp.window_size <= 1024`

### UDP Scans

* Usually conducted with `nmap -sU` command.

`icmp.type==3 and icmp.code==3`
