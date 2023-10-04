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



## Security Assessment Exercises



## Security Information and Event Management



## Common Technology-based Attacks





## Ransomware Attacks



## Common Malware Attacks



## On-path Attacks





## Common Password Security Attacks





## Denial of Service Attacks





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





















