# Nmap Post Port Scans

|          Option         |                     Meaning                     |
| :---------------------: | :---------------------------------------------: |
|           -sV           |   determine service/version info on open ports  |
|           -sV           |  --version-light try the most likely probes (2) |
|           -sV           |    --version-all try all available probes (9)   |
|            -O           |                    detect OS                    |
|       --traceroute      |             run traceroute to target            |
|     --script=SCRIPTS    |               Nmap scripts to run               |
| -sC or --script=default |               run default scripts               |
|            -A           |      equivalent to -sV -O -sC --traceroute      |
|           -oN           |           save output in normal format          |
|           -oG           |          save output in grepable format         |
|           -oX           |            save output in XML format            |
|           -oA           | save output in normal, XML and Grepable formats |

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

| Script Category |                               Description                              |
| :-------------: | :--------------------------------------------------------------------: |
|       auth      |                     Authentication related scripts                     |
|    broadcast    |              Discover hosts by sending broadcast messages              |
|      brute      |          Performs brute-force password auditing against logins         |
|     default     |                      Default scripts, same as -sC                      |
|    discovery    | Retrieve accessible information, such as database tables and DNS names |
|       dos       |          Detects servers vulnerable to Denial of Service (DoS)         |
|     exploit     |             Attempts to exploit various vulnerable services            |
|     external    |  Checks using a third-party service, such as Geoplugin and Virustotal  |
|      fuzzer     |                         Launch fuzzing attacks                         |
|    intrusive    |     Intrusive scripts such as brute-force attacks and exploitation     |
|     malware     |                           Scans for backdoors                          |
|       safe      |                Safe scripts that won’t crash the target                |
|     version     |                        Retrieve service versions                       |
|       vuln      |        Checks for vulnerabilities or exploit vulnerable services       |

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
