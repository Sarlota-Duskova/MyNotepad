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

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

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





## Network Security Policies





## Common Network Operations Documentation



## Common Network Operations Agreements





## Test



