# Security Concepts & Threats

## Confidentiality, Integrity, and Availability (CIA)

* Known as the CIA triad
* Guides organizational policies for information security
* Most crucial security components

### Confidentiality

* Protect sensitive information
* Allow necessary access to information
* Special training may be required
* Data categorized by potential damage

### Integrity

* Maintain data accuracy and consistency
* Protect data from change in transit
* Protect data from unauthorized people
* Apply permissions and access controls
* Apply version control and detect changes

### Availability

* Maintain hardware and perfom repairs
* Redundant storage
* Regular and frequent backups
* Avoid software conflicts
* Firewalls, proxy servers, anti-malware

### Best Practices

* Confidentiality
* Integrity
* Availability

## Common Network Threats

* External
* Internal

### External Risks

* Malware
* Malvertizing
* Phishing
* Denial-of-service (DoS) attacks
* Ransomware



* Cybercriminals may remain unchecked in systems for months after gaining access
* Penetration testing can help with building adequate perimeters
* External attackers are generally more common than internal

### Top External Attacks

* DoS/DDoS
* Session hijacking
* Drive-by
* Password
* Phishing and spear phishing

### Internal Risks

* Risks stem from employees (could be intentional or accidental)
* Criminals aim to obtain employee or admin credentials
* Employees should be trained about cybersecurity

### Preventing External and Internal Risks

* Train employees to not share or reuse passwords
* Change passwords often and always on employee departure
* Monitor employee access and always adjust as needed
* Require passwords meet security guidelines

## Common Network Vulnerabilities

* Development mistakes that could be used to allow unauthorized system access
* Allow access to system info or network information
* Allow attackers to steal/modify/destroy data or run harmful code

### Exposure

* Allows indirect network access
* Often results in data breach
* Gathering secure information

### Common Vulnerabilities and Exposures (CVE)

* Categorized list of known software security vulnerabilities and exposures, other organizations can use to protect their systems

### Zero-day Vulnerability

* Known security flaw in software that doesn't have a patch
* Newly discovered
* Must be fixed quickly
* Hackers may exploit before fixed

### Protection from Zero-day Vulnerabilities

* Use security software to block know vulnerabilities
* Immediately install software updates and releases
* Implement security best practices throughout your organization

## Network Security Exploits

* Blank or default passwords
* IP spoofing and eavesdropping
* Application vulnerabilities
* Default shared keys
* Service vulnerabilities
* Denial of service attacks (DoS)

### Blank or Default Passwords

* Blank admin password
* Default product password
* Common with firewalls and routers

### IP Spoofing

* Remote machine appears as local network node
* Server vulnerabilities are found
* Backdoor program or trojan horse installed

### Eavesdropping

* Eavesdropping on a connection between two nodes to collect data
* Generally applies to Telnet, FTP, and HTTP transfers
* Attacker must have LAN access to system
* Prevent using cryptographic key exchange, encrypted authentication, and one-time passwords

### Application vulnerabilities

* Attackers take advantage of application faults to implant trojan horses, execute harmful code, or crash systems

### Default Shared Keys

* Default security keys for dev or eval testing left unchanged in production environment
* Any users with these same default keys will have access to the resource

### Service Vulnerabilities

* Flaw in a network service
* Compromise the service
* Possible additional compromised systems

### Denial of Service Attacks

* Network server or device is attacked by flooding it with requests
* Leaves legitimate users unable to access resources

## Principle of Least Privilege

* A user, program, or process should only have privileges needed to perform a job or function and nothing more
* Users
* Computers
* Services
* Networks
* Databases
* Applications

### Benefits

* Improved security
* Smaller attack surface
* Propagation of malware is limited
* Improved stability

### Implementing the Principle of Least Privilege

* Perform an audit of existing privileges
* Set new account privileges as low as possible
* Keep admin and standard accounts separate
* Implement just-in-time privileges
* Ensure individual actions are traceable
* Perform regular auditing

## Role-based Access Control (RBAC)

* User network access is based on their role in the organization
* User granted access only to what they need to perform their job
* Access can be restricted based on authority, job competency, and responsibility

### Sample RBAC Tool Designations

* Management role
* Management role group
* Management role scope
* Management role assignement

### RBAC Benefits

* Reduced IT support and admin work
* Increased operational efficiency
* Enhanced compliance

### RBAC Implementation Best Practices

* Snapshot current security configuration
* Be familiar with employee roles
* Document policy
* Make changes
* Adapt as required

