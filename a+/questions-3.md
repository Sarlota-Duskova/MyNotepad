# Questions

1.  What type of cloud service offers the best security?

    1. Community
    2. Private
    3. Public
    4. Hybrid

    Answer:

    B. Companies can purchase virtualization software to set up individual clouds within their own network. That type of setup is referred to as a private cloud. Running a private cloud pretty much eliminates many of the features that companies want from the cloud, such as rapid scalability, and eliminating the need to purchase and manage computer assets. The big advantage, though, is that it allows the company to control its own security within the cloud. A hybrid model would be the scenario providing benefits of both public and private clouds. The community model is something akin to a shared private cloud, with responsibilities and benefits collaboratively shared.
2.  Your manager tells you to purchase cloud-based services. Your network needs extra processing power and file storage. What type of service should you purchase?

    1. PaaS
    2. IaaS
    3. SaaS
    4. FWaaS

    Answer:

    B. Let's say that your company needs extra network capacity, including processing power, storage, and networking services (such as firewalls), but doesn't have the money to buy more network hardware. Instead, your company can purchase infrastructure as a service (IaaS), which is a lot like paying for utilities; you pay for what you use. Of the four, IaaS requires the most network management expertise from the client side. In an IaaS setup, the client provides and manages the software. PaaS is platform as a service and SaaS is software as a service. FWaaS is sometimes used to mean firewall as a service, but is not widely recognized nor on the CompTIA A+ 220-1101 objectives.
3.  Your company has decided to purchase cloud services from Google. They will be getting infrastructure with on-demand computing services including processing power, storage and bandwidth over the Internet. Anyone can purchase these same services from Google, and a third party is responsible for maintaining and managing the hardware. What type of cloud is Google providing for your company?

    1. Public
    2. Private
    3. Hybrid
    4. Community

    Answer:

    A. The traditional type of cloud that usually comes to mind is a public cloud, like the ones operated by third-party companies such as Microsoft, Google, HP, Apple, Netflix, and Amazon with its Amazon Web Services (AWS). These clouds offer the best in scalability, reliability, flexibility, geographical independence, and cost effectiveness. Whatever the client wants, the client gets. For example, if the client needs more resources, it simply scales up and uses more.
4.  Your company produces software and employs about 20 developers. They need to program apps for different operating systems. You decide to purchase cloud-based services to support the development team. What type of service should you purchase so that they can develop their programs and then test them in environments other than where they were developed?

    1. IaaS
    2. SaaS
    3. PaaS
    4. NaaS

    Answer:

    C. Platform as a service (PaaS) adds a layer to IaaS that includes software development tools such as runtime environments. Because of this, it can be helpful to software developers; the vendor manages the various hardware platforms. This frees up the software developers to focus on building their application and scaling it. The best PaaS solutions allow for the client to export its developed programs and run them in an environment other than where they were developed.
5.  Which type of cloud service provides your company with application hosting such as productivity applications, calendaring software, and development tools, that the employees can access over the Internet from wherever they are?

    1. PaaS
    2. FWaaS
    3. IaaS
    4. SaaS

    Answer:

    D. The highest of the three levels of cloud service is software as a service (SaaS), which handles the task of managing software and its deployment. This is the model used by Google Docs, Microsoft Office 365, and even storage solutions such as Dropbox.
6.  Which feature of cloud service allows you to instantly obtain additional storage space or processing power as your company needs it?

    1. Ubiquitous access
    2. Rapid elasticity
    3. Resource pooling
    4. Measured service

    Answer:

    B. In most cases, clients can get more resources instantly (or at least quickly or on-demand), which is called rapid elasticity. For the client, this is a great feature because they can scale up without needing to purchase, install, and configure new hardware. Ubiquitous access refers to clients being able to access the cloud ubiquitously, or from anywhere, anytime. Resource pooling, particularly when a cloud provider deals with multiple tenants, refers to the provider effectively saving money by not duplicating available capacity. Finally, when the service provided to those tenants is monitored and paid for according to their use, it's metered service or metered utilization.
