# Disaster Recovery & High Availability Concepts

## Load Balancing Devices and Solutions

* Distributes incoming network traffic
* Cost-effective
* Maximizes speed and efficiency

### Load Balancer Functions

* Distribute client requests and network load
* Improves availability and reliability
* Provides flexibility

### Load Balancing Algorithms

* Round robin
* Fewest connections
* Least time
* Hash
* IP Hash
* Random with two choices

### Hardware vs. Software Load Balancing

#### Hardware

* Proprietary
* Specialized processors
* Additional infrastructure

#### Software

* Non-proprietary
* Less expensive
* Flexible
* Cloud options

### Load Balancer Locations

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

## Dynamic Multipathing Techniques

* Automatically directs communication between a client and remote storage to alternative paths during failures

#### Benefits

* Greater reliability
* Maintains critical data access
* Uniform balancing across multiple paths

### How Dynamic Multipathing Works

#### DMP maps nodes

* Storage clients (nodes) access remote disks
* Each node can have multiple physical connections to the disks
* In the event of failure, the operating system transparently fails over to the other connection

### Dynamic Multipathing Input/Output Policies

* Adaptive
* Balanced
* Minimumq
* Priority
* Round-robin
* Singleactive

## Redundant Hardware and Clusters

### Redundancy and Clustering

#### Redundancy

* Redundant components
* Replicated instances
* RAID
* Databases

#### Clustering

* Group of functionally equivalent devices
* Structurally redundant
* Active-passive = when a first server goes down then clustering automatically reroutes clients to the other server and there is no disruption of service

#### Redundancy Advantages

* Less expensive
* Easier to implement and manage
* Can distribute load across multiple servers
* Scalability

#### Redundancy Disadvantages

* Poor availability during failures
* Slow response
* Fail to meet client requirements

#### Clustering Advantages

* Automatic failure recovery

#### Clustering Disadvantages

* Complexity
* Lack of corruption recovery

### Failure Handling

* Single hardware failure
* Service failures
* Recovery

## Facilities and Infrastructure Support

* Disaster and recovery strategies
* Recovering your systems and data

### Uninterruptable Power Supply (UPS) Types

* Standby - only going to be used in the event of a power failure, most basic UPS
* Line interactive
* Double-conversion - consistent near-perfect power regardless of the state of what is coming in, they will accept incoming AC power then convert it to DC, then back to AC

### Power Distribution Unit (PDU) Considerations

It distributes the power typically coming from a separate source, which can include a UPS

* Location
* Input power
* Equipment power needs
* Outlet needs
* Plug types
* Other requirements

### Facility Generators

#### Key considerations

* Classification or type
* Size
* Fuel type
* Location
* Emissions standards
* Runtime

### Heating, Ventilation, and Air Conditioning (HVAC) Considerations

* Location
* Access
* Parameters

### Fire Protection Levels

* Building
* Room
* Rack

## Network Interface Card (NIC) Teaming

* Enables multiple physical network adapter cards to work as a single logical interface
* Shared IP address

#### Benefits

* Load balancing
* Fault tolerance

### Configurations

* Active-passive
* Active-active

### Components

* Team members - physical adapters
* Team interfaces - assigned an IP address

### Modes

* Switch independent - taking the physical connections from the adapters and plugging them into different switches
* LACP
* Static

## High Availability Solutions

* Nearly full-time availability
* Redundant hardware and software
* Avoids single points of failure
* Moves resources
* Recovers failed operations
* Restores services

### Measurements

* MTTR (Mean Time To Repair)
* MTBF (Mean Time Between Failures)

### Recovery Objectives

* RPO (Recovery Point Objective)
* RTO (Recovery Time Objective)

### High Availability in the Cloud

* Uses clusters
* Provides continuous uptime
* Shared storage access
* Failover and load balancing

### High Availability Cloud Configurations

* Active-actvie - multiple servers active in the same time, using when a lot of people using service
* Active-passive - still redundant, only one server will be serving for example database and if the active copy fails, then it fails over to the passive copy
* Multiple datacenters
* Diverse paths

### Redundancy Protocols

* FHRP (First Hop Redundancy Protocol)
* VRRP (Virtual Router Redundancy Protocol)

### Recovery Site Types

* Hot - another site that is active
* Warm - has all of the infrastructure in place but is not necessarily running it might,not be entirely up-to-date, maybe it would be neccessary to restore everything from backup
* Cold - Manually moving resources from one place to another

## Network Backup and Restore Options

* Copying data and configuration information to a separate, secondary device
* Recover data and applications after loss or damage
* Disaster recovery strategy

### Backup Devices and Services

* Tape drive
* HDD or SSD
* Backup server
* Cloud

### Common Backup Methods

* Full - whether the data has changed or not
* Incremental - check what has change the day before, so if back up is every Monday and I changed something on Tuesday, on Wednesday check what has change and Differential still check what has change on Monday and doesn't care that something change on Tuesday
* Differential - backup only data that has change, check what has change since last backup
* CDP - automaticaly&#x20;
* Bare-metal
* Instant recovery (Virtual Machines)

### System State Backup

* Copy of crucial OS components
* Quick
* Uses native backup tools

### Backup Considerations

* Corruption
* Accessibility
* Failures or schedule issues
* Incomplete
* Slow

## Test

**Which value provides an indication of how reliable your equipment or services have been over time?**

* MTBF

**Which feature is almost always an advantage of clustering that might not be a feature of redundancy?**

* Automatic recovery from failure

**Which method of load balancing works based on sequentially directing requests to a group of servers?**

* Round robin

**Which method of dynamic multipathing directs traffic based on specified values as defined by an administrator?**

* Priority

**Which type of UPS should be implemented if you require the highest levels of reliability and the cleanest type of power?**

* Double conversion

**Which NIC teaming configuration would be required if you want to provide both fault tolerance and load balancing?**

* Active/active

**Which types of backup would you implement when you are more concerned with the configuration of a server rather than the data?**

* Bare metal
