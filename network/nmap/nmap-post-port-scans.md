# Nmap Post Port Scans

<table><thead><tr><th width="241.5" align="center">Option</th><th align="center">Meaning</th></tr></thead><tbody><tr><td align="center">-sV</td><td align="center">determine service/version info on open ports</td></tr><tr><td align="center">-sV</td><td align="center">--version-light try the most likely probes (2)</td></tr><tr><td align="center">-sV</td><td align="center">--version-all try all available probes (9)</td></tr><tr><td align="center">-O</td><td align="center">detect OS</td></tr><tr><td align="center">--traceroute</td><td align="center">run traceroute to target</td></tr><tr><td align="center">--script=SCRIPTS</td><td align="center">Nmap scripts to run</td></tr><tr><td align="center">-sC or --script=default</td><td align="center">run default scripts</td></tr><tr><td align="center">-A</td><td align="center">equivalent to -sV -O -sC --traceroute</td></tr><tr><td align="center">-oN</td><td align="center">save output in normal format</td></tr><tr><td align="center">-oG</td><td align="center">save output in grepable format</td></tr><tr><td align="center">-oX</td><td align="center">save output in XML format</td></tr><tr><td align="center">-oA</td><td align="center">save output in normal, XML and Grepable formats</td></tr></tbody></table>

## Service Detection

* `-sV` to your Nmap command will collect and determine service and version information for the open ports.
* Control the intensity with `--version-intensity LEVEL` where the level ranges between 0, the lightest, and 9, the most complete.
  * `-sV --version-light` has an intensity of 2
  * `-sV --version-all` has an intensity of 9.
  * Using `-sV` will force Nmap to proceed with the TCP 3-way handshake and establish the connection.
  * Stealth SYN scan `-sS` is not possible when `-sV` option is chosen.

## OS Detection and Traceroute

### OS Detection

* OS detection can be enabled using `-O`.
* Example: `nmap -sS -O 10.10.75.241`

### Traceroute

* Find the routers between you and the target, use `--traceroute`
* Example: `nmap -sS --traceroute 10.10.75.241`

## NSE (Nmap Scripting Engine)

<table><thead><tr><th width="179.5" align="center">Script Category</th><th align="center">Description</th></tr></thead><tbody><tr><td align="center">auth</td><td align="center">Authentication related scripts</td></tr><tr><td align="center">broadcast</td><td align="center">Discover hosts by sending broadcast messages</td></tr><tr><td align="center">brute</td><td align="center">Performs brute-force password auditing against logins</td></tr><tr><td align="center">default</td><td align="center">Default scripts, same as -sC</td></tr><tr><td align="center">discovery</td><td align="center">Retrieve accessible information, such as database tables and DNS names</td></tr><tr><td align="center">dos</td><td align="center">Detects servers vulnerable to Denial of Service (DoS)</td></tr><tr><td align="center">exploit</td><td align="center">Attempts to exploit various vulnerable services</td></tr><tr><td align="center">external</td><td align="center">Checks using a third-party service, such as Geoplugin and Virustotal</td></tr><tr><td align="center">fuzzer</td><td align="center">Launch fuzzing attacks</td></tr><tr><td align="center">intrusive</td><td align="center">Intrusive scripts such as brute-force attacks and exploitation</td></tr><tr><td align="center">malware</td><td align="center">Scans for backdoors</td></tr><tr><td align="center">safe</td><td align="center">Safe scripts that won’t crash the target</td></tr><tr><td align="center">version</td><td align="center">Retrieve service versions</td></tr><tr><td align="center">vuln</td><td align="center">Checks for vulnerabilities or exploit vulnerable services</td></tr></tbody></table>

\- `sudo nmap -sS -sC 10.10.19.133`, where `-sC` will ensure that Nmap will execute the default scripts following the SYN scan.

* Specify the script by name using `--script "SCRIPT-NAME"`
* `--script "ftp*"` which would include `ftp-brute`

## Saving the output

Whenever you run a Nmap scan, it is only reasonable to save the results in a file:

* Normal
* Grepable (grepable)
* XML

### Normal

* `-oN FILENAME`; N stands for normal.

### Grepable

* Name from the command grep.
* grep stands for Global Regular Expression Printe.
* Save the scan result in grepable format using `-oG FILENAME`.

### XML

* Save the scan results in XML format using `-oX FILENAME`.

### Script Kiddie

* `nmap -sS 127.0.0.1 -oS FILENAME`