7.  You are installing virtualization on a workstation that needs to support multiple operating systems. Which type of hypervisor is best suited for this environment?

    1. Type 1.
    2. Type 2.
    3. Either Type 1 or Type 2 will function in the same way.
    4. Virtual machine manager.

    Answer:

    B. A Type 2 hypervisor sits on top of an existing operating system, called the host OS. This is most commonly used in client-side virtualization, where multiple OSs are managed on the client machine as opposed to on a server. The hypervisor is also called a virtual machine manager (VMM).
8.  You are configuring client-side virtualization on an existing Windows 10 64-bit workstation. You will be running a second installation of Windows 10 64-bit in the virtual environment as a test system. The bare minimum RAM required for each OS is 2 GB. Each Windows installation needs 20 GB of disk space. What are the absolute minimum hardware requirements for this workstation?

    1. 4 GB of RAM, 40 GB of disk space
    2. 2 GB of RAM, 20 GB of disk space
    3. 2 GB of RAM, 40 GB of disk space
    4. 4 GB of RAM, 20 GB of disk space

    Answer:

    A. If presented with a scenario for installing multiple operating systems (OS) on a computer running client-side virtualization, just add the minimum hardware requirements (or recommendations) together. Treat it as if each OS needs its own minimum (which it does) and they are just sharing the available physical hardware (which they are). Also, each OS needs its own virtual network card to participate on the network and needs its security to be individually configured based on OS requirements and user needs. Treat it as though it is a separate computer. In reality, you're never going to go with just the absolute minimum because although the OS will run, it won't run well.
9.  You are setting up virtualization on a server that will be running four instances of Windows Server 2019. Four different departments will be using one instance each, and all departments have been promised 32 GB of RAM. Using resource pooling and using a bare-metal hypervisor, what is the minimum amount of physical RAM needed on the server?

    1. 32 GB
    2. 64 GB
    3. 128 GB
    4. 16 GB

    Answer:

    C. If each client has been promised 32 GB of RAM, then the server must have enough RAM to give each client their allotment. This means 128 GB in this case. The assumption is that the hypervisor will require no RAM on its own. In reality, it probably will require a little but not much. Resource pooling, when a cloud provider deals with multiple tenants, refers to the provider having additional capacity available but saving money by sharing that availability.
10. Your company has an application developer who creates programs for Windows, Linux, and macOS. What is the most cost-effective solution for them to be able to test their programs in multiple operating systems as quickly as possible?

    1. Buy workstations for each of the OSs they will be writing code in.
    2. Set up their workstation to dual-boot.
    3. Set up their workstation with virtual machines.
    4. Create one version of each application that will run in all three OSs.

    Answer:

    C. The major feature of virtualization is breaking down that one-to-one hardware and software barrier. The virtualized version of a computer is appropriately called a virtual machine (VM). Thanks to VMs, it is becoming far less common to need dual-boot machines today than in the past. VMs allow computers to do things like run five instances of an OS or one instance each of several different OSs.
11. Your company wants to begin transferring particular services to the cloud, but the team cannot yet decide on the migration schedule. Management wants to pay for cloud computing based on usage, not a fixed flat fee. What payment model would you recommend?

    1. On-demand
    2. Resource pool
    3. Metered utilization
    4. Shared resources

    Answer:

    C. Metered utilization is synonymous with pay-as-you-use. The resources are available, but payment is calculated according to the actual usage. This is a common model for enterprise environments, especially during the early “migration of services” period. On-demand means services can be added as needed on the fly. A resource pool refers to the resources owned by a cloud provider such as RAM and storage capacity that are available to the cloud provider's clients. Shared resources refer to the idea that a cloud provider's physical resources may be shared among many different companies.
12. A client complains about the occupied space, abundant power usage, and hardware costs of the multiple machines used in its small data center. Still, the client does not wish to lose control over any of the machines. What might you recommend to the client to resolve all of those issues?

    1. Establish clusters for high availability.
    2. Create virtual machines.
    3. Outsource to an IaaS provider.
    4. Shut down the nonessential machines.

    Answer:

    B. The creation of virtual machines would alleviate the issue of space, power, and most of the hardware costs associated with maintaining bare-metal systems. Virtual machines can provide much of the same services, at a fraction of the costs. Control and management of the machines would not change.