## Zero Trust Security Model

* No automatic trust for what's inside or outside an organization's perimeters
* Everything must be verified before being allowed access to systems

### Why Implement Zero Trust?

* Security breaches occur at tremendous cost to organizations

### Zero Trust Security Model

* Castle-and-moat approach no longer sufficient
* Many default and open connections cause challenges
* Must deal with on-premises and cloud applications being accessed by various devices

### Zero Trust Technologies

* Multifactor authentication (MFA)
* Identity and access management (IAM)
* Orchestration and analytics
* Encryption and scoring
* File system permissions

## Defense in Depth (DiD)

* Security approach
* Layered defense mechanisms
* Redundancy increases system security

### Security Controls

* Security controls protect assets
  * Employees
  * Property
  * Equipment
  * Services
  * Data
  * Customers

### Security Control Types

* Physical
* Technical
* Administrative

### Security Controls

* Risk management, IT security strategy
* Objectives determine security controls to use

### Security Control Functions

* Preventative
* Detective - find that already occur&#x20;
* Corrective - fix the problem, rebooting a server or device, quarantering or removing virus

## Common Network Authentication Methods

* Multifactor authentication (MFA)
* Terminal Access Controller Access-Control System Plus (TACACS+)
* Remote Authentication Dial-in User Service (RADIUS)
* Single sign-on (SSO)
* Lightweight Directory Access Protocol (LDAP)
* Kerberos
* Local authentication
* 802.1X
* Extensible Authentication Protocol (EAP)

### Radius

* Provides centralized authentication, authorization, and accounting for network service users

### LDAP

* Software protocol for locating network resources
* Foundation for Active Directory and cloud-base directories
* Binds a LDAP user to a LDAP server

### Kerberos

* Protocol for providing secure authentication using secret-key cryptography
* Very common use in Windows

## Security Assessment Exercises

* Network security measure used to find vulnerabilities

### Security Assessment

* Vulnerability assessment
* Penetration test

### General Security Assessment Steps

* Inventory resources
* Determine asset vulnerability
* Test defenses
* Remediate weak points
* Monitor security continuously

## Security Information and Event Management (SIEM)

* Combines security event management (SEM) with security information management (SIM)
* Reporting on security events and incidents
* Alerting on potential security issues and store for analysis
* Threat intelligence
* Security analytics
* Machine learning
* IT governance
* Automated remediation

### Enterprise SIEM

* Generally used by large organizations
* High annual cost
* Software-as-a-service offering
* Usually run on-premises due to sensitive data

## Common Technology-based Attacks

### Network Attack

* Unauthorized network access with objective to steal information or perform harmful activities
* Passive (steal data without changing) and active (changing, removing, or harming data)

### Common Network Attacks

* Unauthorized access
* DDoS
* Man in the middle
* Code and SQL injection
* Privilege escalation
* Insider threats

### &#x20;Common Technology-based Attacks

* DNS poisoning
* VLAN hopping
* ARP spoofing
* Rogue DHCP
* Rogue access point
* Evil twin
* Brute-force
* Dictionary
* MAC spoofing
* IP spoofing
* Deauthentication

### Best Practices for Network Protection

* Network segragation
* Regulated Internet access through Proxy servers
* Use security devices
* Secure wireless networks
* Regularly apply updates

## Ransomware Attacks

* Malware used by attacker to encrypt files, allowing them to then demand a ransom to restore the files

### Ransomware

* Commonly accesses computers via phishing
* May contain social engineering tools
* Encrypted files are held for ransom
* Decryption requires the key held only by the attacker

### Ransomware Targets

* Universities and colleges
* Hospitals and medical facilities
* Low firms and government offices

### Preventing Ransomware Attacks

* Keep up with OS patches and updates
* Be cautious about giving software admin privileges
* Install antimalware software
* Regularly back up files

## Common Malware Attacks

### Malware

* Cyber attack where malicious software performs harmful actions on a system
* Includes ransomware, spyware, and command and control

### Aspects of Malware

* Objective
* Delivery
* Concealment

### Malware Objectives

* Stealing data
* Disrupting operations
* Extorting payment

### Malware Attack Vectors

* Trojan horse
* Virus
* Worm

### Malware Prevention

* Install an antimalware application
* Ongoing education of users
* Prioritizing network security
* Performing security audits regularly
* Performing and verifying backups regularly

## On-path Attacks

