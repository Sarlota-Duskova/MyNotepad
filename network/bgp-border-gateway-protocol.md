# BGP (Border Gateway Protocol)

* Once your system sends the packet to the gateway, the packet has to be routed through the Internet
* The Internet is a network of networks, comprised of many autonomous systems (AS)
  * Each AS handles its own internal routing
  * Each AS is uniquely identified by its autonomous system number (ASN)
  * Each AS is comprised of one or more LANs
  * The AS can forward packet to other connected ASes
* The protocol for communicating between different Autonomous Systems is Border Gateway Protocol (BGP) Each router announces what networks it can provide and the path onward from the router The most precise route with the shortest path and no loops is the preferred route
* The Internet is made of smaller autonomous systems (AS)
* Each AS broadcasts the shortest routes it knows of (dependent on the shortest routes of its neighbors and distance to neighbors)