13. Which term describes physical and virtual servers, storage, and software that are used by multiple clients in a cloud computing environment?

    1. Measured resources
    2. Shared resources
    3. Private cloud
    4. Community cloud

    Answer:

    B. Shared resources describe the cloud infrastructure shared among clients of a cloud provider. For example, a cloud provider may have one physical server that is shared by multiple companies. Shared resources are also those resources made available to multiple employees or users on a local network. Measured resources are synonymous with pay-as-you-go services where the company pays only for the resources they are using. A private cloud negates many of the advantages of a public cloud such as rapid elasticity, but control remains with the owner of the cloud. A community cloud is shared by a small group of users with similar needs who pool their resources for a more cost-effective solution.
14. What are potential problems associated with the shared resource structure of public cloud computing? (Choose two.)

    1. Security and confidentiality
    2. Flexibility
    3. Poor application performance
    4. Increased hardware costs

    Answer:

    A, C. Many companies go to cloud computing and the inevitable shared resources for the advantages of lowering their hardware costs and for the flexibility of adding resources on the fly. There are, however, some concerns with cloud computing, such as who has access to the data, the potential for another cloud computing client to introduce malware, and potentially poor application performance if another application is monopolizing the shared resources. Another potential problem is Internet connection downtime.
15. Network control and security management of cloud assets is the difference between what two types of shared resources?

    1. Internal vs. external
    2. Private vs. public
    3. Hybrid vs. community
    4. Synchronized vs. unsynchronized

    Answer:

    A. Internal shared resources would be under local network control and local security management, perhaps provided to different units within the same organization, whereas external assets are very likely secured and controlled by an external cloud provider.
16. A company using cloud services wishes to better prepare for surges for what it needs. What sort of capacity provisioning by its cloud provider should the company ask for?

    1. Rapid metering
    2. Infrastructure as a service
    3. Metered utilization
    4. Resource pooling

    Answer:

    C. For a company needing additional cloud resources on demand, they should request metered utilization, in which a cloud service will bill much like a utility would, as resources are used. Infrastructure as a service (IaaS) refers to hardware and networking in the cloud, and resource pooling is used in cloud computing to mean that resources are pooled and delivered as needed to many clients. Rapid metering is not an IT term.
17. You're setting up a virtual machine for one of your customers who needs a legacy OS to run software for a paper-cutting machine in an envelope factory. Windows 10 64-bit is the host OS. The legacy client OS requires a minimum 1 GB of RAM and the software running on it requires a minimum of 2 GB of RAM. What is the absolute minimum RAM needed on the virtual machine?

    1. 1 GB
    2. 4 GB
    3. 5 GB
    4. 10 GB

    Answer:

    C. This configuration would need 2 GB for Windows 10 (the host) plus 3 GB for the client OS and running software at a minimum. In reality, more RAM would be better.
18. The company's sales manager wants to ensure that the laptop files of its traveling sales engineers stay consistent with the files on the company cloud. What sort of applications could assist with that business need?

    1. File security monitoring
    2. File virtualization
    3. File emulator
    4. File synchronization

    Answer:

    D. Synchronization applications work to keep all files consistent, updating from multiple locations as needed. Emulation is when one thing acts like (emulates) something else. File security is ubiquitous and is needed everywhere, but it does not address the need to keep the files consistent, whether the users are traveling or on premises. Virtualization is using a single set of hardware as if it were multiple machines to run multiple OS instances or multiple operating systems.
19. What service allows a user to access a virtual OS either in the cloud using a browser or client on their local devices or from a local virtualization server?

    1. On-demand desktop (ODD)
    2. Binary application desktop (BAD)
    3. Virtual desktop infrastructure (VDI)
    4. Desktop streaming (DTI)

    Answer:

    C. Virtual desktop infrastructure (VDI) can be managed/hosted on either a local server (local cloud) or over the Internet by a third party. When in the cloud and managed by a third party, it is sometimes called desktop as a service (DaaS). The advantages of VDI are savings in hardware costs and configuration time. Data sensitivity and data security may preclude using VDI in the cloud.
