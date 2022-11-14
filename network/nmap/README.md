# NMAP

`nmap -sC -sV -oN 10.10.120.4`

`-sC` = equivalent to --script=default

`-sV` = Probe open ports to determine service/version info

`-oN` = Output scan in normal, XML, s|\<rIpt kIddi3



Using version scan to detect the OS:

`nmap -O -v 10.10.120.4`

or:

`nmap -A 10.10.120.4`
