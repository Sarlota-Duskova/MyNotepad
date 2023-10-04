# Network Operations

## Network Performance Metrics

### Network Performance Factors

* CPU usage
* Cabling/connectivity
* High bandwidth
* DNS issues
* Malfunctioning devices

### CPU Usage

* High traffic
* Latency, jitter, packet loss
* External devices

### Cabling/ Connectivity

* Defective cables
* Inside/outside LAN
* Monitoring traffic

### High Bandwidth

* High traffic
* Slows overall performance

### DNS Issues

* Domain Name System
* No connectivity

### Malfunctioning Devices

* Little/no functionality
* Misconfiguration
* Routine testing

### Network Metrics

* Latency
* Packet loss
* Throughput
* Jitter
* Packet duplication/reordering

### Identifying Network Performance Issues

* Determine baseline
* Monitor and analyze
* Map network
* Identify cause
* Record findings

## Simple Network Management Protocol (SNMP)

* Identify devices
* Track network changes
* Monitor performance
* Obtain device status

### SNMP Architecture

* Managers
* Agents

### SNMPv1

* Poor security
* No encryption
* Vulnerable&#x20;

### SNMPv2

* In 1993
* Better security
* Replaced by SNMPv3

### SNMPv3

* Best security
* Encryption
* Authentication

### SNMP Hierarchy

* Data tree
* Tables
* Management Information Bases (MIBs)

### Management Information Bases

* Nodes
* Devices&#x20;
* Object Identifier (OIDs)

## Network Device Logging

### Log Files

* What happened?
* Who did it?
* When did it happen?
* Where did it come from?

### Device Logging

* Enabling logging is the critical first step

### Network Logging

* Determine which events are meaningful

### Audit Logging

* Security
* Resource access
* Be accountable

### Considerations

* Collection - how to collect data
* Storage - where and how to store&#x20;
* Protection
* Parsing
* Analysis

### Syslog

* Standard network-based logging protocol used to collect various device logs

### Codes

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

## Common Network Interface Statistics

### Network Interface Monitoring

* Ensure network devices are working and communicating efficiently

### Interface Statistics

* Most operating systems collect information relating to interfaces

### Link Status

* Link up
* Link down

### Interface Errors

* Runts
* Input errors
* CRC errors
* Giants

### Interface Statistics

* Speed
* Duplex

### Network Interface Send/Receive Errors

* Frequent errors indicate hardware problems

### Protocol Statistics

* Packets
* Bytes

## Common Network Interface Errors

* Identify and resolve network issues

### File Check Sequence Errors

* Uses cyclic redundancy checking (CRC) algorithm

### Giants

* Provides the number of packets that exceed maximum packet size
* Ethernet packets greater than 1518 bytes are considered giants

### Runts

* Ethernet packets smaller than 64 bytes

### Cyclic Redundancy Check (CRC)

* Verifes the integrity of received data

### Encapsulation Errors

* Can occur if an incorrect encapsulation method is assigned to an interface

## Environmental Factors and Sensors

### Heating, Ventilating, and Air Conditioning

* Extreme heat
* Extreme cold
* Extreme dryness

### HVAC Security

* Chemical attack
* Control location
* Monitor configuration

### Hot and Cold Aisles

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

### Humidity

* Humidity levels must be monitored

### Temperature Control Considerations

* Too cold
* Too hot

### Flood Warning Systems

* Protect property and equipment

### Fire Controls

* Prevention
* Detection
* Suppression

## Network Performance and Availability Baselines

### Network Performance Baseline

* Help determine normal working conditions

### Performance Baselines

* Point-in-time reference to performance
  * Overall network
  * Individual devices

### Defining Operations

* Baselines can be used to identify anomalies

### Testing and Reporting

* Physical connectivity
* Normal network utilization
* Average throughput
* Peak network utilization

### Baseline Timing

* Should be taken at different times of the day
* Should represent both quiet and busy times

## NetFlow Data Analysis

* Network protocol developed by Cisco
* Used for collecting network traffic information and monitoring network flow

### NetFlow Features

* Monitoring
* Planning
* Analysis

### Flow

* Source IP address
* Destination IP address
* Source port
* Destination port
* Protocol

### Flow Entry Expiration

* Inactive timeout
* Active timeout

### Output

* Basic output of NetFlow is a flow record

### Templates

* Adapted to provide future support for new or developing protocols
* Easily and quickly implement new features
* IETF standard mechanism

## Network Uptime and Downtime

### Network Uptime

* Refers to the amount of time that a network is up and running

### Network Availability Standard

* 99.999%&#x20;

### Service Level Agreements

* Commitment offered by a service provider
* Detailed descriptions of services offered
* Agreement on service performance

### Downtime

* Period of time when a system cannot complete its primary function
* Can result in services being unavailable to customers

### Types of Downtime

* Planned
* Unplanned

### Planned Downtime