20. An employee travels between multiple offices, using a desktop system in each office. What technology would ensure that the employee's desktop icons, files, and applications stay uniform across systems in all the offices?

    1. On-demand desktop
    2. VDI in the cloud
    3. Desktop emulation
    4. Synchronized folders

    Answer:

    B. A virtual desktop infrastructure (VDI) moves the desktop icons, files, and folders to a server instead of the desktop originating from the local machine. When the desktop experience is hosted on a centralized server location, the icons, files, and folders are the same. With this user working from different offices, the best solution for them is VDI in the cloud.
21. When running a hypervisor, what enables a guest machine to connect to a network?

    1. Cat 5 network cable
    2. Guest applications
    3. Virtual NIC
    4. Host operating system

    Answer:

    C. In a virtual environment, a virtual network interface card (NIC) connects the guest machine to its local virtual network and any external networks.
22. How can an organization permit employees who need to run an application on one mobile device to instead run it from multiple devices?

    1. Application virtualization
    2. Wrapping
    3. Binary application desktop
    4. On-demand desktop

    Answer:

    A. Application virtualization delivers software using a virtual structure, which allows an organization to make a needed application available across multiple devices without having to install it on each of these devices. This might apply to any platform the organization needs, whether a desktop computer or a mobile device.
23. In setting up and configuring client-side virtualization, what is necessary to consider before purchasing computing and storage hardware?

    1. Resource requirements
    2. Management response
    3. Resale value
    4. Physical size

    Answer:

    A. Before purchasing hardware of a host system to support a number of virtual systems, it is wise to consider the resource requirements of those virtual systems. The more virtual systems a single hardware system supports, the more resources are needed.
24. What must be defined when wanting to maintain confidentiality, integrity, and availability of the system resources, and should be a part of the decision when choosing a cloud solution?

    1. Scalability
    2. Emulation
    3. Elasticity
    4. Security requirements

    Answer:

    D. When wanting to maintain confidentiality, integrity, and availability, security requirements and regulations must first be defined. A company can then consider if an Internet cloud solution would be appropriate.
25. In setting up and configuring client-side virtualization, what is necessary to consider before configuring a VLAN?

    1. Network requirements
    2. Emulation demands
    3. Cloud service providers
    4. Storage capacity

    Answer:

    A. Network requirements dictate the need for and configuration of virtual local area networks (VLANs). A VLAN is a network design feature that isolates network traffic by the switch port. Just like a physical machine, a virtual machine must be compatible with the network it is intended to run on.
26. When considering how efficiently a hypervisor runs, which of the following is best when it is minimized?

    1. Storage
    2. Emulator requirements
    3. Memory
    4. Scalability

    Answer:

    B. Emulator requirements should be as small as possible in order to keep resources free for use by the host and guest operating systems. Generally speaking, more storage and RAM lead to greater scalability, which means you can install more virtual machines on the same physical box.
27. Which of the following is not considered to be a major category of cloud computing?

    1. SaaS
    2. PaaS
    3. IaaS
    4. XaaS

    Answer:

    D. While software as a service (SaaS), platform as a service (PaaS), and infrastructure as a service (IaaS) are widely considered to be the major categories of cloud computing, everything as a service (XaaS) is not.
28. Which of the cloud computing models combines on premises infrastructure and Internet accessed resources?

    1. Private cloud
    2. Public cloud
    3. Hybrid cloud
    4. Combined cloud

    Answer:

    C. A private cloud pools the on premises resources of a company for use within the company; there is no Internet component. A public cloud is owned by a third-party provider who delivers resources, including storage, platforms, and software via the Internet. A hybrid cloud combines the two other forms, where some resources are on premises and others are available over the Internet. The on premises resources may provide more control over data, while the Internet resources offer on-demand scalability. Different types of data could be kept in different locations depending on the company's needs.
