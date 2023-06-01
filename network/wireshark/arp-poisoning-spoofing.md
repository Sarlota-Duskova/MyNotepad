# ARP Poisoning/Spoofing

A.K.A. Man In The Middle Attack

<table data-header-hidden><thead><tr><th width="258.5"></th><th></th></tr></thead><tbody><tr><td><strong>Notes</strong></td><td><strong>Wireshark filter</strong></td></tr><tr><td>Global search</td><td><code>arp</code></td></tr><tr><td>Opcode 1: ARP requests.</td><td><code>arp.opcode == 1</code></td></tr><tr><td>Opcode 2: ARP responses.</td><td><code>arp.opcode == 2</code></td></tr><tr><td><strong>Hunt:</strong> Arp scanning</td><td><code>arp.dst.hw_mac==00:00:00:00:00:00</code></td></tr><tr><td><strong>Hunt:</strong> Possible ARP poisoning detection</td><td><code>arp.duplicate-address-detected or arp.duplicate-address-frame</code></td></tr><tr><td><strong>Hunt:</strong> Possible ARP flooding from detection:</td><td><code>((arp) &#x26;&#x26; (arp.opcode == 1)) &#x26;&#x26; (arp.src.hw_mac == target-mac-address)</code></td></tr></tbody></table>