* Network maintenance
* Updates/upgrades and reboots
* System diagnostics
* Configuration updates

### Unplanned Downtime

* Hardware failure
* Human error
* Server vulnerabilities
* Natural disasters - can be handle by stand by datacenters

### Costs of Downtime

* Recovery costs
* Lost revenue
* Lost productivity

## Organizational Planning and Procedures

### Change Management

E.g. software upgrades

### Incident Response Plan

* Roles
* Responsibilities

### Incident Response

* The International Standards Organization (ISO) defines that an Incident Response plan should involve six key phases.
  * Preparation
  * Detection
  * Containment
  * Investigation
  * Remediation
  * Recovery

### Planning for Failure

* Disaster recovery
* Business continuity

### Key Components of a DR/BC Plan

* Employee training
* Crisis communication planning
* Continuity exercises
* Testing and evaluation
* Stakeholder involvement

### Business Impact Analysis (BIA)

* Identify crucial processes and systems

### System Development Life Cycle (SDLC)

* Used to define policy, organizational, personnel, and budgeting constraints

### SDLC Phases

## ![](../../.gitbook/assets/image.png)



## Network Security Policies

### Password Policy

* Establish a standard for creating and enforcing the use of strong passwords
* Poorly chosen passwords may result in unauthorized access of a system or network resources

### Acceptable Use Policy (AUP)

* Document that outlines expectations for users to use Internet or corporate network services
* Defines acceptable use and breaches of acceptable use

### Bring Your Own Device (BYOD)

* Laptops
* Smartphones
* Tablets

### Onboarding

#### Process

* Job/responsibility
* Organizational culture

#### Goals

* To engage and connect immediately with new hires
* Reduce turnover
* Increase productivity and success

### Offboarding

* Strategic process for transitioning or removing an employee from an organization
* Checklist can be developed to ensure general tasks are completed prior to the employee leaving
* Offboarding can help ensure that an employee departs the organization on good terms

### IT Security Policy

* Rules
* Procedures

### Data Loss Prevention (DLP)

* Controls how valuable data is used
  * Intellectual property
  * Confidential corporate data
  * Personally identifiable information
* Prevents data leakage
  * Data disclosure outside of the organization

### Remote Access

* Technology that controls how users can remotely connect to an organization's local area network
* Remote access policies
  * Outline acceptable methods for allowing remote connections to the LAN

## Common Network Operations Documentation

### Physical Network Diagram

* Location
* Wired
* Wireless
* Infrastructure devices
* Physical security

### Logical Network Design

* VLANs
* Virtual network switches
* Software-defined networking

### Rack Diagram

* Metal frame used to contain different network hardware devices
  * Servers
  * Routers
  * Switches
  * Security devices

### MDF/IDF Documentation

* Main distribution frame
* Intermediate distribution frame

### Wiring Diagram

* Connectors
* Wiring
* Devices

### Site Survey Reports

* Commonly used to survey wireless networks
* Helps visualization
  * Coverage areas
  * Data rates

### Network Audits and Assessments

* Device support
* Inventory
* Architecture
* Security

### Baselines

* Determine what is considered to be normal
* Useful troubleshooting and planning

## Common Network Operations Agreements

### Non-disclosure Agreement (NDA)

* Legally binding contract

### NDA Key Elements

* Participants involved in the agreement
* Length of agreement
* What is considered to be confidential
* Exclusions

### Service Level Agreement (SLA)

* Service provider
* Customers

### SLA Components

* Objectives
* Responsibilities
* Scope
* Performance metrics
* Penalties

### Memorandum of Understanding (MOU)

* Helpful when establishing official partnerships

## Test

**Which type of agreement would typically be implemented between two organizations who are forming an initial partnership?**

* MOU

**At which phase of an incident response plan would you detail the severity, priority, and root cause of a problem?**

* Investigation

**The process of Netflow intervening to produce an output for analysis is known as what?**

* Active timeout

**If your network monitoring consistently reveals packets that are 3000 bytes in size, which condition does that indicate?**

* Giants

**Which type of network documentation or diagram would indicate the means by which your building is wired?**

* MDF/IDF

**Which percentage of service uptime would you most likely see from a reputable network service provider?**

* 99.9%

**Which type of networking statistic would indicate that the integrity of a packet has been compromised?**

* CRC errors

**When determining a baseline for your network, which methods should be used?**

* Gather at different times of day
* Gather during both busy and slow times

**Which type of network logging is primarily concerned with security-based events such as resource access?**

* Audit

**Which type of policy deals with attempting to ensure that confidential information is not leaked outside of your organization?**

* Data loss prevention

**If all users within your network report that they are unable to access the internet, which networking issue would be the most likely cause?**

* DNS

**The space between two racks that are rear facing each other is typically referred to in which manner?**

* Hot aisle

**The collection of all known attributes and values on a client device using SNMP is known as what?**

* MIB
