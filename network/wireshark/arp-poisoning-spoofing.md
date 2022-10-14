# ARP Poisoning/Spoofing

A.K.A. Man In The Middle Attack

| **Notes**                                       | **Wireshark filter**                                                     |
| ----------------------------------------------- | ------------------------------------------------------------------------ |
| Global search                                   | `arp`                                                                    |
| Opcode 1: ARP requests.                         | `arp.opcode == 1`                                                        |
| Opcode 2: ARP responses.                        | `arp.opcode == 2`                                                        |
| **Hunt:** Arp scanning                          | `arp.dst.hw_mac==00:00:00:00:00:00`                                      |
| **Hunt:** Possible ARP poisoning detection      | `arp.duplicate-address-detected or arp.duplicate-address-frame`          |
| **Hunt:** Possible ARP flooding from detection: | `((arp) && (arp.opcode == 1)) && (arp.src.hw_mac == target-mac-address)` |