* Intercept/modify communication between two devices
* Steal data or impresonate agents
* Target e-mail, DNS lookups, and public Wi-Fi

### E-mail Hijacking

* Attackers insert themselves between e-mail server and the web and monitor e-mail communications

### Public Wi-Fi Risks

* Cloned Wi-Fi networks
* User's online activity is monitored

### Protecting against On-path Attackers

* SSL/TLS
* Authentication certificates
* Secure/Multipurpose Internet Mail Extensions (S/MIME)
* Virtual Private Network (VPN)

## Common Password Security Attacks

* Brute force
* Dictionary
* Phishing
* Rainbow table
* Credential stuffing
* Password spraying
* Keyloggers

### Brute Force Attack

* Easiest for attackers
* Attackers tries all possible password combinations to access a user account
* Easy to guess passwords and usernames

### Dictionary Attack

* Attacker programmatically cycles through common words to discover password

### Phishing

* Disguised in e-mails that appear lefitimate
* Claim suspicious activity has been detected
* Alternatively obtain private user information, which may help in guessing passwords

### Rainbow Table Attack

* Uses mathematical equations to hask algorithm password combinations to discover passwords

### Credential Stuffing

* Stolen usernames and passwords are tried in varying combinations until a match is found
* Assumes users have the same passwords for multiple accounts

### Password Spraying

* Attack attempts to match millions of accounts with commonly used passwords

### Keylogger Attack

* Attacker installs program that logs all user keystrokes

## Denial of Service Attacks

* Server is flooded with packets or requests until it becomes overwhelmed

### Distributed Denial of Service

* Multiple systems launch DoS attacks on one system

### Categories

* Volumetric
* Fragmentation
* TCP state exhaustion
* Application layer

### Forms

* Ping of death (ICMP flood)
* UDP flood
* SYN (TCP) flood
* HTTP flood
* Teardrop

### Reasons for DoS and DDoS Attacks

* Disgruntled employees
* Competitors
* Hacktivism
* Ransom
* Troublemaking

### Minimizing Attack Damage

* Network monitoring
* Simulated attacks
* Post-attack plan

## Social Engineering Attacks

* Attacks that generally do not involve technology
* Trick users into divulging information
* Generally involves multiple steps
* Relies on perceived trust

### Techniques

* Baiting
* Scareware
* Pretexting
* Phishing
* Spear phishing

### Prevention

* Use caution opening e-mails and attachments from unfamiliar sources
* Research things that seems too good to be true
* Use multifactor authentication (MFA) to protect accounts
* Regularly update antivirus and antimalware software

## Test

**Which common technology-based attack presents a false wireless network to users?**

* Evil twin

**Security cameras would be considered which type of control in the defence-in-depth model?**

* Physical

**Which statement or scenario best describes the zero-trust security model?**

* No one should be trusted

**Security Information and Event Management applications would be analogous to which type of operation or process?**

* Writing records to an operational database and querying a data warehouse simultaneously

**Which mitigation technique can be used to enhance the security of your email by ensuring that only the intended recipient can access a message, and be assured that the message was not altered?**

* S/MIME

**When or where would you be most likely to encounter a default password?**

* On a router or a firewall

**Which type of external attack is implemented by targeting a specific user or organization with social engineering tactics?**

* Spear phishing

**Which type of malware is capable of self-propagation and is most commonly spread via email?**

* Worm

**Which statements correctly characterize vulnerability assessments and penetration tests?**

* A penetration test attempts to breach your security
* Vulnerability assessments are generally performed to gather information only

**Which type of password attack works on the assumption that a weak password is being used within an organization?**

* Password spraying

**Which authentication method is based on using keys and tickets?**

* Kerberos

**A zero-day vulnerability is characterized by which aspect or component?**

* They have no current patch or fix

**Which approach to implementing the principle of least privilege grants only the necessary level of access, only when it is necessary?**

* Just-in-time privileges

**Which mitigation technique is most capable of defeating a ransomware attack?**

* Performing regular backups

**Leaving a flash drive labelled “Confidential” that actually contains malware, in an easily found location would be classified as which type of social engineering?**

* Baiting

**Which type of Denial-of-Service attack is based on fragmented packets that cannot be reassembled?**

* Teardrop

**Which component of role-based access control gives a user the abilities of a role?**

* Management role assignment

**In the CIA triad, integrity refers to which aspect of information protection?**

* Ensuring that an original version is not modified
