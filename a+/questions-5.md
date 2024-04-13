# Questions

1.  You want to transfer files from your computer to a remote server. To do this, you want to connect to a shared directory on the server and copy the files. Which command-line utility will allow you to do this?

    1. `netstat`
    2. `net`
    3. `netshare`
    4. `netdom`

    Answer:

    B. Depending on the version of Windows you are using, `net` can be one of the most powerful commands at your disposal. While all Windows versions include a `net` command, its capabilities differ based on whether it is used on a server or workstation and the version of the operating system. Commonly `net share` is used to create shared folders, and `net use` is used to connect to shared resources. The `net user` command allows administrators to create and manage user accounts. `netstat` shows what sockets (IP address plus port) are being used and by which protocols. `net share` is a valid command for managing shared resources, but `netshare` and `netdom` are not valid commands.
2.  A technician is troubleshooting a computer that occasionally will not read data from the hard drive. What should they try first?

    1. Run Defragment and Optimize Drives.
    2. Run `chkdsk` at a command prompt.
    3. Format the hard drive and reinstall the OS.
    4. Replace the hard drive.

    Answer:

    B. It's possible that the hard drive has some bad sectors, so run `chkdsk` to scan the drive and attempt to repair them. If that doesn't work, formatting is the second option, and replacing the drive is the third. If your drive is getting read/write errors, having an extra hard drive on hand would be wise.
3.  You have replaced a failed hard drive and need to prepare the new drive for data storage. Which utility will you use first?

    1. `format`
    2. `chkdsk`
    3. `diskpart`
    4. `gpupdate`

    Answer:

    C. The `diskpart` utility lets the user see and manage partitions on the computer's hard drives. Because of the enormous power it holds, the user must have administrator status to run `diskpart`. Once a partition is created, the `format` command will set up the filesystem on the new volume. The `chkdsk` command verifies the disk integrity, and `gpupdate` forces Group Policy changes to take effect immediately.
4.  You are at a Windows computer with the Command Prompt open. You believe that a user is improperly accessing files on a shared folder named `docs`. On the Windows computer, the `D:\userfiles` folder is shared as docs. Which command will immediately stop the sharing of this folder?

    1. `net share D:\userfiles /delete`
    2. `net share D:\userfiles /stop`
    3. `net share docs /delete`
    4. `net share docs /stop`

    Answer:

    C. The `net share` command is used to share folders on a network as well as stop sharing folders. The proper syntax to share a folder is `net share <`_`share name`_`>=<`_`drive letter`_`>:<`_`path`_`>`. To stop sharing, use `net share <`_`share name`_`> /delete`. You must be running the Command Prompt as an administrator to create and delete shares.
5.  You want to use BitLocker to encrypt the company president's laptop drive, but when you go into Control Panel to find it, it isn't there. What Windows 10 edition does this computer have?

    1. Home
    2. Pro
    3. Pro for Workstations
    4. Enterprise

    Answer:

    A. Windows 10 Home edition does not offer BitLocker as an option. BitLocker is available in the Pro, Pro for Workstations, and Enterprise editions.
6.  Which of the following Windows editions support ReFS (Resilient File System)? (Choose two.)

    1. Home
    2. Pro
    3. Pro for Workstations
    4. Enterprise

    Answer:

    C, D. Resilient File System (ReFS) is a feature available on Windows Pro for Workstations and Windows Enterprise editions. ReFS will detect when data on a mirrored drive has been corrupted and will use a healthy copy of the data on other drives to attempt to correct corrupted data and protect data.
7.  You just purchased a new computer that has four CPUs. What edition of Windows will you need, at a minimum, to take advantage of the computer's processing capability?

    1. Home
    2. Pro
    3. Pro for Workstations
    4. Enterprise

    Answer:

    C. Windows Pro for Workstations is designed so that users can take advantage of the capabilities of high-end workstations. Windows Home edition can support one physical processor, Windows Pro can support up to two physical processors, while Windows Pro for Workstations can support up to four physical processors.
8.  An employee wants to bring their Windows device to use at work. At work they will need to log into a domain. Which reason below will prohibit the employee from using their device on the domain?

    1. Their device only has one processor.
    2. Their device OS is Windows Home.
    3. Their device only has 8 GB of RAM.
    4. Their device must be Windows Enterprise.

    Answer:

    B. Windows Home does not have the capability of joining a domain, so the employee will not be able to use their personal device. Windows Pro, Pro for Workstations, and Enterprise editions are all able to log into a domain. The number of processors and amount of RAM are irrelevant to the ability to log into a domain.
9.  One of your technicians needs to use the Task Manager utility. What are ways they can open Task Manager? (Choose two.)

    1. Press Ctrl+Alt+Delete and then click Task Manager.
    2. Press Ctrl+Shift+T.
    3. Press Ctrl+Alt+T.
    4. Press Ctrl+Shift+Esc.

    Answer:

    A, D. Task Manager is a powerful tool that works in all versions of Windows, although it has different capabilities in different versions. In Windows 10 and 11 it allows you to shut down nonresponsive applications; view performance of CPU, memory, disks, Wi-Fi, and GPUs; as well as show application usage history, services, and programs that are launched at startup, users who are attached to the system, and other useful information.
10. You need to configure Internet connections on a Windows workstation. Which tabs of the Internet Options utility in Control Panel would you use to set the home page and enable the pop-up blocker?

    1. Connections, Security
    2. General, Security
    3. General, Privacy
    4. Connections, Privacy

    Answer:

    C. The Internet Options utility in Windows Control Panel has six tabs that allow you to configure how your browser interacts with the Internet. The six tabs are General, Security, Privacy, Content, Connections, Programs, and Advanced. Not all versions of Windows have the Content tab. The General tab allows you to change the home page whereas the Privacy tab has a Turn On Pop-up Blocker option.
11. A network connection doesn't seem to be working as it should. You've verified that the cables are good from end to end. Where can you quickly look in the OS to see if there is a problem with the onboard NIC driver?

    1. Device Manager
    2. Programs and Features
    3. File Explorer Options
    4. Ease of Access

    Answer:

    A. A quick look at Device Manager is often all you need to troubleshoot a problem with an onboard device. If the device drivers aren't installed for the device, you'll see a yellow exclamation point in Device Manager. Programs and Features allows the user to add, remove, or troubleshoot installed programs (the options will change by program) and add Windows features that are not yet installed. The File Explorer Options utility changes how File Explorer works such as showing hidden files or extensions and other view options. Ease of Access provides alternative ways to interact with the computer for differently abled users.
12. A salesperson in your company travels regularly to foreign countries, through different time zones. They have asked you if there is a way to set their Windows 10 PC so that it will always show the time and date for their location. How can this be done?

    1. In Windows Settings, choose Time & Language, then Date & time, and select Set time automatically.
    2. In Control Panel, choose Date and Time, then select Set Time Zone Automatically.
    3. In Windows Settings, choose Date And Time, then select Synchronize Your Clock.
    4. In Windows Settings, choose Time & Language, then choose Date & time, and select Set time automatically and Set time zone automatically.

    Answer:

    D. To always show the time and date correctly for the salesperson's location, you would need to enable both Set time automatically and Set time zone automatically, as shown in the graphic. Synchronize your clock would work in the moment but will not automatically change the time and time zone as the salesperson travels. The Date And Time utility of Control Panel will let you change the date and time, but it does not have a setting for automatically changing them as you move from place to place. In Windows 11 Time And Language appears as Time & Language, but otherwise the choices are the same.

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/bapp01uf001_0.jpg?width=821" alt=""><figcaption></figcaption></figure>
13. One of your Windows 10 users has limited eyesight and has asked you to enable voice activation for as many applications as possible. Where can this be done?

    1. In Control Panel, Default Programs
    2. In Windows Settings, under Privacy, Notifications
    3. In Windows Settings, under Privacy, Voice Activation
    4. In Control Panel, Indexing Options

    Answer:

    C. Voice activation, found under Privacy in Windows Settings will allow the user to turn on microphone access and choose which apps are allowed to use voice activation, even when the device is locked. The choices are slightly different in Windows 11. In Windows Settings, choose Privacy & security, then Speech. The setting is on by default. The Default Programs app of Control Panel allows you to manage default applications for opening types of files such as photos or mail by opening those settings in Windows Settings. By choosing Privacy, then Notifications in Windows Settings, you can allow or deny applications to access your notifications. Control Panel's Indexing Options looks at words in files and the files' metadata to provide faster file searches.
14. You are working with a customer that has a small workgroup (peer-to-peer) network with Windows 10 PCs. The employee computers have a program that requires using the X: drive. Several computer users need to be able to access this drive, which is actually a shared folder located on the manager's PC. What can you do to make this drive available for other computers to access as drive X:? (Choose two.)

    1. On each client computer, open File Explorer, click This PC, then click Map network drive. Choose drive letter X, then navigate to the shared resource.
    2. On the manager's PC, navigate to the shared folder, then right-click it and choose Map network drive.
    3. On the manager's PC, ensure that each user who will connect to the manager's PC has a user account.
    4. On the client computer, create a folder called `Drive X:`, then on the manager's PC, map `Drive X:` to that folder.

    Answer:

    A, C. In a workgroup (peer-to-peer) network, you would first need to ensure that each person who will be using the shared resource has a username and password on the manager's computer. The resource would then be shared on the manager's PC, and on each employee's computer, go into File Explorer, click This PC, then Map network drive and follow the onscreen prompts to map drive X: to that shared resource. The choices in Windows 11 are slightly different. In File Explorer, after clicking This PC you would click the three dots in the ribbon then choose Map network drive.
15. You are setting up a network for a very small company. They have a total of 10 computers running a mix of Windows 10 Home and Windows 10 Pro computers, and they have a network-attached printer. What will you use to allow them to share files and their printer?

    1. Domain
    2. Workgroup
    3. Homegroup
    4. Crossover cables

    Answer:

    B. In order to have a domain, you would need a domain controller (DC), for which the company would need Windows Server software installed on a network connected computer. They only have Windows 10 workstations. Homegroups were a networking scheme that shared a computer's libraries with other people on the same Homegroup, but Homegroups are no longer an option. Crossover cables are not a practical way to share anything among 10 computers. By default, the computers would belong to the workgroup named workgroup. Each computer that is sharing a resource would need to have the user they are sharing with listed on that computer, then the person sharing information could right-click a folder and choose Give access to, then Specific people and choose who they want to share that particular resource with. Workgroups are great for small groups of people, but if there are more than 20 or 30 people in the group, you'll likely want to move up to a DC and centralized security.
16. A user's Windows workstation seems to be using an excessive amount of memory. Which management tool could you use to identify the application that is causing the problem?

    1. Performance Monitor
    2. Computer Management
    3. Windows Memory Diagnostics
    4. Processes tab of Task Manager

    Answer:

    D. One of Task Manager's many capabilities is allowing you to see what resources (memory, CPU, GPU, network, and disk) are being used by application, and it allows you to end the process or the entire process tree to free up those resources. Performance Monitor will show resources used but not by application. Computer Management gives access to several other resources, but not Task Manager, whereas Windows Memory Diagnostics is used to test the health of RAM modules.
17. The CEO will be attending several meetings whose discussions must remain confidential. They want to ensure that the microphone on their Windows 10 PC is not available while they are using certain apps. Where can these settings be configured?

    1. In Windows Settings, choose Privacy, then Microphone.
    2. Device Manager.
    3. Computer Management.
    4. In Windows Settings, choose Personalization.

    Answer:

    A. In Windows Settings, choosing Privacy, then Microphone opens a window that provides granular settings for microphone use, including which apps can use the microphone. Device Manager could be used to disable the microphone, but it would be for all purposes. Computer Management provides access to several tools, but not granular microphone settings. In Windows Settings, Personalization options allow the user to change settings such as background, colors, and lock screen. In Windows 11 the only difference is that you would choose Privacy & Security, not Privacy.
18. You are manually configuring IPv4 addresses on a computer. The IP address is `200.100.1.10`, and the network number is 200.100.0.0. What is the appropriate subnet mask for this computer?

    1. `200.100.0.0`
    2. `255.255.0.0`
    3. `0.0.255.255`
    4. `192.168.0.0`

    Answer:

    B. The best way to understand IPv4 addressing is to convert the IP address and subnet mask to binary numbers. This is essentially what the operating system is looking at when determining the network and host portion of an IP address. What we see as dotted decimal notation is seen by the computer as four sets of eight binary bits (either a 1 or a 0). In the subnet mask, a binary 1 indicates that the position of that bit is part of the network number and a 0 indicates that it is part of the host number. Network numbers always go consecutively from left to right with no breaks between. Eight binary bits that are all ones (11111111) equates to 255 in decimal, so the maximum value of a subnet mask's octet is 255. Options A and D are invalid subnet masks because for a number to exist in the second octet from the left, the first octet would need to be all 1s, which is equal to decimal value 255. Option C is an invalid subnet mask because the ones indicating the network number would be in the first octets reading from left to right, not the last. If we then compare the IP address of `200.100.1.10` to the subnet mask in option B, `255.255.0.0`, we can see that the first two octets are network number and the last two are host numbers, making the network number `200.100.0.0` for that IP address and subnet mask combination. The host computer is then `0.0.1.10`.
19. You are configuring a Windows client computer on a network that has a DHCP and DNS server attached. Where will the computer get its IP address and subnet mask?

    1. You will manually configure them in Windows Settings by choosing Personalization.
    2. You will manually configure them in Windows Settings, by choosing Network & Internet.
    3. It will automatically get them from the DHCP server.
    4. It will automatically get them from the DNS server.

    Answer:

    C. The default setting for obtaining an IP address is automatic, which means that the computer will look for a DHCP server to assign an IP address and subnet mask. No manual configuration is required, but in Windows 10, you can verify that the connection is set to automatically obtain an IP address, as shown in the graphic, by following these steps: Open Windows Settings, then click Network & Internet. Choose Change adapter options, and right-click the network connection in question. Then choose Properties, click Internet Protocol Version 4 (TCP/IPv4), and click Properties. The process is the same for IPv6, except that you would choose IPv6 instead of IPv4. This can also be done through Control Panel by clicking Network and Sharing Center instead of Network and Internet, then the next steps are the same. In Windows 11, Windows Settings, choose Network & Internet, click Properties of the active network connection at the top of the page. This will bring you to the network's configuration page where you can ensure that the setting for IP assignment is configured to Automatic (DHCP). The Control Panel options for Windows 11 are the same as Windows 10.

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/bapp01uf002_0.jpg?width=821" alt=""><figcaption></figcaption></figure>
20. You have been told to configure a static IP of `110.110.1.5` for a server. This server will need to be able to access the Internet. Which one of the following is not a required setting to configure?

    1. Default gateway
    2. IP address
    3. Proxy server
    4. Subnet mask

    Answer:

    C. An IP address on a device can be either dynamic or static. In a static IP address, the minimum amount of information that needs to be configured is the IP address, subnet mask, and, if the computer will access the Internet or other networks, a default gateway. A proxy server is an added security measure between a device and the Internet. It is used to translate between protocols and filter out certain types of traffic such as keeping inappropriate websites out and confidential data in the network.
21. Considering the graphic, what is most likely the IP address of a router?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf003_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. `192.168.1.229`
    2. `192.168.1.1`
    3. `48-45-20-C1-12-BD`
    4. `255.255.255.0`

    Answer:

    B. Often on a network, especially a smaller one, the router will serve multiple purposes. In this scenario it is the default gateway, the DHCP server, and the DNS server. `192.168.1.1` is the address of the router, gateway, DHCP server, and DNS server. `192.168.1.229` is the local computer's IP address. 48-45-20-C1-12-BD is the MAC address, which is embedded in the computer's network interface card (NIC). `255.255.255.0` is the subnet mask.
22. You're creating a network diagram for a company that has just hired you as a network admin. Which of the following could be the default gateway on the company's network? (Choose two.)

    1. Web server
    2. Proxy server
    3. Router
    4. Switch

    Answer:

    B, C. Web servers provide web pages to users sometimes inside but often outside of the company by answering HTTP (Hypertext Transfer Protocol) or HTTPS (HTTP Secure) requests. They are often separate from the main network on a screened subnet for security reasons. A proxy server can serve as a gateway for a network because, if one exists, traffic will go through the proxy server before going into or out of the network. In the absence of a proxy server, the router serves as a gateway, forwarding traffic on to the next network or receiving external traffic and sending it to the proper device inside a network. A switch is an internal networking device that provides a central connection point for network nodes and uses the node's MAC (Media Access Control) address that is found on the NIC (network interface card) to send packets to the proper destination.
23. What is the purpose of a subnet mask?

    1. Identifies the network portion of an IPv4 address
    2. Identifies the network portion of an IPv6 address
    3. Masks (hides) part of the IP address from a hacker
    4. Masks (hides) the host number from a hacker

    Answer:

    A. In IPv4 networking, a computer system will compare the subnet mask to the IP address to identify the network and host number of the IP address. IPv6 addresses don't use a subnet mask. IPv6 addresses consist of eight segments. The first three are a site prefix, the fourth is the subnet ID, and the last four segments are the interface ID, which is essentially the host address. The subnet mask doesn't hide anything.
24. You've been asked to help with a network for a company that has 50 computers. They've been using workgroups, but it is getting too difficult. There is an assortment of Windows editions on the computers, including Windows Home, Windows Pro, and Windows Pro for Workstations. What will you do to set up their new network? (Choose two.)

    1. Upgrade all the Windows Home PCs to Windows Pro.
    2. Install a server with Active Directory.
    3. Downgrade all the Windows Pro for Workstations to Windows Pro.
    4. Upgrade all the workstations to Windows Enterprise.

    Answer:

    A, B. A network with that many computers (typically more than 10) needs a domain for security management. The Windows Home edition PCs can't log into a domain, so they would need to be upgraded to at least the Pro edition. It's not necessary to upgrade them to Pro for Workstations or Enterprise editions.
25. You work for a multinational corporation that is using Windows 10 laptops. All the company laptops are configured to use United States English, but a worker that speaks Bajan (Barbados English) would prefer to see apps and websites in their native language. Is this possible?

    1. No, this is not possible.
    2. Yes, Add English (Barbados) in the Control Panel, Programs and Features utility.
    3. Yes, add English (Barbados) in Windows Settings, Time & Language, Language section.
    4. Yes, but it will require reinstalling the OS in Bajan.

    Answer:

    C. It is possible to view apps and websites in many languages and dialects. In Windows Settings, choose Time & Language, then Language (see the graphic). Click Add a language to choose the appropriate language to install, then move it to the top of the language list. Apps and websites that support that language will appear in the language that is at the top of the list. The language may require downloading a Language pack. Icons to the right of the installed language are used to indicate what is available in that language. In the graphic, to the right of English (United States) from left to right the icons indication options available are as follows: Display language, Text-to-speech, Speech recognition, Handwriting, and Spell-check.

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/bapp01uf003_0.jpg?width=821" alt=""><figcaption></figcaption></figure>
26. A Windows workstation has an application that appears to be locked up, but the keyboard is responsive in other applications. What system tool can you use to terminate the nonresponsive application?

    1. Event Viewer
    2. Task Manager
    3. Computer Management
    4. `msconfig.exe`

    Answer:

    B. The Processes tab of Task Manager will allow you to terminate the nonresponsive application. Event Viewer keeps a log of security, application, and system events. Computer Management gives access to several other resources, but not one that lets you end wayward applications. The `msconfig.exe` application launches System Configuration, which gives you access to boot configuration settings, running services, and links to other Windows tools.
27. Which of the following Control Panel utilities enables configuration of a proxy server?

    1. Internet Options
    2. File Explorer Options
    3. Device Manager
    4. Security and Maintenance

    Answer:

    A. In Control Panel, choosing Internet Options, selecting the Connections tab, and then clicking LAN settings will take you to a window that enables configuration of a proxy server. Proxy server settings can also be configured through Windows Settings by choosing Network & Internet and choosing Proxy. The File Explorer Options utility is used to configure how files and folders are viewed, and how searches are conducted. Device Manager is a great utility to use when troubleshooting hardware issues, and the Security and Maintenance utility provides a quick way to see if security is configured on the PC and to see any recent messages.
28. Considering the graphic, what do you know about the network configuration of this computer? (Choose three.)

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf005_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. The PC is configured to obtain an address dynamically.
    2. This computer is getting its address from a DHCP server.
    3. The IPv4 address is a routable address.
    4. The internal network number is `192.168.1.0`.

    Answer:

    A, B, D. The computer is configured to obtain the address dynamically because the graphic says Yes next to DHCP Enabled. If it was set to obtain an address dynamically but not able to reach the DHCP server, the operating system would have obtained an address using APIPA (Automatic Private IP Addressing) and would have been in the range that begins with `169.254.0.0`, so this PC is not being assigned an APIPA address. It is set to DHCP and getting an address that is not APIPA, so we know that it is getting its address from the DHCP server. Addresses in the `192.168` _`.x.x`_ range are nonroutable addresses, meaning that they can only be used internally. To reach the Internet they would go through a gateway (router) that has NAT (network address translation) enabled (essentially all modern routers use NAT). We know the network number is `192.168.1.0` and that the host address is `0.0.0.229` by comparing the IP address to the subnet mask.
29. Given the IP address of `fe80::308c:fee2:2abc:8337`, what do we know about this address? (Choose two.)

    1. It is an IPv4 address.
    2. It is an IPv6 address.
    3. The subnet mask is 0.
    4. It is not routable.

    Answer:

    B, D. IPv4 addresses are 32 bits long and consist of 4 octets, which is a group of 8 bits each, separated by a period (.) They are normally presented in dotted decimal notation, meaning each group of 8 bits is shown as a decimal number less than 256, with a period (.) between each number, such as `192.168.1.1`. IPv6 addresses are a 128-bit IP address presented as eight segments of four hexadecimal numbers each, separated by a colon (:). Where the hexadecimal number is 0 in any segment, it can be omitted and replaced simply by double colons (::). If consecutive segments are 0, they can all be replaced by a single set of double colons, but only one set of double colons can exist in any given address—otherwise you wouldn't be able to tell how many sets of zero are in each part of the IP address. In the example, `fe80::308c:fee2:dabc:8337`, the expanded address would be `fe80:0:0:0:308c:fee2:dabc:8337`. The first three segments (48 bits) are the site prefix, and the fourth segment (16 bits) is the subnet ID, also known as private topology or site topology. The site prefix and subnet number together constitute the subnet prefix. The last four segments (64 bits) are the interface ID, also sometimes called a token. The subnet ID in this case would be `0`. IPv6 addresses do not have a subnet mask. The value of the first octet, `fe80`, tells us that this number is a link-local address, an internal number only and not routable.