29. With today's more mobile workforce, what technology provides the benefits of centralized security, ease of configuring new desktops for remote workers, and scalability regardless of where a user is or works from? (Choose the best answer.)

    1. IaaS
    2. SaaS
    3. VDI in the cloud
    4. VDI on premises

    Answer:

    C. Virtual desktop infrastructure (VDI) in the cloud, sometimes called desktop as a service (DaaS), allows a network admin to easily and almost immediately configure desktops for new users, even if they are in a remote location halfway around the world. Infrastructure as a service (IaaS) provides the physical computing, network, memory, and storage resources enabling the cloud provider's customers to set up virtual servers and networks in the cloud. IaaS can also provide server software and databases, although not all providers do. Think of IaaS as renting the entire network structure. The cloud provider is responsible for resource provisioning and maintenance needed for the organization's infrastructure. Software as a service (SaaS) provides applications but not necessarily desktops. VDI on premises offers similar advantages, but scalability is limited by local servers.
30. A group of real estate agents has realized that they have similar computing resource needs. They've reached out collectively to your IT services company and asked if there is a solution that will let them pool their resources and save money, possibly sharing industry-specific software, but still have their servers and information held securely and locally. What will you recommend?

    1. Community cloud
    2. Public cloud
    3. Private cloud
    4. VDI in the cloud

    Answer:

    A. A community cloud is the solution for such situations. It allows shared cloud resources to a limited group of people or companies. The group can benefit from economies of scale but keep their resources separate from other organizations. They could even share in joint projects. Their servers could be in a data center or stored locally by one of the members. The group will have more control than they would over a public cloud but could share the maintenance costs of their cloud. A community cloud is similar to a private cloud, but with multiple members.
31. Which of these terms is a benefit of cloud computing that means the information is available constantly, regardless of location?

    1. Shared resources
    2. High availability
    3. Rapid elasticity
    4. File synchronization

    Answer:

    B. While all of the items listed are advantages of using cloud-computing, high availability means that data and applications are available around the clock, regardless of the users' location. Shared resources often lead to lower costs and rapid elasticity. File synchronization means that users' files are updated with the newest changes whether they're working at home or in the office.
32. A graphic artist at your company needs to manipulate files in both Linux and Windows environments. You, as the IT support person, want as few physical machines to support as possible. What technology allows both OSs to run on a single machine?

    1. File sharing.
    2. Cross-platform virtualization.
    3. Dual-boot system.
    4. It can't be done.

    Answer:

    B. Configuring a virtual machine using VMM software whose features include cross-platform virtualization will allow you to configure multiple desktop platforms on one physical machine regardless of the host OS. Dual-boot systems may not work well together, depending on the operating systems being used. Sharing files isn't really the question being addressed; using different operating systems is.
33. You've received a file from a salesperson who recently separated from your company. You want to open this file and see what it contains without subjecting your computer to possible malicious content. What Windows 10 Pro feature can you turn on that will create a protected environment for opening this file?

    1. Shared Files
    2. System Information
    3. Sandbox
    4. File Manager

    Answer:

    C. In general terms, a sandbox is an isolated test environment separate from your network where you can “play” with applications and settings without worrying about negative effects on your network or computers. Sandbox is also a feature that can be enabled in Windows 10 and Windows 11 Pro and higher editions. When launched, it opens a separate instance of the Windows operating system running as a virtual machine on your Windows desktop. A file can be opened in that virtual machine to help protect your computer against malicious code. When the sandbox is closed, anything running in it is discarded.
34. Your friend is a software developer. They have Windows 10 Pro installed on their SOHO computer. They are creating an application that needs to run smoothly on both Windows and Linux machines, so it will need to be tested in both of those environments. What would be the best solution for your friend?

    1. Windows 10 sandbox
    2. Dual-boot system
    3. Two separate machines
    4. Virtual machines on their PC

    Answer:

    D. Your friend will need to run both OSs to test the software. A Windows 10 sandbox will protect their host OS from any problems the application might cause, but it won't let them test the application on a Linux OS. Dual-boot systems are clunky at best, and they require rebooting between OSs. Running two computers would cost more in utilities and hardware, not to mention precious office space. The best solution for your friend is to install virtual machines on their office PC. This would enable them to test in either Linux or Windows without shutting the PC down between, saving time while making corrections. It will also protect their machine against unintentional bad code that could otherwise cause damage.
