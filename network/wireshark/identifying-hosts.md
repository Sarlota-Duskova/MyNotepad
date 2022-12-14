# Identifying Hosts

### DHCP Analysis <a href="#dhcp-analysis" id="dhcp-analysis"></a>

**NotesWireshark Filter**Global search.

* `dhcp` or `bootp`

Filtering the proper DHCP packet options is vital to finding an event of interest.

* **"DHCP Request"** packets contain the hostname information
* **"DHCP ACK"** packets represent the accepted requests
* **"DHCP NAK"** packets represent denied requests

Due to the nature of the protocol, only "Option 53" ( request type) has predefined static values. You should filter the packet type first, and then you can filter the rest of the options by "applying as column" or use the advanced filters like "contains" and "matches".

* Request: `dhcp.option.dhcp == 3`
* ACK: `dhcp.option.dhcp == 5`
* NAK: `dhcp.option.dhcp == 6`

**"DHCP Request"** options for grabbing the low-hanging fruits:

* **Option 12:** Hostname.
* **Option 50:** Requested IP address.
* **Option 51:** Requested IP lease time.
* **Option 61:** Client's MAC address.
* `dhcp.option.hostname contains "keyword"`

**"DHCP ACK"** options for grabbing the low-hanging fruits:

* **Option 15:** Domain name.
* **Option 51:** Assigned IP lease time.
* `dhcp.option.domain_name contains "keyword"`

**"DHCP NAK"** options for grabbing the low-hanging fruits:

* **Option 56:** Message (rejection details/reason).

As the message could be unique according to the case/situation, It is suggested to read the message instead of filtering it. Thus, the analyst could create a more reliable hypothesis/result by understanding the event circumstances.

### NetBIOS (NBNS) Analysis <a href="#netbios-nbns-analysis" id="netbios-nbns-analysis"></a>

**NetBIOS** or **Net**work **B**asic **I**nput/**O**utput **S**ystem is the technology responsible for allowing applications on different hosts to communicate with each other.NotesWireshark FilterGlobal search.nbns"NBNS" options for grabbing the low-hanging fruits:Queries: Query details.Query details could contain "name, Time to live (TTL) and IP address details"nbns.name contains "keyword"​Kerberos Analysis​\