30. You see an IP address with /48 after it. What does the /48 tell you? (Choose two.)

    1. There are 48 PCs on this network.
    2. The prefix length is 48 bits.
    3. This network uses the IPv6 addressing scheme.
    4. This network uses the IPv4 addressing scheme.

    Answer:

    B, C. The IP address in question must be IPv6 because IPv4 addresses are only 32 bits long. The / indicates that the number behind it is the number of bits for the network address in IPv4 or the prefix length in IPv6, both of which identify the network number of an IP address. In IPv4 we call this CIDR (Classless Inter-domain Routing) notation.
31. Which of the following IPv6 address types are routable?

    1. Global unicast
    2. Link-local
    3. Loopback
    4. Unique local

    Answer:

    A. Global unicast addresses are routable, like IPv4 public addresses. That means that a global unicast address can be reached by any other PC on the Internet, unless you put security measures in place like a firewall. You would likely want a global unicast address on a web server, but not on your workstation. Link-local addresses can only be used to communicate with devices that are on the same local link. They will start with fe80 and are assigned in a manner similar to IPv4 APIPA addresses. The IPv6 loopback address is ::1, and is used for testing just like the loopback address in IPv4 (127.0.0.1). A unique local address is akin to an IPv4 private address. Unique local addresses are nonroutable, so a computer with only a unique local address and a link-local address (but no global unicast address) would need a router with IPv6 NAT in order to access the Internet.
32. You are on a Windows computer that is joined to a workgroup. You're going home and ready to shut your computer down but want to be certain that no one is using the shared files on the computer first. Where would you go to check?

    1. Task Manager
    2. Users and Groups
    3. Performance Monitor
    4. Control Panel ➢ Networking

    Answer:

    A. The Task Manager's Users tab provides information about any users that are connected to the local machine. The Users tab shows the user's identification and the resources that are being used by them. Right-click and choose Expand to see what they are using on your computer. You can also disconnect them from here, but it might be nicer to message them first.
33. You have a workstation with a 64-bit processor and no operating system. When you install an operating system on the workstation, which of the following is true?

    1. You can only install a 64-bit operating system.
    2. You can only install a 32-bit operating system.
    3. You can install either a 64-bit or 32-bit operating system.
    4. You can install a 64-bit operating system or a 32-bit operating system running in compatibility mode.

    Answer:

    C. With a 64-bit processor, you can install either a 32-bit or 64-bit operating system. A 32-bit system will not be able to take advantage of the full processing power of the 64-bit processor, though.
34. A customer has a PC from 2017 on which they would like to install Windows 10 Pro. What is the minimum processor speed they must have to install Windows 10 64-bit?

    1. 1 GHz
    2. 2 GHz
    3. 3 GHz
    4. 10 GHz

    Answer:

    A. Windows 10 minimum requirements are a 1 GHz or faster processor or SoC (System on a Chip), DirectX 9 or later with the WDDM (Windows Display Driver Model) 1.0 driver, and a minimum 800×600 display. For storage, the 32-bit version requires 16 GB and the 64-bit version requires 20 GB available for the OS. RAM requirements are 1 GB for the 32-bit operating system and 2 GB for the 64-bit operating system. Keep in mind that these are the absolute minimum requirements, and the OS will run but not as well as we have come to expect. In reality, a faster processor, more RAM, and more storage would be expected.
35. Which of the following is not a Windows 10 edition?

    1. Home
    2. Enterprise
    3. Pro Artist
    4. Pro Workstation

    Answer:

    C. Windows 10 is available in many different editions. The editions on the CompTIA A+ exam (for both Windows 10 and Windows 11) are Home, Pro, Pro for Workstations, and Enterprise. Other Windows editions (not on the CompTIA A+ exam) include Education, Pro Education, Windows 10 in S mode, Windows for IoT, and Windows 10 Team.
36. What information do you need to connect to a PC using Remote Desktop?

    1. The IP address of the PC
    2. The password to the network that the PC resides on
    3. The name under “How to connect to this PC” when Remote Desktop was enabled
    4. The password of the signed-on PC user

    Answer:

    C. To connect, all you need to know is the name of the device you're connecting to, but there are steps that must have already taken place. If you're using your smartphone to connect, you need Remote Desktop Mobile installed on the smartphone and Remote Desktop must be enabled on the target PC. Then you would simply open the app on your smartphone and type the name that appeared under “How to connect to this PC” when Remote Desktop was enabled on that PC.
37. You're troubleshooting a PC and want to see what ports TCP is connected on and the IP addresses of those connections. What command-line utility can you use to see statistics on network interfaces?

    1. `ping`
    2. `nbtstat`
    3. `nslookup`
    4. `netstat`

    Answer:

    D. The `netstat` command-line utility presents statistics related to the installed network interfaces. By default, on a Windows machine, running the command will display a list of connections and the associated protocol, the source and target address, and the current state of the connection. `Ping` is used to test connectivity between two computers, `nbtstat` is used for troubleshooting NetBIOS over TCP/IP, and `nslookup` is used to query a DNS server.
38. A new technician asked you how to use a Windows command. In the spirit of sharing knowledge with others, you show them how to get help on many commands instead of just one. Which one of the following does not work with any commands?

    1. `help` `[`_`command name`_`]`
    2. `[`_`command name`_`] help`
    3. `[`_`command name`_`] /?`
    4. `/? [`_`command name`_`]`

    Answer:

    D. The `/? [`_`command name`_`]` syntax simply does not work. The CompTIA A+ objectives list `[`_`command name`_`] /?`, but there are other ways to get help at a command prompt. Typing **`help`** and pressing Enter at a command prompt will provide a list of commands that `help` can help you with. Armed with that information, you can type **`help [`**_**`command name`**_**`]`**, for example, **`help xcopy`**, and you will see the syntax, switches, and explanations for how the command works. Some commands, for example, `sfc`, will not work with that help syntax. To find help with `sfc`, you would type **`sfc /?, sfc /help`** or **`sfc help`**, but none of those options work with all commands. For example, `gpresult /?` works, but `gpresult /help` will tell you that `/help` is an invalid option. Remember that the option CompTIA wants you to know is `[`_`command name`_`] /?`. There are upward of 200 commands supported by Windows 10 and Windows 11. CompTIA's A+ objectives list just a few, so focus on those.
39. Which Windows utility allows you to view error messages generated by system events, applications, or login failures?

    1. System Information
    2. Windows Defender
    3. Event Viewer
    4. Disk Management

    Answer:

    C. Event Viewer (`eventvwr.msc`) is a Windows tool, available in most versions, that allows you to view application error logs, security audit records, and system errors. System Information (`msinfo32.exe`) shows a plethora of information about the hardware and software of a system, but it doesn't keep a log of changes. It provides static information available at the time you launch the program. Windows Defender is a Control Panel utility that provides a software firewall for the local computer. Disk Management (`diskmgmt.msc`) is a graphic utility for creating and formatting volumes on any physical drives attached to the system. Worth noting is that Disk Management shows you the physical disks attached to the system and their volumes, whereas opening File Explorer and choosing This PC shows only the logical volumes.
40. To learn how much RAM is in this system, what command did you type in the search bar and launch to quickly bring up the window shown in the graphic?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf006_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. `msinfo32.exe`
    2. `resmon.exe`
    3. `msconfig.exe`
    4. `devmgmt.msc`

    Answer:

    A. The screen shown is System Information. It quickly provides a snapshot of the system's hardware and software, including the OS version, RAM, processor, motherboard, and much, much more. The program to launch it is `msinfo32.exe.` Resource Monitor's program name is `resmon.exe.` Unlike System Monitor, Resource Monitor is changing every moment, alerting you to resources that are overused or experiencing difficulty. System Configuration (`msconfig.exe`) has been appearing in Windows operating systems for many years, but Its features have changed over time. In Windows 10 and Windows 11, this utility is used to control how Windows boots up and to provide quick access to other Windows tools. Finally, `devmgmt.msc` is Device Manager, which should be your go-to app when resolving hardware issues. From there you can update or install drivers, see what isn't working, and disable hardware if need be.
41. You find that you are often using System Configuration, Disk Cleanup, and Event Viewer. What Windows 10 Control Panel utility gives you quick access to these and more tools?

    1. Computer Management
    2. Resource Monitor
    3. Administrative Tools
    4. Task Scheduler

    Answer:

    C. Administrative Tools, which can be found in the Windows 10 Control Panel, has many of the computer management tools that are used to maintain and troubleshoot computer systems, not just the ones listed in this question. Computer Management is a Microsoft Management Console (MMC) that contains other tools as well. In it you can find Task Scheduler, Even Viewer, Shared Folders, Performance, Device Manager, and Disk Management, as well as Services and Windows Management Instrumentation (WMI) Control. In Windows Pro and above editions Computer Management also contains Local Users and Groups. Resource Monitor shows resources being used by process in real time, and Task Scheduler is just as the name sounds—it can be used to schedule other applications, even batch files, to run based on time or other predetermined events. Administrative Tools is not available in Windows 11, but the other tools listed in this question are.
42. Your manager has a laptop running Windows. They want to configure the laptop so that when it is on battery power, the display shuts off after five minutes of inactivity. When the laptop is plugged in, the display needs to stay active for up to 45 minutes of inactivity. Which Control Panel utility is used to configure these settings?

    1. Power Options
    2. Computer Management
    3. Performance Monitor
    4. System Configuration

    Answer:

    A. A power plan needs to be created with the user's desired settings. This is done in the Power Options utility of Control Panel. Different options, such as Hibernate or Standby, can be configured for when the laptop is on battery power versus when it's plugged in. There are also power settings in Windows Settings, but they are not listed in the CompTIA A+ objectives.