35. A manufacturing client has a piece of equipment that is running on a Windows 7 OS. The equipment-specific software won't run on any other OS, and the client is concerned about what they will do when the Windows 7 computer inevitably crashes. Cost is always a concern. What is a viable, cost-effective solution for your client?

    1. Have the programmers rewrite the code to run on Windows 10.
    2. Migrate the software to a Windows 7 VM running on a Windows 10 host.
    3. Wait until the hardware crashes, then shut the equipment down permanently.
    4. Tell the client they need to upgrade their manufacturing equipment to something more modern as soon as possible.

    Answer:

    B. Developing software for a specific manufacturing function is often costly and time-consuming, so a manufacturer might want to keep that equipment and software running as long as possible. If the equipment is doing the job they need it to do, they will be disinclined to upgrade to something new. Shutting the equipment down when it fails may spell disaster for the company. The best option here is to prepare a Windows 10 PC to run the legacy OS and software within a virtual machine, and test the software. Then, during a planned shutdown, transfer the control of the manufacturing machine over to the new PC with the virtual machine, and, of course, make sure you have an image to rapidly deploy if the new machine fails in the future.
36. Why would a company prefer to run multiple applications each on its own VM rather than on a single server?

    1. Security
    2. Scalability
    3. Less maintenance
    4. Less cost

    Answer:

    A. The advantage of having applications each running in their own virtual machine is that if one application's or VM's security is penetrated, the others may still be secure. Scalability would still be limited to the resources of the server. The hardware maintenance would be the same, but the security maintenance might actually be more; however, being able to set up different access for each machine may simplify security configuration. The cost would actually be more because a separate license would be needed for each OS running in its own virtual machine.
37. Which of the following would essentially be the same whether running an OS on a virtual server or a physical server? (Choose two.)

    1. Security configuration
    2. Hardware
    3. Licensing
    4. Portability

    Answer:

    A, C. Regardless of whether a server is physical or virtual, it will need the same security configuration, and a license must exist for every virtual server just as it must for every physical server. While RAM and storage requirements would be the same, one of the advantages of using a virtual machine is being able to put more than one server on a single piece of computer hardware, so overall hardware cost would be less, and maintaining that hardware would be less expensive. Virtual servers are much more portable than physical servers, meaning they can easily be moved from one piece of hardware to another.
38. Which cloud model offers the greatest control over data and security?

    1. Private cloud
    2. Public cloud
    3. Hybrid cloud
    4. Community cloud

    Answer:

    A. While each model has its advantages, if security is the greatest concern, then a private cloud is the best solution. Public, hybrid, and community clouds all involve other entities, which may introduce additional potential security problems.
39. You are a manager in a call center that employs 300 people who may be working any of three shifts on any given day, taking whichever of your 100 seats is available. Company regulations require that all information remain hosted locally. What technology can you use so that their files, folders, and desktop icons all appear the same regardless of which computer they log on to?

    1. On-demand desktop
    2. VDI in the cloud
    3. Desktop emulation
    4. VDI on premises

    Answer:

    D. A virtual desktop infrastructure (VDI) moves the desktop icons, files, and folders to a server instead of the desktop originating from the local machine. When the desktop experience is hosted on a centralized server location, the icons, files, and folders are the same regardless of where a user logs on. VDI on premises hosts the desktop on a local server, whereas VDI in the cloud hosts the desktop on a remote server.
40. Which of these is not an advantage of cloud computing?

    1. Reduced capital expenditures
    2. Frees IT employees time for other needs
    3. Complete control over data
    4. Rapid elasticity (dynamic growth)

    Answer:

    C. Cloud computing has many advantages, including (a) reduced capital expenditures, which can help growing companies and (b) relieve IT personnel of infrastructure management so that they can focus on other objectives such as customer support, and (c) rapid elasticity, which means a company can grow its IT infrastructure on a moment's notice as needed. Also, adding new employees can be easier with cloud computing. There are a few downsides, though. Some of them are that someone else has control of your data, fees can be surprising when usage is more than expected, and moving from one IaaS provider to another might be difficult. There are more advantages and disadvantages than can reasonably be listed here.
