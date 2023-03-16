# Basics

**Communicating remotely**

* TELNET (Teletype Network) is an application network protocol that enables user communication with a remote computer via a text-based interface.
* SSH (secure shell)
* VPN (virtual private network) for connecting.

**HTTP**

* HTTP (Hyper Text Transfer Protocol)
* HTTPS uses the protocol HTTP together with SSL or TLS for the web browser to communicate with the web server.
  * The details of the certificate, including the issuing authority and the corporate name of the website owner, can be viewed by clicking on the lock symbol on the browser bar.
* SSL (Secure Socket Layer)
* TLS (Transport Layer Security) is just an updated, more secure, version of SSL.

**SSL/TLS handshake** In SSL/TLS and other digital certificates, both methods – Symmetric and Asymmetric – are employed.

* First, when two parties (browser and server in the case of SSL) come across each other, they validate each other’s private and public key through **Asymmetric Encryption**.
* Once the verification is successful and both know whom they’re talking to, the encryption of the data starts – through **Symmetric Encryption**. Thereby saving significant time and serving the purposes of confidentiality and data-protection. **Examples:** RSA
* Choose two large prime numbers **p** and **q**
* n = p.q
* **The public key** is represented by the integers **n** and **e** (e = 2^16 + 1 = 65 537)
* **The private key** by the integer **d** (although **n** is also used during the decryption process, so it might be considered to be a part of the private key too).
* **m** represents the message (previously prepared with a certain technique explained below).

**Symmetric Key Encryption**

* Encryption is a process to change the form of any message in order to protect it from reading by anyone.
* In Symmetric-key encryption the message is encrypted by using a key and the same key is used to decrypt the message which makes it easy to use but less secure.
* It also requires a safe method to transfer the key from one party to another. **Examples:**
* Advanced Encryption Standard (AES)
* the Data Encryption Standard (DES)
* along with IDEA
* Blowfish
* RC4 (Rivest Cipher 4)
* RC5 (Rivest Cipher 5)
* RC6 (Rivest Cipher 6).

**Asymmetric Key Encryption**

* Asymmetric Key Encryption is based on public and private key encryption techniques.
* It uses two different key to encrypt and decrypt the message.
* It is more secure than the symmetric key encryption technique but is much slower.

**HTTP response status code**

1. Informational responses 1XX
   * 100 Continue
   * 101 Switching Protocols
     * This code is sent in response to an Upgrade request header from the client and indicates the protocol the server is switching to.
   * 102 Processing
2. Successful responses 2XX
   * 200 OK
3. Redirection messages 3XX
   * 301 Mover Permanently
   * 302 Found
   * 307 Temporary Redirect
   * 308 Permanent Redirect
4. Client error responses 4XX
   * 400 Bad Request
   * 401 Unauthorized
   * 403 Forbidden (The client does not have access rights to the content)
   * 404 Not Found
5. Server error responses 5XX
   * 500 Internal Server Error
   * 502 Bad Gateway
   * 503 Service Unavailable
   * 504 Gateway Timeout

**MAC address and IP address?** **IP Address**

* IP address is in L3 (Network) in OSI (Open Systems Interconnection) model.
* IPv4 (32 bits) grouped into four decimal numbers (0000.0000.0000.0000)
* IPv6 (128 bits) grouped into eight sets of four digits (0000.0000.0000.0000.0000.0000.0000.0000)

**MAC Address**

* MAC address is in L2 (Data Link) in OSI model.
* MAC (Media Access Control) is a 12-character alphanumeric, it is assigned to network card during manufacture
* MAC addresses are generally unique to a device, but some manufacturers re-use MAC addresses within a particular model or part number.
* Some devices allow you to change the MAC address advertised in software, for instance Ethernet adapters or wifi adapters. This is useful for connecting to other devices which are supposed to be locked to specific other devices (cable modems).
* https://macaddress.io

**Nmap what is it?**

* Finds which devices (IP Addresses) are in the network.
* What port is it running on, what is the service and what is it.

**Example of exploits**

* SQLi (injection)
* XXS (Cross-Site Scripting)
  * Reflected XSS Attacks
    * Reflected attacks are those where the injected script is reflected off the web server, such as in an error message, search result, or any other response that includes some or all of the input sent to the server as part of the request.
  * Stored XSS Attacks
    * Stored attacks are those where the injected script is permanently stored on the target servers, such as in a database, in a message forum, visitor log, comment field, etc.
    * The victim then retrieves the malicious script from the server when it requests the stored information
  * Blind Cross-site Scripting
    * Blind Cross-site Scripting is a form of persistent XSS. It generally occurs when the attacker’s payload saved on the server and reflected back to the victim from the backend application. For example in feedback forms.
* A path traversal attack (also known as directory traversal) aims to access files and directories that are stored outside the web root folder.
  * By manipulating variables that reference files with “dot-dot-slash (../)” sequences and its variations or by using absolute file paths, it may be possible to access arbitrary files and directories stored on file system including application source code or configuration and critical system files.
  * Don’t store sensitive configuration files inside the web root.
  * All but the most simple web applications have to include local resources, such as images, themes, other scripts, and so on.
* Man in the middle attack
  * Sniffing
    * Attackers use packet capture tools to inspect packets at a low level. Using specific wireless devices that are allowed to be put into monitoring or promiscuous mode can allow an attacker to see packets that are not intended for it to see, such as packets addressed to other hosts.
  * Packet Injection
    * An attacker can also leverage their device’s monitoring mode to inject malicious packets into data communication streams.
    * The packets can blend in with valid data communication streams, appearing to be part of the communication, but malicious in nature.
    * Packet injection usually involves first sniffing to determine how and when to craft and send packets.
  * Session Hijacking
    * Most web applications use a login mechanism that generates a temporary session token to use for future requests to avoid requiring the user to type a password at every page.
    * An attacker can sniff sensitive traffic to identify the session token for a user and use it to make requests as the user.
    * The attacker does not need to spoof once he has a session token.
  * SSL Stripping
    * Since using HTTPS is a common safeguard against ARP or DNS spoofing, attackers use SSL stripping to intercept packets and alter their HTTPS-based address requests to go to their HTTP equivalent endpoint, forcing the host to make requests to the server unencrypted.
    * Sensitive information can be leaked in plain text.
* XML (Extensible Markup Language) code injection, it is used for data serialization, in which it rivals JSON (JavaScript Object Notation)
* DDOS (Distributed Denial of Service)
* DOS (Denial of Service)
  * DoS attacks accomplish this by flooding the target with traffic, or sending it information that triggers a crash. In both instances, the DoS attack deprives legitimate users (i.e. employees, members, or account holders) of the service or resource they expected.