43. You need to work at a command prompt on a Windows PC. When you open the prompt, you are at `C:\window\system32`. You need to work on the second partition, which is listed as drive D:. How will you navigate to drive D:? Assume you press Enter after the command.

    1. `root D:`
    2. `D:`
    3. `cd D:`
    4. `cd D:\`

    Answer:

    B. The way to change to a different drive is to type the drive letter and a colon, such as `D:`, and press Enter. `cd` is the change directory command. It can take you to a different directory or change the working directory on a different drive but cannot take you to a different drive. `root` is not a Windows command.
44. Which Windows 10 Editions support up to four CPU sockets? (Choose two.)

    1. Home
    2. Pro
    3. Pro for Workstations
    4. Enterprise

    Answer:

    C, D. Windows Pro for Workstations and Enterprise editions support up to four physical CPU sockets and 6 TB of RAM. The Home edition supports 128 GB of RAM and one CPU socket whereas the Pro edition supports 2 TB of RAM and a maximum of two CPU sockets.
45. You have a workstation with a 32-bit processor and no operating system installed. When you install an operating system on the workstation, which of the following is true?

    1. You can only install a 32-bit operating system.
    2. You can install a 64-bit operating system but it will run in compatibility mode.
    3. You can install either a 32-bit or 64-bit operating system and either will run fine.
    4. You can install a 64-bit operating system but it will only run half as fast.

    Answer:

    A. A 32-bit processor doesn't have the capability to run a 64-bit operating system in any mode. It also won't be able to run a 64-bit program. It simply doesn't have a wide enough data path.
46. You are installing the Windows 10 Home 64-bit operating system on a friend's computer. What is the minimum storage space that must be available for the OS installation?

    1. 1 GHz
    2. 2 GHz
    3. 16 GB
    4. 20 GB

    Answer:

    D. Windows 10 minimum requirements are a 1 GHz or faster processor or SoC (System on a Chip), DirectX 9 or later with the WDDM (Windows Display Driver Model) 1.0 driver, and a minimum 800×600 display. For storage, the 32-bit version requires 16 GB, and the 64-bit version requires 20 GB available for the OS. RAM requirements are 1 GB for the 32-bit operating system and 2 GB for the 64-bit operating system. Keep in mind that these are the absolute minimum requirements, and the OS will run but not as well as we have come to expect. In reality, a faster processor, more RAM, and more storage would be expected.
47. You are in the Windows 10 Command Prompt, using Run as administrator. There is a directory named `d:\files` that you want to delete. It currently has six subdirectories and dozens of files in it. Which command should you use to delete `d:\files`?

    1. `del d:\files /s`
    2. `del d:\files /q`
    3. `rmdir d:\files /s`
    4. `rmdir d:\files /q`

    Answer:

    C. The `cd`, `md`, and `rd` commands are used to change, make, and remove directories, respectively. They're shorthand versions of the `chdir`, `mkdir`, and `rmdir` commands. The `rd` or `rmdir` command will only delete empty directories by default. With that command, the `/s` switch will remove all subdirectories and files. The `/q` switch is quiet mode, and when used with the `/s` switch, it will not ask if it's OK to remove all the files and subdirectories; it will remove them without warning. The `del` command is for deleting files.
48. You've installed several identical new PCs and want to capture a baseline of their performance for future troubleshooting. What tool would be best suited for that purpose?

    1. Event Viewer
    2. Performance Monitor
    3. System Information
    4. System Configuration

    Answer:

    B. Performance Monitor (`perfmon.msc`) offers a graphic display of a wide range of counters to track how well hardware such as RAM, drives, and CPUs are performing over time. Those reports can be printed and filed as a baseline to compare to future performance and used to identify bottlenecks in a system. Event Viewer (`eventvwr.msc`) keeps logs of system, application, and security events that can be used for activities such as detecting attempted unauthorized access to resources. System Information provides a snapshot of the system's hardware and software, including the OS version, RAM, processor, motherboard, and much, much more. The program to launch it is `msinfo32.exe`. System Configuration (`msconfig.exe`) has been appearing in Windows operating systems for many versions now, but its features have changed over time. In Windows 10 and Windows 11, this utility is used to control how Windows boots up and to provide quick access to other Windows tools.
49. A user has called the help desk saying that the Internet is down on their Windows computer. After asking a few questions, you want to examine their network configuration to determine the cause of their computer's connectivity problem. You've talked them through accessing the Windows Command Prompt. What command will you have them type so they can read the computer configuration to you?

    1. `ipconfig /all`
    2. `ipconfig /renew`
    3. `ip`
    4. `tracert`

    Answer:

    A. The `ipconfig` command is used to display information about the computer's current network configurations. The `/all` switch will show more detailed information than `ipconfig` alone will, such as whether DHCP (Dynamic Host Configuration Protocol) is enabled and what the DNS (Domain Name System) settings are. Typing `ipconfig /renew` will request a new IP address from a DHCP server, if one is available to the host PC. The macOS equivalent of `ipconfig` is `ip` (replacing the old `ifconfig` command), and `tracert` shows the path a packet takes to get from one computer to another.
50. A computer user that you support is having difficulty reading the words on the screen because they have a visual impairment that makes distinguishing colors difficult for them. What can you change in Windows Settings to make their screen more readable?

    1. Go to Personalization, then Fonts.
    2. Go to Personalization, then Background, and choose High contrast settings.
    3. Select System, then Display, then Nightlight.
    4. Select Accounts, then choose High Contrast Settings.

    Answer:

    B. Select Windows Settings, then Personalization, choose Background, then click on High contrast settings. On the next screen click the toggle to turn on high contrast, which will make the colors more distinct and easier for visually impaired users to distinguish between them. This may make it easier for the user to read the words on the screen. Like most Windows options, there are other ways to access the High Contrast Settings. The Fonts selection under Windows Settings, then Personalization, allows the user to add fonts to the system that are not already there. While changing to a different font might help the computer user, this isn't the place to do it. The nightlight settings use warmer colors at night, which might make PC use even more difficult for this user. High contrast settings are not available under Accounts.
51. You need to work at a command prompt on a Windows PC. When you open the prompt, you are at `C:\window\system32`. You need to be at the root of the C: drive for what you'll be doing. How do you get to C:\\? Assume you would press Enter after the command.

    1. `cd c:`
    2. `cd\`
    3. `C:\`
    4. `cd root`

    Answer:

    B. Typing **`cd\`** will take you to the root of whatever drive you are on. You could also type **`cd..`** and press Enter to go back one directory at a time. For example, to go from `C:\windows\system32` to `C:\`, you would need to type **`cd..`** and press Enter, then type **`cd..`** and press Enter. The other options will not get you to the root of the C: drive.
52. A laptop user has traveled to visit a client and forgot their power adapter. The user is heading to lunch with the client and wants to conserve battery power but enable the fastest possible startup when they get back, with the applications already open. Which power mode will conserve battery life but enable the fastest startup?

    1. Shut down
    2. Sleep
    3. Hibernate
    4. Resting

    Answer:

    B. Sleep stores everything that's open in RAM and enters a low power state. The display and drives aren't using power, but power is needed to continually refresh memory so that it can retain the information. It uses very little power but “wakes up” very quickly with everything open as it was. Sleep in some computer systems and other electronic devices may be called standby or suspend. Shutting the computer down would cause the laptop to use no power but starting up would take longer. Hibernate stores open programs and data to the hard drive and once the computer is hibernated it would use no power, but it will not resume its state as quickly as using Sleep would. There is no resting power state.
53. Which of the following operating systems is open source, allowing its users to customize it as they wish to suit their individual needs?

    1. Windows
    2. Linux
    3. macOS
    4. Chrome OS

    Answer:

    B. Linux is free and open source, so a user can modify the operating system's source code to behave and appear however they choose. The downside is that there might not be as much support if something goes wrong as there would be with a commercial package. Windows and macOS are commercial operating systems, meaning that you pay for them and can use their utilities to configure the OS, but you don't have access to the operating system's source code. Chrome OS is a commercial, proprietary operating system found only on Chromebooks, but there is an open source version called Chromium OS.
54. What does Keychain provide for the user in macOS?

    1. Password management
    2. Local file sharing
    3. Certificate management
    4. Screen protection

    Answer:

    A. Remembering the passwords for various websites is easily managed in macOS with Keychain.
55. You're installing Windows 10 Pro edition on a workstation. How much memory must there be? (Choose two.)

    1. 20 GB for the 64-bit version
    2. 16 GB for the 32-bit version
    3. 1 GB for the 32-bit version
    4. 2 GB for the 64-bit version

    Answer:

    C, D. Regardless of the version that is being installed, Windows 10 has the same minimum requirements, which are a 1 GHz or faster processor or SoC (System on a Chip), DirectX 9 or later with the WDDM (Windows Display Driver Model) 1.0 driver, and a minimum 800×600 display. For storage, the 32-bit version requires 16 GB, and the 64-bit version requires 20 GB available for the OS. RAM requirements are 1 GB for the 32-bit operating system and 2 GB for the 64-bit operating system. Keep in mind that these are the absolute minimum requirements, and the OS will run but not as well as we have come to expect. In reality, a faster processor, more RAM, and more storage would be expected. Windows 11 requirements are different. It requires a 1 GHz or faster processor with a minimum of 2 cores on a 64-bit processor or SoC. The minimum RAM is 4 GB, UEFI firmware (not BIOS), Trusted Platform Module (TPM) version 2.0, DirectX 12 or later with the WDM 2.0 driver, and a high-definition display greater than 9″ diagonally. The Home edition requires a Microsoft account and Internet access for installation.
56. Which Windows 10 edition supports up to 2 TB of RAM?

    1. Home
    2. Pro
    3. Pro for Workstations
    4. Enterprise

    Answer:

    B. Windows 10 Pro edition supports up to 2 TB of RAM and a maximum of two CPU sockets. The Home edition supports only 128 GB of RAM and one CPU socket. Windows Pro for Workstations and Enterprise editions support up to four physical CPU sockets and 6 TB of RAM.
57. You work at home with a computer that has a Windows Home edition installed. You're trying to run `gpedit.msc` to establish group policies on the computer that will limit what your children can do on it. For some reason, `gpedit.msc` won't launch. What do you do?

    1. Reboot the computer, then run `gpedit.msc`.
    2. Upgrade to Windows Pro edition.
    3. Install Windows Active Directory.
    4. Launch it from Administrative Tools.

    Answer:

    B. The Local Group Policy Editor (`gpedit.msc`) is not available in the Home editions of Windows. It is available in the Pro, Pro for Workstation, and Enterprise editions. You don't need to have Active Directory installed on a server to use the Local Group Policy Editor, although it is available there as well. Going to Administrative Tools won't help because the Group Policy Editor is not available anywhere on Windows Home editions, and Administrative Tools is included in Windows 10 but not included in Windows 11.
58. You are at a Windows command prompt, on the C: drive. You need to create a directory named `files` on the D: drive. What is the proper command and syntax to do this?

    1. `cd d:\files`
    2. `cd files d:\`
    3. `md d:\files`
    4. `md files d:\`

    Answer:

    C. The `cd`, `md`, and `rd` commands are used to change, make, and remove directories, respectively. They're shorthand versions of the `chdir`, `mkdir`, and `rmdir` commands. The syntax of the command is `md [`_`drive`_`:]`_`path`_, so the directory would appear after the drive letter when typing the command. The drive letter must be included because it is not the drive that you are on.
59. You will be installing several new resource-intensive applications on a Windows workstation, and the user has concerns over system performance. You want to monitor memory and CPU performance and set up the workstation so that it logs performance over time. Which utility should you use to set this up?

    1. Resource Monitor
    2. Performance Monitor
    3. Task Viewer
    4. Event Viewer

    Answer:

    B. There are three tools that quickly show you CPU and memory usage in Windows: Resource Monitor, Performance Monitor, and Task Manager. The only one that lets you set up logs is Performance Monitor. It will collect counter information and then send that information to a console or event log. Event Viewer logs system, application, and security events, not performance.
60. You don't like the pictures that are on your desktop and change from time to time. Where will you go in Windows Settings to change this setting?

    1. Accounts
    2. Apps
    3. Personalization
    4. System

    Answer:

    C. From the Personalization menu of Windows Settings, you can change the desktop theme and background colors. Accounts enables the user to manage what accounts have access to this computer and at what level. The Apps settings deal with application-specific parameters and not operating system settings. Finally, the System settings in Windows Settings has a multitude of settings that relate to the system but not to the image that appears on the desktop.
61. What operating system developed by Google is used on tablets or laptops used mainly for accessing the Internet and using Android applications?

    1. Ubuntu
    2. iOS
    3. Windows 11 Pro
    4. Chrome OS

    Answer:

    D. The Google Chrome OS was developed by Google. It comes preinstalled on laptops and tablets called Chromebooks. A freeware version, Chromium OS, can be installed on tablets, smartphones, laptops, and desktops. The main user interface for Chrome OS is the Google Chrome browser. Chrome OS can also support Android apps. Ubuntu is based on the open source Linux OS kernel. iOS is Apple's proprietary operating system, and Windows 11 Pro was developed by Microsoft.
62. On your laptop running macOS, what is the name of the utility used to browse through files and folders?

    1. Spotlight
    2. Remote Disc
    3. iCloud
    4. Finder

    Answer:

    D. Finder in macOS is similar to File Explorer in Windows. Both allow you to browse through folders and find files, disks, and applications. Both can be used to change the view so that entries can be seen as images, a list, a column, and so on. Spotlight is the tool for searching on a Mac, and iCloud is similar to Microsoft's OneDrive for storage.
63. You're troubleshooting a network connectivity issue and want to see if the local computer can reach a particular server on the web. What command will you use?

    1. `ping`
    2. `tracert`
    3. `ipconfig`
    4. `pathping`

    Answer:

    A. The `ping` (packet Internet groper) command sends a series of four packets to a remote computer and waits for a reply. If the reply is received, you know that the local computer is able to reach the remote host. It also displays how long the transaction took. `ping` can be used with domain names like [`Wiley.com`](http://wiley.com/) or the IP address, if known. When `ping localhost` or `ping 127.0.0.1` or `ping ::1` is run, the command verifies that TCP/IP is working on the local computer. `tracert` shows the routers that a packet traverses to reach its destination. The `ipconfig` command is used to view network configuration, and `pathping` is a combination of the abilities of `ping` and `tracert`.
64. Which command in a Linux environment is used to display the full path to the current directory?

    1. `ls`
    2. `pwd`
    3. `cp`
    4. `yum`

    Answer:

    B. All of the answer options are Linux commands. The `pwd` (print working directory) command writes the full path to the current (working) directory from the root on whatever the default output device is (usually the display.) The path might be, for example, `/home/audrey/documents`. The `ls` command provides a list of all the files and folders found in the current directory, the `cp` command is used to copy files and directories, and `yum` (Yellowdog Updater Modified) is used to install, update, remove, and search for software packages.
65. One of the users you support has a MacBook. They're finding that their desktop is too cluttered. What can they use to have quick access to what they want and help them organize their desktop? (Choose two.)

    1. Finder
    2. Time Machine
    3. Spaces
    4. Multiple desktops

    Answer:

    C, D. If a user finds their desktop getting out of hand, they can create multiple desktops, which macOS calls Spaces, to organize their desktop objects, or simply to make more space. Multiple desktops are created using Mission Control. Once multiple desktops are created, apps can be moved from one desktop to another by dragging, similar to using a smartphone. Finder is used to drill down through the file structure to find what you're looking for, and Time Machine is used to make backups.
66. What is the name of the bar on the bottom of the screenshot shown in the graphic, where shortcuts to commonly used programs and utilities are kept in the macOS?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf007_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. Taskbar
    2. Dock
    3. File Explorer
    4. Finder

    Answer:

    B. The macOS Dock provides quick access to the programs you'll likely use most often. Taskbar provides a similar function in Windows OSs. File Explorer and Finder are both used to drill down through the filesystem to find what you're looking for—File Explorer is the Windows utility and Finder is the macOS utility.
67. What Windows feature best describes Event Viewer (`eventvwr.msc`), Disk Management (`diskmgmt.msc`), and Certificate Manager (`certmgr.msc`)?

    1. Services
    2. Processes
    3. Policies
    4. Snap-ins

    Answer:

    D. Event Viewer, Disk Management, and Certificate Manager are all Microsoft Management Console (MMC) snap-ins. A Microsoft Management Console provides an interface where a user can configure and easily access their own list of tools that they use most often. These tools are called snap-ins, and there are more than twenty of them available. A console contains shortcuts to the tools, and when the console is saved, it can be identified by a toolbox icon. Services are programs that run in the background on a Windows system such as a print manager and WLAN AutoConfig. Processes are parts of a program that are running, usually consisting of multiple threads. Threads are the section of code being worked on by the processor. Policies are rules for granting access such as the ability to log on locally or settings for passwords that require complexity. Policies are configured through the Group Policy Editor (`gpedit.msc`) and are not available in Windows Home editions. There are literally hundreds of policies that can be set in a Windows system. The Group Policy Editor is also an MMC snap-in.
68. Your laptop battery is getting older and won't hold a charge as long as it once did, so you want to ensure that, when you walk away from it for a period of time and it isn't plugged in, it will not use any power but save everything and let you pick up where you left off working. What power state will work for this scenario?

    1. Always On
    2. Sleep
    3. Hibernate
    4. Hyper-V

    Answer:

    C. Once the Hibernate power setting has saved everything from RAM to a system file (`hiberfil.sys`) on the hard drive, it will turn the system off and use no power. Hibernate takes longer to get back to a running state than Sleep does, but Hibernate won't use any power after it has stored the data. When the system is resumed, the contents of the system file are copied back into RAM and the user can continue where they left off. Sleep needs a small amount of power to keep the data in RAM refreshed. Always On will obviously use power continuously, and Hyper-V is Microsoft's virtualization product, not a power setting.
69. You are at a command prompt on a Windows PC, at C:\\, and need to get to `C:\Windows\system32`. Which command listed will get you there? Assume you press Enter after the line. (Choose two.)

    1. `c:\windows cd system32`
    2. `cd C:\windows\system32`
    3. `cd windows\system32`
    4. `cd system32 windows`

    Answer:

    B, C. Because you are already on the C: drive, you would not need to specify the drive letter to change to a directory on that drive. If you did specify the drive (as in option B) it's not a problem, because if you were going to a directory on a different drive, you would need to specify the drive letter. Because you're already at the root of the C: drive, you can simply enter the cd command and the path (option C), **`cd windows\system32`**. If you were anywhere else in the C: drive, you would need to include the `\` to denote the root of the drive in your command (**`cd \windows\system32`**). You could go to that directory with two commands, changing one directory at a time, by typing **`cd windows`** and pressing Enter, then typing **`cd system32`** and pressing Enter, but that would be inefficient and is not one of the options given.
70. Your system is running sluggishly, and you want to know why. Which application, as shown in the graphic, shows CPU usage by core and allows you to end problematic processes and stop running services?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf008_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. `eventvwr.msc`
    2. `lusrmgr.msc`
    3. `perfmon.msc`
    4. `resmon.exe`

    Answer:

    D. The program `resmon.exe` launches Resource Monitor, which is shown in the graphic. Resource Monitor is a powerful performance monitoring tool. It provides more granular information than Task Manager or Performance Monitor, but it doesn't have the ability to save a log of performance. The Event Viewer can be launched with `eventvwr.msc`. The Local Users and Groups application can be launched with `lusrmgr.msc`, and Performance Monitor can be launched with `perfmon.msc`.
71. You have installed Windows 10 32-bit on a desktop computer that has a 32-bit processor. It seems to be working fine, but when you install more RAM, bringing the total up to 12 GB, the operating system doesn't recognize anything above 4 GB. What is the problem?

    1. You need to tell the BIOS that the extra RAM is there.
    2. A 32-bit OS can support a maximum of only 4 GB of RAM.
    3. You need to go to Device Manager to add the RAM.
    4. You need to replace the motherboard.

    Answer:

    B. Any 32-bit operating system has a limit of 4 GB of RAM. The limitation is caused by the bus width. There simply aren't enough numbers available to identify memory locations above 4 GB.
72. You're at a friend's house when a manager at your company calls to say they are having a problem with their Windows Pro PC while working at home. You listen and tell them you can easily fix it using Remote Desktop to take over their computer for a minute or two. Which of the following would not be an option to use Remote Desktop from where you are?

    1. Use your friend's Windows Home PC.
    2. Use your friend's Windows Pro PC.
    3. Use Remote Desktop Mobile on your iOS device.
    4. Use Remote Desktop Mobile on your Android device.

    Answer:

    A. Remote Desktop can only be enabled on a Windows Pro or better operating systems. Windows Home edition does not have this capability. However, using a PC with Windows Pro, Pro for Workgroups, or Enterprise edition is not the only way to access the manager's computer. The Remote Desktop Mobile app is available for iOS and Android devices.
73. You are at a Windows workstation and have a command prompt open. Which of the following commands is used to refresh Group Policy settings and force their changes to take effect?

    1. `gpedit`
    2. `gpresult`
    3. `gprefresh`
    4. `gpupdate`

    Answer:

    D. The `gpupdate` tool is used to update Group Policy settings immediately. It refreshes, or changes, both local and Active Directory–based policies. The `gpedit` command allows the user to edit group policies, and the `gpresult` command will show the Resultant Set of Policy (RSoP) for a user or computer. RSoP is the culmination of all policies that affect the target user or computer. It is particularly helpful in troubleshooting conflicting policies. `gprefresh` is not a valid command.
74. You've been having trouble with network communications to one of your company's offices. You want to determine the source of latency on the connection. What command will you use in the Windows Command Prompt to see where the latency is?

    1. `grep`
    2. `pathping`
    3. `tracert`
    4. `mv`

    Answer:

    B. The `pathping` command works like `ping` and `tracert` combined. It shows the path a packet takes from point A to point B, and then will show the time at each hop. (A hop is the number of times a packet moves from one router to another to get to its destination after it leaves the initial router.) `grep` and `mv` are Linux Terminal commands, which are used to search for text from a file, and to move files and folders, respectively. The `tracert` command shows the path a packet takes to its destination.
75. Your spouse is trying to work at home but has started to complain about the constant notifications appearing on the computer and interrupting their work. What category can you access in Windows Settings to turn them off?

    1. System
    2. Gaming
    3. Update and Security
    4. Apps

    Answer:

    A. To turn off all notifications, or manage whether and how individual notification senders can interact with you, go to Windows Settings, choose System, then Notifications & actions. From there you can turn off all notifications or some, and choose whether or not a sound is played when they arrive. The Gaming option lets you configure the system to be optimized for gameplay and recording. Update & Security settings don't address notifications. The Apps option lets you manage where apps can be installed from, default apps for opening files, and other application configuration settings.
76. Which of the following commands is used by an administrator on a Red Hat Linux system to update software?

    1. `pwd`
    2. `ls`
    3. `cp`
    4. `yum`

    Answer:

    D. All of the answer options are Linux commands. The `yum` (Yellowdog Updater Modified) command is used to install, update, remove, and search for software packages. The syntax is `yum [`_`options`_`] <`_`command`_`> [<`_`args?`_`…]`. For example, to see a list of the installed packages, you would type **`yum list installed`**. The `pwd` (print working directory) command writes the full path to the current (working) directory from the root on whatever the default output device is (usually the display.) The `ls` command provides a list of all the files and folders found in the current directory, while the `cp` command is used to copy files and directories.
77. A macOS user is complaining that their MacBook has been acting strangely lately, and it's very slow to start. What utility will you use to repair any potential disk errors?

    1. FileVault
    2. Terminal
    3. Disk Utility
    4. Force Quit

    Answer:

    C. The macOS Disk Utility can be used to find and fix errors in the directory structure of a Mac disk. If the Mac won't boot into the OS, the utility can be accessed through macOS Recovery. Depending on the hardware your Mac is using, you would either hold the power button until startup options appear, or press and hold Command+R while the computer is starting to bring up macOS Recovery. From there choose Utilities and then Disk Utility. FileVault provides encryption, Terminal is the macOS and Linux command- line user interface, and Force Quit can be used when a single app is causing problems and refuses to close.
78. You've created a batch file that needs to run every day before the employees arrive. What can you use to ensure that this batch file is run every weekday at 6 a.m.?

    1. Task Scheduler
    2. Event Viewer
    3. Device Manager
    4. Local Users And Groups

    Answer:

    A. Task Scheduler is a Microsoft Management Console (MMC) snap-in and, as its name implies, a tool for running programs and performing tasks based on a trigger such as date, time, or events such as logon, idle, or locking the workstation. Event Viewer keeps logs of system, security, and application events. Device Manager is a tool for working with hardware and lets you update drivers and scan for newly attached devices, for example. Local Users and Groups is an MMC snap-in for creating and managing users and groups.
79. A smartphone user recently found their phone on an EOL list. They asked you what this means. Why will you recommend they purchase a new phone?

    1. They can't download any more apps.
    2. Their phone will stop working by the date on the list.
    3. Their phone may not receive any more security updates.
    4. Their phone will no longer connect to cellular service.

    Answer:

    C. When an OS, smartphone, PC or any electronic device is at end-of-life (EOL), it generally is no longer sold or supported, meaning that replacement parts and product and security updates are no longer available. While you may be able to scavenge parts, not getting security updates should be a great concern. At an electronics end-of-life, the best course of action is to recycle the device and procure a newer one.
80. You are on a Windows computer working at a command prompt and need to see a list of files in the directory that you are working in. What command will you type?

    1. `dir`
    2. `ls`
    3. `pwd`
    4. `grep`

    Answer:

    A. The `dir` command will show you a list of all the files and folders that are in the directory you are working in, along with the date created. Using the switches that work with `dir`, you can view much more information. `ls` is a Linux command that lists information about files in the working directory. The `pwd` Linux command prints the complete path to the working directory, and the `grep` Linux command will search for files with a pattern that you specify.
81. A user with a Windows workstation recently received a second hard drive. Another administrator created a partition on the hard drive, and it's ready for use. The user will store the raw video files they create on that drive and insists that it be called the R: drive. Which of the following statements is true?

    1. You can use Disk Management to change the drive letter to R:.
    2. You can use Disk Management to change the drive letter to R:, but only if it's a dynamic disk.
    3. You can use Disk Management to change the drive letter to R:, but only if it's in an extended partition.
    4. You will need to use Disk Management to delete the partition first, then re-create it as R:.

    Answer:

    A. Disk Management is a Windows tool that has been available for many Windows versions. With it you can reassign or change a drive letter, create and format volumes, shrink or expand volumes, change basic drives to dynamic drives, import foreign drives, and even establish software RAID. In Windows 10 it can be launched through Control Panel by choosing Administrative Tools, then Computer Management, or you can launch it by typing **`diskmgmt.msc`** in the search box. Administrative Tools is not available in Windows 11, but Disk Management is. The easiest way to access Disk Management in Windows 10 or 11 is to press Windows Key+X to bring up the Quick Link menu, which is a list of commonly used tools, and click Disk Management on the list.
82. A salesperson at your company travels with their macOS laptop every week. You want to encrypt the data on their startup disk to ensure data security. What macOS utility will you use?

    1. Finder
    2. Time Machine
    3. FileVault
    4. BitLocker

    Answer:

    C. FileVault is the macOS utility for encrypting data. Finder is the macOS utility for drilling down through folders to find objects. Time Machine is used to create and restore backups of data on a Mac, and BitLocker is the Windows drive encryption utility.
83. A user wants to perform a backup on their MacBook. Which software utility should be used to make backups?

    1. Image Recovery
    2. Time Machine
    3. iBackup
    4. Accessibility

    Answer:

    B. Time Machine is the macOS backup utility. It can be accessed through System Preferences, and once set up, it will run on schedule much like any other backup software. Image Recovery and iBackup are not macOS tools. Accessibility options can be found in System Preferences and are used to adjust settings for different vision, hearing, and mobility needs.
84. One of your network users has a MacBook Pro. Where should this user go to see whether there are any OS updates available?

    1. Open the App Store and click Updates in the toolbar.
    2. Open Safari and click Updates in the toolbar.
    3. Open System Preferences and click Updates in the toolbar.
    4. Open Finder and click Updates on the menu bar.

    Answer:

    A. Updates to MacOS can be found at the App Store. Open it and click Updates in the toolbar to see which updates are available. There will be an Install button to begin the installation. In System Preferences, there is generally a Software Update icon to help with updates as well. Update is not an option on the toolbar of Safari, which is the web browser. Finder is used for drilling down through directories to find files and folders.
85. What command will bring up the screen shown in the graphic?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf009_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

    1. `winver`
    2. `version`
    3. `osver`
    4. `build`

    Answer:

    A. If you are working at a command prompt and need to know the version of Windows on the PC, type **`winver`** and press Enter. You'll get a screen similar to the one shown in the graphic. The other options are not valid commands.
86. Which of the following commands was used to display the screen snippet shown in the graphic?

    <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf010_0.jpg" alt="" height="1000" width="801"><figcaption></figcaption></figure>

    1. `gpedit`
    2. `gpresult`
    3. `gprefresh`
    4. `gpupdate`

    Answer:

    B. The `gpresult` command will show the Resultant Set of Policy (RSoP) for a user or computer. RSoP is the culmination of all policies that affect the target user or computer. It is particularly helpful in troubleshooting conflicting policies. The screen shown used the `/r` switch, which shows the RSoP summary for the currently logged-on user on the local computer. The `gpedit` command allows the user to edit group policies, and the `gpupdate` tool is used to update Group Policy settings. It refreshes, or changes, both local and Active Directory–based policies. `gprefresh` is not an existing command.
87. Which Linux command is used to copy files, groups of files, or whole directories from one place to another?

    1. `mv`
    2. `cp`
    3. `find`
    4. `cat`

    Answer:

    B. All of the commands listed are Linux commands. The `cp` command is used to copy files. There are three syntaxes for the `cp` command, as follows:

    * `cp [option]` _`source destination`_
    * `cp [option]` _`source directory`_
    * `cp [option]` _`source-1 source-2 source-n directory`_

    For example, if the copy command has two filenames, it will create a copy of the first filename and save it as the second. The command would be `cp` _`file1 file2`_. The `mv` command is used to move files, and the `find` command is used to find files and directories and perform operations on them. The `cat` command is a powerful tool that can be used to view contents of a file, create new files, and concatenate (put together) files.
88. Despite your great objections, someone you know is still running a Windows OS that predates Windows 10 and has reached its end of extended support. The software they regularly use on it still works, and they have an antivirus installed. Why should they update to a newer OS? (Choose two.)

    1. They will not receive security updates.
    2. They will not receive feature updates.
    3. Their apps will stop working.
    4. Their OS will stop working at end-of-life.

    Answer:

    A, B. Operating systems (OS) and electronics have a life cycle, just as living things do. They are introduced, grow, reach maturity (mainstream support), decline (extended support), and reach their end-of-life (EOL) which means there is no support. The last Windows OS prior to Windows 10 was Windows 8.1, which ended mainstream support on January 9, 2018, and the end of extended support date is January 10, 2023. End of mainstream support means there are no updates other than security. End of extended support means there is no support, including security updates and patches. Essentially, if (when) a vulnerability is discovered by a hacker, the user of an end-of-life OS is at risk for being attacked. Applications may continue to work just fine, but updates might not work with the OS. The OS will not magically stop working, but if a problem occurs there will be no official support available.
89. A smartphone user has come to you for help. They would like a laptop so they can use a bigger screen but don't know what to choose. They're accustomed to doing their work online with Google Docs and their smartphone and saving it to the cloud. They would like to be able to use some of the same apps that they have available on their Android phone. Cost is a factor. What type of laptop would you recommend for this user?

    1. Windows Home
    2. Linux
    3. macOS
    4. Chromebook

    Answer:

    D. The Chromebook, which has Chrome OS preinstalled, is the best option for this user. It's main user interface is the Google Chrome browser, and it can run apps designed for Android smartphones. Chromebooks are also known for being less expensive laptop options. Windows Home and macOS would be fine for accessing the Internet, but they would not support the applications that the user is accustomed to using, and the user would experience a learning curve. Linux might be able to run their Android apps using third-party software, but again the user would have a learning curve.
90. A user called the help desk because they were denied access to a secure server and received a message that they have an invalid certificate. Their computer was recently updated. Where can you go to manage their certificates?

    1. Device Manager
    2. Local Users and Groups
    3. Certificate Manager
    4. Group Policy Editor

    Answer:

    C. Certificates are a way of proving who someone or a website is by means of a digital signature. A user's certificates hold the private key of a key pair for encryption. If certificates are outdated or otherwise no longer valid, then encryption doesn't happen and the transmission can be intercepted by someone with malicious intent. Normally you wouldn't need to worry about certificates, but if a problem occurs, the certificate may need to be deleted and a new one requested. Certificate Manager allows you to view and manage certificates by user or computer. Device Manager is a hardware management tool. Local Users and Groups allows for organizing users by access need and assigning permissions and access to the group rather than the user, simplifying access management. Group Policy Editor allows administrators to further control what users and computers are allowed to do on the network.
91. Which desktop operating system is a proprietary product of Apple?

    1. Apache
    2. Red Hat Linux
    3. macOS
    4. FreeBSD

    Answer:

    C. macOS is Apple's proprietary desktop operating system (OS). Apache is a popular web server OS, not a desktop OS. Red Hat Linux is a distribution of the open source Linux OS, and FreeBSD is a freeware, open source OS based on Unix.
92. A user on your network complains that they are unable to type a human-friendly name like [`Sybex.com`](http://sybex.com/) into their browser to reach a website, but typing an IP address in the browser works. What client network configuration setting do you suspect is the problem?

    1. Authentication server
    2. DNS server
    3. DHCP server
    4. Proxy server

    Answer:

    B. DNS has one function on the network, and that is to resolve hostnames to IP addresses. For a computer or phone to open a website, it needs to know the IP address of that website. Each DNS server has a database, called a zone file, which maintains records of hostname-to-IP address mappings. If the network settings for DNS server on a client computer are improperly configured and the client can't reach the DNS server, then human-friendly names are not resolved to IP addresses, causing the problem this user is having. Authentication servers are used to verify whether a user has the proper credentials to gain access to resources on a network. A Microsoft domain controller is a type of authentication server. DHCP (Dynamic Host Configuration Protocol) is used to automatically provide an IP address to a client based on a list (scope) of IP addresses made available on the DHCP server. A proxy server sits between the client and the outside world and is used to filter content incoming or outgoing.
93. You need to start a new shell on a Linux workstation with `root` permissions. Which command should you use to do this?

    1. `su`
    2. `sudo`
    3. `apt-get`
    4. `ps`

    Answer:

    A. The `su` command (switch user, substitute user, or super user) is used to start another shell on a Linux computer. Without specifying the username, it's assumed you are trying to start a shell with super user (or `root`) authority. This can be dangerous because as the `root`, the user can do anything on the system, including delete parts of the operating system, and there is no undo or warning message. You must know the `root` password to run `su`. It's far safer to run the `sudo` command. The `sudo` command stands for superuser do, or substitute user do, and will run a single command as the alternate user. The `apt-get` command is used to download or remove software packages, and the `ps` command will list the processes that are currently running along with their process IDs (PIDs).
94. A user wants to change the resolution on their MacBook. Which System Preferences pane would they use to do that?

    1. Printers & Scanners
    2. Desktop & Screen Saver
    3. Accessibility
    4. Displays

    Answer:

    D. The Displays pane in System Preferences is used to set resolution and brightness (turn Night Shift on and off), and possibly other settings depending on whether there is a display connected. The Printers & Scanners pane is where you would add or manage a printer and its print jobs. Accessibility preferences include settings for hearing, mobility, and vision. The Desktop & Screen Saver options allow you to configure the desktop and screen saver.
95. You want to be able to access your Windows Pro desktop PC at home no matter where you are. Which of the following do you not need to do?

    1. Upgrade to Windows Enterprise.
    2. Enable Remote Desktop on your PC.
    3. Open Remote Desktop Connection, provide the PC name, and click Connect.
    4. Install the Remote Desktop App on your smartphone.

    Answer:

    A. Home editions of Windows do not support Remote Desktop, but the Windows business editions (Pro, Pro for Workstation, and Enterprise) do. Since you have Windows Pro, you would not need to upgrade your operating system edition. The steps to use Remote Desktop to access a PC from a smartphone are as follows:

    1. Enable Remote Desktop on the PC.
    2. Note the PC name.
    3. Install Remote Desktop Mobile on the smartphone.
    4. Open the Remote Desktop app on your smartphone.
    5. Enter the name of the PC that you want to connect to.
    6. Select the PC name and wait for the smartphone to connect.
96. You are at a Windows command prompt. You believe that some of the Windows system files are corrupted. Which command should you use to scan and repair problematic system files?

    1. `sfc /scanfile`
    2. `sfc /scannow`
    3. `sfc /verifyfile`
    4. `sfc /verifyonly`

    Answer:

    B. The System File Checker (SFC) is a command-line utility that checks and verifies the versions of system files on your computer. If system files are corrupted, the SFC will replace the corrupted files with correct versions. The `/scannow` option will scan and repair files, whereas `/scanfile` will just check one specified file. The `/verifyonly` option will scan the integrity of protected system files but not attempt to repair them. The `/verifyfile` option will verify the integrity of a specific file.
97. You are at a Windows command prompt. Which command allows you to copy files and directories, copy NTFS permissions, and mirror a directory tree?

    1. `copy`
    2. `xcopy`
    3. `robocopy`
    4. `copyall`

    Answer:

    C. The `robocopy` utility (Robust File Copy for Windows) has the big advantage of being able to accept a plethora of specifications and keep NTFS permissions intact in its operations. For example, the `/mir` switch, can be used to mirror a complete directory tree. `copy` and `xcopy` are both valid commands but have nowhere near the power that `robocopy` does. `copyall` is not a valid command.
98. The hard drive performance on your Windows workstation has deteriorated over time. To attempt to improve performance, you want to ensure that files on the hard drive are written in contiguous blocks. Which Windows tool should you use to make this happen?

    1. Disk Management
    2. Optimize Drives
    3. Disk Optimizer
    4. Device Manager

    Answer:

    B. When files are written to a hard drive, they're not always written contiguously or with all the data in a single location. Defragmenting a disk involves analyzing the disk and then consolidating fragmented files and folders so that they occupy a contiguous space (consecutive blocks), thus increasing performance during file retrieval. The executable for Disk Defragment is `dfrgui.exe`, which brings up the Optimize Drives window. By default, drives are automatically scheduled to be optimized, but it can be done here on command or the schedule settings changed. The Disk Management utility is used to create and format volumes and other tasks related to managing drives. Disk Optimizer is not a Windows tool, and Device Manager is useful in examining and troubleshooting issues with hardware.
99. Your client is taking over a business and wants to upgrade the computer systems, which are currently all legacy Windows machines. They will be using Microsoft 365 along with accounting and manufacturing software that is part of the business. They are concerned about compatibility of other files with their customers, vendors, and historical company data. What operating system would you recommend for them?

    1. Chrome OS
    2. Linux
    3. macOS
    4. Windows

    Answer:

    D. Since the majority of business users are still using Microsoft products, and there may be compatibility concerns with data from older systems, a Windows OS would be the correct choice in this situation. Chrome OS is most appropriate where users would be working in the cloud. Linux and macOS may have compatibility issues with data from other sources. Microsoft 365 does come in a version for macOS, but the company-specific software must also be considered.
100.    In macOS, where can the menus Displays, Printers, and Privacy be found and settings changed?

        1. System Preferences
        2. Accessibility
        3. Settings
        4. App Store

        Answer:

        A. dSystem Preferences is where settings can be viewed and modified. System Preferences are divided into various panes, including Displays, Networks, Printers & Scanners, Privacy, Accessibility, Time Machine, Power, and many other selections for changing settings. Windows Settings is a part of the Microsoft Windows operating system. App Store is where you would go on macOS to find new applications to download and to update the operating system.
101.    Your friend has a Windows 10 PC and has never made a backup. You provide them with an external drive to use. What category will you choose in Windows Settings to turn on automatic backups for your friend every hour?

        1. System
        2. Apps
        3. Update & Security
        4. Network & Internet

        Answer:

        C. The Update & Security category of Windows Settings contains more than the name would suggest. In Update & Security there is, of course, Windows Update and Windows Security, but users can also find Backup, Troubleshoot, Recovery, Activation, Find my Device, For developers, and Windows Insider Program selections. To back up using File History, an additional drive (you can't back up to the drive Windows is installed on) is needed, and under More options, you'll find settings for how often to automatically back up, and you'll be able to choose which folders to back up. (In Windows 11, Windows Settings, Backup can be found in the Accounts category and is called Windows Backup.) The Systems category contains Display, Sound, Power, and other system-related settings. The Apps category is where you can uninstall apps, set default apps, and change what apps load on startup. The Network & Internet category has Wi-Fi settings and a network troubleshooter, among other common network-related settings.
102.    Your company has a DHCP server to automatically assign IP addresses to any nodes that connect to it. Which of the following would you want to assign a static IP address to? (Choose two.)

        1. Workstation
        2. File server
        3. Printer/MFD
        4. Local printer

        Answer:

        B, C. Typically on a network, static IP addresses, rather than dynamic, would be assigned to shared resources such as file servers and printers/MFDs to avoid problems with connecting to those resources. A user's workstation normally does not need a static IP address, and allowing it to obtain one automatically makes workstation configuration easier and avoids accidental duplication of IP addresses. A local printer, by definition, is attached to a local computer, not directly to the network, so it wouldn't even have its own IP address.
103.    You're installing an application that requires 4 GB of RAM on a Windows 10 64-bit workstation. The workstation has 4 GB of RAM. Will you need to make any configuration changes to the system to install this application?

        1. No, since the system already has 4 GB of RAM.
        2. No, because the OS and the Application won't be running at the same time.
        3. Yes, you'll need at least 4 additional GB of RAM.
        4. Yes, you'll need at least 2 additional GB of RAM.

        Answer:

        D. When the application is running, the operating system will also be running, so you need to add their respective RAM requirements together to determine the amount of system RAM needed. The minimum amount of RAM for a Windows 10 64-bit installation is 2 GB, and since the application's RAM requirement is 4 GB, you'll need a total of 6 GB, and since you only have 4 GB, an additional 2 GB will need to be installed. While that will run the program on this system, having only 2 GB for the operating system will not allow it to run as fast as the user is accustomed to, so in reality you'd likely want to add more.
104.    Which of these filesystem types is used when running a Linux distribution?

        1. FAT32
        2. NTFS
        3. ext4
        4. APFS

        Answer:

        C. When you install a Linux distribution, it will use an ext3 or ext4 filesystem. FAT32 is the filesystem that was used when only 32-bit processors were available, and it can still be used for compatibility issues with legacy devices, but Windows 10 and Windows 11 require NTFS (New Technology File System) for installating the OS. NTFS has been available for decades and offers security features that FAT32 doesn't have. APFS is the Apple File System and is used for macOS.
105.    You are going to install Windows on a workstation from an image located on a server. What does the workstation need to support to install Windows this way?

        1. `netboot`
        2. Unattended installation
        3. PXE boot
        4. USB boot

        Answer:

        C. An installation can be started many ways—with a USB drive, a DVD, and so on—and an image and setup files can also be located on and installed from a network. Often called a PXE-initiated boot (for Preboot Execution Environment), it allows the workstation involved in the installation to retrieve the files from the network, as needed, and configure variables accordingly. `netboot` refers to booting a computer from a network drive, not installing an OS. Unattended installation is a type of installation that uses an answer file and little or no interaction from a human. While it's possible to install Windows from a USB, if you're using a USB to boot and install an image from a server, the bare-metal machine still needs PXE support.
106.    You're in a secure environment where the workstations are not allowed to have USB ports or DVD drives. You've just received 10 new bare-metal workstations, with PXE support, that need to have Windows installed. How will you install the Windows OS on these 10 PCs?

        1. Optical media
        2. External drive
        3. Internet based
        4. Network

        Answer:

        D. Since the workstations don't have DVD drives, you can't use optical media to install Windows 10, and since there are no USB ports, it's unlikely that you would be able to use an external drive. Internet based installation requires that you can boot and get to the Internet, so you would need an operating system already installed, and the question states that these are bare-metal machines. You're left with a network installation using the PXE boot as the only option.
107.    You need to run just one command as `root`. What will you use?

        1. `su`
        2. `sudo`
        3. `apt-get`
        4. `ps`

        Answer:

        B. The `sudo` command stands for superuser do, or substitute user do, and will run a single command as the alternate user. The user can authenticate with their own password instead of the `root` password, which is a security feature. Another command, `visudo`, is used to configure exactly what each user can do when they run `sudo`. The `visudo` command is not on the CompTIA A+ objectives, but it answers the question of how you would control the access of users who are not `root`. The `su` command (switch user, substitute user, or super user) is used to start another shell on a Linux computer. Without specifying the username, it's assumed you are trying to start a shell with super user (or `root`) authority, and you need the root password to run it. Note the difference between `su` and `sudo`, starting a whole new shell versus running a command. The `apt-get` command is used to download or remove software packages, and the `ps` command will list the processes that are currently running, along with their PIDs (process IDs).
108.    You're working in a school district in a computer lab full of Windows workstations, setting up an application that uses the name of the computer to identify it on the application. What command can you use at a workstation to determine its name? (Choose two.)

        1. `nslookup`
        2. `clientname`
        3. `hostname`
        4. `ping localhost`

        Answer:

        C, D. The `hostname` command returns the name of the computer that it is entered on and, while not its primary purpose, `ping localhost` will also return the name of the computer. `nslookup` will show the default DNS server and its IP address. `clientname` is not a valid command.
109.    You're at a Windows workstation, troubleshooting a connectivity problem with a computer in another office of your campus area network. You need to determine where packets between the two are being dropped. Which command will tell you the last router the packet traversed?

        1. `ipconfig /all`
        2. `ping`
        3. `ip`
        4. `tracert`

        Answer:

        D. The `tracert` command will show the routers that a packet went through and how long each hop took, which can narrow down your search for the problem by showing how far it got. Typing **`ipconfig /all`** will show the current TCP/IP configuration of the local machine, such as its IP address, MAC address, and default gateway. The macOS equivalent of `ipconfig` is `ip`. The `ping` command will only show that the packet is not making the trip there and back by timing out.
110.    You're setting up a computer for a user with limited vision, who would like to have the contents of the screen read to them. What Control Panel utility will you use to accomplish this?

        1. Devices and Printers
        2. Programs and Features
        3. Ease of Access Center
        4. Sound

        Answer:

        C. Ease of Access Center has settings to help users who have limited sight, mobility, or hearing. Devices and Printers is for managing and troubleshooting printers, print jobs, and other devices like connected smartphones or keypads. Programs and Features lets you uninstall or change installed programs, and Sound is used to configure recording and playback devices, or to choose a sound scheme.
111.    The Linux workstation you are using seems slow. You want to see what processes are running on the computer. Which command should you use?

        1. `su`
        2. `sudo`
        3. `apt-get`
        4. `ps`

        Answer:

        D. The `ps` (process status) command will list the currently running processes, along with their PIDs (process IDs), the controlling terminal for the process, the time the CPU has been used by the process, and the name of the command that started the process. The `su` command (switch user, substitute user, or super user) is used to start another shell on a Linux computer. The `sudo` command stands for superuser do, or substitute user do, and will run a single command as the alternate user. The `apt-get` command is used to download or remove software packages.
112.    Which of the following is not an advantage that the ext4 filesystem has over ext3 filesystem?

        1. Supports larger volumes and files
        2. Compatible with macOS and Windows
        3. Unlimited number of subdirectories
        4. Faster filesystem checks

        Answer:

        B. Ext4 (Extended File System, version 4) is not compatible with macOS and Windows. Neither is ext3. For compatibility between Linux, macOS, and Windows, format an external drive with exFAT or FAT32 so that it can be read by any of the three. Ext3 only supports file sizes up to 2 TB and volumes up to 16 TB, whereas ext4 supports files up to 16 TB and volumes up to 1 EB. ext3 is limited to about 32,000 subdirectories, and ext4 has no limit. ext4 also provides superior resistance to fragmentation as well as faster filesystem checking.
113.    A user installed a new headset, but the audio is still playing through the speakers. Where can you go to change that configuration? (Choose two.)

        1. Control Panel, Security and Maintenance
        2. Windows Settings, Devices
        3. Control Panel, Sound
        4. Windows Settings, Apps

        Answer:

        B, C. Going to Control Panel and choosing the Sound utility will enable you to change the default playback device for sound; so will opening Windows Settings and clicking Devices, where you can also configure Bluetooth, printers, and mice. Opening Windows Settings, then System and then Sound will as well, but that is not one of the options. The Security and Maintenance utility in Control Panel has settings for the firewall, malware protection, and other features. The Apps group in Windows Settings is where you would uninstall or choose default apps.
114.    A user wants to know if it's possible to change what happens when they close the lid on their Windows 11 laptop. Currently closing the lid does nothing, but they would like the laptop to hibernate when the lid is closed. Where can this setting be changed?

        1. Control Panel, Power Options utility
        2. Control Panel, Devices and Printers utility
        3. Windows Settings, System group, choose Power & Battery
        4. Windows Settings, Devices group, choose Power Options

        Answer:

        A. The Power Options utility in Control Panel is where you can find the setting for changing what happens when you close the lid, as well as other sleep and hibernate options. For Windows 10, in Windows Settings, in the System group, choose Power Options, then Additional Power Settings, which takes you to the Control Panel utility. Windows Settings in Windows 11 is missing this link, but in both versions of Windows, the other power settings (when to sleep, when to hibernate) are available in Windows Settings. Devices and Printers is where you would manage printers and print jobs, as well as other devices like connected cell phones. The System group in Settings controls Display, Sound, Notifications & actions, and several other areas related to the system as a whole. The Devices group in Windows 10, Windows Settings allows you to configure Bluetooth, printers, and mouse settings. In Windows 11, this group is called Bluetooth & devices.
115.    Which of the following Windows operating systems and editions cannot be upgraded to Windows 10 Pro directly from the desktop by performing an in-place upgrade? (Choose two.)

        1. Windows 7 Enterprise
        2. Windows 8.1 (core)
        3. Windows 10 Home
        4. Windows 8 Pro

        Answer:

        A, D. A PC can be upgraded to Windows 10 Professional directly from the desktop of the PC, provided the PC is running an OS that is in the upgrade path. Surprisingly, Windows 7 Enterprise edition is the only Windows 7 edition that can't be upgraded to Windows 10 Pro. It could only be upgraded to Windows 10 Education or Enterprise editions. Windows 8.1 Enterprise and Embedded Industry editions cannot be upgraded to Windows 10, but the other Windows 8.1 editions can. No Windows 8 editions can be directly upgraded to Windows 10. They must be first upgraded to Windows 8.1, then Windows 10. Only Windows 10 Home can be upgraded to Windows 10 Pro, or an in-place upgrade from Windows 10 Pro to the same or newer version of Windows 10 Pro can be done to troubleshoot problems with the existing installation.
116.    You need to uninstall an app that is on your Linux computer. What command will you use?

        1. `su`
        2. `sudo`
        3. `apt-get`
        4. `ps`

        Answer:

        C. In many Linux distributions, the `apt-get` command is used to download or remove software packages. The syntax for this command is `apt-get [`_`options`_`]` _`command`_. There are too many options to explain them all here, but in the question, we are uninstalling an app, so the command could be `apt-get purge [`_`package name`_`]`, but remember that you would want to precede the `apt-get` command with `sudo`. If the package name were `milou`, then the command you use is `sudo apt-get purge milou`. Using `purge` deletes all configuration files as well as the package. The `sudo` command stands for superuser do, or substitute user do, and will run a single command as the alternate user. The `su` command (switch user, substitute user, or super user) is used to start another shell on a Linux computer. Without specifying the username, it's assumed you are trying to start a shell with super user (or `root`) authority. The `ps` command will list the processes that are currently running, along with their PIDs (process IDs).
117.    You are working at a Windows command prompt. Which command should you use to copy directories and subdirectories but not empty directories?

        1. `xcopy /e`
        2. `xcopy /s`
        3. `xcopy /h`
        4. `xcopy /a`

        Answer:

        B. The `xcopy` command is a more powerful version of `copy`. It lets you copy directories and also will copy file ownership and NTFS permissions. The `/s` switch is used to copy directories and subdirectories, except for empty ones. To copy those as well, use `/e`. The `/h` switch copies hidden and system files, and the `/a` switch copies only files with the Archive attribute set. There are many more options with the `xcopy` command. To find out more, type **`xcopy /?`** at a command prompt.
118.    You're having trouble with a new digitizing pad that the operating system doesn't seem to be recognizing. Which MMC (Microsoft Management Console) would you use to troubleshoot the problem?

        1. Event Viewer
        2. Performance Monitor
        3. Device Manager
        4. Disk Management

        Answer:

        C. Device Manager is the first place to go when troubleshooting hardware. A yellow exclamation point will let you know that there is a problem that needs to be addressed. Event Viewer keeps logs of system, security, and application events. Performance Monitor helps locate bottlenecks in a system by showing resources being used in real time, and Disk Management allows for formatting, partitioning, and managing of hard drives.
119.    You suspect that one of your running services is causing problems with the operating system. What is the tool, shown in the graphic, that lets you choose a diagnostic startup on the next restart?

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf011_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

        1. Event Viewer
        2. Performance Monitor
        3. System Information
        4. System Configuration

        Answer:

        D. System Configuration (`msconfig.exe`) has been appearing in Windows operating systems since 2006, but its features have changed over time. The General tab lets you choose a Diagnostic startup that will load just basic devices and services, which can sometimes aid in troubleshooting. The Boot tab lets you choose other boot options. Timeout, on the right of the Boot tab, can be set if you have more than one OS on the hard drive and want time to choose between them, but a more common option now is to use virtual machines when more than one OS is needed. The Services tab is where you can stop and start many services, although that can also be done through the Services console (`services.msc`), which has all the services. The Startup tab only has a link to Task Manager, and the Tools tab is used to provide quick access to other Windows tools. Event Viewer (`eventvwr.msc`) keeps logs of system, application, and security events that can be used for activities such as detecting attempted unauthorized access to resources. Performance Monitor (`perfmon.msc`) offers a graphic display of a wide range of counters to track how well components such as RAM, drives, and CPUs are performing over time. System Information provides a snapshot of the system's hardware and software, including the OS version, RAM, processor, motherboard, and much, much more. The program that launches it is `msinfo32.exe`.
120.    You need to check the integrity of key Windows system files on the C: drive, which are hidden from view by default. Which Control Panel utility allows you to view hidden files?

        1. Programs and Features
        2. File Explorer Options
        3. Indexing Options
        4. System

        Answer:

        B. Some of the most important files that you will need to work on are hidden by default as a security precaution. To make certain folders or files visible, you need to change the display properties of File Explorer. This can be done by going to the View tab of File Explorer Options in Control Panel and deselecting Hide Protected Operating System Files (Recommended). Programs and Features is for uninstalling or changing programs and turning Windows features on and off. Indexing makes a log of the metadata of files and helps search work faster. The System utility of Control Panel opens System in Windows Settings.

        Note that the CompTIA A+ objectives list File Explorer Options under Control Panel utilities that you should know, so you need to know that you can access them there. But this book's author and technical editor agree that most technicians would access this through File Explorer by selecting Options, then Folder Options (or Change folder and search options, depending on the version) on the View tab. Like most things in the Windows operating system, there is more than one way to perform a task. When sitting for the CompTIA A+ exam, make sure you are familiar with the method that CompTIA has identified in their objectives.
121.    What is the name of the macOS command-line user interface?

        1. Terminal
        2. Finder
        3. Command Prompt
        4. File Explorer

        Answer:

        A. Terminal is the name of the command-line user interface in both macOS and Linux. In it, a user can type commands to perform actions and launch programs. Often for experienced users, using a command-line terminal is faster than navigating menus. Finder is the macOS utility for drilling down through folders to find objects. Command Prompt is the name of the Windows command-line user interface, and File Explorer is the Windows rendition of Finder.
122.    You're setting up an online storage system for backing up your data, but the remote storage company said that you need to open up your software firewall to allow it to communicate with your computer. Where in the Windows Control Panel can you do this?

        1. Programs and Features
        2. Internet Options
        3. Windows Defender Firewall
        4. Network and Sharing Center

        Answer:

        C. Windows Defender Firewall is a software firewall residing on the local system that provides features designed to protect your system from malware. Unfortunately, sometimes those settings interfere with other applications and need to be changed. Turning the firewall off is not advisable, but you can open it up to applications by clicking Allow an app or feature through Windows Defender Firewall. Programs and Features is used to uninstall or change applications, and to turn Windows features on and off. Internet Options affect how browsers work and can be used to connect to a VPN (virtual private network). The Network and Sharing Center is the Windows tool for viewing and configuring network connections and changing adapter settings.
123.    You have a Windows command prompt open. You are in the `D:\users` directory and want to copy all 20 of the files with a `.docx` extension into the `D:\files` directory. Which of the following statements is true?

        1. You need to copy the files one at a time.
        2. You can use the command `copy ∗.docx d:\files`.
        3. You can use the command co`py all.docx d:\files`.
        4. You can use the command `copy .docx d:\files`.

        Answer:

        B. The `copy` command makes a copy of a file in a second location. (To copy a file and then remove it from its original location, use the `move` command.) One useful tip is to use wildcards. For example, the asterisk (`∗`) is a wildcard that means _everything_. So, you could type **`copy ∗.exe`** to copy all files that have an `.exe` filename extension, or you could type **`copy ∗.∗`** to copy all files in your current directory. The other popular wildcard is the question mark (?), which does not mean everything but instead replaces one character. The **`copy abc?.exe`** command would only copy `.exe` files with four-letter names of which the first three letters are `abc`.
124.    In Linux, what is the name of the interpreter between the user and the operating system?

        1. Terminal
        2. Command Prompt
        3. GUI
        4. Shell

        Answer:

        D. The shell is the interpreter between the user and operating system. Common Linux shells include Bash (an acronym for Bourne Again Shell), csh (C-shell), and ksh (Korn shell), but a number of others are also in use. The Terminal is akin to the Windows Command Prompt and is used to enter commands and to interface with the shell. GUI (graphical user interface) describes a type of user interface where the user clicks an icon or picture to launch a program or open a file (that is, interact with the shell).
125.    You are working on a Linux file server. Which command would you use to see the amount of free disk space on a volume?

        1. `grep`
        2. `df`
        3. `ps`
        4. `dig`

        Answer:

        B. The `df` (disk free) command is used to show free and used disk space on a volume. The syntax of this command is `df [`_`option`_`] [`_`file`_`]`. If you type `df` and press Enter, it will show the space that is available on all filesystems that are mounted. If you specify a particular file, it will provide information on that file. The `grep` Linux command will search for files with a pattern that you specify. The `ps` command will list the processes that are currently running, along with their PIDs (process IDs). The `dig` (domain information groper) command works in Linux and macOS to find information about DNS name servers, mail exchanges, and hosts.
126.    A user wants to ensure that the hard drive in their Windows PC is encrypted for maximum data security. What are two commands you can have the user type into the Run box (Windows Key+R) or Windows Command Prompt to see whether the BitLocker Drive Encryption Service is enabled and running? (Choose two.)

        1. `services.msc`
        2. `perfmon.exe`
        3. `compmgmt.msc`
        4. `diskmgmt.msc`

        Answer:

        A, C. There are several ways to see what services are running and to enable and disable services. They include the Services console (`services.msc`) and Computer Management (`compmgmt.msc`). Or you can open Task Manager and select the Services tab (although that has access to only a subset of the services available), and in Windows 10 only, go to Control Panel, Administrative Tools, then click Services to open the Services console. Performance Monitor (`perfmon.exe`) does not show running services, and Disk Management (`diskmgmt.msc`) does not have a link to the Services console.
127.    You're setting up security for a company that is expanding rapidly. Part of your plan is to create groups to manage permissions to folders, and then add users to those groups to grant them the permissions they need. What utility will let you add users to groups?

        1. Device Manager
        2. Local Users and Groups
        3. Certificate Manager
        4. Group Policy Editor

        Answer:

        B. Local Users and Groups allows you to organize users by access need and assign permissions and access to the group rather than individual users, simplifying access management. Incidentally, assigning NTFS permissions to groups rather than individuals is considered a best practice. Suppose your accounting manager suddenly quits and you hire a new one. Rather than set up permissions for the new manager, you would merely add their user name to the appropriate groups (and, of course, disable the former manager's account). Group Policy Editor allows administrators to further control what users and computers are allowed to do on the network, such as enforcing password complexity, disabling USB drives, and limiting what users can do in Control Panel. Device Manager is a hardware management tool, and Certificate Manager allows you to view and manage certificates by user or computer. Certificates hold the private key of a key pair used in encryption.
128.    One of your users has a MacBook Air, and an application appears to have crashed. What can they use to compel the app to close?

        1. Task Manager
        2. Force Quit
        3. Terminal
        4. Time Machine

        Answer:

        B. When an app hangs in macOS, you can use Force Quit to force it to close. Most devices, whether running macOS or iOS, offer similar options. You access Force Quit through the Apple menu or by pressing Command+Option+Esc, which is analogous to pressing Ctrl+Alt+Del on a Windows PC. Task Manager is a Windows utility, Terminal is the macOS and Linux command-line user interface, and Time Machine is used for backups.
129.    You would like to monitor CPU, memory, and Wi-Fi usage in real time on a Windows computer. Which of the following options will provide you with that information? (Choose two.)

        1. The Task Manager Performance tab
        2. Administrative Tools, System Information
        3. Event Viewer
        4. Resource Monitor

        Answer:

        A, D. Although the graphs look different in each application, both the Performance tab of Task Manager and the Resource Monitor utility will show CPU, memory, and Wi-Fi statistics in real time. In Performance Monitor, a Wi-Fi connection can be found on the Network tab. Event Viewer logs system, software, and security events. The System Information utility, which can be found in Administrative Tools, shows a snapshot of a system's configuration, but not real-time information. Note that Administrative Tools is a utility in Windows 10 but is not a part of Windows 11.
130.    You are on a Linux computer working in Terminal and need to see a list of files in the directory that you are working in. What command will you type?

        1. `dir`
        2. `ls`
        3. `pwd`
        4. `grep`

        Answer:

        B. `ls` is a Linux command that lists information about files in the working directory. The `dir` command in Windows does the same. The `pwd` Linux command prints the complete path to the working directory, and the `grep` Linux command will search for files with a pattern that you specify.
131.    What Linux utility is like the Windows Command Prompt?

        1. Time Machine
        2. Mission Control
        3. Terminal
        4. Shell

        Answer:

        C. The Linux Terminal is a command-driven user interface that allows the user to interact with the shell by typing command at a prompt, much like Windows Command Prompt. The command-driven user interface in macOS is also called Terminal. The shell is the part of the OS that sits between the user and the rest of the operating system, allowing the user to interact with the operating system. Time Machine and Mission Control are features of macOS used for backups and viewing all open applications, respectively.
132.    A system has been doing some quirky things and you think it might have something to do with a temporary file. A best practice to avoid malware is to remove files and programs that aren't being used. Which tool, shown in the graphic (with the name redacted), will you use to delete temporary and unused files from a computer system?

        <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf012_0.jpg" alt="" height="896" width="802"><figcaption></figcaption></figure>

        1. Resource Monitor (`resmon.exe`)
        2. Disk Management (`diskmgmt.msc`)
        3. Registry Editor (`regedit.exe`)
        4. Disk Cleanup (`cleanmgr.exe`)

        Answer:

        D. Disk Cleanup will look through your hard drive and show how much space unused files are taking up. You then have the option to choose which files you would like to delete. Clicking a file type will provide a description of what is being deleted. On modern, large hard drives, the space saved is usually negligible. Resource Monitor shows resources being used by process in real time. Disk Management is a graphic utility for creating, formatting, and managing volumes on any physical drives attached to the system. You can even use it to configure software RAID. The Registry is a huge database that contains information about all the users, hardware, software, and configuration information in a computer. Typically, changing the Registry by using `regedit` is a last resort because changes are immediate and there is no undo button. Control Panel and Windows Settings can do much of the Registry management for you, and they're much safer.
133.    You are at a Windows command prompt. A remote Windows workstation named advertising4 is misbehaving and needs to be shut down and rebooted. What is the proper syntax to shut down this remote system?

        1. `shutdown /r /m \\advertising4`
        2. `shutdown /s /m \\advertising4`
        3. `shutdown /r /c \\advertising4`
        4. `shutdown /s /c \\advertising4`

        Answer:

        A. The `shutdown` command can be used to shut down and restart computers, either the system you are on or a remote one. The `/s` switch is used to shut down a computer, and `/r` is used for a full shutdown and reboot. The `/m` switch followed by the computer name is used to specify the remote computer. The `/c` switch is for comments. There are other switches available. To find out more about the command, type **`shutdown /?`** at a command prompt.
134.    You have recently deployed a custom application to several Windows workstations on your network. The application appears to have a bug, and the developer suggests you edit the Registry to fix it. Which administrative tool would you use to do this?

        1. `msinfo32`
        2. `command`
        3. `regedit`
        4. `notepad`

        Answer:

        C. Windows configuration information is stored in a special configuration database known as the Registry. This centralized database also contains environmental settings for various Windows programs. To edit the Registry, use the `regedit.exe` program. Be careful, though, because an incorrect Registry change can render a system inoperable. Changes are immediate and there is no undo. `msinfo32` is the System Information utility that provides a snapshot of the hardware, software, and some configuration information for the system; `command` is not a valid tool; and `notepad` launches the Notepad program, which is a simple text editor. Commands like these can be run using Command Prompt or the Run command (which can be accessed by pressing Windows Key+R).
135.    A couple of applications that run at startup are causing problems with a computer. Where can you change settings so that those programs won't automatically start when the computer does?

        1. Task Manager, Services tab
        2. Task Manager, Startup tab
        3. Services console
        4. Task Scheduler

        Answer:

        B. To stop (disable) programs from running on startup, use the Startup tab of Task Manager. The System Configuration utility was the place to go in older versions of Windows, but now it merely has a link to Task Manager. Services are programs that run in the background and are part of the operating system, not applications that have been added. A limited subset of them can be configured on the Services tab of Task Manager, or all services can be accessed through the Services console (`services.msc`). Task Scheduler is used to automatically perform some action(s) when a trigger, such as a date, time, or other event, occurs.
136.    You are working on a computer with macOS, and about a dozen applications are open. Which feature allows you to easily see all of them and switch to your desired application?

        1. Spotlight
        2. Keychain
        3. Mission Control
        4. Finder

        Answer:

        C. On a Mac, it's possible to run a large number of things at one time, whether those things in question are apps or Windows desktops. Apple's Mission Control is an easy way to see what is open and to switch between applications. To access Mission Control, you can press the Mission Control key (identified by an image of three different-sized rectangles) on an Apple keyboard, click the Mission Control icon in the Dock (or Launchpad), or swipe up with three or four fingers on a trackpad. Spotlight is used to search for files, folders, images, and such. Keychain is the macOS password management feature, and Finder enables the user to drill down through directories to find what they're looking for, much like File Explorer in Windows.
137.    You have a Windows Pro computer with multiple printers installed. Which Control Panel utility allows you to manage multiple print servers and printers from a single interface?

        1. Devices and Printers
        2. Programs and Features
        3. Network and Sharing Center
        4. Device Manager

        Answer:

        A. From Devices and Printers, you can manage multiple printers and do tasks such as choosing a default printer, installing new printers, and changing printer settings. Programs and Features allows the user to add, remove, or troubleshoot installed programs (the options will change by program) and add or remove Windows features. The Network and Sharing Center is the Windows tool for viewing and configuring network connections, and changing adapter settings. Device Manager should be your go-to app when resolving hardware issues. From there you can update or install drivers, see what isn't working, and disable hardware if need be.
138.    One power state will close applications and files, and log off users like a full shutdown would, then save the kernel state and system session to a hibernation file before shutdown. Then, when the computer is restarted, it will automatically and quickly restore that file, saving some of the time involved in a normal boot. Which of the following states is being described?

        1. Hibernate
        2. Sleep
        3. Selective Suspend
        4. Fast Startup

        Answer:

        D. Fast Startup is similar to Hibernate in how it works, but instead of saving all your applications and data as you had them so that you're instantly back at work, it saves the system state. As described in the question, Fast Startup will close running apps and log off any users, then save the contents of RAM to a hibernation file. When the computer starts back up, it reads the hibernation file and loads drivers, system state, and the kernel much more quickly than it would if the system had to read all of that individually back into RAM as it would in a normal cold boot. Sleep stores everything that's open in RAM and enters a low power state. The display and drives aren't using power, but power is needed to continually refresh memory so that it can retain the information. Sleep uses very little power but “wakes up” very quickly with everything open as it was. The Hibernate option stores open programs and data to the hard drive and, once the computer is hibernated, would use no power, but it will not resume its state as quickly as Sleep would.
139.    You're troubleshooting a computer that is unable to resolve domain names to IP addresses. What command-line utility can help identify what DNS server the computer relies on?

        1. `nslookup`
        2. `netstat`
        3. `ping`
        4. `tracert`

        Answer:

        A. The `nslookup` utility will query the DNS server the computer is currently configured to use. The utility can be used to perform a variety of DNS queries. The `netstat` command shows what TCP connections exist on a computer and the port number they are using. The `ping` command is used to determine whether there is connectivity with a remote computer. When entered as `ping localhost`, it is used to determine if TCP/IP is running on the local computer. `tracert` displays the path (routers) that a packet took to get to a remote computer.
140.    A user recently left the company, and you need to change ownership of their files on the Linux server to a new user. Which command should you use to do this?

        1. `chown`
        2. `chmod`
        3. `cat`
        4. `cp`

        Answer:

        A. The `chown` (change owner) command is used to change ownership of files in Linux. The syntax to change the owner of a file is `chown` _`owner-name filename`_. The `chmod` (change mode) command is used to modify the mode of the file, meaning who has what access to the file. The `cat` command is a powerful tool that can be used to view contents of a file, create new files, and concatenate (put together) files. The `cp` command is used to copy files.
141.    You need to configure a virtual private network (VPN) for an employee working remotely on a Windows Pro computer. What category group in Windows Settings provides options for establishing dial-up or VPN connections?

        1. Network and Sharing Center
        2. Network & Internet
        3. System
        4. Accounts

        Answer:

        B. Network & Internet is the Settings category that provides options for setting up VPN or dial-up connections. Network and Sharing Center is a Control Panel utility. The System category of Settings deals with display, sound, power, notification, and other settings. The Accounts category is useful for managing users and syncing settings. In Windows 11, but not Windows 10, Windows Backup is included in the Accounts category.
142.    While using your Windows laptop remotely, you want to set up a secure connection over a Wi-Fi network. What type of connection do you need to establish?

        1. VPN
        2. Dial-up
        3. Fios
        4. Hotspot

        Answer:

        A. A virtual private network (VPN) is a secured network connection made over an unsecure network. For example, if you wanted to connect your laptop to your corporate network over the Internet in order to read email but you also wanted to secure the connection, you could use a VPN. Dial-up is a very slow and seldom used connection that requires a telephone landline to make a connection. Fios is a vendor name for a fiber-optic connection that provides Internet access and other services, and a hotspot is sharing a cellular device's connection with other devices, essentially making the cellular device a gateway to the Internet.
143.    A print queue has stalled, so you're going to stop and restart the Print Spooler service. Where can you do this? (Choose two.)

        1. The Services console
        2. Task Manager, Services tab
        3. Disk Management, Services tab
        4. Task Scheduler

        Answer:

        A, B. The Services console will enable you to manage all of the computer's services. The Services tab of Task Manager is a subset of those services with a link at the bottom to the full Services console. There are several ways to see what services are running and to enable and disable services. They include the Services console, Computer Management, and the Services tab in Task Manager. In Windows 10, but not Windows 11, you can find the services console in Control Panel, Administrative Tools, and click Services. Disk Management does not have a link to the Services console, and Task Scheduler is designed to perform tasks when a trigger happens, such as a date, time, or event.
144.    A user types their username and password into a workstation that is configured in a domain. What examines their information and determines whether they are allowed access to network resources?

        1. Local operating system
        2. File server
        3. Authentication server
        4. DHCP server

        Answer:

        C. A domain uses an authentication server to determine whether a user is granted access to shared resources. In Windows, an authentication server is also known as a domain controller. Domains are not available with Windows Home editions. Windows Home editions can only use a workgroup, and in that case the operating system on the device with the shared resource would allow or deny access. A file server is a computer that provides access to shared files. A DHCP server is used to automatically assign IP addresses and configure network settings. A DHCP server is often included in the software on a SOHO router.
145.    Your spouse takes gaming seriously and has complained that restart notifications sometimes pop up on the screen at crucial moments, disrupting their game. What settings group can you use to stop restart notifications from appearing and stop unnecessary programs from running in the background?

        1. System
        2. Gaming
        3. Update and Security
        4. Apps

        Answer:

        B. To turn off all notifications, or choose to manage whether and how individual notification senders can interact with you, you could go to Windows Settings, select the System group, and then click Notifications & Actions. This is not the correct answer, though, because it doesn't stop the background activity—it only stops the notifications. Game mode, found in the Gaming options group, enables you to configure the system to be optimized for gameplay and recording. In addition to preventing driver update installations and stopping restart notifications, it modifies settings affecting video frame rate. Update and Security settings don't address notifications. The Apps option lets you manage where apps can be installed from, default apps for opening files, and other application configuration settings.
146.    What type of operating system is found on an Apple iPhone?

        1. iPhone OS
        2. iOS
        3. Android
        4. Windows for iPhone

        Answer:

        B. iOS is the proprietary operating system for iPhones. iPhone OS and Windows for iPhone don't exist. The Android OS was developed by Google and is used on smartphones, tablets, and other touchscreen devices. Other operating systems include iPadOS for use on iPads, and of course Windows, Linux, and macOS found on desktop and laptop PCs, and Chrome OS, which is proprietary and found on Chromebooks.
147.    You want to find and download a new application to use for network monitoring on your MacBook. Where can you do this in the macOS?

        1. Finder
        2. App Store
        3. Mission Control
        4. FileVault

        Answer:

        B. The App Store is where you would go to locate and download new programs. Finder enables a user to drill down through folders to find what they are looking for. Mission Control is an easy way to see what is open and to switch between applications, and FileVault provides encryption.
148.    You work as the IT manager of a telephone call center. Your company just purchased one hundred computers in anticipation of a large wave of hiring, and you need to configure them all with the OS, applications, and settings that your company uses. What type of installation will you do?

        1. Upgrade
        2. Recovery partition
        3. Repair installation
        4. Image deployment

        Answer:

        D. Image deployments are usually done in a large-volume setting where you have many computers configured identically. One machine will have the OS and applications installed and settings configured. Then an image is created. The image can be stored on a network drive, a USB drive, or other media. When it is installed, it will include the OS, software, and settings that were configured on the original machine. An upgrade installation will keep all of your files and settings but install a different version of an OS on your computer. A recovery partition is often created on a laptop that is purchased from a major supplier. There will be a key or multiple keys to press while the computer is booting. The exact key(s) will depend on the laptop manufacturer. Using a recovery partition will erase everything that is on the drive and restore the computer to the state it was in when it was received from the manufacturer. This is sometimes called a factory reset. A repair installation will use the same OS and attempt to leave all your files and settings while fixing any of the operating system files.
149.    A MacBook user has a program that they no longer use. What are their options for removing it from their computer? (Choose two.)

        1. Use Finder, then Applications to locate the app, then right-click and choose Delete.
        2. Use Finder, then Applications to locate the app's folder, then look for an uninstaller and run it.
        3. Use Finder, then Applications to find the app, then drag the app from the Applications folder to the trash.
        4. Click Apple, then Uninstall, and then choose the app.

        Answer:

        B, C. An app can be deleted simply by dragging it to the trash, but if it has its own folder, look for an uninstall program. Right-clicking and choosing Delete is how you might remove a file in a Windows OS. There is no uninstall option from the Apple menu.
150.    You're on a Linux system and need to change a user's access to a file. Which command will you use to do this?

        1. `chown`
        2. `chmod`
        3. `cat`
        4. `cp`

        Answer:

        B. The `chmod` (change mode) command is used to modify the mode of the file, meaning who has what type of access to the file. The _who_ is divided into file owner, group members, and others (everyone else). The permissions they can have are read, write, or execute. The command can get quite complicated, but in its basic form it is `chmod [`_`reference`_`][`_`operator`_`][`_`mode`_`]`_`file`_. As an example, if you want to restrict a user (the owner) of a file named `bogus` from writing to that file, the command is `chmod u=r bogus`. In the command, `u` is the reference to the user, `=` is the operator, and `r` is the mode. Then, to see the result, you enter **`ls -l`** . Before changing the permission on the file named `bogus`, running the `ls -l` command may have shown `-rw-rw-r--`; the first `-` means it's a file, not a folder. After that, the three sets of characters (_`rwx`_) are first set for owner, second set for group, and third set for others. As shown in the graphic, after the `chmod u=r bogus` command is run, the permissions shown for the `bogus` file when `ls -l` is run should be `-r--rw-r--`, showing that the write permission for the owner was removed. The `chown` (change owner) command is used to change ownership of files in Linux. The `cat` command is powerful and can be used to view contents of a file, create new files, and concatenate (put together) files. The `cp` command is used to copy files.

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/bapp01uf004_0.jpg?width=821" alt=""><figcaption></figcaption></figure>
151.    You just got a new MacBook for a child, but they said the text on the screen is too hard to read. What system preference would you use to help them?

        1. Accessibility options
        2. Displays
        3. Privacy
        4. Time Machine

        Answer:

        A. Click Apple, then Preferences, and choose Accessibility Options to find several features that make interacting easier for people with different abilities. Zoom can enlarge text on the screen, VoiceOver will read screen contents, Sticky Keys lets the user press key combinations one key at a time, and there are several other accessibility options.
152.    An application on a user's Windows Pro workstation has become corrupted. Where can you go in Control Panel to attempt to repair or reinstall the application?

        1. Devices and Printers
        2. Programs and Features
        3. Network and Sharing Center
        4. Device Manager

        Answer:

        B. Programs and Features allows the user to add, remove, or troubleshoot installed programs (the options will change by program) and add or remove Windows features. From Devices and Printers you can manage multiple printers and do tasks such as choosing a default printer, installing new printers, and changing printer settings. The Network and Sharing Center is the Windows tool for viewing and configuring network connections and changing adapter settings. Device Manager should be your go-to app when resolving hardware issues. From there you can update or install drivers, see what isn't working, and disable hardware if need be.
153.    A Wi-Fi user at your company said that their MacBook isn't connecting to the network. What option will you choose from Preferences in the Apple menu to turn Wi-Fi on and select Automatically join this network?

        1. Ethernet
        2. Wi-Fi
        3. Network
        4. Accessibility

        Answer:

        C. The correct option is Network, where you can see all the network connections of the MacBook. Ethernet and Wi-Fi are not options in Preferences. Accessibility provides access to features that make working with a Mac easier for differently abled people.
154.    You are at a Linux workstation and need to search for text within several files. Which command should you use?

        1. `sudo`
        2. `grep`
        3. `cp`
        4. `ls`

        Answer:

        B. The `grep` command (short for the impossibly long “globally search a regular expression and print”) does just what it says it does: it searches for a string of text and then displays the results of what it found. The syntax for `grep` is `grep [`_`options`_`]`_`pattern`_`[`_`files`_`]`. The `sudo` command stands for superuser do, or substitute user do, and will run a single command as the alternate user. The `cp` command copies files, and `ls` provides a list of contents of the working directory.
155.    You need to install Windows on a new machine. Which of the following is not an installation option?

        1. USB
        2. Network
        3. External drive
        4. CD

        Answer:

        D. Compact discs (CDs) don't hold enough information to be used for installation media for Windows. Windows media can be installed from a USB or an external drive, or via a network connection provided there is a way to boot to the network such as PXE support.
156.    Which of the following is not a best practice for hardening your macOS against attack?

        1. Use Time Machine to back up your Mac.
        2. Use BitLocker to encrypt your drive.
        3. Install updates and patches as soon as they are available.
        4. Turn on the firewall in the Security & Privacy pane.

        Answer:

        B. The program that is used to encrypt a drive on a Mac is FileVault, not BitLocker. BitLocker does the same in the Windows operating system. Best practices for hardening a Mac system against malware include backing up the data using Time Machine, encrypting the drive, installing patches and updates as soon as they are available, disabling remote access, turning on the software firewall, using a password manager, using a non-admin account, and setting a password-protected screen saver.
157.    Which of the following file extensions indicates a drive image that can be mounted in macOS and treated like a drive?

        1. `.pkg`
        2. `.bat`
        3. `.dmg`
        4. `.app`

        Answer:

        C. A file with a `.dmg` extension is a disk image and can be treated like a drive in macOS. It can be “mounted” like a physical hard drive, the contents read, and files opened, or applications installed. A file with a `.pkg` extension in macOS is a compressed package file. You may be able to view the contents of the file in Finder, but if not, it would need to be extracted first. Files with a `.bat` extension are batch files used in Windows to run a string of commands that have been entered into a text file, and files with an `.app` extension are applications.
158.    The graphics department of your company just purchased a new printer, and now you need to install it. What System preference pane can you use to install new printers in macOS?

        1. Printers
        2. Printers & Scanners
        3. Devices
        4. Sharing

        Answer:

        B. The Printers & Scanners pane is where you would go to install a new printer or configure a printer in the macOS System Preferences folder. Printers and Devices are not options there, but Sharing is, and from there you can share your screen or files and choose from several other options.
159.    You want to find and download a new Wi-Fi analyzer application to use on your Android phone. Where on your phone would you do this?

        1. Finder
        2. App Store
        3. Mission Control
        4. Play Store app

        Answer:

        D. Use the Play Store app on your Android phone to access Google Play, where you can find new apps to install on your Android phone. Finder and Mission Control are applications found on a computer with macOS running. The App Store is where you would go to locate and download new programs for an iPhone.
160.    Your friend just bought a new iPad. What type of operating system will it have?

        1. iPhone OS
        2. iOS
        3. iPadOS
        4. Android

        Answer:

        C. Unlike iOS for iPhones, the iPadOS has features such as Split View that allow it to use multiple applications at the same time. It also boasts support for external drives and displays. iOS is the operating system of iPhones, and the Android OS developed by Google is used on smartphones, tablets, and other touchscreen devices. iPhone OS is not a real term.
161.    You would like to see the contents of a file named `bogus.txt`. What command will you use to view the file's contents?

        1. `chown`
        2. `chmod`
        3. `cat`
        4. `cp`

        Answer:

        C. The `cat` command is powerful and can be used to view contents of a file, create new files, and concatenate (put together) files. For example, to view the line-by-line contents of the `bogus.txt` file, you would simply enter **`cat bogus.txt`**. To add line numbers to the output, enter the command **`cat -n bogus.txt`**. The `chown` (change owner) command is used to change ownership of files in Linux. The `chmod` (change mode) command is used to modify the mode of the file, meaning who has what access to the file. The `cp` command is used to copy files.
162.    Your customer, an artist, uses their Windows 10 tablet PC to enter sales and accept customer payments. They walk around the gallery with it and want to conserve as much power as possible. What Control Panel utility will you use to enable USB Selective Suspend? (Choose two.)

        1. Power Options
        2. Device Manager
        3. Programs and Features
        4. Indexing Options

        Answer:

        A, B. The Power Options utility in Control Panel has a setting to enable or disable USB Selective Suspend. To get there, choose Power Options, then Change Plan Settings, and then Change Advanced Power Settings; then click USB Settings in the Settings list. Note that Windows 11 does not have that option in the Control Panel Power Options utility. In Device Manager, choose Universal Serial Bus Controllers, then double-click USB Root Hub, choose the Power Management tab, and choose “Allow the computer to turn off this device to save power.” Refer to the graphic. USB devices such as a card reader or signature pad may be used so seldom that it makes sense to turn them off when they are not in use, and that is exactly what USB Selective Suspend does. USB Selective Suspend is enabled by default, and this option is available in both Windows 10 and Windows 11. Programs and Features allows the user to add, remove, or troubleshoot installed programs (the options will change by program) and add or remove Windows features. Indexing Options catalogs words in files and the files' metadata to provide faster file searches.

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/bapp01uf005_0.jpg?width=821" alt=""><figcaption></figcaption></figure>
163.    Your company just purchased five new MacBook computers for employee use. You will be providing tech support for them. What filesystem will they have?

        1. HFS+
        2. APFS
        3. ext4
        4. NTFS

        Answer:

        B. APFS, the Apple File System, has been the filesystem used by Mac computers since 2017. It supports up to 9 quintillion files and folders, full-disk encryption, and space sharing, so the free space on a drive is available to all volumes of that drive. HFS+ is an older filesystem that was used by Apple. The ext4 filesystem is used in the Linux world, and NTFS (New Technology File System) is the Windows filesystem that supports file encryption and NTFS permissions for file sharing.
164.    Your friend wants a new phone but has told you that they are not fond of Apple products. They've decided to buy a Microsoft Duo product. What operating system will likely be on their new phone?

        1. iPadOS
        2. iOS
        3. Android
        4. Windows

        Answer:

        C. Although the Duo products are made by Microsoft, they run an Android OS, not Windows. There is no Windows version for phones. iPadOS and iOS are Apple's proprietary operating systems.
165.    On a Mac using macOS 10.6 or later, what is the best way to protect the system against viruses and other malware? (Choose two.)

        1. Install an antivirus from a vendor you trust.
        2. Ensure the system data files and security updates are set to run automatically.
        3. Only install software from reliable sources.
        4. Use Finder to find and delete viruses and malware.

        Answer:

        B, C. Since Snow Leopard (macOS 10.6) Apple has included malware detection, called File Quarantine, in its software. File Quarantine will not allow a known malware file to be opened. In order to protect your system from the most recent malware, you need to ensure that updates will run automatically. This is done by choosing System Preferences from the Apple menu, selecting App Store, and selecting Automatically Check For Updates and then Install System Data Files And Security Updates. It's also good advice to only download programs and files from reputable sources, like the App Store. You could install an antivirus or anti-malware product, but it probably isn't necessary. Finder is used to find folders and files in the directory structure, much like Windows File Explorer.
166.    A user calls the hotline saying that they can't get directions and Siri can't give them the weather. What System Preferences pane do they need to use to remedy the situation?

        1. Security & Privacy
        2. Mission Control
        3. Accessibility
        4. Networks

        Answer:

        A. The Privacy tab in the Security & Privacy pane is where you would enable Location Services, which is how Siri knows where you are to tell you about the weather, provide maps, and give you directions. The window for each type of privacy concern will show what applications have requested Location Services. Also on the Privacy tab are Contacts, Calendars, Reminders, Photos, Accessibility, and Analytics. Mission Control will show all the open apps for quick access. Accessibility allows you to configure settings for differently abled people, and the Networks pane will show all the computer's network settings.
167.    A salesperson will be working remotely, and you need to set up a virtual private network (VPN) for them. What Control Panel utility will you use to do this?

        1. Devices and Printers
        2. Programs and Features
        3. Network and Sharing Center
        4. User Accounts

        Answer:

        C. The Network and Sharing Center is the Windows tool for viewing and configuring network connections and changing adapter settings. From here you can also manually set up a new connection or network such as dial-up, VPN connections, or even a wireless access point (WAP). From Devices and Printers, you can manage multiple printers and do tasks such as choosing a default printer, installing new printers, and changing printer settings. Programs and Features allows the user to add, remove, or troubleshoot installed programs (the options will change by program) and add or remove Windows features. User Accounts is the utility for adding new user accounts, changing their passwords, or managing profiles as well as other user-related configurations.
168.    A user brought you a laptop that wouldn't boot into the OS. After trying some troubleshooting techniques, you inform them that you will need to reinstall the operating system. After ensuring that they have a backup of their files, you restart the computer, press F10, and the OS installation begins. What type of installation are you doing?

        1. Upgrade
        2. Recovery partition
        3. Repair installation
        4. Image deployment

        Answer:

        B. This is a recovery partition installation. A recovery partition is often created on a laptop that is purchased from a major supplier. There will be a key or multiple keys to press while the computer is booting. The exact key(s) will depend on the laptop manufacturer. Using a recovery partition will erase everything that is on the drive and restore the computer to the state it was in when it was received from the manufacturer. This is sometimes called a factory reset. An upgrade installation will keep all your files and settings but install a different version of an OS on your computer. A repair installation will use the same OS and attempt to leave all your files and settings while fixing any of the operating system files. Image deployments are usually done in a large-volume setting where you have many computers configured identically. One computer will have the OS and applications installed and settings configured. Then an image of that computer is created. The image can be stored on a network drive, a USB drive, or other media. When it is installed, it will include the OS, software, and settings that were configured on the original computer.
169.    A second person is going to be using the Windows computer at your desk when you're not there. What would you choose in Windows Settings to create their user account?

        1. Accounts
        2. User Accounts
        3. Personalization
        4. System

        Answer:

        A. Accounts is the group in Windows Settings that will enable you to add a new user. From there, click Family & Other Users; then, in Windows 10, click Add Someone Else To This PC. In Windows 11, you click Add Other User. User Accounts is the Control Panel utility for managing users. From the Personalization menu of Windows Settings, you can change the desktop theme and background colors. The System group in Windows Settings has a multitude of settings, including Display, Sound, Notifications & Actions, and Power.
170.    You're working in the Linux Terminal and need to locate a file. Which command lets you locate and perform actions on a file?

        1. `find`
        2. `ps`
        3. `man`
        4. `nano`

        Answer:

        A. The `find` command is used to find files and directories and perform operations on them. The syntax of the command is _`find`_`[`_`where to look`_`] [-`_`options`_`][`_`what to find`_`]`. For example, `find Documents -name ∗.jpg` will find all the files in `Documents` and its subfolders that have `.txt` at the end. Find can also search by folder, name, creation date, modification date, owner, and permissions. The `ps` command will list the processes that are currently running, along with their PIDs (process IDs); the `man` command displays a user manual for any Linux command, much like the Windows `/?` command; and `nano` is a Linux text editor.
171.    A user wants to install an application that requires a 1 GHz processor on a Windows 10, 64-bit installation. What is the minimum speed processor that their computer must have?

        1. 1 GHz
        2. 2 GHz
        3. 3 GHz
        4. 4 GHz

        Answer:

        B. Windows 10 64-bit requires a 2 GHz or faster processor, so that's what the system in question must already have. Unlike RAM, where you must add the requirements together, choose a processor that is at least the fastest requirement of all the running software—in this case, the 2 GHz processor that is needed for the operating system. You would not need to buy a faster processor to accommodate the new software.
172.    Which of the filesystems listed is compatible with more operating systems than the others?

        1. FAT32
        2. exFAT
        3. NTFS
        4. ext4

        Answer:

        A. File Allocation Table 32 (FAT32) is more compatible than the other filesystems. It can be read by Windows, Linux, macOS, and many game consoles. Extensible File Allocation Table (exFAT) partitions require a third-party software to be read by Linux, and New Technology File System (NTFS) doesn't play well with any operating system other than Microsoft Windows. Fourth Extended Filesystem (ext4) partitions are used in Linux. Microsoft systems can't even recognize ext4 partitions.
173.    What operating systems can be found on a smartphone? (Choose two.)

        1. iOS
        2. macOS
        3. Android
        4. Windows 11

        Answer:

        A, C. Once upon a time Microsoft had a Windows version for smartphones, but they no longer do. On modern smartphones you'll most likely find either iOS or Android, although there is also Tizen, which is a Linux, open source mobile operating system developed by Samsung. macOS and Windows 10 are for laptop and desktop computers. BlackBerry once had a smartphone operating system but now relies on Android and is known for and focused on their security software for smartphones. Bada and Symbian are other discontinued smartphone operating systems. Remember to focus on the mobile OSs that are listed on the CompTIA A+ objectives. Those are iPadOS, iOS, and Android.
174.    Before you upgrade your Windows 8.1 OS to Windows 10, you want to create a backup of your Windows 8.1 system configuration so that you can restore it if something goes wrong. What should you create?

        1. Restore point
        2. System restore
        3. Windows backup
        4. Shadow copy

        Answer:

        A. A restore point is a copy of your system configuration at a given point in time. Restore points are useful for when Windows fails to boot but the computer appears to be fine otherwise, or when Windows doesn't seem to be acting right and you think it was because of a recent configuration change. In Windows 10, restore points are created on the System Protection tab of System Properties.
175.    A friend has a game that they love on their macOS desktop computer, and they want to put it on the Windows laptop that they travel with. What will you tell them?

        1. Sure, it's no problem to install it.
        2. They can only install it if both are 64-bit systems.
        3. They can install macOS software on a Windows machine, but not Windows software on a Mac.
        4. They will need to find a Windows-compatible version of the software to install it on their Windows laptop.

        Answer:

        D. Software intended for macOS and Windows are not interchangeable, but some software packages come in a macOS version and a Windows version, so it's important to make sure you purchase the correct one. Windows can be run on a Mac, but not at the same time. You would need to run a program called Boot Camp to create a Windows partition on the Mac's hard drive, then install the Windows OS on that partition. At boot, you can choose either Windows or macOS, but you can't run Windows applications on macOS.
176.    You're looking at the specifications for a new computer and notice that it says, “Intel® UHD Graphics 630 with shared graphics memory.” What is true about this graphics card? (Choose two.)

        1. The GPU is on an expansion card.
        2. The GPU is located on the processor.
        3. It uses part of the system's RAM.
        4. It has its own VRAM.

        Answer:

        B, C. A video card can either be discrete or integrated. If it is integrated, then the graphics processing unit (GPU) resides on the processor, and the GPU will share RAM with the system. A discrete video card will contain a GPU and VRAM (Video RAM) and will be installed in an expansion slot.
177.    You want to uninstall an app on a Windows computer. Where will you go in Windows Settings to uninstall it?

        1. System
        2. Apps
        3. Update And Security
        4. Gaming

        Answer:

        B. The Apps group of Windows Settings lets you delete or update apps, choose apps to start when you log in, choose default apps for opening files, and other application configuration settings. The System group has settings for display, power, sound, and notifications, and several other options. Update And Security (Windows 10 only) has a plethora of tools, including Windows Update, Troubleshooting, Activation, Recovery, and Windows Security. (The similar Settings group in Windows 11 is Windows Update, but it is only for updates and recovery options. Troubleshooters and Activation are found in the System group, and Windows Security settings are found in the Privacy & Security group of Windows 11 Settings.) The Gaming option enables you to configure the system to be optimized for gameplay and recording.
178.    You just built your first computer from components. What type of operating system installation will you perform?

        1. Upgrade installation
        2. Recovery partition
        3. Clean installation
        4. Image deployment

        Answer:

        C. You will be performing a clean installation. Clean installations happen on a new machine that doesn't have an operating system at all (bare metal) but can also happen when you want to completely wipe out the drive and begin fresh. An upgrade installation can only happen when there is an existing operating system, and will keep all of your files and settings but install a different version of an OS on your computer. A recovery partition is often found on laptops, and sometimes on desktop PCs, that are purchased from a major supplier. There will be a key or multiple keys to press while the computer is booting. The exact key(s) will depend on the laptop manufacturer. Using a recovery partition will erase everything that is on the drive and restore the computer to the state it was in when it was received from the manufacturer. This is sometimes called a factory reset. Image deployments are usually done in a large-volume setting where you have many computers configured identically. One computer will have the OS and applications installed and settings configured. Then an image of that computer is created. The image can be stored on a network drive, a USB drive, or other media. When it is installed on new computers, it will include the OS, software, and settings that were configured on the original computer.
179.    You're upgrading your Windows 10 Home edition to Windows 10 Pro. What utility will you use to make a backup of your data before upgrading the system? (Choose two.)

        1. File History
        2. Windows Update
        3. Recovery
        4. Backup

        Answer:

        A, D. Type **`backup`** in the Windows 10 search box and click Backup Settings, and you'll be taken to a screen that says “Back up using File History.” You can also find the Backup window in Settings in the Update & Security group. You'll need a storage device such as an external hard drive, then from the Backup window you'll choose to automatically create backups and click More Options to choose the frequency. Every hour is the default, but the backup schedule options vary from 10 minutes up to Daily. Here you can also choose what files to back up. Windows Update checks for operating system updates, and Recovery is the utility that is used to reset a PC, meaning that the operating system is reinstalled but you can choose to keep your personal files.
180.    You're buying a new graphics-intensive program that says it must have a GPU with 256 MB of dedicated VRAM. Your existing graphics adapter's properties are shown in the graphic. What is your best option?

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf015_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

        1. Purchase a new graphics card that meets the requirement.
        2. Replace the CPU with one that has an integrated GPU.
        3. Add VRAM to your graphics card.
        4. Add RAM to your system.

        Answer:

        A. VRAM is memory that is dedicated solely to be used by the graphics processing unit (GPU). The GPU takes the work of processing graphics away from the CPU. GPUs can either be integrated (on the CPU) or dedicated (on a discrete graphics card). A graphics card will have its own cooler and VRAM. VRAM on a video card can't usually be upgraded. To increase it, you would need to buy a different video card. In this scenario, you might be able to replace the CPU with one with integrated graphics, if the system supports the new processor, but that isn't the best option.
181.    You're working in the Linux Terminal and aren't sure how to use the `ps` command. Which of the following will show you detailed information about the command?

        1. `find ps`
        2. `ps man`
        3. `man ps`
        4. `nano ps`

        Answer:

        C. Linux has a built-in manual that can be accessed using the `man` command, similar to using Windows `help [`_`command`_`]` or `[`_`command`_`] /?` at a command prompt. The syntax is `man [`_`command`_`]`. The `find` command is used to find files and directories and to perform operations on them. The `ps` command will list the processes that are currently running, along with their PIDs (process IDs), and `Nano` is a Linux text editor. `[`_`command`_`] --help` can also be used at a Linux Terminal prompt to get help on a specific command.
182.    You're moving your Windows 8.1 computer to Windows 10. What type of installation are you doing?

        1. Upgrade installation
        2. Recovery partition
        3. Clean installation
        4. Image deployment

        Answer:

        A. You will be performing an upgrade installation. An upgrade installation can only happen when there is an existing operating system. It will keep all of your files and settings but install a different version of an OS on your computer. A recovery partition is often found on a laptop (and some desktops) that is purchased from a major supplier. There will be a key or multiple keys to press while the computer is booting. The exact key(s) will depend on the laptop manufacturer. Using a recovery partition will erase everything that is on the drive and restore the computer to the state it was in when it was received from the manufacturer. This is sometimes called a factory reset. Clean installations happen on a new machine that doesn't have an operating system at all (bare metal) but can also happen when you want to completely wipe out the drive and begin fresh. Image deployments are usually done in a large-volume setting where you have many computers configured identically. One computer will have the OS and applications installed and settings configured. Then an image of that computer is created. The image can be stored on a network drive, a USB drive, or other media. When it is installed on the new computers, it will include the OS, software, and settings that were configured on the original computer.
183.    You're considering upgrading your Windows 8.1 PC to Windows 10. Which of the following does not need to be done before upgrading?

        1. Backups of user files and preferences
        2. Operating system refresh
        3. Check application and driver compatibility
        4. Check hardware compatibility

        Answer:

        B. To refresh an OS (operating system) you would reinstall the same version over the existing one to correct issues with OS files. You don't need to do that when you are upgrading a system to a new OS. Whenever you're doing an upgrade, it is important to consider several things. Backups must be made in case something goes wrong. Before you start the upgrade, you'll want to ensure that the applications you run are compatible with the new OS and that compatible drivers are available for your hardware. You'll also want to ensure that the hardware you have will work with the new OS.
184.    You're purchasing a software that says it uses 32-bit processing. Your computer has a 64-bit processor. Can you use this software on your computer?

        1. Yes, a 32-bit software can run on a 64-bit processor.
        2. No, a 32-bit software must have a 32-bit processor.
        3. Yes, if you replace the processor with a 32-bit one.
        4. Yes, it will just need more RAM.

        Answer:

        A. You can run a 32-bit software on a 64-bit processor—it just doesn't take advantage of the 64-bit processor's full capabilities. However, you cannot run a 64-bit software on a 32-bit processor.
185.    Which of the following commands, when entered into a Linux terminal, will open a text editor?

        1. `find`
        2. `ps`
        3. `man`
        4. `nano`

        Answer:

        D. `Nano` is a user-friendly text editor available in many Linux distributions. The Nano software is launched using the `nano` command. Other text editors such as Vim and Emacs may also be available, but Nano is easier to use. The `find` command is used to find files and directories and perform operations on them. `find` can also search by folder, name, creation date, modification date, owner, and permissions. The `ps` command will list the processes that are currently running, along with their PIDs (process IDs), and the `man` command displays a user manual for any Linux command, much like the Windows `[`_`command name`_`] /?` command.
186.    You would like to know the IP address of a website. What Linux tool will you use?

        1. `chown`
        2. `dig`
        3. `top`
        4. `ip`

        Answer:

        B. The `dig` command can be used to retrieve the IP address of a website; for example, `dig` [`Sybex.com`](http://sybex.com/)`+short` will return the IP address of [`Sybex.com`](http://sybex.com/). The `chown` (change owner) command is used to change ownership of files in Linux. The `top` command displays dynamic information about the running processes, and the `ip` command is used to display configuration information for network interfaces.
187.    Which of the following is not true regarding managed Apple IDs?

        1. They are created by a company for its employees.
        2. They can't make purchases.
        3. An IT administrator can remove or update your account.
        4. You can reset your own password.

        Answer:

        D. With managed Apple IDs, your company, not you, can reset your password. Your company owns a managed Apple ID, so there are restrictions in place. A managed ID is created by a company for use in company business. Since it's linked to your company, your managed Apple ID can't be used to make purchases, and an IT administrator at your company can restrict access to your account, remove it, or update it.
188.    Your accounting department uses an application that requires they enter a username and password, then insert a fob into a USB port on the computer in order to move money between accounts at the bank. Which of the following are true? (Choose two.)

        1. They are using two-factor authentication.
        2. They are using an external software token.
        3. They are using an external hardware token.
        4. Their bank account can never be hacked.

        Answer:

        A, C. Requiring multifactor or two-factor authentication has become somewhat standard for applications that require a high level of security. By entering a password (something you know) and requiring the fob (something you have), the application is requiring two-factor authentication. An example of a software token would be a code emailed to you that you can check on the same device you are using to access the application. An external hardware token is anything physical that you must have in your possession, such as a key fob that must be inserted into the computer, a key fob that generates a code that changes every 30 seconds, or your cell phone with an authenticator app.
189.    Which of the following filesystems is optimized for flash drives?

        1. FAT32
        2. NTFS
        3. ext4
        4. exFAT

        Answer:

        D. Extensible File Allocation Table (exFAT) is optimized for flash drives because it has low overhead like the File Allocation Table 32-bit (FAT32) filesystem (as opposed to New Technology File System \[NTFS]). However, like NTFS it will support much larger file sizes than FAT32, which is limited to 4 GB. exFAT is less compatible with non-Microsoft operating systems than FAT32 is, but more compatible than NTFS. For example, macOS can only read NTFS partitions, but it can read and write to exFAT partitions.
190.    You are working on a Linux workstation. A file named `docs` needs to be renamed to `newdocs`. What is the right command to do this?

        1. `ren docs newdocs`
        2. `mv docs newdocs`
        3. `cp docs newdocs`
        4. `rm docs newdocs`

        Answer:

        B. In Linux, the `mv` (move) command is used to rename files. As shown in the answer, the syntax is `mv [`_`old-file-name`_`] [`_`new-file-name`_`]`. The `cp` command copies a file, but that is a different process than moving it. `rm` is short for remove, and it deletes files. `ren` is a Windows command to rename files.
191.    Which of the following software packages lets Linux, Windows, and other operating system platforms use shared files, shared printers, and other resources across a network or the Internet?

        1. Spotlight
        2. Time Machine
        3. Samba
        4. FileVault

        Answer:

        C. Samba is a widely used freeware program based on SMB (Server Message Block) and CIFS (Common Internet File System) that lets operating systems communicate despite their differences. A request for resources is sent from a client to a Samba server, which forwards the request to the host. The host can either accept or deny the request. Spotlight, Time Machine, and FileVault are macOS tools for finding files, folders, and programs; making backups; and file encryption, respectively.
192.    You have Control Panel open and want to quickly check how much RAM is installed in the system and what processor it has. Which Control Panel utility will you use to view this information?

        1. System
        2. Device Manager
        3. Devices And Printers
        4. Programs And Features

        Answer:

        A. The System utility of Control Panel provides a link to the System Settings group, where you can choose the About option in Windows Settings. The screen that pops up by default shows information about the PC such as its name, the specific processor it has, how much physical RAM is installed, the Windows version and edition, and so on. Device Manager is used for troubleshooting hardware and installing device drivers. Devices And Printers is used for managing printers and multifunction devices, as well as other devices that are connected to the computer. Programs And Features helps in uninstalling applications and adding or removing Windows features.
193.    You downloaded a new application that you want to install on your Windows 10 PC and noticed that it has only one file, and that file has an `.iso` extension. Which of the following is true regarding this file?

        1. Double-click it and let it run to install the application.
        2. Right-click the file and choose Mount. Windows will then see and treat the file as a disk in an optical drive.
        3. You will need a third-party utility to open this file.
        4. Right-click and choose Extract to install the software.

        Answer:

        B. Files with an .iso extension are disk image files. In order to install the software they contain, you need to first mount the image. You may be able to double-click it; if not, right-click and choose Mount, or locate the file in File Explorer. Select the file, then click Mount under Disk Image Tools. Once mounted, the operating system will treat the file as a disk in an optical drive. You'll look for an installer or autorun file to start the software installation. When you're done using the image, right-click it and choose eject. Extract is an option for zipped files, not ISO files.
194.    You're considering installing a new software for monitoring network traffic. You know that it will generate additional network traffic of its own. Which of the following should be considered before purchasing the software? (Choose three.)

        1. Impact to the network
        2. Impact to operations
        3. Impact to the software company
        4. Impact to business

        Answer:

        A, B, D. Whenever you're considering a new software purchase, there are many things to consider. The technical aspects such as OS and application compatibility and hardware concerns are only a part of it. You must also consider what impact this will have on any devices, the network, how internal systems work and the operation of the business, and the business as a whole—how will it affect the company's bottom line? In the case of the network monitoring software presented in the question, consider whether the additional network overhead will cause a significant enough impact on the network to cause adverse effects on production, and will it decrease company profits by slowing production, or is it a wise investment because it can help protect against malware? Will it work well with routers, switches, and other network hardware? Do the positive impacts outweigh the negative ones?
195.    An application that you're installing requires 20 GB of space plus storage for data files of 400 GB. What is the absolute minimum size your hard drive must be if you're running Windows 10 64-bit, which requires 20 GB of storage?

        1. 20 GB
        2. 400 GB
        3. 420 GB
        4. 440 GB

        Answer:

        D. With today's hard drives measured in TB, storage is seldom a problem, but in an industrial setting it might be. When determining how big a hard drive needs to be, add together the storage requirements of everything that will be on that drive, including the operating system, the applications that will be installed, and all the data that will be generated by those applications. With RAM, you need to consider what will be running at the same time, but with storage, consider all the applications and all the data whether or not they are all working at the same time. It's also important to consider what type of data files will be stored. Word documents take up much less space than video files do.
196.    You're working at a Linux command prompt (that is, you're in the Linux Terminal) and need to delete a file called `oldstuff.txt`. Which of the following commands will work?

        1. `rm oldstuff.txt`
        2. `del oldstuff.txt`
        3. `er oldstuff.txt`
        4. `rd oldstuff.txt`

        Answer:

        A. In Linux, `rm` (remove) is the command for deleting files and directories. As shown, the syntax is `rm [`_`option`_`] [`_`what-to-remove`_`]`. If you're removing more than one file at a time, list the files after the remove command such as `rm`_`file1.ext file2.ext`_. By using options, the `rm` command can also remove directories and work in verbose mode, meaning that it will tell you what it's doing. `del` is used to delete one or more files at a Windows command prompt. `er` is not a known command in either Linux or Windows, and `rd` is a Windows command to remove directories.
197.    Which of the following extensions indicates a file that can be extracted or opened with an installer app to install an application?

        1. `.pkg`
        2. `.bat`
        3. `.dmg`
        4. `.app`

        Answer:

        A. A file with a `.pkg` extensions in macOS is a compressed package file. You may be able to view the contents of the file in Finder, but if not, it would need to be extracted first. It can be installed by double-clicking it or opening it with an installer. A file with a `.dmg` extension is a disk image and can be treated like a drive in macOS. It does not need to be extracted. It can be “mounted” like a physical hard drive, the contents read, and files opened or applications installed. Files with an `.app` extension are applications, and files with a `.bat` extension are batch files used in Windows to run a string of commands that have been entered into a text file.
198.    Which of the following is not an advantage of downloadable software distribution over using physical media to distribute software?

        1. It's always current.
        2. It costs the distributor less.
        3. It works on a system without a DVD drive.
        4. It works on all bare-metal systems.

        Answer:

        D. A bare-metal system is one that doesn't have any software yet, including the operating system. It would not be able to download software to install. It could be used for a network installation of an OS if it supported Preboot Execution Environment (PXE) booting to the network, but that would be using a LAN to distribute software as opposed to downloadable distribution, which by definition uses the Internet. Distributing software via download means that it could be the most up-to-date version of the software. It costs less because no one must pay for the USB or DVD to distribute it, and it only requires an Internet connection, not a DVD drive. Many new PCs don't have optical drives.
199.    You're working on a Windows computer that is having some trouble booting. After trying System File Checker (SFC) and other troubleshooting techniques, you decide that you need to reinstall the operating system files. What type of installation will you be doing?

        1. Upgrade
        2. Repair
        3. Clean
        4. Remote

        Answer:

        B. A repair installation (or repair upgrade, as Microsoft calls it) means that you're installing the same version of the same operating system over on top of the existing operating system. A repair installation can be done from within the existing operating system or from other media. It will go through a licensing screen and some others, eventually showing a screen where you will choose to keep Windows settings, personal files, and apps. An upgrade installation will also keep your files, apps, and settings, but you will be using a newer version of the operating system. A clean installation wipes out everything on the hard drive. A remote installation is done across a network and could be any of the other three types.
200.    You need to quickly view the network configuration on a Linux computer. What command will you use?

        1. `ipconfig`
        2. `ipconfig /all`
        3. `ip`
        4. `cfg`

        Answer:

        C. The `ip` command is used to configure and view network settings in modern Linux distributions, replacing the former `ifconfig` command. Like most Linux commands, there is a multitude of objects and options that can be used. Likely the most frequently used one is `ip addr show`, which will show all the network interfaces and their respective IP addresses. `ipconfig` and `ipconfig /all` are Windows commands for viewing IP configuration. `cfg` isn't an actual command.
201.    You purchased a Windows 10 laptop and notice that it immediately resumes when you open the lid. What allows it to do that?

        1. Hibernate
        2. Idle mode
        3. Modern Standby
        4. Auto off

        Answer:

        C. Windows supports a feature called Modern Standby. Modern Standby must also be supported by the hardware. With Modern Standby, the system will wake from the lowest power to allow short bursts (milliseconds) of software execution as the system needs them. The system uses just enough power to process background tasks but still preserves battery life. The result is that when in sleep mode, a computer can stay connected to a LAN and reacts much like a smartphone with instant on/instant off ability.
202.    You're at a command prompt in Windows and need to quickly add a user named student. What command will you use?

        1. `net user student ∗ /add`
        2. `net use /add student ∗`
        3. `net user student ∗`
        4. `user /add student`

        Answer:

        A. The `net user` command can be used at a command prompt to add a user on the fly. The syntax is `net user` _`username`_ `[`_`password`_ `| ∗] /add [`_`options`_`] [`_`/domain`_`]`. In this example, we are adding a user named student, and the ∗ replacing _`password`_ tells the system to prompt us for a password. If no domain is specified, the command assumes the user is added to the local computer. As soon as this command is executed, the named user will appear in the Users utility of Control Panel.
203.    What shortcut keys can you use to quickly access many of the technician tools used in Windows operating systems?

        1. Press Windows Key+D.
        2. Press Windows Key+L.
        3. Press Windows Key+I.
        4. Press Windows Key+X.

        Answer:

        D. Pressing Windows Key+X will open the Quick Link menu. On it, in Windows 11 you will find shortcuts to Apps And Features, Mobility Center, Power Options, Event Viewer, Device Manager, Network Connections, Disk Management, Computer Management, Task Manager, Settings, File Explorer, Search, and Run. The Windows 10 Quick Link menu includes links to Windows PowerShell and Windows PowerShell (Admin). You can also click Shut Down or Sign Out from the Quick Link menu, or click Desktop, which will display or hide all open applications on the desktop. Pressing Windows Key+D will also hide or display all open applications. Pressing Windows Key+L is a quick way to lock the computer, and pressing Windows Key+I brings you to Windows Settings.
204.    A friend just installed Windows 10 on their bare-metal machine. They called you because everything works except for their network. What do they need to do?

        1. Reinstall the operating system.
        2. Install third-party drivers.
        3. Remove and reinstall the network card.
        4. Replace the faulty network card.

        Answer:

        B. The Windows operating system contains many drivers that will help make setting up a new operating system easy, but it would be impossible for the installation media to have all drivers for all the devices that are available. When you have a device whose driver, or a compatible one, doesn't automatically install, you'll have to install the driver from a third party, such as the motherboard manufacturer. Often these drivers can be downloaded from an online source.
205.    What Linux command is used to display the partial dynamic table shown in the graphic?

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf016_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

        1. `chown`
        2. `dig`
        3. `top`
        4. `ip`

        Answer:

        C. The `top` command provides a dynamic chart of the running processes with the details as shown in the graphic. The top section of the screen shows resources used and process statistics. The bottom shows the processes that are currently running. The `dig` command can be used to retrieve the IP address of a website. The `chown` (change owner) command is used to change ownership of files in Linux, and the `ip` command is used to display configuration information for network interfaces.
206.    A Mac user accidentally deleted an app and wants to reinstall it. They believe that the file to install the software again is still on their computer. What file extensions will you be looking for? (Choose two.)

        1. `.pkg`
        2. `.bat`
        3. `.dmg`
        4. `.app`

        Answer:

        A, C. A file with a `.pkg` extension in macOS is a compressed package file. You may be able to view the contents of the file in Finder, but if not, it would need to be extracted first. It can be installed by double-clicking it or by opening it with an installer. A file with a `.dmg` extension is a disk image and can be treated like a drive in macOS. It can be “mounted” like a physical hard drive, the contents read, and files opened, or applications installed from it. Files with an `.app` extension are applications, and files with a `.bat` extension are batch files used in Windows to run a string of commands that have been entered into a text file.
207.    What feature, known more for mobile devices than desktops, is available for the desktop macOS by using a trackpad or Magic Mouse?

        1. SDK
        2. Power options
        3. Gesture-based interactions
        4. Emergency notifications

        Answer:

        C. Modern touchpads/trackpads can accept multiple finger gestures that function similarly to gestures on a smartphone or tablet, such as swipe left or right to move between pages. To see what gestures are available, choose System Preferences from the Apple menu, then select Trackpad. Software development kit (SDK) is more of a programming term. Emergency notifications and power options have little to do with a trackpad or Magic Mouse. Incidentally, gestures are also available in Windows. To view or modify multi-finger gestures on your Windows 10 PC, in Windows Settings, choose Devices, then Touchpad. In Windows 11, from Windows Settings, choose Bluetooth & Devices, then Touchpad.
208.    You have a workgroup with all Windows Home PCs. One of the computers is sharing a folder with two users who don't have an account on this PC. What Control Panel utility will you use to add the users and their passwords to this computer?

        1. Administrative Tools
        2. User Accounts
        3. Local Users and Groups
        4. Mail

        Answer:

        B. You would use the User Accounts Control Panel utility to add new accounts for the users. If you were on a Windows Pro or better computer, you could use the Local Users and Groups app, but that is not available in Windows Home editions. It also isn't listed as a separate Control Panel utility, but in Windows 10 Pro and higher editions (not Windows 11) it can be accessed through Administrative Tools (choose Computer Management, then Local Users and Groups). The Administrative Tools utility doesn't have a link to the Control Panel User Accounts utility, which is not as versatile as Local Users and Groups. The Mail utility is where you would configure user profiles for use with Microsoft Outlook.
209.    You need to check the integrity of key Windows system files on the C: drive, which are hidden from view by default. Which tool can you use to allow you to view hidden files and their extensions?

        1. Computer Management
        2. System Configuration
        3. Local Security Policy
        4. File Explorer

        Answer:

        D. Some of the most important files that you will need to work on are hidden by default as a security precaution. To make certain folders or files visible, you need to change the view properties of Windows File Explorer. This is generally done by going to the View tab and selecting Hidden Items in the Show/hide group. Here you can also hide or show file extensions. The same window can be accessed through File Explorer Options in Control Panel. Computer Management is a collection of tools, including Disk Management and System Tools. System Configuration has settings for changing how the computer boots and links to other tools. Local Security Policy allows you to configure options like password complexity and duration.
210.    On your personal computer, it seems that searching through files has gotten slower and slower. What utility will organize data so searches run faster?

        1. In Control Panel, choose the Indexing Options utility.
        2. In Windows Settings, choose the System group.
        3. In Windows Settings, choose the Apps group.
        4. In Control Panel, choose the Default Programs utility.

        Answer:

        A. Control Panel's Indexing Options looks at words in files and the files' metadata to provide faster file searches. The System group of Windows Settings enables you to configure notifications, power, and many other settings, but not Indexing. The Apps group of Systems is where you can choose default programs and remove applications that you no longer need. The Default Programs app of Control Panel allows you to manage default applications for opening types of files such as photos or mail by opening those settings in Windows Settings.
211.    You are on a domain controller and need to share a folder of data files for some users and not others. Where will you configure access to the folder? (Choose two.)

        1. On a domain controller.
        2. In Windows Active Directory.
        3. Configure Sharing on individual workstations.
        4. Run a batch file to copy the files to each user who needs access.

        Answer:

        A, B. When a computer logs into a domain, access to resources is controlled through Active Directory. The server that Active Directory resides on is called a domain controller (DC). In a workgroup, sharing would be configured on the computer that was providing access to the files. Running a batch file to copy the files to each user would result in multiple copies of the files, likely with all different information after a time, not a single file repository where the files are shared among users.
212.    On your network, a few users have been accessing material on inappropriate websites. What type of server can you install to block content from a list of prohibited websites?

        1. DNS server
        2. Authentication server
        3. Proxy server
        4. Web server

        Answer:

        C. A proxy server makes requests for resources on behalf of a client. Proxy servers are known for three things. One, the proxy server can cache the information requested, speeding up subsequent searches. Two, the proxy can act as a filter, blocking content from prohibited websites and blocking sensitive data from leaving the network. Three, the proxy server can modify the requester's information when passing it to the destination, blocking the sender's identity and acting as a measure of security; the user can be made anonymous. A DNS server resolves IP addresses to domain names. An authentication server verifies the identity of a user and their access to resources, and a web server provides information in files that can be read by a web browser, whether internal to the company or on the Internet.
213.    You're installing Windows 11 Enterprise in a bare-metal system. What is the maximum amount of RAM you can put into this system?

        1. 128 GB
        2. 2 TB
        3. 6 TB
        4. 256 TB

        Answer:

        C. Windows 11 maximum RAM limits are 128 GB for the Home edition, 2 TB for the Pro edition, and 6 TB for the Pro for Workstations and Enterprise editions. They are the same limits for Windows 10 64-bit, but the maximum RAM for any 32-bit Windows operating system is only 4 GB.
214.    You are creating a network for a small office with Windows Pro computers. They do not want centralized security, but they want it to be easy to share printers and files, including libraries. What type of network setup should you recommend?

        1. Workgroup
        2. Homegroup
        3. Personal area network
        4. Domain

        Answer:

        A. You would want a workgroup. By default, Windows 10 computers will join a workgroup called workgroup, making it easy to share files, printers, and other resources. Access to resources is configured on each workstation that is sharing a resource. The drawbacks of a workgroup are that security is configured on each PC, and it's only appropriate for very small networks. Homegroup was a networking scheme in prior versions of Windows that shared libraries. A personal area network (PAN) consists of a PC and its wireless devices, usually paired Bluetooth devices such as printers, headphones, and input devices. A domain is a network where access to resources is configured on a central server that all users of the resources must log into.
215.    Which File Explorer layout shows filename, data modified, type, and size of the file?

        1. Extra large icons
        2. Details
        3. List
        4. Content

        Answer:

        B. Select File Explorer, then the View tab and the Layout group. Here the Details will show the filename, file size, date last modified or created, and other data. The Extra large icons shows each file as a picture. The List option will show a list of the filenames and folders with no other details, and the Content option shows the file's metadata.
216.    Which of the following is not a best practice for updating/patching Red Hat Linux?

        1. Keep installed software updates current.
        2. Verify that installed packages have a valid signature.
        3. Update packages quarterly.
        4. Download packages only from trusted sources.

        Answer:

        C. Updating packages only quarterly would be disastrous to the security of your systems. It's important to plan for updates and follow the plan. If your system has many Linux installations, test package updates in a sandbox before installing on all systems. Managing patches can be time-consuming, which is why companies providing patch management services exist for both Linux and Windows installations. Checking for patches can be scripted using the `yum` command. Updates should only be downloaded from reliable sources, and if using Red Hat Linux, verify that the packages are signed by Red Hat.
217.    What Linux program includes security features that can be used to find, list, and install security updates?

        1. `chmod`
        2. `man`
        3. `find`
        4. `yum`

        Answer:

        D. The `yum` command can be used to install security updates. The command to check for security updates can be used in scripts, making it easy to run automatically and daily. The command is `yum check-update --security`. If there are none, the command returns a value of 0. The command `yum update --security` can be used to install security updates. The `chmod` (change mode) command is used to modify the mode of the file, meaning who has what access to the file; the `man` command displays a user manual for any Linux command, much like Microsoft Windows `[`_`command`_`] /?` command; and the `find` command is used to find files and directories and to perform operations on them.
218.    You're using the Mail utility of Control Panel to configure a new user's computer so that their Microsoft Outlook mail will automatically be downloaded onto their Windows computer. What pieces of information will you need to set up their profile? (Choose two.)

        1. The protocol the server uses
        2. The user's email address
        3. The user's password
        4. The server port number

        Answer:

        B, C. To enable a user to retrieve their email from Microsoft Outlook using the Mail utility in Control Panel, you would only need the user's email address and password. If the server is other than a Microsoft Outlook server, then you might need more information such as the protocol the server uses and the server address. You don't need to know the port number.
219.    You have a MacBook Pro and want to share files with a small group of Mac users. Because your team edits the files frequently, you want to make sure everyone has access to the same version of the files online. What storage solution should you use?

        1. iCloud
        2. Finder
        3. Remote Disc
        4. Spotlight

        Answer:

        A. One of the best ways always to have the latest version of files, regardless of the device that you are using to access them, is to have them stored and accessed in the cloud. iCloud is Apple's answer to remote storage, and you can configure your Apple devices to place files there automatically or use it for backup. Finder enables a user to drill down through folders to find what they are looking for. Remote Disc is for using a shared optical drive, and Spotlight is used to search for objects in macOS. It uses the familiar spyglass icon.
220.    Which of the following is not a best practice for backing up Linux (or any) desktop systems?

        1. Follow the 3-2-1 rule.
        2. Make only monthly backups.
        3. Carefully document backups.
        4. Periodically verify that backups are not corrupted and can be restored.

        Answer:

        B. Making only monthly backups would likely not be often enough for anyone. In a business setting it's important to have a backup plan, taking into consideration how much data you're willing to lose and how long it would take to restore data if restoring from a backup were needed. The 3-2-1 rule states that you need to have three backups on two different media, and one needs to be off-site. It's also important to consider having backups that are separate from your main system so that an infection of the main system won't infect the backup. Your backup plan should include regularly verifying that the backups are able to be restored, meaning that the backups complete properly and are not corrupted, and that your restore plan works. Even emergency medical services have practice runs from time to time to ensure that when a major event happens, they will be ready. You should, too. Finally, document, document, document. If an event occurs, you need to ensure that you're restoring from the correct backups, and if the person in charge of backups is not available for any reason, a thoroughly documented backup system will make it easier for someone else to continue the process in their place and/or restore backups if needed.
221.    You're working at a Windows command prompt and need to prepare a volume on a hard drive to receive data using the NTFS filesystem. The volume should be designated as drive X. Which command would you use at a command prompt to do this?

        1. `format x: /fs:ntfs`
        2. `initialize x: /fs:ntfs`
        3. `format x: /ntfs`
        4. `initialize x: /ntfs`

        Answer:

        A. The `format` command is used to format hard drives. Before you format any drive, be sure that you have it backed up or are prepared to lose whatever is on it. The `/fs:[`_`filesystem`_`]` switch specifies the filesystem to prepare the disk with. `initialize` is not a command.
222.    You're running a computer with macOS. Which of the following will protect your data against accidental deletion?

        1. Mirrored drives
        2. An online utility
        3. Time Machine
        4. Nothing

        Answer:

        C. Time Machine is a part of macOS, and it makes backups hourly daily and weekly that can be used to restore a single file from months ago if it was accidentally deleted. Mirrored drives provide redundancy if the hard drive fails, but not against human error. Online utilities are often set up to do the same. Backups should be a priority if retaining the data is important. The only drawback with Time Machine is that if the external drive being used by Time Machine gets full, it will start deleting the first backups to make room for new ones.
223.    You are a junior IT administrator, and the senior IT administrator has just set up a proxy server, so you need to add settings for it to every workstation. What information do you need to properly set up the proxy server in the Network & Internet group of Windows Settings? (Choose two.)

        1. The proxy server's IP address
        2. The router's IP address
        3. The DHCP server's IP address
        4. The port number to use for the proxy server

        Answer:

        A, D. To set up a proxy server in Windows Settings, you only need the server's IP address and port number to use. You likely should also check the box that says “Don't use the proxy server for local (intranet) addresses.” You would not need the router's IP address or the DHCP server's IP address unless it is also functioning as the proxy server. A router decides if a packet belongs on the LAN or another network, and a DHCP server's job is to provide IP addresses and other settings to devices that log into a network.
224.    You are working on a MacBook Pro and need to search the computer for a document you wrote a few months ago. Which feature should you use to search the hard drive?

        1. Keychain
        2. Spotlight
        3. Finder
        4. Siri

        Answer:

        B. The search feature in macOS is Spotlight, and a magnifying glass icon in the upper-right corner of the menu bar represents it (or you can press Command+spacebar from any app). Spotlight can search for documents, images, apps, and so on. Keychain is Apple's password management system. Finder enables a user to drill down through folders to find what they are looking for. Siri is Apple's voice-activated virtual assistant.
225.    Which of the following is not a best practice for avoiding viruses/malware in a Linux system?

        1. Create a different user and disable the root user.
        2. Install antivirus and update it regularly.
        3. Use sudo instead of su.
        4. Only use eight-character alphanumeric passwords.

        Answer:

        D. Eight-character alphanumeric passwords are simply too easy to hack. Whether a Windows or Linux system, more complex passwords should always be required. There are other ways to keep malware and viruses out. Linux has a few advantages on that front. First and foremost, there are many, many people looking at Linux code, which means many people to catch and rectify a vulnerability that could be taken advantage of by viruses and hackers. In Linux, the user and system are more compartmentalized. If malware attacks a user, it will only have access to what that user account has access to, not system files and folders. This means if you must run commands as root, it's extremely important to, whenever possible, do so using `sudo` instead of `su`. `sudo` will run just that command as root, but `su` opens up an entire new shell as root and greater vulnerability to attack. If you're logged in as `root`, the whole system is vulnerable. Also, hackers know that `root` is the default name for the system administrator, so create another user and disable `root` so that a hacker has to guess not only the password but the username as well. It's always good advice to install an antivirus program and update it regularly. Other security actions for Linux are to configure a firewall to filter traffic on unused ports, keep the Linux packages and kernel updated, remove any software that is no longer being used, and change the `/boot` directory to read only so that it can't be changed. In addition to requiring complex passwords, force users to change them periodically and not reuse passwords. You'll also want to monitor for failed login attempts and lock accounts after a reasonable number of failed logins. Email can be encrypted, and of course, train users on the dangers of opening email from unfamiliar sources.
226.    You are installing a new network for a small office. They are concerned about security and therefore want it managed by one computer. When installing the Windows computers, what type of network setup will you choose?

        1. Workgroup
        2. Homegroup
        3. Personal area network
        4. Domain

        Answer:

        D. A domain is a group of computers that are tightly connected or associated and share a common domain name. It has a single authority (called a domain controller) that manages security and access to resources for all the computers. All users will log in to the Windows domain using their centrally created user account. If no domain is used, then by default Windows computers will join a workgroup called workgroup, making it easy to share files, printers, and other resources. Access to resources is configured on each workstation that is sharing a resource. The drawbacks of a workgroup are that security is configured on each PC and it's only appropriate for very small networks. Homegroup was a networking scheme in prior versions of Windows that shared libraries. A personal area network (PAN) consists of a PC and its wireless devices, usually paired Bluetooth devices such as printers, headphones, and input devices. A domain is a network where access to resources is configured on a central server that all users of the resources must log in to.
227.    You are viewing the screen shown in the graphic. Which of the following is not true about the network connection from this screen?

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713084894.e6f6e038ed4648f14e86ea4941451aabb2eb879f/eod/books/159469/images/c06uf017_0.jpg?width=821" alt=""><figcaption></figcaption></figure>

        1. It is a public network.
        2. File And Printer Sharing is likely enabled.
        3. It is likely a network you or your company controls.
        4. Network Discovery is likely enabled.

        Answer:

        A. In the View Your Active Networks pane, you can see that this network profile is set to Private Network. A private network is one that is trusted, like where you work, or that you control, like your home network. By default, this computer will be discoverable on the network and File And Printer Sharing is enabled. To change these settings, click Change Advanced Sharing Settings. The other two types of network profiles are public and domain. To change the network type, go to Settings, choose Network & Internet, then select Status. Click Properties of the network connection that you want to change and choose the profile type. The domain profile type is detected automatically when the local computer logs in to an Active Directory domain.
228.    A user has shared a folder with you. Working in File Explorer, how can you configure access to this shared network location each time you log in without reentering the path? (Choose two.)

        1. Left-click This PC and choose the network share.
        2. Select This PC on the left then click Map Network Drive icon in the File Explorer ribbon and follow the onscreen prompts, ensuring that you choose Reconnect at sign-in.
        3. Use File Explorer to drill down to the shared network resource. Right-click the shared resource, then choose Map Network Drive and follow the onscreen prompts, ensuring that you choose Reconnect at sign-in.
        4. Click Quick Access and choose the network share.

        Answer:

        B, C. Mapping a network drive to a share makes it easy to access that share every time you log into your computer, provided you're on the same network. Left-clicking on This PC will show the mapped drive in the right pane, after it has been set up as a mapped drive, so that you can easily choose it from there. The network share will appear on Quick Access after you've used it.
229.    You're on your private wired network at home and notice that your mouse is moving across the screen but you aren't moving it. Also, your computer seems to be running slowly, so you suspect someone with malicious intent has hacked into it. You want to immediately block access through the local machine's firewall. Where can you quickly do this?

        1. Search for Firewall. Choose Firewall & Network Protection, click Private, then click Block All Incoming Connections, including those in the list of allowed apps.
        2. Start typing Windows in the search box, choose Windows Defender Firewall, then click Private Networks and Disable.
        3. Search for **air**, click Turn Airplane mode on or off, then turn Airplane mode on.
        4. Search for Windows Defender Firewall and choose it, then turn the firewall off.

        Answer:

        A. Choosing to block all incoming connections, including those in the list of allowed apps, would certainly stop all incoming connections quickly. There is no Disable option under Private Networks in the Windows Defender Firewall window. Turning Airplane mode on would stop the computer from communicating on wireless networks, but it wouldn't stop communication on a wired network, and turning off the firewall is the opposite of what you would want to do.
230.    You have a Windows Pro computer set up in a workgroup, and you need to perform some routine management tasks on it. Before you do, you want to see what shares already exist on the local computer. What utility can you use to do this?

        1. In Windows Settings, choose Network & Internet.
        2. In Windows Settings, choose Ease Of Access.
        3. In Computer Management, choose Shared Folders, then double-click Shares.
        4. In the Network And Sharing Center utility of Control Panel, click Change Advanced Sharing.

        Answer:

        C. Choosing Computer Management, then Shared Folders, and Shares will show all of the resources that are shared on the local computer. Some are created by default. Hidden shares will have a $ at the end of the name and can only be accessed if you know the share name. Network & Internet deals with configuring network connections, not network shares. Ease Of Access enables alternate configurations that work better for differently abled people. Network And Sharing Center is used to configure networks, and it has settings to turn sharing on and off but no way to show all the current network shares.
231.    Your laptop is equipped with a WWAN card, and you've arranged for service with a cellular provider. Where in Windows 10 can you connect to the network? (Choose two.)

        1. Click the wireless network icon on the taskbar and choose the network with the cellular network icon (vertical bars) in the list.
        2. In the Network & Internet group of Windows Settings, click Mobile Hotspot.
        3. In the Network & Internet group of Windows Settings, click Wi-Fi.
        4. In the Network & Internet group of Windows Settings, click Cellular.

        Answer:

        A, D. The simplest way to connect to your WWAN, once it has been set up, is to choose it from the available wireless networks shown when clicking the wireless network icon on the taskbar. Or, go to Windows Settings, choose Network & Internet, then Cellular to choose your network. A mobile hotspot is when you share the Internet connection on your device with other devices that are near you. Choosing Wi-Fi in the Network & Internet group of Windows Settings will not show you the WWAN connection.
232.    You want to block an application from communicating through your Windows Defender Firewall. What will you set up for this application?

        1. An exception
        2. A restriction
        3. A mapped drive
        4. A network share

        Answer:

        B. A network restriction means that you will not allow an application to communicate through a firewall, whereas an exception means that you will allow that application to communicate through the firewall. To configure a restriction in Windows Defender Firewall, open it from Control Panel and click Advanced Settings, then click Outbound Rules, then New Rule. Ensure that Program is selected and click Next. Click Browse to locate the program file, click to select it, then click Open. The program path should appear in the New Outbound Rule Wizard dialog box. Click Next, then choose Block The Connection. Click Next twice, then give your rule a name and click Finish. A mapped network drive means that you have assigned a drive letter on a local computer to a folder that is shared on a remote computer. A network share would take place on a computer with folders that you want to allow others on your network to have access to.
233.    You need to connect to the Internet, but you regularly are working in remote areas, and your only option is to use a cellular network. What type of network are you establishing when you connect to the Internet?

        1. PAN
        2. CAN
        3. WWAN
        4. LAN

        Answer:

        C. When you use a cellular network to connect to the Internet, you are using a WWAN. Most of us are familiar with the local area network (LAN) in our home or office and the personal area network (PAN) that we use to connect devices such as wireless keyboards, mice, and headsets to our computer. A campus area network (CAN) could exist on a property that is owned by a single entity but housed in discrete buildings. The network might even cross government-owned streets. You may be less familiar with a wireless wide area network (WWAN), which are used more and more frequently. Unlike wireless LANs that use radio, microwave, or infrared signals, WWANs take advantage of the cellular network. You can purchase a WWAN device, often called a mobile hotspot, from a cellular service provider. They generally require a contract, but some don't. The great advantage of a WWAN is that they will work almost anywhere—the cellular network is virtually worldwide. The biggest disadvantage is likely the cost.
234.    You're working on your laptop at a friend's house and click your browser to research something, but a window pops up saying No Internet. How do you resolve this? (Choose two.)

        1. Right-click the browser shortcut and choose New Window.
        2. Start typing **network** in the search box, then choose Network Status, then Show Available Networks, and get the network name and password from your friend.
        3. Click the taskbar icon that looks like a globe, then choose your friend's network and ask for the password.
        4. Type **firewall** in the search box and choose Firewall & Network Protection, then click Private Network.

        Answer:

        B, C. The fastest way to join your friend's network is to click the globe icon (or Wi-Fi icon) and choose the network, but going through Network Status, then Show Available Networks also works. Right-clicking a browser shortcut will show websites that you've recently been to and a few other options. Firewall & Network Protection ➢ Private Network will enable you to configure firewall settings for use with a private network.
235.    You need to allow Open Office to communicate through the local Windows computer's firewall. Where is this configured? (Choose two.)

        1. In the Search box, type **Firewall & Network Protection**, then choose it from the results and click Allow An App Through Firewall.
        2. In Windows Settings, choose the Apps group.
        3. In Control Panel, choose Windows Defender Firewall, then select Allow An App Or Feature Through Windows Defender Firewall.
        4. In Control Panel, open the Programs And Features utility.

        Answer:

        A, C. You can drill down through Windows Settings to find Firewall & Network Protection Settings, but it's far easier to search for it, then choose Allow An App Through Firewall. Once there, if the app is in the list, click the Change Settings button, then select the box next to the application you want to allow access for under the listing for Private or Public network, depending on your needs. If it isn't in the list, click Allow Another App. Drilling down through Control Panel, choose Windows Defender Firewall, then An App Or Feature Through Windows Defender Firewall will take you to the same setup screen. The other two options will enable you to uninstall applications.
236.    A user has a laptop that they think has WWAN capabilities. Where can you quickly check?

        1. Disk Management
        2. Device Manager
        3. Apps & Features
        4. Programs And Features

        Answer:

        B. Opening Device Manager and clicking Network Adapters should show you what you have for network devices. Most likely you'll see a Bluetooth Device (Personal Area Network), possibly an Ethernet Local Area Network (LAN) adapter, a wireless area network (WAN) adapter and, if you have one, a wireless wide area network (WWAN) adapter. If it doesn't show there, either it isn't being detected by the system or one does not exist in your system. Disk Management is for configuring and managing drives. Apps & Features and Programs And Features both have the same job: providing a way to install or repair applications and add or remove Windows features. The former is in Settings and the, latter is in Control Panel.
237.    A user wants to use a WWAN connection to the Internet because they travel and Ethernet and Wi-Fi networks aren't always available to connect to. What will this user need? (Choose two.)

        1. A Wireless NIC
        2. A WWAN card or device
        3. A cellular service provider
        4. An RJ-45 connector

        Answer:

        B, C. Wireless wide area networks use the cellular system to connect to the Internet. To make a connection you would need either a WWAN card in your laptop or a WWAN device, which is sometimes called a mobile hotspot device, and a cellular service connection. Some cellular companies require a contract for this type of cellular service, but not all do. The WWAN card or WWAN device need to be compatible with your cellular provider. Wireless NICs are used for Wi-Fi connections, and an RJ-45 connector is used for wired Ethernet connections.
238.    A user at your company just signed up for WWAN service through their cellular provider. Their data is capped at 10 GB per month. It's very costly if they go over, so they've asked you if there is a way for them to avoid going over their data limit. What will you do for them?

        1. Set up their cellular WWAN as a metered service.
        2. Use Performance Monitor to track their WWAN use.
        3. Switch them to a VPN so it won't cost anything.
        4. Use a proxy server so their data downloads won't count.

        Answer:

        A. Metered network settings can be configured for wired, Wi-Fi, or a wireless wide area network (WWAN) connection. For example, to configure a Wi-Fi network as a metered connection, go to Settings, then choose the Network & Internet group, then click Wi-Fi, then Manage Known Networks, and select the network. In Windows 10, you need to click Properties, but in Windows 11 you're already on the Properties screen. Locate the metered connection setting and turn it on. You can then set a data limit to control data usage. Performance Monitor won't show data usage. A WWAN can connect to a virtual private network (VPN), but it will still use data. Your connection might go through a proxy server when connecting to a network, but a proxy server's job is to filter network traffic. Any time you're connecting to the Internet or a VPN via your WWAN connection, you'll be using data.
239.    A junior network administrator wants to know the fastest way to access File Explorer, because they use it often. What do you tell them?

        1. Press Windows Key+F.
        2. Press Windows Key+M.
        3. Press Windows Key+E.
        4. Press Windows Key+X, then choose File Explorer from the menu.

        Answer:

        C. Pressing Windows Key+E will open the File Explorer window. Pressing Windows Key+X and then selecting File Explorer from the menu will also work, but it's not the fastest, most direct way. Windows Key+F will bring up a feedback window, and Windows Key+M will minimize all the open windows, leaving you at the desktop.
240.    You need to establish a wired connection between a newly installed Windows Pro computer and an Ethernet home network. The router is next to the desk and provides DHCP services. What will you need to connect a desktop computer to this network? (Choose two.)

        1. Patch cable
        2. Wireless NIC
        3. NIC with RJ-45 port
        4. IP address and subnet mask

        Answer:

        A, C. For a new Windows installation, the default network setting is to configure IP addresses dynamically, so the computer should get its IP address and subnet mask from the DHCP server. All you need is a patch cable to connect to the router and a compatible NIC installed (with its drivers, of course) with an RJ-45 port. You would not use a wireless NIC for an Ethernet network; a wireless NIC is for a Wi-Fi network. You don't need to know the IP address and subnet mask because the DHCP server will assign them automatically.
241.    You need to know the path to a network resource. How can you locate it?

        1. Type **mynetworkdrives** in a browser window to see them.
        2. In File Explorer, right-click the resource, choose Properties, then click the Sharing tab.
        3. In File Explorer, select This PC, Network Drives, and their path will show under Network Locations.
        4. Select Computer Management ➢ Shared Folders ➢ Shares.

        Answer:

        B. There are multiple ways to view the path to a resource. In File Explorer you can right-click the resource and then choose Properties and select the Sharing tab. The screen will say Network Path and list the path just below it. Typing **mynetworkdrives** in a browser doesn't help at all, and Shares in Computer Management shows what you are sharing, not what is being shared with you.
242.    You're installing Windows 10 64-bit on the only drive in a computer that uses BIOS, not UEFI. You'll be booting from this drive. Which of the following are true? (Choose two.)

        1. The partition scheme must be MBR.
        2. The partition scheme must be GPT.
        3. The partition must be less than 2 TB.
        4. You won't be able to boot from this drive.

        Answer:

        A, C. When a motherboard uses BIOS rather than UEFI to manage firmware, it must use the MBR partition type or the drive will not be bootable. A GPT partition will be able to be read but not booted to. The partition size limit for MBR is 2 TB.
243.    You've installed a new hard drive in a Windows PC and need to partition the drive and format the volumes. What tools can you use to format it? (Choose two.)

        1. `diskmgmt.msc`
        2. `diskpart`
        3. `perfmon.msc`
        4. `services.msc`

        Answer:

        A, B. Once a hard drive is installed, partitions must be created (even if there is only one) and the volumes must then be formatted before they will show in File Explorer and be ready for the user to store information on them. Disk Management (`diskmgmt.msc`) and `diskpart` are two excellent and powerful tools for doing just that. Disk Management is a utility that has a user-friendly GUI, whereas `diskpart` is run from the command line. `diskpart` is the more powerful of the two, and it's worth spending some time exploring. Performance Monitor (`perfmon.msc`) shows resource usage in real time, and the Services console (`services.msc`) shows all of the services available in the system and their current status.
