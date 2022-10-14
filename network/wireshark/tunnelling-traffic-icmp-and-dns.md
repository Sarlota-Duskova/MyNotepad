# Tunnelling Traffic: ICMP and DNS

### ICMP Analysis

| **Notes**                                                                                                                                                                               | **Wireshark filters**                                 |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
| Global search                                                                                                                                                                           | <ul><li><code>icmp</code></li></ul>                   |
| <p>"ICMP" options for grabbing the low-hanging fruits:</p><ul><li>Packet length.</li><li>ICMP destination addresses.<br></li><li>Encapsulated protocol signs in ICMP payload.</li></ul> | <ul><li><code>data.len > 64 and icmp</code></li></ul> |

### DNS Analysis



| **Notes**                                                                                                                                                                                                                                                                                                                                                                                                                        | **Wireshark Filter**                                                                                               |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Global search                                                                                                                                                                                                                                                                                                                                                                                                                    | <ul><li><code>dns</code></li></ul>                                                                                 |
| <p>"DNS" options for grabbing the low-hanging fruits:</p><ul><li>Query length.</li><li>Anomalous and non-regular names in DNS addresses.</li><li>Long DNS addresses with encoded subdomain addresses.</li><li>Known patterns like dnscat and dns2tcp.</li><li>Statistical analysis like the anomalous volume of DNS requests for a particular target.</li></ul><p><strong>!mdns:</strong> Disable local link device queries.</p> | <ul><li><code>dns contains "dnscat"</code></li></ul><ul><li><code>dns.qry.name.len > 15 and !mdns</code></li></ul> |

###
