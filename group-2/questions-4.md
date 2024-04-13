# Questions

1.  Which of the following troubleshooting steps involves prioritizing trouble tickets based on the severity of the problem?

    1. Identify symptoms of the problem
    2. Establish a theory of probable cause
    3. Test the theory to determine cause
    4. Establish a plan of action to resolve the problem and identify potential effects
    5. Implement the solution or escalate as necessary
    6. Verify full system functionality and, if applicable, implement preventive measures
    7. Document findings, actions, and outcomes

    Answer:

    A. The first step in troubleshooting is to identify the problem by establishing symptoms related to the network issue being reported. In this step, problems are typically reported as trouble tickets, which are prioritized based on the severity of the problem. You complete the other steps after the trouble ticket has been prioritized and is being investigated.
2.  Which of the following is considered a systemwide error?

    1. A problem with an order entry or customer service call center resource
    2. A problem with a router that affects only one Local Area Network (LAN)
    3. A fatal error that causes a single computer to fail
    4. A problem with an email server that affects all network users

    Answer:

    C. A systemwide error is a problem that renders an individual user's system (computer) completely unusable. All the other problems listed would affect more than one system or user.
3.  Which of the following is a networkwide problem?

    1. A problem with an order entry or customer service call center resource
    2. A fatal error that causes a single computer to fail
    3. A problem with an application server that affects a single Local Area Network (LAN)
    4. A problem with a router that connects an entire network to the Internet

    Answer:

    D. Any problem that affects all the users on the network is a networkwide problem and should be given the highest priority. An example of this would be a problem with an Internet router. All other problems listed do not affect the entire network.
4.  A user reports that she cannot connect to a server on her network. Ed wants to identify the scope of the problem, so he tries to reproduce the problem on the user's computer. The problem still remains. No other users are reporting this problem. What is the next logical step that Ed should perform to identify the affected area?

    1. Verify that the local router is forwarding traffic.
    2. Try performing the same task on another computer attached to the same segment.
    3. Verify that the server is configured properly.
    4. Verify that the switch the client is connected to is functioning.

    Answer:

    B. In this scenario, only one user is reporting a problem. Therefore, the likeliest next step is to perform the same task on another computer attached to the same segment. If Ed can perform the task successfully, the problem most likely lies within the user's computer or the connection to the switch. Since no other users are reporting the same problem, the server and switches on the network are probably up and functioning. Checking the router is not necessary since the user and server are on the same network.
5.  Which of the following troubleshooting steps involves asking the user preliminary questions such as, “What were you doing when the problem occurred?”

    1. Identify the problem
    2. Establish a theory of probable cause
    3. Test the theory to determine cause
    4. Establish a plan of action to resolve the problem and identify potential effects
    5. Implement the solution or escalate as necessary
    6. Verify full system functionality and, if applicable, implement preventative measures
    7. Document findings, actions, and outcomes

    Answer:

    A. The first step in troubleshooting is to identify the problem by establishing symptoms related to the network problem being reported. In this step, you ask the user many questions to identify and define the symptoms of the problem and prioritize the trouble ticket. Although you might continue to ask the user questions throughout the troubleshooting process, this is typically associated with the first step of the troubleshooting process.
6.  When troubleshooting, you begin by taking steps to identify the problem. After you do this, which of the following steps should you perform next?

    1. Implement the solution
    2. Establish a plan of action
    3. Establish a theory of probable cause
    4. Verify full system functionality

    Answer:

    C. After identifying the problem, the next step is to establish a theory for the probable cause of the problem. After that, you can test your theory, establish a plan of action, implement a solution, verify the functionality of the system, and document the entire process.
7.  In which troubleshooting step do you try to duplicate a network problem to logically and methodically eliminate elements that are not the source of the problem?

    1. Identify the problem.
    2. Establish a theory of probable cause.
    3. Test the theory to determine cause.
    4. Establish a plan of action to resolve the problem and identify potential effects.
    5. Implement the solution or escalate as necessary.
    6. Verify full system functionality and, if applicable, implement preventative measures.
    7. Document findings, actions, and outcomes.

    Answer:

    B. The second step in troubleshooting is to attempt to duplicate a problem and develop a theory of its probable cause. As you troubleshoot a problem, you then test your theory to confirm your findings. You complete the other troubleshooting steps after the specific cause has been identified.
8.  Ralph is a first-tier technician working the help desk. After identifying a network problem submitted by multiple users, Ralph comes up with a theory specifying a possible source of the problem and sets about testing his theory. Unfortunately, testing indicates that Ralph's theory is wrong; the source he suspected is not the cause of the problem. Which of the following should not be the next step in Ralph's troubleshooting process?

    1. Reinterview the users to gather more information about the problem
    2. Escalate the problem to a second-tier technician
    3. Repeat the process of establishing a theory of probable cause
    4. Begin replacing components that might contribute to the problem

    Answer:

    D. Replacing components by guesswork could resolve the problem through chance, but it would more likely be a waste of time and hardware. When Ralph's first theory is disproven, the next logical step would be to devise another theory. This could conceivably involve reinterviewing the users or escalating the issue to a senior technician. If the theory had been confirmed, the next step would be to devise a plan of action to resolve the problem.
9.  Ralph is a first-tier technician working the help desk. A user calls in, saying that when she turned her computer on that morning, nothing appeared on the screen. Which of the following should be Ralph's first question to the user?

    1. What is your computer's IP address?
    2. Have you applied the latest system updates?
    3. Are the computer and monitor plugged in to AC power?
    4. Has anyone else been using your computer?

    Answer:

    C. In troubleshooting, one of the first steps in the process of identifying the problem is to question the obvious, such as whether the computer is plugged in or switched on. It would be unlikely that the user would know her computer's IP address or what updates had been installed when the screen is blank. Questioning whether other people have used the computer might come up later, but it will be little help at this stage of the troubleshooting process.
10. You have a problem with a server or other network component that prevents many users from working. What type of problem is this?

    1. A networkwide problem
    2. A shared resource problem
    3. A systemwide problem
    4. A user application problem

    Answer:

    B. If a problem lies within a specific server or other network component that prevents many users from working, it is a shared resource problem. A problem that lies within resources that provide services to the entire network is a networkwide problem. Systemwide problems put a specific computer out of commission, preventing a user from getting any work done. An application problem is a problem that affects only a single user's access to a device or application.
11. A single Windows user suddenly cannot connect to any hosts on the network (local or remote). Alice interviews the user and finds out that he made some changes to his computer's Internet Protocol (IP) configuration properties. What should she do next?

    1. Run the `ipconfig` command to view the local configuration
    2. Check the Domain Name System (DNS) server to see if it is resolving IP hostnames
    3. Check the Windows Internet Name Service (WINS) server to see if it is resolving Network Basic Input/Output System (NetBIOS) names
    4. Verify that the router is functioning

    Answer:

    A. Since only one user is reporting the problem, and he had admitted to making changes to his IP configuration, Alice should probably start by checking the configuration using the `ipconfig` command. If the router, DNS server, or WINS server were causing the problem, more than one user would be experiencing difficulties.
12. Alice has a network with a Domain Name System (DNS) server, a proxy server, and an Internet router. A user is complaining that she suddenly cannot connect to hosts on her own Local Area Network (LAN) and other internal LANs, and she cannot access hosts on the Internet. What is the likeliest problem?

    1. The user's local configuration
    2. The proxy server
    3. The DNS server
    4. The router

    Answer:

    A. Since only one user is reporting the problem, the user's computer and its configuration are the likeliest suspect components. A DNS, proxy, or router problem would affect more than one user.
13. Alice takes a call from a user who is unable to send email to a colleague in one of the company's branch offices. Alice begins by having the user try to send emails to different people at the branch office, to people in the local office, and to people on the Internet. She then checks the user's Internet Protocol (IP) configuration settings, the computer's Local Area Network (LAN) communication, and the cable connection to the network. Which of the following approaches is Alice using to troubleshoot the problem?

    1. OSI bottom-to-top
    2. Divide and conquer
    3. OSI top-to-bottom
    4. Question the obvious

    Answer:

    C. Alice is using a top-to-bottom approach, based on the Open Systems Interconnection (OSI) reference model. She begins at the top of the model (the application layer) by checking the system's email capabilities, and then proceeds downwards to check the computer's IP configuration (at the network layer), the local network connectivity (the data link layer), and the computer's cables (the physical layer). A bottom-to-top approach would begin with the cables. The divide-and-conquer approach and questioning the obvious would not involve the steps Alice took in the order that she took them.
14. Alice is working the help desk when a user calls and reports that she is unable to connect to the Internet. Which of the following steps is the one Alice is least likely to perform first when troubleshooting the problem?

    1. Check the configuration of the router connecting the LAN to the Internet
    2. Ask the user if she can access resources on the local network
    3. Check to see if anyone else is experiencing the same problem
    4. Check the user's job title to see if she is an important person in the company

    Answer:

    A. There are many possible causes for the problem that are more likely than a router configuration error, so this is not something Alice would check first. Asking if the user can access the local network attempts to isolate the problem. If she cannot, the problem could be in her computer; if she can, then the problem lies somewhere in the Internet access infrastructure. If other users are experiencing the problem, then the issue should receive a higher priority, and Alice knows that the problem does not lie in the user's computer. While it might not be the first thing she checks, it is a political reality that higher ranking users often get preferential treatment.
15. In the standard troubleshooting methodology, which of the following steps appears last, but must actually be practiced throughout the troubleshooting process?

    1. Test the theory to determine cause
    2. Document findings, actions, and outcomes
    3. Verify full system functionality and, if applicable, implement preventive measures
    4. Implement the solution or escalate as necessary
    5. Establish a plan of action to resolve the problem and identify potential effects
    6. Establish a theory of probable cause
    7. Identify the problem

    Answer:

    B. Documenting everything you discover and everything you do is a crucial part of the troubleshooting method that must begin before you take any other action whatsoever. However, it appears as the last step in the troubleshooting methodology.
16. In which troubleshooting step is a trouble ticket created?

    1. Establish a theory of probable cause
    2. Verify full system functionality and, if applicable, implement preventive measures
    3. Implement the solution or escalate as necessary
    4. Test the theory to determine cause
    5. Identify the problem
    6. Document findings, actions, and outcomes
    7. Establish a plan of action to resolve the problem and identify potential effects

    Answer:

    E. The first step in troubleshooting involves identifying the problem and creating a trouble ticket. You complete the other troubleshooting steps after the trouble ticket has been prioritized.
17. Which step of the troubleshooting model involves identifying whether hardware or software has been recently installed or reconfigured?

    1. Identify symptoms
    2. Establish a theory of probable cause
    3. Establish a plan of action to resolve the problem and identify potential effects
    4. Determine if anything has changed.
    5. Test the theory to determine cause
    6. Document findings, actions, and outcomes

    Answer:

    D. During the troubleshooting process, you must establish whether anything has changed. This typically involves asking the user whether any new or existing hardware or software has been installed or reconfigured.
18. Which step of the troubleshooting model involves replacing components until a faulty hardware device is identified?

    1. Duplicate the problem
    2. Gather information
    3. Test the theory to determine the cause
    4. Establish a plan of action to resolve the problem
    5. Verify full system functionality
    6. Document findings, actions, and outcomes

    Answer:

    C. After you have established a theory of probable cause, you can try to test the theory by replacing hardware components one by one until you find the faulty device.
19. Which of the following are not general troubleshooting steps? (Choose all that apply.)

    1. Identify the problem
    2. Establish a theory of probable cause
    3. Test the theory to determine cause
    4. Verify that the client's Internet Protocol (IP) configuration is correct
    5. Establish a plan of action to resolve the problem and identify potential effects
    6. Verify that the router is forwarding.
    7. Implement the solution or escalate as necessary
    8. Verify full system functionality and, if applicable, implement preventive measures
    9. Document findings, actions, and outcomes

    Answer:

    D, F. Verifying that a router is functioning and forwarding traffic and verifying that a client's IP configuration is correct are not considered general troubleshooting steps. You might perform these two steps as a subset of general troubleshooting steps.
20. Which of the following are reasons for documenting a network problem or incident? (Choose all that apply.)

    1. Documentation makes it easier to escalate calls to senior technicians.
    2. Documentation makes it easier to prioritize administrative tasks.
    3. Documentation makes it easier to prioritize each help call.
    4. Documentation makes it easier to escalate calls to first-tier technicians.

    Answer:

    A, C. When a network problem or incident is reported, documentation begins. Proper documentation makes it easier for a first-tier support technician to prioritize and to escalate the call to senior technicians, if necessary.
21. Which of the following statements about prioritizing help calls are true? (Choose all that apply.)

    1. Individual desktop problems take precedence over problems with shared resources.
    2. Problems with shared resources take precedence over individual desktop problems.
    3. Departmental problems take precedence over networkwide problems.
    4. Networkwide problems take precedence over departmental problems.

    Answer:

    B, D. When establishing priorities, networkwide problems take precedence over departmental problems, and problems with shared resources take precedence over individual desktop problems.
22. Which of the following statements about multitiered technical support organizations are true? (Choose all that apply.)

    1. Help calls are always escalated to second-tier technicians when they involve mission-critical network components such as routers.
    2. First-tier technicians generally handle desktop problems.
    3. Second-tier technicians are generally less experienced than first-tier technicians.
    4. First-tier technicians are generally less experienced than second-tier technicians.

    Answer:

    A, B, D. First-tier technicians are generally less experienced than second-tier technicians. First-tier technicians are the first point of contact for users. They receive and prioritize help desk calls and escalate problems to second-tier technicians, if necessary. First-tier technicians generally handle individual desktop problems, whereas second-tier technicians troubleshoot mission-critical network components such as routers and switches.
23. Ed is a first-tier support technician. He receives the help calls listed here. His job is to prioritize them based on their severity. Which of the following should be the problem that receives the highest priority?

    1. A problem with an order entry or customer service call center resource that affects an entire department, with multiple Local Area Networks (LANs)
    2. A fatal error that causes a single computer to fail
    3. A problem with a mission-critical backbone router that affects an entire network
    4. A problem with an application server that affects a single LAN

    Answer:

    C. A problem that affects the entire network should be given highest priority. This includes a mission-critical backbone router. Problems that affect multiple LANs or an entire department are generally given the next highest priority. An application problem that affects a shared application server on a LAN should be given the next highest priority. A problem with a single user's computer should be given the lowest priority if the other problems have been reported.
24. Ed is a first-tier support technician. He receives the help calls listed here. His job is to prioritize them based on their severity. Which of the following should be the problem that receives the lowest priority?

    1. A problem with an order entry or customer service call center resource that affects an entire department, with multiple Local Area Networks (LANs)
    2. A fatal error that causes a single computer to fail
    3. A problem with a mission-critical backbone router that affects an entire network
    4. A problem with an application server that affects a single LAN

    Answer:

    B. A problem that affects the entire network should be given highest priority. This includes a mission-critical backbone router. Problems that affect multiple LANs or an entire department are generally given the next highest priority. An application problem that affects a shared application server on a LAN should be given the next highest priority. A problem with a single user's computer should be given the lowest priority if the other problems have been reported.
25. When you troubleshoot a network problem, it is possible to introduce another problem while attempting to fix the original one. In which step of the troubleshooting process should you be aware of the residual effects that changes might have on the network?

    1. Identify the problem
    2. Establish a theory of probable cause
    3. Test the theory to determine cause
    4. Establish a plan of action to resolve the problem
    5. Implement the solution or escalate as necessary
    6. Verify full system functionality
    7. Document findings, actions, and outcomes

    Answer:

    D. After you identify a problem and establish and test a theory of its probable cause, you must create a plan of action to resolve the problem and identify any potential effects (positive or negative) your solution might have. Then, you implement your solution, test the results, and finish documenting the incident.
26. In which troubleshooting step do you create a record of your activities and inform the user of what happened and why?

    1. Identify the problem
    2. Establish a theory of probable cause
    3. Test the theory to determine cause
    4. Establish a plan of action to resolve the problem and identify potential effects
    5. Implement the solution or escalate as necessary
    6. Verify full system functionality and, if applicable, implement preventive measures
    7. Document findings, actions, and outcomes

    Answer:

    G. The last step of the troubleshooting process is to document the solution and explain to the user what happened and why. In reality, documentation should begin when the problem is reported, and the documentation should be updated throughout the troubleshooting process.
27. On Monday morning, Alice arrives at work to find multiple email and telephone messages from users who are unable to access the Accounting department's file server. Which of the following are the best questions to ask during the beginning stage of the troubleshooting process? (Choose two.)

    1. What has changed since the users were last able to access the server?
    2. Are there any software updates that Alice should apply to the server?
    3. Has the server suffered a hard disk failure?
    4. Which users are reporting a problem, and where are they located?

    Answer:

    A, D. The first stage of the troubleshooting process calls for Alice to identify the problem by gathering information. Learning about who is reporting the problem and what has changed since the server was last accessible can provide Alice with information that could help her determine whether the problem is located in the users' workstations, somewhere in the network, or in the server itself. The other options are intended to test a theory about a probable cause, a troubleshooting stage that comes later.
28. A user calls Alice at the help desk to report that her mouse has stopped working, she cannot access the Internet, and all of her email has disappeared from her inbox. Which of the following would be the best course of action for Alice to take?

    1. Create a separate trouble ticket for each problem
    2. Escalate the call to a senior technician
    3. Have the caller's computer replaced with a new one
    4. Send a technician to the user's site to address all of the problems

    Answer:

    A. Because the multiple problems seem to be unrelated, Alice should handle them individually by creating a separate trouble ticket for each one and prioritizing each one. None of the problems seem to be severe enough to warrant escalation, nor should it be necessary to replace the computer. While it would be possible to send a technician to address all of the problems at once, it would be more efficient to assign each its own priority and handle it like any other trouble call.
29. Alice receives a call in which a user reports that he is unable to send print jobs to the network-attached workgroup printer near his desk. Which of the following tasks should Alice perform first?

    1. Reinstall the printer driver on the user's workstation.
    2. Test network connectivity to the printer using the `ping` utility.
    3. Examine the switches to which the user's workstation and the printer are connected.
    4. Check to see if there are printer firmware upgrades available.

    Answer:

    B. The first phase of the troubleshooting process is gathering information. Learning whether the printer is accessible over the network can help Alice to isolate the location of the problem and develop a theory of probable cause. Installing drivers, checking switches, and upgrading firmware are all part of a later phase in the troubleshooting process: testing a theory to determine the cause of the problem.
30. Which of the following types of Unshielded Twisted Pair (UTP) wiring faults cannot be detected by a wiremap tester?

    1. Split pairs
    2. Open circuits
    3. Short circuits
    4. Transposed wires

    Answer:

    A. A wiremap tester consists of a main unit that connects to all eight wires of a UTP cable at once and a loopback device that you connect to the other end, enabling you to test all of the wires at once. A wiremap tester can detect opens and shorts, as well as transposed wires. However, it cannot detect split pairs because, in that fault, the pins are properly connected.
31. After connecting a tone generator to the green wire at one end of a twisted-pair cable run, Ralph proceeds to the other end of the cable and touches the locator to each of the eight pins in turn. The green wire and the green striped wire both produce a tone. What type of wiring fault has Ralph discovered?

    1. Split pair
    2. Far end crosstalk
    3. Transposed wires
    4. Short circuit
    5. Delay skew

    Answer:

    D. The first and most essential test that installers must perform on every cable run is a continuity test, which ensures that each wire on both ends of the cable is connected to the correct pin and only the correct pin. If a pin on one end of a cable run is connected to two or more pins on the other end, the cable has a short circuit.
32. Which of the following types of cables is used to connect a terminal to the console port of a router or switch?

    1. Rollover
    2. Straight through
    3. Crossover
    4. Plenum
    5. Shielded
    6. Tap

    Answer:

    A. A rollover cable is a type of null modem cable, usually flat and light blue in color, with the pinouts reversed on either end, to enable a terminal to communicate with a router or switch through the device's dedicated console port. None of the other options are suitable for this purpose. A straight through cable is the standard network cable used to connect a computer to a switch. A crossover cable is designed to connect two network adapters directly. A plenum cable is a type of cable intended for use within air spaces and has an outer sheath that does not produce toxic fumes when it burns. A shielded cable is intended to protect signals from electromagnetic interference. A tap is a device used to branch a coaxial cable to two devices.
33. Which of the following types of patch cables is used to connect a computer to a wall plate?

    1. Straight through
    2. Crossover
    3. Rollover
    4. Plenum

    Answer:

    A. A straight through cable is the standard network patch cable used to connect a computer to a wall plate. A crossover cable is designed to connect two network adapters directly. A rollover cable is used to enable a terminal to communicate with a router or switch through the device's console port. A plenum cable is a type of cable intended for use within air spaces that has an outer sheath that does not produce toxic fumes when it burns.
34. What is the name for a device that determines the length of a cable by transmitting a signal at one end and measuring how long it takes for a reflection of the signal to return from the other end?

    1. Fox and hound tester
    2. Wiremap tester
    3. Time-domain reflectometer
    4. Voltage event recorder
    5. Butt set
    6. Spectrum analyzer

    Answer:

    C. The technique that provides this capability is called time-domain reflectometry (TDR). The tester transmits a signal over the cable and measures how long it takes for a reflection of the signal to return from the other end. Using this information and the cable's nominal velocity of propagation (NVP)—a specification supplied by the cable manufacturer—the device can calculate the length of a cable run. The other devices listed do not work in this way.
35. A routine test of a newly installed twisted-pair cable run with a wiremap tester indicates that there is a short circuit on one of the wires. Which of the following procedures might possibly correct the fault?

    1. Use a different pinout on both ends of the cable
    2. Replace the connectors at both ends of the cable run
    3. Move the cable away from any potential sources of electromagnetic interference
    4. Use a higher grade of Unshielded Twisted Pair (UTP) cable

    Answer:

    B. A short circuit is a wiring fault indicating that a pin at one end of a cable run is connected to two pins at the other end. To correct the problem, you must replace the connector with the faulty wiring. None of the other suggestions are solutions for a wiring fault.
36. Ralph is a new hire working on a network that uses Category 5 (Cat 5) Unshielded Twisted Pair (UTP) cable, which was installed several years ago. Over time, some of the paper labels that the original cable installers used to identify the wall plates and patch panel connectors have worn away or fallen off. As a result, Ralph has quite a few cable runs that he is unable to identify. After checking with his supervisor, Ralph discovers that the company has no cable testing equipment and is unwilling to hire a consultant just to identify cable runs. What is the most inexpensive tool Ralph can use to associate unlabeled wall plates with the correct patch panel ports?

    1. A wiremap tester
    2. A cable certifier
    3. A tone generator and locator
    4. A time-domain reflectometer (TDR)

    Answer:

    C. All of the suggested tools are capable of associating wall plates with the correct patch panel ports, but the tone generator and locator is by far the most inexpensive solution.
37. Which of the following devices is an essential tool for technicians working on telephone cables but is not needed for data networking cable installations?

    1. Tone generator and locator
    2. Wiremap tester
    3. Cable certifier
    4. Butt set

    Answer:

    D. Telephone cable technicians have their own specialized tools, such as the butt set, a one-piece telephone handset with alligator clips that enables its operator to connect to a line anywhere that the cables are accessible.
38. Which of the following tools might you use when connecting internal twisted-pair cable runs to the keystone connectors that snap into wall plates? (Choose all that apply.)

    1. A crimper
    2. A punchdown tool
    3. A pigtail splicer
    4. A wire stripper
    5. A fusion splicer

    Answer:

    B, D. The punchdown tool is critical to this operation. In one motion, the tool strips the insulation off of the wire, presses it down into the connector, and cuts off the excess at the end. A wire stripper simplifies the task of preparing the cable for the connection process. A crimper is used only for attaching connectors to patch cables. Pigtail splicers and fusion splicers are used only on fiber-optic networks.
39. Which of the following tools can you use to test the optical loss in a fiber-optic cable?

    1. An OLTS
    2. A TDR
    3. A tone generator and locator
    4. A wiremap tester

    Answer:

    A. An optical loss test set (OLTS) identifies signal loss in fiber-optic cabling. A time-domain reflectometer (TDR) measures electrical signals in copper-based cabling, not light signals. Tone generator and locator tools and wiremap testers are used in copper-based cabling installations, not fiber-optic cabling.
40. Which of the following troubleshooting tools can test cabling for length, attenuation, near-end crosstalk (NEXT), equal level far-end crosstalk (ELFEXT), propagation delay, delay skew, and return loss?

    1. Wiremap tester
    2. Cable certifier
    3. Time-domain reflectometer (TDR)
    4. Optical loss test set (OLTS)
    5. Spectrum analyzer

    Answer:

    B. You can use a cable certifier to identify a variety of cable performance characteristics, typically including cabling lengths, signal attenuation, crosstalk, propagation delay, delay skew, and return loss, in addition to providing all the functionality of a wiremap tester. The other tools listed are dedicated to a single testing modality and do not test for crosstalk.
41. Under which of the following conditions is a cable installer required to use plenum cable?

    1. When cables run close to sources of electromagnetic interference (EMI)
    2. When cables are running through building air flow spaces
    3. When data and voice traffic will be running over the same cable
    4. When cables are running through areas of low temperature

    Answer:

    B. Plenum cable is a type of cable intended for use within building air spaces (called plenums) that has an outer sheath that is more resistant to high temperatures and does not produce toxic fumes when it burns. The use of plenum cable has no effect on EMI or the type of traffic on the cable, nor is it required for low temperature areas.
42. Which of the following troubleshooting tools is not used to test copper cabling installations?

    1. Wiremap tester
    2. Multimeter
    3. Tone generator and locator
    4. OTDR

    Answer:

    D. An Optical Time Domain Reflectometer (OTDR) is a device that transmits light pulses over a fiber-optic network and measures the time interval and strength of the returning pulse, to measure the length of the cable run. An OTDR can be used to locate fiber-optic cable breaks, as well as characterize a cable run's reflectance, optical return loss, and other characteristics. Multimeters, tone generators, and wiremap testers are all devices that work only with copper networks.
43. Which of the following devices is not one of the tools generally used by a data networking cable installer?

    1. Tone generator and locator
    2. Wiremap tester
    3. Butt set
    4. Cable certifier

    Answer:

    C. A butt set is a one-piece telephone handset with alligator clips that enables its operator to connect to a telephone line anywhere that the cables are accessible. They are used by telephone cable technicians, but generally not by installers of network data cables. The other options are all standard tools used by data networking cable installers.
44. Ralph is a new hire for a consulting firm that frequently performs cable installations. He is trying to learn more about the tools needed to install internal cable runs. To that end, which of the following statements about cable crimpers has Ralph found to be true?

    1. Cable installers use a crimper to attach keystone connectors to lengths of bulk cable.
    2. Cable installers use a crimper to attach RJ45 connectors to lengths of bulk cable.
    3. You need to purchase a separate crimper for each type of cable to which you want to attach connectors.
    4. Making your own patch cables by applying connectors yourself is always more economical than buying prefabricated patch cables.

    Answer:

    B. A crimper is a plier-like device that cable installers use to create patch cables by attaching RJ45 connectors to lengths of bulk cable. Installers use a punchdown tool, not a crimper, to attach a cable end to a keystone connector. It is not always necessary to purchase a crimper for each cable type. Some crimpers are designed for a single cable/connector combination, but there are many that have replaceable bits, supporting a variety of cables and connectors. Making patch cables yourself can represent a false economy. Buying bulk cable and connectors and making patch cables yourself can conceivably be cheaper than purchasing prefabricated cables. However, when you factor in the time needed to attach the connectors, the learning curve required to attach the connectors correctly, and the failure rate requiring the re-application of connectors, it might be more economical to purchase prefabricated patch cables in quantity instead.
45. Which of the following statements about cable certifiers are true? (Choose all that apply.)

    1. A cable certifier eliminates the need for tools like tone generators and wiremap testers.
    2. Cable certifiers are the most inexpensive cable testing solution.
    3. Cable certifiers must be reconfigured whenever a new cable specification is standardized.
    4. Cable certifiers can only test copper-based cables.

    Answer:

    A, C. Cable certifiers can detect all of the faults that tone generators and wiremap testers can detect, and they can do a great deal more, such as specify whether a cable run meets the performance specifications defined in a cable standard. When testing a new cable type, the specifications defined in the cable standard must be added to the device. Cable certifiers are far more expensive than most other cable testing solutions. Cable certifiers are available that support various cable media, including copper and fiber optic.
46. Alice is the network administrator of her company's network. The company has just moved into a building that has existing Category 6 (Cat 6) Unshielded Twisted Pair (UTP) cabling. However, none of the cable connections have been labeled, and Alice is trying to identify and document where each cable run starts and ends. Which tools can Alice use for this purpose? (Choose all that apply.)

    1. A packet sniffer
    2. A loopback adapter
    3. A tone generator and locator
    4. A wiremap tester

    Answer:

    C, D. Alice can use a tone generator and locator or a wiremap tester to identify and test cable connections. By connecting the tone generator or the remote wiremap unit to one end of a cable run, she can use the locator or the master wiremap unit to find the other end. This can enable her to identify a starting point and an ending point for a cable run. A loopback adapter is used to test the transmission and reception capabilities of a port. A packet sniffer captures and analyzes network traffic; it cannot identify cables.
47. Which of the following tools can you use to create your own twisted pair patch cables? (Choose all that apply.)

    1. Punchdown tool
    2. Crimper
    3. Pliers
    4. Wire stripper

    Answer:

    B, D. A crimper is a device used for attaching connectors to patch cables. A wire stripper, while not essential to the process, can simplify the task of preparing the cable. A punchdown tool is used for attaching keystone connectors to cable ends, for use in wall plates and patch panels. A standard set of pliers is not used in the process of attaching connectors.
48. Which of the following cable installation tools is likely to be the most expensive?

    1. A crimper
    2. A cable certifier
    3. A punchdown tool
    4. A wiremap tester

    Answer:

    B. Crimpers and punchdown tools are relatively simple and inexpensive mechanical devices that cable installers use to connect bulk cable to connectors. A wiremap tester is an electronic device for cable testing, but it is still relatively simple. A cable certifier is a complex electronic device that can perform a battery of tests on a cable run, confirm that the cable conforms to the required wiring standards, and maintain records of the testing procedure. Cable certifiers are by far the most expensive of the devices listed.
49. What is the function of the tool shown in the following figure?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c05uf001_0.jpg" alt="" height="833" width="597"><figcaption></figcaption></figure>

    1. By placing the tool at one end of a wire, it generates a tone that can be detected at the other end.
    2. To connect a bulk cable to a keystone connector, you use the tool to punch each wire down into the correct receptacle on the connector.
    3. By touching the end of the tool to a copper cable, you can detect and measure the electrical current flowing through it.
    4. By connecting the tool to the end of a fiber-optic cable, you can measure the length of the cable run.

    Answer:

    C. The device shown in the figure is a multimeter, which is used to measure the electric current on a copper conductor, such as an Unshielded Twisted Pair (UTP) network. This tool is not capable of performing any of the tasks described in the other options.
50. What is the function of the tool shown in the following figure?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c05uf002_0.jpg" alt="" height="330" width="833"><figcaption></figcaption></figure>

    1. When you place the tool at one end of a wire, it generates a tone that can be detected at the other end.
    2. To connect a bulk cable to a keystone connector, you use the tool to punch each wire down into the correct receptacle on the connector.
    3. By touching the end of the tool to a copper cable, you can detect and measure the electrical current flowing through it.
    4. By connecting the tool to the end of a fiber-optic cable, you can measure the length of the cable run.

    Answer:

    B. The device shown in the figure is a punchdown tool, used to connect Unshielded Twisted Pair (UTP) cable ends to the keystone connectors used in modular wall plates and patch panels. After lining up the individual wires in the cable with the connector, one uses the tool to press each wire into its slot. The tool also cuts the wire sheath to make an electrical contact and trims the end of the wire. This tool is not capable of performing any of the tasks described in the other options.
51. What is the function of the tool shown in the following figure?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c05uf003_0.jpg" alt="" height="802" width="833"><figcaption></figcaption></figure>

    1. When you place the tool at one end of a wire, it generates a tone that can be detected at the other end.
    2. To connect a bulk cable to a keystone connector, you use the tool to punch each wire down into the correct receptacle on the connector.
    3. By touching the end of the tool to a copper cable, you can detect and measure the electrical current flowing through it.
    4. By connecting the tool to the end of a fiber-optic cable, you can measure the length of the cable run.

    Answer:

    A. The device shown in the figure is a tone generator and locator, used to test Unshielded Twisted Pair (UTP) wiring and detect certain basic wiring faults. This tool is not capable of performing any of the tasks described in the other options.
52. What is the function of the tool shown in the following figure?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c05uf004_0.jpg" alt="" height="668" width="833"><figcaption></figcaption></figure>

    1. When you place the tool at one end of a wire, it generates a tone that can be detected at the other end.
    2. To attach a bulk cable end to an RJ45 connector, you use the tool to squeeze the connector closed, forcing the wire ends to contact the connector's pins.
    3. By touching the end of the tool to a copper cable, you can detect and measure the electrical current flowing through it.
    4. By connecting the clips to pins in a punchdown block, you can access telephone circuits in order to test them or place telephone calls.

    Answer:

    B. The device shown in the figure is a crimper, which is used to create patch cables by attaching connectors to both ends of a relatively short length of bulk cable. This tool is not capable of performing any of the tasks described in the other options.
53. What is the name of the tool shown in the following figure?

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c05uf005_0.jpg" alt="" height="654" width="667"><figcaption></figcaption></figure>

    1. Butt set
    2. Crimper
    3. Tone generator and locator
    4. Punchdown tool

    Answer:

    A. The device shown in the figure is a butt set, a basic tool of telephone installers and line workers. By connecting the clips to pins in a punchdown block, you can access telephone circuits in order to test them or place telephone calls.
54. Ralph has to spend the day completing a twisted-pair cable installation in his office. Contractors have already pulled the cables through the walls and ceilings. Ralph only has to attach connectors to the ends of the cables, both internal cable runs and patch cables. Which of the following tools will Ralph need? (Choose all that apply.)

    1. Telepole
    2. Crimper
    3. Punchdown tool
    4. Pigtail splicer

    Answer:

    B, C. A crimper is a plier-like tool that cable installers use to attach RJ45 connectors to patch cables. A punchdown tool is a tool that cable installers use to attach keystone connectors to cable ends, for use in wall plates and patch panels. A telepole is a device used to run cables through walls, floors, and ceilings, but since the cable runs have already been pulled, Ralph will not need this tool. A pigtail splicer is a tool used only in fiber-optic cable installations.
55. Ralph is testing a twisted-pair cable run using a tone generator and locator. When he applies the tone generator to one particular wire at one end of the cable, he fails to detect a tone at the other end. Which of the following faults has Ralph discovered?

    1. Open
    2. Short
    3. Split pair
    4. Crosstalk

    Answer:

    A. The failure to detect a tone on a wire indicates that there is either a break in the wire somewhere inside the cable or a bad connection with the pin in one or both connectors. This condition is called an open circuit. A short is when a wire is connected to two or more pins at one end of the cable. A split pair is a connection in which two wires are incorrectly mapped in exactly the same way on both ends of the cable. Crosstalk is a type of interference caused by signals on one wire bleeding over to other wires.
56. Ralph is testing a twisted-pair cable run using a tone generator and locator. When he applies the tone generator to a particular pin at one end of the cable, he detects a tone on two pins at the other end. Which of the following faults has Ralph discovered?

    1. Open
    2. Short
    3. Split pair
    4. Crosstalk

    Answer:

    B. A short is when a wire is connected to two or more pins at one end of the cable or when the conductors of two or more wires are touching inside the cable. This would cause a tone applied to a single pin at one end to be heard on multiple pins at the other end. An open circuit would manifest as a failure to detect a tone on a wire, indicating that there is either a break in the wire somewhere inside the cable or a bad connection with the pin in one or both connectors. A split pair is a connection in which two wires are incorrectly mapped in exactly the same way on both ends of the cable. Crosstalk is a type of interference caused by signals on one wire bleeding over to other wires.
57. Ralph is using a tone generator and locator to test some newly installed twisted-pair cable runs on his network. Which of the following cable faults will he be unable to detect?

    1. Open
    2. Short
    3. Split pair
    4. Transposed pairs

    Answer:

    C. A split pair is a connection in which two wires are incorrectly mapped in exactly the same way on both ends of the cable. Each pin on one end of the cable is correctly wired to the corresponding pin at the other end, but the wires inside the cable used to make the connections are incorrect. In a properly wired connection, each twisted pair should contain a signal wire and a ground wire. In a split pair, it is possible to have two signal wires twisted together as a pair. This can generate excessive amounts of crosstalk, corrupting both of the signals involved. Because all of the pins are connected properly, a tone generator and locator cannot detect this fault. An open circuit would manifest as a failure to detect a tone on a wire, indicating that there is either a break in the wire somewhere inside the cable or a bad connection with the pin in one or both connectors. A short is when a wire is connected to two or more pins at one end of the cable or when the conductors of two or more wires are touching inside the cable. Transposed pairs is a fault in which both of the wires in a pair are connected to the wrong pins at one end of the cable. All three of these faults are detectable with a tone generator and locator.
58. Which of the following cable faults increases a twisted-pair cable's susceptibility to crosstalk?

    1. Open
    2. Short
    3. Split pair
    4. Transposed pairs

    Answer:

    C. A split pair is a connection in which two wires are incorrectly mapped in exactly the same way on both ends of the cable. Each pin on one end of the cable is correctly wired to the corresponding pin at the other end, but the wires inside the cable used to make the connections are incorrect. In a properly wired connection, each twisted pair should contain a signal wire and a ground wire. In a split pair, it is possible to have two signal wires twisted together as a pair. This can generate excessive amounts of crosstalk, corrupting both of the signals involved. Open circuits, shorts, and transposed pairs interfere with cable performance but do not make it more susceptible to crosstalk.
59. Alice has been told by a consultant that the newly installed twisted-pair cable runs on her network might have split pairs. Which of the following cable testing tools can she use to detect split pairs?

    1. Tone generator and locator
    2. Wiremap tester
    3. Multimeter
    4. Cable certifier

    Answer:

    D. A split pair is a connection in which two wires are incorrectly mapped in exactly the same way on both ends of the cable. Each pin on one end of the cable is correctly wired to the corresponding pin at the other end, but the wires inside the cable used to make the connections are incorrect. In a properly wired connection, each twisted pair should contain a signal wire and a ground wire. In a split pair, it is possible to have two signal wires twisted together as a pair. This can generate excessive amounts of crosstalk, corrupting both of the signals involved. Because all of the pins are connected properly, a tone generator and locator cannot detect this fault, and neither can a wiremap tester or a multimeter. However, a cable certifier is a highly sophisticated electronic device that can detect all types of cable faults, including split pairs, as well as measure cable performance characteristics.
60. Ralph is testing some newly installed twisted-pair cable runs on his network using a wiremap tester, and he has found one run that appears to have a cable break. However, the connectors at both ends are correctly installed, so the break must be somewhere inside the cable itself, which is nearly 100 meters long. Which of the following tools can Ralph use to determine the location of the cable break? (Choose all that apply.)

    1. Tone generator and locator
    2. Multimeter
    3. Time-domain reflectometer
    4. Cable certifier

    Answer:

    C, D. A time-domain reflectometer (TDR) is a device that determines the length of a cable by transmitting a signal at one end and measuring how long it takes for a reflection of the signal to return from the other end. Using this information and the cable's nominal velocity of propagation (NVP)—a specification supplied by the cable manufacturer—the device can calculate the length of a cable run. In a cable with a break in its length, a TDR calculates the length of the cable up to the break. Cable certifiers typically have time-domain reflectometry capabilities integrated into the unit. A tone generator and locator or a multimeter cannot locate a cable break.
61. Alice's company has moved to a building that was prewired for twisted-pair Ethernet. However, since installing the company's Gigabit Ethernet equipment using the existing cable runs, performance has been poor. After performing some packet captures and analyzing the traffic samples, Alice discovers that there are a great many Ethernet frames being retransmitted. Next, she examines the cable runs in the drop ceilings. They do not appear to be overly long, and they do not appear to run near any major sources of electromagnetic interference. Which of the following could be the problem?

    1. Some of the cable runs are using T568A pinouts and some are using T568B.
    2. The cables only have two wire pairs connected, instead of four.
    3. The existing cable is not rated for use with Gigabit Ethernet.
    4. There are mismatched transceivers at the cable ends.

    Answer:

    C. Of the options provided, the only possible source of the problem is that the cable runs are using a cable type not rated for Gigabit Ethernet. Some older buildings might still have Category 3 cable installed, which was used in the original twisted-pair Ethernet specification. Cat 3 is unsuitable for use with Gigabit Ethernet in many ways and can result in the poor performance that Alice is experiencing. A cable installation with runs wired using different pinout standards will not affect performance as long as each run uses the same pinouts at both ends. Gigabit Ethernet will not function at all if only two wire pairs are connected. The transceivers are located in the equipment that Alice's company brought from the old location, so they are not mismatched.
62. Ralph is working on a new twisted-pair network cable installation on which the individual cable runs were not properly labeled as they were pulled. Ralph now has to trace each of the cable ends in the office area to the correct cable end in the data center and label them correctly. Which of the following tools should Ralph use to locate the correct cable in a bundle of unlabeled cable ends?

    1. Cable certifier
    2. Tone generator and locator
    3. OTDR
    4. Multimeter

    Answer:

    B. Ralph can use a tone generator and locator to locate the correct cable associated with each office connection. By connecting the tone generator to one end of a cable run, he can use the locator to find the other end. A cable certifier identifies a variety of cable performance characteristics, typically including cabling length, signal attenuation, and crosstalk. An Optical Time Domain Reflectometer (OTDR) is a device for measuring the lengths and other characteristics of fiber-optic cables. A multimeter is a device for measuring the electric current on a copper cable.
63. Ralph's company has engaged a firm of wiring contractors to install some new fiber-optic cable runs. Before the cables are connected to any devices, Ralph wants to confirm that they have been installed to proper specifications. He brings in a contractor from another firm to test the cable runs. To test each cable run, the contractor connects a light source to one end of the cable and a measuring device to the other end. Which of the following is the correct name for this testing device?

    1. Optical power meter
    2. OLTS
    3. OTDR
    4. Multimeter

    Answer:

    B. An optical loss test set (OLTS) is the term for the combination of an optical light source and an optical power meter. The optical power meter by itself cannot be used to test the cable runs when there are no devices connected to them. An Optical Time Domain Reflectometer (OTDR) is a device for measuring the lengths and other characteristics of fiber-optic cables. A multimeter is a device for measuring the electric current on a copper cable.
64. Ed is experiencing poor network performance on some new twisted-pair cable runs. After ruling out all other causes, he tests the cables with a tone generator and locator and finds no faults. Finally, he examines the cable connectors more closely and finds that, while the pins at one end of the cable are correctly connected to their corresponding pins at the other end, in some cases there are two solid color wires twisted together in a pair. Which of the following types of faults has Ed discovered?

    1. Open circuit
    2. Short circuit
    3. Split pairs
    4. Transposed wires

    Answer:

    C. A split pair is a connection in which two wires are incorrectly mapped in exactly the same way on both ends of the cable. In a properly wired connection, each twisted pair should contain a colored signal wire and a striped ground wire. In a split pair, it is possible to have two signal wires twisted together as a pair. This can generate excessive amounts of crosstalk, corrupting both of the signals involved. Because all of the pins are connected properly, a tone generator and locator cannot detect this fault. An open circuit would manifest as a failure to detect a tone on a wire, indicating that there is either a break in the wire or a bad connection in one or both connectors. A short is when a wire is connected to two or more pins or when the conductors of two or more wires are touching. Transposed pairs is a fault in which both of the wires in a pair are connected to the wrong pins at one end of the cable. All three of these faults are detectable with a tone generator and locator.
65. Which of the following terms describes the progressive weakening of transmitted signals as they travel along a network medium?

    1. Absorption
    2. Latency
    3. Attenuation
    4. Crosstalk

    Answer:

    C. Attenuation is the weakening of a signal as it travels long distances, whether on a wired or wireless medium. The longer the transmission distance, the more the signal weakens. Absorption is the tendency of a wireless signal to change as it passes through different materials. Latency is a measurement of the time it takes for a signal to travel from its source to its destination. Crosstalk is a type of interference that occurs on wired networks when a signal bleeds over to an adjacent wire.
66. After experiencing some problems with devices connected to the company's fiber-optic network, Alice brings in a contractor to test the fiber-optic cable runs. The contractor detects a significant amount of decibel (dB) loss in some of the cable runs, which could be the source of the problems. Which of the following are possible causes of the decibel loss? (Choose all that apply.)

    1. Electromagnetic interference
    2. Dirty optical cables
    3. Excessive cable length
    4. Signal crosstalk

    Answer:

    B, C. Dirt on fiber-optic cable connectors can reduce the strength of the signal, resulting in decibel loss. Excessive cable length can result in greater attenuation and weaker signals due to the decibel loss. Electromagnetic interference and signal crosstalk are both factors that can affect copper cable transmissions, but not fiber optic.
67. Which of the following should a troubleshooter look for when a duplex mismatch is suspected on an Ethernet network? (Choose all that apply.)

    1. Collisions
    2. Runt frames
    3. CRC errors
    4. Failed ping tests

    Answer:

    A, B, C. There should be no collisions at all on a full-duplex network, so collisions indicate that at least one side of the connection is trying to operate in half-duplex mode. Ethernet running over twisted-pair cable, in its original half-duplex mode, detects collisions by looking for data on the transmit and receive pins at the same time. In full-duplex mode, data is supposed to be transmitted and received at the same time. In a duplex mismatch, in which one side of a connection is configured to use full duplex and the other end is configured to use half duplex, the full-duplex communications originating from one side look like collisions to the half-duplex side. The half-duplex adapter transmits a jam signal as a result of each collision, which causes the full-duplex side to receive an incomplete or damaged frame, which are perceived as runts or through Cyclic Redundancy Check (CRC) errors. Both sides then start to retransmit frames in a continuing cycle, causing network performance to diminish. Ping tests do not detect a duplex mismatch, because `ping` only transmits a small amount of data in one direction at a time. The mismatch only becomes apparent when the systems transmit large amounts of data.
68. Ed is trying to troubleshoot a problem that has caused a wired network connection to fail completely. Which of the following wired network problems will cause a complete failure of a network connection? (Choose all that apply.)

    1. Bottleneck
    2. Speed mismatch
    3. Duplex mismatch
    4. TX/RX reversal
    5. Bad switch port

    Answer:

    B, D, E. A speed mismatch on a wired network only occurs when two devices are configured to use a specific transmission speed and those speeds are different. In that case, network communication stops. For network communication to occur on a twisted-pair network, transmit (TX) pins must be connected to receive (RX) pins. If the connections are reversed, no communication occurs. If the switch port to which a computer is connected is bad, there will be no network communication. Bottlenecks and duplex mismatches will slow down network communications, but they will not stop them completely.
69. Ed is trying to troubleshoot a problem that has caused a wired network connection to slow down noticeably. Which of the following wired network problems will cause a drastic slowdown of a network connection, without causing it to fail completely? (Choose all that apply.)

    1. Bottleneck
    2. Speed mismatch
    3. Duplex mismatch
    4. TX/RX reversal

    Answer:

    A, C. A bottleneck is a component involved in a network connection that is not functioning correctly, causing a traffic slowdown that affects the entire network. A duplex mismatch occurs when one side of a connection is configured to use full duplex and the other end is configured to use half duplex. When this occurs, the full-duplex communications on the one side look like collisions to the half-duplex side. The half-duplex adapter transmits a jam signal as a result of each collision, which causes the full-duplex side to receive an incomplete frame. Both sides then start to retransmit frames in a continuing cycle, causing network performance to diminish drastically. A speed mismatch or a Transmit and Receive (TX/RX) reversal will stop network communication completely.
70. Ed has discovered that some of the twisted-pair cable runs on his newly installed Ethernet network are well over 100 meters long. Which of the following problems is his network likely to experience due to cable segments that are greater than the specified length?

    1. Jitter
    2. Attenuation
    3. Crosstalk
    4. EMI

    Answer:

    B. Attenuation is the weakening of a signal as it travels long distances, whether on a wired or wireless medium. The longer the transmission distance, the more the signal weakens. Cable length specifications are designed in part to prevent signals from attenuating to the point at which they are unviable. Jitter, crosstalk, and electromagnetic interference (EMI) are all conditions that can affect the performance of a wired network, but they are not directly related to the length of the cable.
71. Ed is trying to troubleshoot a problem with his wired network, and his research has led him to a list of possible network faults. The list is rather old, however, and Ed is wondering if some of the problems are relevant. Which of the following wired network problems no longer occur with modern Gigabit Ethernet switches and network adapters in their default configurations? (Choose all that apply.)

    1. Bottleneck
    2. Speed mismatch
    3. Duplex mismatch)
    4. Transmit and Receive (TX/RX reversal

    Answer:

    B, C. The Gigabit Ethernet standards call for switches and network adapters to support autonegotiation by default, which enables devices to communicate and select the best network speed and duplex mode available to them both. Therefore, speed mismatches and duplex mismatches no longer occur unless someone modifies the speed or duplex settings to incompatible values on one or both devices.
72. Ed has discovered that some of the twisted-pair cables on his newly installed network are running right alongside fluorescent light fixtures in the drop ceiling. Which of the following problems is the network likely to experience due to the cables' proximity to the fixtures?

    1. Jitter
    2. Attenuation
    3. Crosstalk
    4. EMI

    Answer:

    D. Fluorescent light fixtures and other devices in an office environment can generate magnetic fields, resulting in electromagnetic interference (EMI). When a copper-based cable runs too near to such a device, the magnetic fields can generate an electric current on the cable that interferes with the signals exchanged by network devices. Jitter, crosstalk, and attenuation are all conditions that can affect the performance of a wired network, but they are not directly related to the cables' proximity to light fixtures.
73. Which of the following indicators can you use to determine whether an adapter is connected to a functioning hub or switch?

    1. Speed Light-Emitting Diode (LED)
    2. Collision LED
    3. Link pulse LED
    4. Status LED

    Answer:

    C. The link pulse LED indicates the adapter is connected to a functioning hub or switch. The speed LED specifies the data rate of the link. The collision LED lights up when collisions occur. There is no status LED on a network interface adapter.
74. Ralph wants to use Power over Ethernet (PoE) to supply power to security cameras located throughout his company's datacenter. The Ethernet network is currently running at Gigabit Ethernet speed, but Ralph is planning to downgrade the camera connections to 100Base-TX, because that standard has two wire pairs free for the transmission of power. Which of the following statements about Ralph's plan is true?

    1. Ralph's planning is correct; only 10Base-T and 100Base-TX support PoE.
    2. Ralph's plan will not work because 100Base-TX is not compatible with PoE.
    3. Ralph's plan will work, but it is not necessary to downgrade the connections to 100Base-TX.
    4. Ralph's plan will not work, because PoE cannot supply enough power for the cameras.

    Answer:

    C. The Alternative B PoE variant can use the spare wire pairs in a Category 5 (Cat 5) or better 10Base-T or 100Base-TX cable to supply power to connected devices. The Alternative A and 4PPoE variants cannot use the spare wire pair in this manner; they supply power using the wire pairs that carry data at the same time. For Gigabit Ethernet or faster installations, Alternative B is capable of using the data wire pairs.
75. Delays in the transmission of data packets over a network can result in temporary service interruptions, dropouts, or even data loss. Which of the following terms is used to describe these delays?

    1. Crosstalk
    2. Electromagnetic interference (EMI)
    3. Jitter
    4. Attenuation

    Answer:

    C. Jitter is defined as delays in the transmission of individual network packets. For audio or video transmissions, jitter can result in dropped words or frames. For data file transmissions, jitter can require retransmission of packets.
76. Ralph's company has expanded to include an additional building on the far end of the corporate campus, approximately 4 kilometers away from the building housing the datacenter. A single-mode fiber-optic cable connection has been installed between the new building and the datacenter for a 1000Base-BX10 connection, but the cable is not yet connected to a transceiver at the datacenter end. Noticing that there is a 1000Base-SX transceiver module in the datacenter storeroom, Ralph is wondering if he could use this on the new cable run. Which of the following are reasons why this might not work? (Choose all that apply.)

    1. Transceiver mismatch
    2. Incorrect cable type
    3. Excessive cable length
    4. Wavelength mismatch

    Answer:

    A, B, C, D. The 1000Base-SX standard calls for multimode cable with a maximum length of approximately 500 meters, while the new cable run is 4,000 meters and uses single-mode cable. The 1000Base-SX transceiver will also be incompatible with the 1000Base-BX10 transceiver at the other end. 1000Base-BX10 uses wavelengths from 1,300 to 1,600 nanometers (nm), whereas 1000Base-SX uses wavelengths of 770 to 860 nm.
77. Alice has recently installed some new computers onto her Gigabit Ethernet network. To ensure the best possible network performance, she has configured the network adapters in the new computers to run at 1 Gbps speed and use full-duplex communication. Once the computers are in service, however, Alice begins getting reports of extremely poor network performance on those machines. She tries running some ping tests and does not see any problem. She calls in a consultant to perform a packet analysis, and the consultant detects large numbers of packet collisions, late collisions, Cyclic Redundancy Check (CRC) errors, and runt frames. Which of the following could conceivably be the problem?

    1. Duplex mismatch
    2. TX/RX reversal
    3. Incorrect cable type
    4. Damaged cables

    Answer:

    A. There should be no collisions on a full-duplex network, so the problem is clearly related to the duplexing of the communications. Ethernet running over twisted-pair cable, in its original half-duplex mode, detects collisions by looking for data on the Transmit and Receive (TX/RX) pins at the same time. In full-duplex mode, data is supposed to be transmitted and received at the same time. When one side of a connection is configured to use full duplex, as Alice's new computers are, and the other end is configured to use half duplex (as the switches must be), the full-duplex communications on the one side look like collisions to the half-duplex side. The half-duplex adapter transmits a jam signal as a result of each collision, which causes the full-duplex side to receive an incomplete frame. Both sides then start to retransmit frames in a continuing cycle, causing network performance to diminish drastically. The ping tests do not detect a problem, because `ping` only transmits a small amount of data in one direction at a time. The other options would likely cause the ping tests to fail as well. The solution to the problem is to configure all of the devices to autonegotiate their speed and duplex modes.
78. Ralph is attempting to access a Domain Name System (DNS) server located on the other side of a router, but his attempt fails with an error stating that the destination port UDP 53 is unreachable. His first step in troubleshooting the problem is to try using the `nslookup` utility to access that specific DNS server. This too fails. Next, he uses the `ping` utility with the DNS server's Internet Protocol (IP) address. The ping test is successful, indicating that the server is up and running. Which of the following are possible causes of the problem? (Choose all that apply.)

    1. The router connecting the networks is not running DNS and will not forward this type of datagram.
    2. The DNS process on the remote server is not running.
    3. The TCP/IP host configuration on your computer is improperly configured.
    4. The TCP/IP host configuration on the DNS server computer is improperly configured.
    5. There is a firewall blocking the DNS server's UTP 53 port.

    Answer:

    B, E. One possible cause of the problem is that the DNS process on the remote server is corrupted or not running. Another possible cause is that there is a firewall blocking access to the server's Unshielded Twisted Pair (UTP) port 53. Both of these would render the port unreachable. The Transmission Control Protocol/Internet Protocol (TCP/IP) client on the server is operating, as verified by the `ping` utility. This means that the IP host configurations on Ralph's computer and on the DNS server are both functioning. The router does not need to be running DNS to forward datagrams.
79. Which of the following application layer protocols includes a program that enables a user to log on to a network device and execute commands on the remote system using a command-line interface? (Choose all that apply.)

    1. Telnet
    2. File Transfer Protocol (FTP)
    3. Simple Network Management Protocol (SNMP)
    4. Domain Name System (DNS)
    5. Nslookup

    Answer:

    A, B. Both Telnet and FTP are protocols that include command-line client applications, with Telnet providing terminal emulation and FTP file transfer functionality. SNMP and DNS are both application layer protocols, but neither one includes a program. Nslookup has a command-line interface, but it executes commands on the local system, not a remote one.
80. Which of the following Windows tools uses Internet Control Message Protocol (ICMP) messages and manipulates IPv4 time-to-live values to illustrate the route packets take through an internetwork?

    1. `ping`
    2. `netstat`
    3. `route`
    4. `tracert`
    5. `nslookup`
    6. `hostname`

    Answer:

    D. The Windows `tracert` tool transmits a series of ICMP messages with incrementing Time to Live (TTL) values, which identify each router on the path that the packets take through the network. `Ping` uses ICMP, but it does not manipulate TTL values. `Netstat`, `Route`, `Nslookup`, and `Hostname` do not use ICMP messages, nor do they manipulate TTL values when performing their normal functions.
81. Users are having trouble connecting to Internet hosts. Alice suspects that there is a problem with the Domain Name System (DNS) server, and she wants to verify this. Which of the following steps can she take to determine whether the DNS server is resolving Internet hostnames?

    1. Issue the `ipconfig` command from a local workstation
    2. Try to connect to a host using the IP address instead of the hostname
    3. Ping the DNS server to see if it is functioning
    4. Use the `tracert` command to test the functionality of the DNS server

    Answer:

    B. If Alice suspects that a DNS server is not resolving hostnames, she should try connecting to a remote host using the Internet Protocol (IP) address instead of the name. If she can connect, she knows that all internal Local Area Network (LAN) components and the Internet gateway are functioning, and the remote host is functioning. The problem most likely lies within the DNS server itself. If Alice cannot connect to a remote host using the IP address, the problem is not the DNS server. She would need to do more testing to isolate the problem device and the affected area. `ipconfig` is a workstation command that enables you to verify the local IP configuration; it is not used to test a DNS server's functionality. Using the `ping` command will only tell you whether the computer hosting the DNS service is functioning at the network layer of the Open Systems Interconnection (OSI) model; it will not test the DNS service functionality. The `tracert` (or `traceroute`) command is used to identify the hop-by-hop path taken to reach a destination; it does not allow you to test functionality above the network layer of the OSI model.
82. Which of the following utilities can you use to view resource record information on a particular Domain Name System (DNS) server? (Choose all that apply.)

    1. `netstat`
    2. `nslookup`
    3. `nbtstat`
    4. `arp`
    5. `dig`

    Answer:

    B, E. `nslookup` and `dig` are both command-line utilities that you can direct to a specific DNS server and then generate queries that display resource record information the program retrieves from the server. `netstat` displays information about networking protocols, whereas `nbtstat` displays information derived from the system's Network Basic Input/Output System (NetBIOS) over Transmission Control Protocol/Internet Protocol (TCP/IP) implementation. `arp` is a tool that you can use to display and manage a system's Address Resolution Protocol (ARP) table entries. `netstat`, `nbtstat`, and `arp` are not able to display resource record information.
83. Which of the following Windows command-line utilities produced the output shown here?

    `Interface: 192.168.2.24 --- 0x2 internet Address Physical Address Type 192.168.2.2 d4-ae-52-bf-c3-2d dynamic 192.168.2.20 00-26-c7-7e-00-e0 dynamic 192.168.2.22 00-90-a9-a2-43-8f dynamic 192.168.2.27 1c-c1-de-ca-1f-12 dynamic 192.168.2.28 30-f7-72-38-e9-1d dynamic 192.168.2.255 ff-ff-ff-ff-ff-ff static 224.0.0.22 01-00-5e-00-00-16 static 224.0.0.251 01-00-5e-00-00-fb static 224.0.0.252 01-00-5e-00-00-fc static 224.0.0.253 01-00-5e-00-00-fd static 239.255.255.250 01-00-5e-7f-ff-fa static 255.255.255.255 ff-ff-ff-ff-ff-ff static`

    1. `ping`
    2. `tracert`
    3. `netstat`
    4. `arp`
    5. `hostname`

    Answer:

    D. Running the `arp` utility with the `-a` parameter on a Windows system displays the contents of the Address Resolution Protocol (ARP) cache. The cache contains records of the Internet Protocol (IP) addresses on the network that `arp` has resolved into Media Access Control (MAC) addresses. The `ping`, `tracert`, `netstat`, and `hostname` utilities are not capable of producing this output.
84. Which of the following Windows command-line utilities produced the output shown here?

    `1 <1 ms <1 ms <1 ms RT-N86U [192.168.2.99] 2 3 ms 5 ms 4 ms 192.168.3.1 3 25 ms 30 ms 17 ms 10.172.1.1 4 20 ms 19 ms 29 ms gateway-BE1-EBlocal.eh.lpod.net [207.44.123.89] 5 26 ms 29 ms 29 ms gateway-be1-abn2abn2.ab.lpod.net [207.44.127.49] 6 * * * Request timed out. 7 111 ms 108 ms 109 ms be38.trmc0215-01.ars.mgmt.hox3.kkg [184.168.0.69] 8 108 ms 107 ms 108 ms be38.trmc0215-01.ars.mgmt.hox3.kkg [184.168.0.69] 9 106 ms 109 ms 108 ms ip-216-69-188-102.ip.srvr.net [216.69.188.102] 10 106 ms 108 ms 99 ms p3nlh153.shr.prod.phx3.srvr.net [97.74.144.153]`

    1. `ping`
    2. `tracert`
    3. `netstat`
    4. `arp`
    5. `hostname`

    Answer:

    B. The Windows `tracert` utility functions by transmitting a series of Internet Control Message Protocol (ICMP) Echo Request messages to a specified destination with incrementing Time to Live (TTL) values. Each successive message reaches one hop farther on the route to the destination before timing out. The `tracert` display therefore lists the names and addresses of the routers that packets must traverse to reach the destination. The `ping`, `netstat`, `arp`, and `hostname` utilities are not capable of producing this output.
85. Which of the following Windows command-line utilities produced the output shown here?

    `Reply from 97.74.144.153: bytes=32 time=111ms TTL=53 Reply from 97.74.144.153: bytes=32 time=109ms TTL=53 Reply from 97.74.144.153: bytes=32 time=108ms TTL=53 Reply from 97.74.144.153: bytes=32 time=109ms TTL=53 Statistics for 97.74.144.153: Packets: Sent = 4, Received = 4, Lost = 0 (0% loss), Approximate round trip times in milli-seconds: Minimum = 108ms, Maximum = 111ms, Average = 109ms`

    1. `ping`
    2. `tracert`
    3. `netstat`
    4. `arp`
    5. `hostname`

    Answer:

    A. The Windows `ping` utility functions by transmitting a series of Internet Control Message Protocol (ICMP) Echo Request messages to a specified destination. The destination system responds with ICMP Echo Reply messages that are listed in the output display. The `tracert`, `netstat`, `arp`, and `hostname` utilities are not capable of producing this output.
86. Which of the following Windows command-line utilities produced the output shown here?

    `Active Connections Proto Local Address Foreign Address State TCP 127.0.0.1:5327 CM412:49770 ESTABLISHED TCP 127.0.0.1:49770 CM412:5327 ESTABLISHED TCP 127.0.0.1:52114 CM412:52115 ESTABLISHED TCP 192.168.2.24:2869 RT-M96U:42173 ESTABLISHED TCP 192.168.2.24:2869 RT-M96U:44356 ESTABLISHED TCP 192.168.2.24:51386 autodiscover:https ESTABLISHED TCP 192.168.2.24:51486 autodiscover:https ESTABLISHED TCP 192.168.2.24:51535 108-174-11-1:https ESTABLISHED TCP 192.168.2.24:51578 aki-cache:http TIME_WAIT TCP 192.168.2.24:51579 ia3s43-in-f142:http TIME_WAIT TCP 192.168.2.24:51591 208:https TIME_WAIT TCP 192.168.2.24:51592 208:https TIME_WAIT TCP 192.168.2.24:51593 198.8.20.212:https TIME_WAIT`

    1. `ping`
    2. `tracert`
    3. `netstat`
    4. `arp`
    5. `hostname`

    Answer:

    C. Running the Windows `netstat` utility with no parameters generates a list of the workstation's active connections. The `ping`, `tracert`, `arp`, and `hostname` utilities are not capable of producing this output.
87. Which of the following command-line utilities is capable of performing the same basic function as `traceroute` or `tracert`?

    1. `ping`
    2. `pathping`
    3. `netstat`
    4. `route`

    Answer:

    B. Like `traceroute` and `tracert`, `pathping` is capable of generating a list of the routers that packets pass through on the way to a specific destination system. `pathping` also displays the percentage of lost packets for each hop, which `traceroute` and `tracert` cannot do. The `ping`, `netstat`, and `route` utilities are not capable of displaying route traces.
88. Which TCP/IP utility should you use to most easily identify a malfunctioning router on your network?

    1. `ifconfig`
    2. `ping`
    3. `traceroute`
    4. `netstat`

    Answer:

    C. The `traceroute` (or `tracert`) utility can locate a malfunctioning router by using an Echo Request messages with incrementing Time to Live (TTL) values. `ifconfig` is a network configuration utility for Unix and Linux systems; `ping` can test connectivity to another Transmission Control Protocol/Internet Protocol (TCP/IP) system, but it cannot locate a malfunctioning router; and `netstat` displays information about network connections and traffic but cannot locate a malfunctioning router.
89. Which of the following protocols does the ping program never use to carry its messages?

    1. Ethernet
    2. ICMP
    3. IP
    4. UDP
    5. TCP

    Answer:

    E. All Windows ping transactions use Internet Control Message Protocol (ICMP) messages. ICMP messages are encapsulated directly within Internet Protocol (IP) datagrams; they do not use transport layer protocols, such as User Datagram Protocol (UDP). Ping transactions to destinations on the local network are encapsulated within Ethernet frames. On Unix and Linux, ping uses UDP, which is also encapsulated in IP datagrams.
90. Which of the following commands displays the routing table on the local computer?

    1. `arp –r`
    2. `netstat –r`
    3. `ifconfig –r`
    4. `telnet –r`

    Answer:

    B. The netstat utility can display the routing table, along with other types of network traffic and port information. The arp utility is for adding addresses to the Address Resolution Protocol (ARP) cache; it cannot display the routing table. The `ifconfig` command displays Transmission Control Protocol/Internet Protocol (TCP/IP) configuration information on Unix and Linux systems; it cannot display the routing table. Telnet is a terminal emulation program; it cannot display the routing table.
91. Which of the following command lines will produce the output shown in the figure?

    Larger View

    <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c05uf006_0.jpg?width=836" alt=""><figcaption></figcaption></figure>

    1. `ping 10.0.0.1 -t`
    2. `ping 10.0.0.1 -n 2048`
    3. `ping 10.0.0.1 -l 2048 -n 11`
    4. `ping 10.0.0.1 -l 2048 -t`
    5. `ping 10.0.0.1 -n 2048 -t 11`

    Answer:

    C. Running `ping` with the `-l` parameter enables you to specify the size of the messages sent to the target—in this case, 2028 bytes. The `-n` parameter enables you to specify the number of messages the `ping` tool should transmit—in this case, 11. Combining these two parameters generates the output in the figure. The `-t` parameter causes the `ping` tool to transmit messages until manually halted.
92. Which of the following commands enables you to view the Address Resolution Protocol (ARP) table stored in memory?

    1. `arp -c`
    2. `arp -d`
    3. `arp -a`
    4. `arp -s`

    Answer:

    C. The `arp -a` command displays the entries in the ARP table stored in its cache. The `arp -d` command is for deleting entries, and the `arp -s` command is for adding entries. The `arp -c` command is not a valid option.
93. Which of the following command-line utilities enables you to generate Domain Name System (DNS) request messages?

    1. `ifconfig`
    2. `nslookup`
    3. `nbtstat`
    4. `netstat`
    5. `iperf`

    Answer:

    B. The `nslookup` tool enables you to generate DNS request messages from the command line and send them to a specific DNS server. The other options listed are not DNS utilities.
94. Which of the following command-line utilities enables you to view the Internet Protocol (IP) configuration on a Unix or Linux host?

    1. `ifconfig`
    2. `nslookup`
    3. `ipconfig`
    4. `netstat`
    5. `iperf`

    Answer:

    A. On a Unix or Linux host, the `ifconfig` command displays the system's current IP configuration settings and parameters. `ipconfig` is a Windows command-line utility that performs the same basic function. The other options are command-line utilities that do not display IP configuration information.
95. Which of the following parameters causes the ping tool to transmit messages continually until manually halted?

    1. `-n`
    2. `-t`
    3. `-i`
    4. `-a`

    Answer:

    B. Running the `ping` tool with the `-t` parameter causes it to send messages to the target continuously until it is manually stopped. The `-n` parameter specifies the number of messages the `ping` tool should transmit. The `-i` parameter specifies the time-to-live (TTL) value of the messages ping transmits. The `-a` parameter resolves an Internet Protocol (IP) address specify as the target to a hostname.
96. Which of the following Windows commands enables you to delete the entire ARP cache?

    1. `arp -c ∗`
    2. `arp -d ∗`
    3. `arp -a`
    4. `arp -s`

    Answer:

    B. The `arp -d` command is for deleting cache entries, and by running it with the asterisk wildcard, the command deletes all of the entries in the cache. The `arp -a` command displays the entries in the ARP table stored in its cache, and the `arp -s` command is for adding entries. The `arp -c ∗` command is not a valid option.
97. Ralph has been advised to check his Linux web servers for open ports that attackers might be able to use to penetrate the servers' security. Which of the following utilities can Ralph use to do this?

    1. `tcpdump`
    2. `dig`
    3. `iptables`
    4. `nmap`
    5. `iperf`

    Answer:

    D. The `nmap` utility is capable of scanning a system for open ports that might be a security hazard. The `tcpdump`, `dig`, `iptables`, and `iperf` utilities cannot do this.
98. While performing a protocol analysis, Alice notes that there are many Internet Control Message Protocol (ICMP) packets in her captured traffic samples. She attributes these to her frequent use of Transmission Control Protocol/Internet Protocol (TCP/IP) troubleshooting tools. Which of the following utilities are used to test network layer characteristics of a host using ICMP messages? (Choose all that apply.)

    1. `ipconfig`
    2. `netstat`
    3. `ping`
    4. `tracert`

    Answer:

    C, D. `ping` and `tracert` are both utilities that test network layer characteristics using ICMP messages. `ping` tests the network layer functionality of the host, and `traceroute` displays the path to the host through the internetwork. `ipconfig` and `netstat` do not use ICMP messages.
99. Which of the following parameters enables you to specify the Time to Live (TTL) value of the messages that `ping` transmits?

    1. `-n`
    2. `-t`
    3. `-i`
    4. `-a`

    Answer:

    C. Running the `ping` tool with the `-i` parameter specifies the TTL value of the messages that `ping` transmits. The `-t` parameter causes the `ping` tool to send messages to the target continuously until it is manually stopped. The `-n` parameter specifies the number of messages the `ping` tool should transmit. The `-a` parameter resolves an Internet Protocol (IP) address specified as the target to a hostname.
100.    Ralph is the network administrator of his company's network. He has had three users call the help desk to report that they are having problems connecting to the local application server. Comparing their stories, Ralph suspects that their Transmission Control Protocol (TCP) connections are being dropped. The users are not having problems connecting to any other hosts on the network. To troubleshoot this problem, Ralph decides to use a protocol analyzer. He wants to store and view only the traffic relating to the hosts and server that are having problems. How can Ralph do this?

        1. Configure a display filter
        2. Configure a capture filter
        3. Set a trap on the analyzer
        4. Configure both a capture filter and a display filter

        Answer:

        B. Ralph wants to store and view only the traffic relating to the hosts that are experiencing problems. The best way to do this is to set a capture filter. Capture filters determine what is stored in the buffer. Display filters only determine what is displayed from the contents of the buffer. You do not set a trap on an analyzer—you set traps on Simple Network Management Protocol (SNMP) agents. Also, there is no need to configure both a capture filter and a display filter. If you set a capture filter that blocks all other traffic from entering the buffer, the display filter would be redundant.
101.    Ralph is the administrator of his company's network. All of the users on the network are reporting that they are having difficulty connecting to a particular application server that is located on a perimeter network, on the other side of a router. The users are not having trouble connecting to local hosts. Which of the following troubleshooting tools can Ralph use to verify the network layer functionality of the application server and the router? (Choose all that apply.)

        1. `ping`
        2. `route`
        3. `arp`
        4. `traceroute`

        Answer:

        A, D. Ralph can use the `ping` and `traceroute` tools to verify the network layer functionality of the application server and the router. The `ping` tool tests the network layer through the exchange of Internet Control Message Protocol (ICMP) Echo and Echo Reply messages. The `traceroute` tool can verify that there is a functioning path between the users' workstations and the application server. The `route` tool is used to administer the routing table on the local machine. The `arp` tool is used to view a computer's Internet Protocol to Media Access Control (IP to MAC) address resolution table stored in memory.
102.    Which of the following troubleshooting tools enables you to copy all of the packets transmitted over a network to a buffer, interpret the protocols used in the packets, and display the output?

        1. Event Viewer
        2. Traffic monitor
        3. Protocol analyzer
        4. Management console

        Answer:

        C. A protocol analyzer copies all network traffic, interprets the protocol headers and fields, and displays the output. The Event Viewer displays system, application, and security event logs on a single computer. There is no network troubleshooting tool called a traffic monitor. A management console is a remote monitoring and management device that queries Simple Network Management Protocol (SNMP) agents.
103.    Which of the following is not a tool that runs only on Unix or Linux systems?

        1. `tcpdump`
        2. `dig`
        3. `iptables`
        4. `ifconfig`
        5. `route`

        Answer:

        E. Of the utilities listed, `tcpdump`, `dig`, `iptables`, and `ifconfig` are all tools that run on Unix or Linux systems only. The `route` utility runs on both Unix or Linux and Windows.
104.    Which of the following Windows command-line utilities produced the output shown here?

        `Server: trv213.pljd.net Address: 203.186.120.114 Non-authoritative answer: Name: microsoft.com Addresses: 104.43.195.251 23.100.122.175 23.96.52.53 191.239.213.197 104.40.211.35`

        1. `nslookup`
        2. `pathping`
        3. `netstat`
        4. `route`

        Answer:

        A. `nslookup` is a command-line utility that generates Domain Name System (DNS) resource record requests and sends them to a specific DNS server. The output shown here first specifies the name and address of the DNS server to which the request was sent, and then the response to the request, containing the name to be resolved and the Internet Protocol (IP) addresses contained in the server's resource record for that name. The `pathping`, `netstat`, and `route` utilities cannot perform DNS queries.
105.    Which of the following parameters enables you to specify the number of messages the `ping` tool transmits?

        1. `-n`
        2. `-t`
        3. `-i`
        4. `-a`

        Answer:

        A. Running the `ping` tool with the `-n` parameter specifies the number of messages the tool should transmit with each execution. The `-t` parameter causes the `ping` tool to send messages to the target continuously until manually stopped. The `-i` parameter specifies the Time to-Live (TTL) value of the messages that `ping` transmits. The `-a` parameter resolves an Internet Protocol (IP) address specified as the target to a hostname.
106.    Which of the following command-line utilities can run on Windows, Unix, or Linux systems? (Choose all that apply.)

        1. `ping`
        2. `traceroute`
        3. `ifconfig`
        4. `iptables`
        5. `nslookup`

        Answer:

        A, E. The `ping` and `nslookup` utilities can both run on Windows, Unix, or Linux systems. The `traceroute` command runs only on Unix or Linux, although there is a Windows version called `tracert`. The `ifconfig` and `iptables` commands only exist on Unix and Linux systems.
107.    Which of the following command-line utilities can only run on Unix and Linux systems?

        1. `ping`
        2. `ipconfig`
        3. `tracert`
        4. `ifconfig`
        5. `netstat`

        Answer:

        D. The `ifconfig` command runs only on Unix and Linux systems. The `ping` and `netstat` utilities run on Windows, Unix, or Linux systems. The `ipconfig` and `tracert` commands run only on Windows, although there is a Unix/Linux version of `tracert` called `traceroute`.
108.    Which of the following command-line utilities can only run on Windows systems?

        1. `ping`
        2. `ipconfig`
        3. `traceroute`
        4. `ifconfig`
        5. `netstat`

        Answer:

        B. The `ipconfig` command runs only on Windows, although there is a similar Unix or Linux-only command called `ifconfig`. The `ping` and netstat utilities run on Windows, Unix, or Linux systems. The `traceroute` utility runs only on Unix or Linux systems, although there is a Windows version called `tracert`.
109.    Ralph is working on his company's perimeter network, which has five web servers running Linux, a Cisco router, a CSU/DSU providing a leased line connection, and a Windows-based firewall. While trying to troubleshoot a network communications failure, Ralph types the following command on one of the systems: `traceroute` [`adatum.com`](http://adatum.com/). Which of the following systems might Ralph be working on? (Choose all that apply.)

        1. The Windows-based firewall
        2. The Cisco router
        3. The CSU/DSU console
        4. One of the Linux web servers

        Answer:

        B, D. Both Linux and the Cisco IOS operating systems have the `traceroute` utility. Windows has a version of the utility, but it is called `tracert`. The CSU/DSU cannot run a `traceroute` command.
110.    Which of the following `netstat` commands can tell you how many IPv6 packets have been received on a particular Windows workstation?

        1. `netstat -a`
        2. `netstat -s`
        3. `netstat -e`
        4. `netstat -r`

        Answer:

        B. The `netstat -s` command displays packet counts and other traffic statistics for the IPv6, IPv4, ICMP, TCP, and UDP protocols. The `netstat -a` command displays all of a workstation's current connections and ports on which it is listening. The `netstat -e` command displays Ethernet statistics, such as the number of bytes and packets sent and received. The `netstat -r` command displays the computer's routing table.
111.    Which of the following commands can Ralph use to display the number of bytes that a Windows workstation has transmitted?

        1. `netstat`
        2. `tcpdump`
        3. `ipconfig`
        4. `iptables`

        Answer:

        A. Running `netstat` with the `-e` parameter on a Windows workstation displays Ethernet statistics, including the number of bytes and packets the workstation has sent and received. The `ipconfig` command displays Transmission Control Protocol/Internet Protocol (TCP/IP) configuration data; it does not display network traffic statistics. The `tcpdump` and `iptables` commands both run only on Unix and Linux workstations.
112.    Ralph is working on his company's perimeter network, which has five web servers running Linux, a Cisco router, a CSU/DSU providing a leased line connection, and a Windows-based firewall. While trying to troubleshoot a network communications failure, Ralph types the following command on one of the systems: `ping 192.168.1.76`. Which of the following systems might Ralph be working on? (Choose all that apply.)

        1. The Windows-based firewall
        2. The Cisco router
        3. The CSU/DSU console
        4. One of the Linux web servers

        Answer:

        A, B, D. Windows, Linux, and the Cisco IOS operating systems all include the `ping` utility. The CSU/DSU cannot run a `ping` command.
113.    Alice is troubleshooting a Windows server, and while doing so she runs the following command: `ping 127.0.0.1`. The command completes successfully. What has Alice proven by doing this?

        1. That the computer's network adapter is functioning properly
        2. That the computer's TCP/IP networking stack is loaded and functioning
        3. That the computer's IP address is correct for the network
        4. Nothing at all

        Answer:

        B. The Internet Protocol (IP) address 127.0.0.1 is a dedicated loopback address that directs outgoing IP traffic directly into the incoming IP traffic buffer. A successful ping test using that address indicates that the computer's Transmission Control Protocol/Internet Protocol (TCP/IP) stack is functioning properly, but the traffic never reaches the network adapter or the network, so the test does not confirm that the adapter is functioning or that the computer has a correct IP address for the network.
114.    Ed suspects that his workstation is experiencing Transmission Control Protocol/Internet Protocol (TCP/IP) communication problems. Which of the following commands can he use to confirm that the computer's TCP/IP stack is loaded and functioning? (Choose all that apply.)

        1. `ping loopback`
        2. `ping localhost`
        3. `ping 127.0.0.1`
        4. `ping 127.0.0.0`

        Answer:

        B, C. The Internet Protocol (IP) address 127.0.0.1 is a dedicated loopback address that directs outgoing IP traffic directly into the incoming IP traffic buffer. The hostname localhost resolves to the 127.0.0.1 address on every TCP/IP system. Ed can therefore ping either the hostname or the IP address to test that his TCP/IP stack is functional. Loopback is not a hostname for the loopback address, and 127.0.0.0 is a network address, not a host address, so it will not work in this situation.
115.    Ralph is the administrator of his company's network. He has a Dynamic Host Configuration Protocol (DHCP) server configured to supply Internet Protocol (IP) addresses and configuration information to all of the Windows computers on the network. One of the Windows users reports that she cannot connect to the network. Which of the following commands can Ralph run on her computer to verify the status of the computer's IP settings and configuration parameters?

        1. `ifconfig`
        2. `ipconfig`
        3. `msinfo32`
        4. `tracert`

        Answer:

        B. `ipconfig` is a Windows command that displays a computer's current IP address and Transmission Control Protocol/Internet Protocol (TCP/IP) configuration settings, including whether the computer has obtained its address from a DHCP server. The `ifconfig` command displays the same information for Unix and Linux systems. `msinfo32` is a Windows program that generates a graphical display of the computer's hardware and software configuration, but not its IP address and TCP/IP settings. The `tracert` command in Windows displays the path that packets take through the internetwork to reach a specified destination, but it does not display DHCP information.
116.    Which of the following are the three main categories of information that you can display by running the `netstat` command on a Windows computer?

        1. Connection state
        2. Active connections
        3. Routing table
        4. Interface statistics

        Answer:

        B, C, D. When you run the `netstat` command without any switch options, it displays the computer's active connections. Running `netstat -e` displays the computer's interface statistics. Running `netstat -r` displays the routing table. There is no `netstat` switch that displays the computer's connection state.
117.    Which of the following `route` commands displays the contents of a Windows computer's IPv6 routing table only?

        1. `route print`
        2. `route print -6`
        3. `route list -6`
        4. `route list`

        Answer:

        B. The `route print` command displays both the IPv4 and IPv6 routing tables. To display only the IPv6 routing table, you add the `-6` parameter to the `route print` command. `route list` and `route list -6` are not valid commands.
118.    Which of the following Windows command-line utilities produced the output shown here?

        `Interface Statistics Received Sent Bytes 663321544 1088192828 Unicast packets 29291610 10424979 Non-unicast packets 817568 58116 Discards 1628 0 Errors 0 0 Unknown protocols 0 0`

        1. `ping`
        2. `tracert`
        3. `netstat`
        4. `arp`

        Answer:

        C. Running the Windows `netstat` command with the `-e` parameter displays Ethernet statistics, including the number of bytes and packets that have been transmitted and received. The `ping`, `tracert`, and `arp` utilities are not capable of producing this output.
119.    Which of the following Linux commands generated the output shown in the figure?

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c05uf007_0.jpg?width=836" alt=""><figcaption></figcaption></figure>

        1. `arp -a`
        2. `arp -e`
        3. `arp -d`
        4. `arp -s`

        Answer:

        B. Running the `arp -e` command on a Linux system displays the contents of the Address Resolution Protocol (ARP) cache in the format shown here. The `arp -a` command displays the cache using an alternative format. The `arp -d` command is for deleting cache entries, and the `arp -s` command is for creating cache entries.
120.    Which of the following Windows commands enables you to create a new entry in the Address Resolution Protocol (ARP) cache?

        1. `arp -N`
        2. `arp -d`
        3. `arp -a`
        4. `arp -s`

        Answer:

        D. The `arp -s` command enables you to create a cache record specifying the Media Access Control (MAC) address and its associated Internet Protocol (IP) address. The `arp -N` command enables you to display the ARP cache entries for a specified network interface. The `arp -d` command is for deleting cache entries. The `arp -a` command displays the entries in the ARP table stored in its cache.
121.    Which of the following Unix/Linux tools is a packet analyzer?

        1. `iptables`
        2. `nmap`
        3. `tcpdump`
        4. `pathping`

        Answer:

        C. The `tcpdump` utility is a command-line tool that captures network packets and displays their contents. The `iptables`, `nmap`, and `pathping` utilities cannot capture and analyze packets. `iptables` manages Unix/Linux kernel firewall rules, `nmap` is a port scanner, and `pathping` is a Windows route tracing tool.
122.    Which of the following tools can administrators use to monitor network bandwidth and traffic patterns?

        1. Protocol analyzer
        2. Bandwidth speed tester
        3. NetFlow analyzer
        4. IP scanner

        Answer:

        C. A NetFlow analyzer is a tool that can collect network traffic data and analyze how bandwidth is being used and who is using it. A protocol analyzer is also a tool that captures network packets, but for the purpose of analyzing their contents. A bandwidth speed tester measures a network’s internet access speed. An Internet Protocol (IP) scanner lists the IP addresses that are in use on a network.
123.    Based on the output shown here, what is the average response time of the destination system?

        `1 <1 ms <1 ms <1 ms RT-N86U [192.168.2.99] 2 3 ms 5 ms 4 ms 192.168.3.1 3 25 ms 30 ms 17 ms 10.172.1.1 4 20 ms 19 ms 29 ms gateway-BE1-EBlocal.eh.lpod.net [207.44.123.89] 5 26 ms 29 ms 29 ms gateway-be1-abn2abn2.ab.lpod.net [207.44.127.49] 6 * * * Request timed out. 7 111 ms 108 ms 109 ms be38.trmc0215-01.ars.mgmt.hox3.kkg [184.168.0.69] 8 108 ms 107 ms 108 ms be38.trmc0215-01.ars.mgmt.hox3.kkg [184.168.0.69] 9 106 ms 109 ms 108 ms ip-216-69-188-102.ip.srvr.net [216.69.188.102] 10 106 ms 108 ms 99 ms p3nlh153.shr.prod.phx3.srvr.net [97.74.144.153]`

        1. 109.5 ms
        2. 104.33 ms
        3. 106 ms
        4. 99.66 ms

        Answer:

        B. The destination system is the last one listed in the trace. By averaging the response times of 99, 106, and 108 milliseconds (ms), you can calculate the average response time: 104.33 ms.
124.    Which of the following Linux commands produced the output shown in the figure?

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c05uf008_0.jpg?width=836" alt=""><figcaption></figcaption></figure>

        1. `netstat -ns microsoft.com`
        2. `dig microsoft.com ns`
        3. `nslookup microsoft.com`
        4. `route -s microsoft.com`

        Answer:

        B. The `dig` utility in Linux can display the authoritative Domain Name System (DNS) servers for a particular domain when you specify the domain name and the `ns` (name server) parameter. The `netstat`, `nslookup`, and `route` commands cannot generate this particular output.
125.    Which of the following protocols does the `traceroute` utility on Unix and Linux systems use to test TCP/IP connectivity?

        1. ICMP
        2. HTTP
        3. TCP
        4. UDP

        Answer:

        D. On Unix and Linux systems, the `traceroute` utility tests Transmission Control Protocol/Internet Protocol (TCP/IP) connectivity by transmitting User Datagram Protocol (UDP) messages. This is unlike the `tracert` utility on Windows systems, which uses Internet Control Message Protocol (ICMP) messages. Neither version uses TCP or Hypertext Transfer Protocol (HTTP).
126.    A user calls Alice at the help desk to report that he cannot access the Internet. He can access systems on the local network, however. Alice examines the routing table on the user's workstation. Which of the following statements explains why the user cannot access the Internet?

        `IPv4 Route Table =========================================================================== Active Routes: Network Destination Netmask Gateway Interface Metric 127.0.0.0 255.0.0.0 On-link 127.0.0.1 331 127.0.0.1 255.255.255.255 On-link 127.0.0.1 331 127.255.255.255 255.255.255.255 On-link 127.0.0.1 331 192.168.2.0 255.255.255.0 On-link 192.168.2.37 281 192.168.2.37 255.255.255.255 On-link 192.168.2.37 281 192.168.2.255 255.255.255.255 On-link 192.168.2.37 281 224.0.0.0 240.0.0.0 On-link 127.0.0.1 331 224.0.0.0 240.0.0.0 On-link 192.168.2.37 281 255.255.255.255 255.255.255.255 On-link 127.0.0.1 331 255.255.255.255 255.255.255.255 On-link 192.168.2.37 281 =========================================================================== Persistent Routes: None`

        1. The routing table contains a loopback address.
        2. The routing table does not specify a default gateway address.
        3. The routing table does not specify a DNS server address.
        4. The routing table contains two different routes to the 224.0.0.0 network.

        Answer:

        B. To access the Internet, the workstation's routing table must include a default gateway entry, which would have a Network Destination value of 0.0.0.0. A workstation's routing table does not specify the address of a Domain Name System (DNS) server. The loopback and 224.0.0.0 multicast addresses are normal routing table entries.
127.    Ed has configured his workstation to use Internet Protocol Security (IPSec) encryption for network communications. Which of the following tools can he use to verify that his network traffic is encrypted?

        1. Multimeter
        2. Packet sniffer
        3. Port scanner
        4. Protocol analyzer
        5. IP scanner

        Answer:

        D. A protocol analyzer is a tool that enables a user to view the contents of packets captured from a network. In Ed's case, if IPSec is properly implemented, he should be able to see that the data in packets captured from his workstation is encrypted. A packet sniffer is a tool that captures packets for the purpose of traffic analysis but cannot view their contents. In practice, however, packet sniffer and protocol analyzer capabilities are usually integrated into a single tool. A port scanner examines a system, looking for open Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) ports, and a multimeter is a tool that reads voltages on electrical circuits. An Internet Protocol (IP) scanner queries the network for the IP addresses currently in use and gathers information about the devices using them. None of these tools can examine packet contents.
128.    Which of the following statements describes the difference between a packet sniffer and a protocol analyzer?

        1. A packet sniffer captures network traffic, and a protocol analyzer examines packet contents.
        2. A protocol analyzer captures network traffic, and a packet sniffer examines packet contents.
        3. A packet sniffer only captures the local workstation's traffic, whereas a protocol analyzer can capture all the traffic on the network.
        4. There is no difference. Packet sniffers and protocol analyzers perform the same functions.

        Answer:

        A. A packet sniffer is a tool that captures packets for the purpose of traffic analysis but cannot view their contents. A protocol analyzer is a tool that enables a user to view the contents of packets captured from a network. In practice, however, packet sniffer and protocol analyzer capabilities are often integrated into a single tool. Both tools can function in promiscuous mode to capture packets from an entire network.
129.    Ed has recently discovered a rogue Dynamic Host Configuration Protocol (DHCP) server on his network. After disabling the server, he now needs to terminate all of the rogue Internet Protocol (IP) address leases currently held by Windows DHCP clients on the network and have them request new leases from the authorized DHCP server. Which of the following commands must he use on each Windows client to do this? (Choose all that apply.)

        1. `ipconfig /dump`
        2. `ipconfig /renew`
        3. `ipconfig /lease`
        4. `ipconfig /discard`
        5. `ipconfig /release`

        Answer:

        B, E. The `ipconfig /release` command terminates the current DHCP address lease. Then, the `ipconfig /renew` command causes the client to begin the process of negotiating a new lease, this time with an authorized DHCP server. `dump`, `lease`, and `discard` are not valid `ipconfig` parameters.
130.    Ed is implementing a web server farm on his company's network and has created a screened subnet (or perimeter network) on which the web servers will be located. The screened subnet is using the network Internet Protocol (IP) address 192.168.99.0/24. He has also installed a router connecting the screened subnet to the internal network, which uses the 192.168.3.0/24 network address. The IP addresses of the router's interfaces are 192.168.3.100 and 192.168.99.1. Ed needs to access the web servers from his Windows workstation on the internal network, but right now, he cannot do so. Because he needs to have a different router specified as his default gateway, Ed decides to add a route for the screened subnet to his computer's routing table. Which of the following commands will create a routing table entry that enables Ed to access the screened subnet?

        1. `route add 192.168.3.0 MASK 255.255.255.0 192.168.3.100`
        2. `route add 192.168.99.1 MASK 255.255.255.0 192.168.3.0`
        3. `route add 192.168.3.100 MASK 255.255.255.0 192.168.99.0`
        4. `route add 192.168.99.0 MASK 255.255.255.0 192.168.3.100`

        Answer:

        D. The correct syntax for the Windows `route add` command is to specify the destination network address, followed by the subnet mask for the destination network, followed by the address of the router interface on the local network that provides access to the destination network. The other options do not specify the correct addresses in the syntax.
131.    Alice has recently created a new screened subnet (or perimeter network) for the company's web server cluster, along with a router to connect it to the internal network. When she is finished, she sends Ralph an email instructing him to run the following command on his Windows workstation so that he can access the servers on the screened subnet. What function does the IP address 192.168.87.226 perform in this command?

        `route add 192.168.46.0 MASK 255.255.255.0 192.168.87.226`

        1. 192.168.87.226 is the address of Ralph's workstation.
        2. 192.168.87.226 is the network address of the perimeter network.
        3. 192.168.87.226 is the address of one of the router's interfaces.
        4. 192.168.87.226 is the address of the web server cluster.

        Answer:

        C. The correct syntax for the Windows `route add` command is to specify the destination network address, followed by the subnet mask for the destination network, followed by the address of the router interface on the local network that provides access to the destination network. Therefore, 192.168.87.226 is the address of the router interface on the internal network, where Ralph's workstation is located.
132.    Which of the following processes scans multiple computers on a network for a particular open Transmission Control Protocol (TCP) or User Datagram Protocol (UDP) port?

        1. Port scanning
        2. War driving
        3. Port sweeping
        4. Bluejacking

        Answer:

        C. Port scanning identifies open ports on a single computer, whereas port sweeping scans multiple computers for a single open port. War driving and bluejacking are methods of attacking wireless networks.
133.    Which of the following statements about protocol analyzers is not true?

        1. To troubleshoot using a protocol analyzer, you must be familiar with the OSI model and the protocols that operate at each of its layers.
        2. Protocol analyzers can be a network security risk.
        3. Some network monitoring products are both analyzers and sniffers.
        4. All Windows operating systems include a protocol analyzer.

        Answer:

        D. A protocol analyzer captures frames and displays their contents, including the header fields created by the protocols at the various Open Systems Interconnection (OSI) model layers. To interpret the exchanges between the computers on the network, you must be familiar with the protocols and how they operate. Protocol analyzers are useful tools in the hands of experienced network administrators, but they can also be used for malicious purposes, such as displaying unencrypted passwords and other confidential information in the captured packets. The difference between analyzers and sniffers is that analyzers read the internal contents of the packets they capture, parse the individual data units, and display information about each of the protocols involved in the creation of the packet, while sniffers look for trends and patterns in the network traffic without examining the contents of each packet.
134.    Which of the following utilities can be classified as port scanners? (Choose all that apply.)

        1. Nmap
        2. Nessus
        3. Network Monitor
        4. Performance Monitor

        Answer:

        A, B. nmap is a command-line utility that scans a range of IP addresses, runs a series of scripts against each device it finds, and displays a list of the open ports it finds on each one. Nessus is similar to `nmap` in that it also scans a range of IP addresses to find open ports, but it then proceeds to mount attacks against those ports, to ascertain their vulnerability. Network Monitor is a protocol analyzer or packet sniffer, which is a program that captures network traffic samples and analyzes them. It is not a port scanner. Performance Monitor is a program that displays statistics for specific system and network performance criteria. It is not a port scanner.
135.    Which Unix/Linux performance monitoring tool, with output shown in the figure, enables you to display information about processes that are currently running on a system?

        Larger View

        <figure><img src="https://cdn2.percipio.com/1713089107.3d40f2b6ad6609b2e2b85a64373a6494f4c71afd/eod/books/158796/images/c05uf009_0.jpg?width=836" alt=""><figcaption></figcaption></figure>

        1. `monitor`
        2. `top`
        3. `netstat`
        4. `cpustat`

        Answer:

        B. The `top` utility displays performance information about the currently running processes on a Unix/Linux system. `netstat` is a tool that enables you to view active network connections and Transmission Control Protocol/Internet Protocol (TCP/IP) traffic statistics. It does not measure system performance. There is no Unix or Linux tool called `monitor` or `cpustat`.
136.    You have finished capturing traffic with a protocol analyzer. The analyzer reports that 2000 frames have been seen, but only 1500 frames have been accepted. What does this mean?

        1. 2000 frames have passed the display filter, but only 1500 meet the criteria for display.
        2. Only 1500 frames have passed the capture filter and are currently being held in the buffer.
        3. You lost 500 frames and need to start over—something is obviously wrong.
        4. 500 frames were damaged and never made it into the buffer.

        Answer:

        B. Protocol analyzers report the total number of frames seen compared to the number of frames that were accepted. If a capture filter is in place, there will be a discrepancy between these two values. Only frames that meet the capture criteria will be accepted by the analyzer and placed in the buffer for later display. Protocol analyzers place good and bad frames into the buffer as long as they meet the capture criteria. If only good frames were placed in the buffer, there would be no way to identify problems.
137.    When you run a port scanner on a server, which of the following is the result?

        1. A list of processes running on the system
        2. A list of open ports through which the system can be accessed
        3. A list of protocols used by the system for network communication
        4. A list of Internet Protocol (IP) addresses used on the network

        Answer:

        B. A port scanner examines a system for open endpoints, accessible using the Transmission Control Protocol (TCP) or User Datagram Protocol (UDP), which intruders can conceivably use to gain access to the system from the network.
138.    A port scanner examines a system for network vulnerabilities at which layer of the Open Systems Interconnection (OSI) model?

        1. Application
        2. Transport
        3. Network
        4. Data Link

        Answer:

        B. A port is a numbered service endpoint identifying an application running on a Transmission Control Protocol/Internet Protocol (TCP/IP) system. A port scanner examines a system for open endpoints, accessible using the TCP or User Datagram Protocol (UDP) at the transport layer, which intruders can conceivably use to gain access to the system from the network.
139.    Which of the following best describes the primary function of a port scanner?

        1. A port scanner examines a computer' hardware and compiles a list of the physical ports in the system.
        2. A port scanner examines a computer for TCP and UDP endpoints that are accessible from the network.
        3. A port scanner examines a specified range of IP addresses on a network, to determine whether they are in use.
        4. A port scanner accepts a computer name as input and scans the network for the IP address associated with that name.

        Answer:

        B. The ports that a port scanner examines are the system endpoints identified by port numbers in Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) headers. An open port provides network access to an application running on the computer, which can conceivably be exploited by an intruder.
140.    Programs such as File Transfer Protocol (FTP) and Telnet are widely criticized because they transmit all data as clear text, including usernames and passwords. Which of the following types of tools might unscrupulous individuals use to read those passwords?

        1. Packet sniffer
        2. Terminal emulator
        3. Packet analyzer
        4. Vulnerability scanner
        5. TFTP server

        Answer:

        C. A packet analyzer is capable of looking at the data inside packets, which in the case of packets generated by Telnet and FTP, can contain passwords in clear text. Packet sniffers analyzer traffic patterns, vulnerability scanners search for open ports, and Trivial File Transfer Protocol (TFTP) servers transfer boot files to Dynamic Host Configuration Protocol (DHCP) client workstations. Telnet is itself a terminal emulator and does not display packet contents.
141.    Which of the following best states the potential security threat inherent in running a protocol analyzer?

        1. A protocol analyzer can display the application data in packets captured from the network.
        2. A protocol analyzer can display the IP addresses of the systems on the network.
        3. A protocol analyzer can decrypt protected information in packets captured from the network.
        4. A protocol analyzer can detect open ports on network systems and launch attacks against them.

        Answer:

        A. Protocol analyzers capture packets from the network and interpret their contents including the display of the application layer payload, which can include confidential information. Protocol analyzers can display the Internet Protocol (IP) addresses of systems on the network, but this is not as great a security threat. Protocol analyzers cannot decrypt the protected information it finds in captured packets. Vulnerability scanners detect open ports and launch attacks against them; protocol analyzers do not do this.
142.    Which of the following is not a tool that provides vulnerability scanning capabilities?

        1. Nessus
        2. MAP Toolkit
        3. Nmap
        4. MBSA

        Answer:

        B. Microsoft Assessment and Planning Toolkit (MAP Toolkit) is a free application that performs an agentless inventory of a network and uses the information to create reports on specific scenarios, such as whether computers are prepared for an operating system upgrade. Nessus, Nmap, and Microsoft Baseline Security Analyzer (MBSA) are all tools that include vulnerability scanning but that have other capabilities as well.
143.    Which of the following is a function typically classified as vulnerability scanning?

        1. Network mapping
        2. Remediation
        3. Penetration testing
        4. Port scanning

        Answer:

        D. Port scanning, the process of looking for open Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) ports that are exploitable by attackers, is one of the many functions that qualifies as a type of vulnerability scanning. Network mapping, the remediation of vulnerabilities, and penetration testing, which is the process of deliberately performing a planned attack, are not considered vulnerability scanning techniques.
144.    Alice is attempting to troubleshoot a communication problem between two hosts on the same network. She decides to use a protocol analyzer to capture traffic on the network. After finishing the capture, Alice notices that there are over 15,000 frames in the protocol analyzer's capture buffer. She is having a difficult time identifying the frames that relate to the problem because there are so many in the buffer. She wants to eliminate the extraneous frames from her view, enabling her to view only the frames transmitted by these two hosts. What does Alice have to do to accomplish this?

        1. Configure a display filter
        2. Configure a capture filter
        3. Delete the extraneous frames from the buffer
        4. Configure a capture and display filter

        Answer:

        A. Once the frames are in the buffer, Alice can configure a display filter to block the unwanted frames from view. This does not delete them from the buffer. Since the capture was already performed, there is no need to restart the capture. Configuring a capture filter will not meet the requirements, because the filter will eliminate the other frames completely from the buffer. It is not possible to delete specific frames from an analyzer buffer.
145.    Ralph has purchased some old 802.11b wireless networking equipment at a garage sale, which he plans to use to build a home network. When he installs the network adapters in his computers and sets up the Access Point (AP), he finds that the connections between the devices are no faster than 11 Mbps. What can Ralph do to improve the performance of his network?

        1. Nothing. The network is functioning at its top speed.
        2. Change the channel used by the devices.
        3. Move the computers closer to the AP.
        4. Install a larger antenna on the AP

        Answer:

        A. The 802.11b standard calls for a maximum speed of 11 Mbps, so there is nothing that Ralph can do to increase his network's speed except purchase new equipment.
146.    Ralph is setting up a wireless network using the 2.4 GHz band. Which of the following channels should he use to avoid channel overlap? (Choose all that apply.)

        1. 1
        2. 4
        3. 6
        4. 8
        5. 11

        Answer:

        A, C, E. The 2.4 GHz band used by Wireless Local Area Networks (WLANs) consists of channels that are 20 (or 22) MHz wide. However, the channels are only 5 MHz apart, so there is channel overlap that can result in interference. Channels 1, 6, and 11 are the only channels that are far enough apart from each other to avoid any overlap with the adjacent channels. Channels 4 and 8 are susceptible to overlap.
147.    Ralph is adding new workstations to his wireless network, which uses an Access Point (AP) that is configured to use WiFi Protected Access II (WPA2) encryption. However, after configuring the wireless network adapter on the first workstation, Ralph finds that it is not connecting to the network. The AP is listed on the Available Networks display, and there are no error messages or indications of a problem, just a failure to connect. Which of the following is most likely to be the problem?

        1. Incorrect passphrase
        2. Channel overlap
        3. Incorrect SSID
        4. Incorrect antenna placement

        Answer:

        A. Specifying the wrong passphrase for the encryption protocol is the most common cause of a failure to connect to the network with no indication of an error. Incorrect antenna placement and channel overlap could result in a weak signal or no signal, either of which would be indicated in the Available Networks list. An incorrect Service Set Identifier (SSID) is not likely to be the error, as long as Ralph selected the AP from the list.
148.    Ralph is adding new workstations to his wireless network, which uses an Access Point (AP) that is configured to use WiFi Protected Access II (WPA2) encryption. However, after installing the wireless network adapter on the first workstation, Ralph finds that he cannot see the Wireless Access Point (WAP) on the Available Networks display. Which of the following could be the problem? (Choose all that apply.)

        1. Incorrect passphrase
        2. Channel overlap
        3. Incorrect SSID
        4. Incorrect antenna polarization
        5. Antenna cable attenuation

        Answer:

        B, D, E. Interference resulting from channel overlap, a weak signal due to incorrect antenna polarization, and signal loss due to antenna cable attenuation could render the workstation unable to make contact with the AP. An incorrect passphrase would not be the problem unless Ralph had already seen the AP and attempted to connect to it. An incorrect Service Set Identifier (SSID) would be the problem only if Ralph had already attempted to manually enter an SSID.
149.    Ralph is the administrator of a small company's wireless network. He has recently discovered evidence that users outside of the company's office space have been accessing its wireless network. The office is located in a narrow space against the building's outside wall. Ralph is concerned that the network's Wireless Access Point (WAP) is extending coverage outside the building. Speaking with a consultant friend of his, Ralph is advised to install a different type of antenna on his Access Point (AP). Which of the following antenna types would most likely help Ralph to alleviate the problem?

        1. Dipole
        2. Yagi
        3. Patch
        4. Unidirectional

        Answer:

        C. A patch antenna is a flat device that transmits signals in a half-spherical pattern. By placing the antenna against the building's outer wall, Ralph can provide coverage inside the building and minimize coverage extending to the outside. A dipole antenna is another name for the omnidirectional antenna usually provided with an AP. A unidirectional antenna directs signals in a straight line, which would not provide the coverage Ralph needs. A Yagi antenna is a type of unidirectional antenna.
150.    Trixie has recently moved to a new office in her company's building, down the hall from her old one. Since the move, she has only been able to access the wireless network with her laptop intermittently. She never had a problem in her previous location. Which of the following could possibly be the cause of her problem? (Choose all that apply.)

        1. Trixie's new office is farther from the Access Point (AP) than her old one.
        2. Her laptop is connecting to the wrong SSID.
        3. The AP is using an omnidirectional antenna.
        4. There are too many walls between Trixie's new office and the AP.

        Answer:

        A, D. Greater distance from the AP or interference from intervening walls can both cause a weakening of wireless signals, resulting in the intermittent connectivity that Trixie is experiencing. An incorrect Service Set Identifier (SSID) would prevent Trixie's laptop from ever connecting to the network. An omnidirectional antenna generates signals in every direction, which would not account for Trixie's problem.
151.    Alice is a new hire at Adatum Corp., and when she asks about wireless network access for her laptop, she is given a Service Set Identifier (SSID) and a WiFi Protected Access II (WPA2) passphrase. Later, in the lunchroom, when she tries to connect her laptop to the network, she cannot see the SSID she was given in the Available Networks list, although she can see other networks. What should Alice do next to try to resolve the problem?

        1. Type in the WPA2 passphrase.
        2. Type the SSID in manually.
        3. Move closer to the Wireless Access Point (WAP).
        4. Move away from the microwave in the lunchroom.

        Answer:

        B. It is possible that the WAP has been configured to not broadcast the network's SSID as a security measure, so Alice should first attempt to access it by typing the SSID in manually. She would not be able to type in the WPA2 passphrase until she is connecting to the SSID. Moving the laptop closer to the WAP or away from possible sources of electromagnetic interference might be solutions to the problem, but they should not be the first thing Alice tries.
152.    Alice is a new hire at Adatum Corp., and when she asks about wireless network access for her laptop, she is given a Service Set Identifier (SSID) and a passphrase. She is also told that she must add the SSID manually. Later, she types in the SSID she was given, and the computer prompts her to select a security type. Not knowing which option to choose, she selects 802.1x, because it sounds as though it should be the most secure. However, this option does not enable her to enter her passphrase, so she selects another option, WEP, and is able to type in the passphrase. However, her laptop says she “Can't connect to this network.” Which of the following is the most likely cause of Alice's problem?

        1. Overcapacity
        2. Distance limitations
        3. Frequency mismatch
        4. Encryption protocol mismatch

        Answer:

        D. The most likely cause of Alice's problem is that she has selected an incorrect encryption protocol. Wired Equivalent Privacy (WEP) is still provided as an option on many wireless devices, but it has long since been found to be insecure and is almost never used. Alice should try selecting the other security types that enable her to enter her passphrase, such as WiFi Protected Access II (WPA2). Although the other options are possible causes of the problem, encryption protocol mismatch is the most likely cause.
153.    Ralph purchases some 802.11a wireless network adapters for desktop computers at a yard sale, which he intends to use on his 802.11g home network. He installs one of the adapters in a computer and attempts to connect it to the network, but he cannot see his Service Set Identifier (SSID). He tries a different adapter, thinking the first one might be broken, but that one does not work either. What can Ralph do to resolve the problem and connect the computer to his network?

        1. Move the computer closer to the Access Point (AP).
        2. Configure the AP to use the 5 GHz frequency.
        3. Manually enter the SSID in the computer's client software.
        4. Nothing. 802.11a equipment cannot connect to an 802.11g network.

        Answer:

        D. Wireless Local Area Network (WLAN) equipment built to the 802.11a standard can only use the 5 GHz frequency. However, an 802.11g AP can only use the 2.4 GHz frequency. Therefore, the network adapters cannot connect to Ralph's AP.
154.    Ralph is responsible for a Wireless Local Area Network (WLAN) that consists of an 802.11n 2x2:2 Access Point (AP) and laptop computers with a variety of network adapters. Some of the laptops support 802.11n, most support 802.11g, and a few older models have 802.11a adapters. The WLAN is located in a large office building with many other wireless networks, and Ralph is having trouble finding a channel on the 2.4 GHz band that is not congested with traffic. Scanning the 5 GHz band, he finds relatively little traffic, so he reconfigures the AP to use a 5 GHz channel. The result is that some of the laptops are able to connect to the network, whereas others are not. What is the most likely reason for the connection failures, and what must Ralph do to enable all of the laptops to connect to the wireless network?

        1. The 5 GHz band does not support automatic channel selection. Ralph must configure each laptop to use the same channel as the AP for all the laptops to connect successfully.
        2. The 802.11g standard does not support communication using the 5 GHz band. Ralph must configure the AP to support 2.4 GHz for all the laptops to connect successfully.
        3. The 5 GHz band does not support Multiple Input, Multiple Output (MIMO) communications, so the 802.11n laptops are unable to connect to the network. Ralph must replace the AP with an 802.11g unit for all the laptops to connect successfully.
        4. The 802.11a standard does not support communication using the 5 GHz band. Ralph must replace the network adapters in those laptops with newer models for them to connect successfully.

        Answer:

        B. The 802.11b and 802.11g standards do not support 5 GHz communications. Configuring the AP to support 2.4 GHz is the only way for the 802.11g computers to connect to the network. The 5 GHz band does support automatic channel selection, so there is no need to configure the channel on each laptop manually. The 5 GHz band does support MIMO, and the 802.11n laptops should be able to connect. Replacing the adapters with 802.11g will prevent them from connecting, as that standard does not support 5 GHz communications. The 802.11a standard does support the 5 GHz band, and those laptops should be able to connect.
155.    Alice is the administrator of a wireless network that has client computers in a number of small offices, all located on the same floor of an office building built in the mid-twentieth century. The network has an IEEE 802.11g Access Point (AP) located at the approximate center of the floor. Workstations in most of the rooms connect to the network at 54 Mbps, but the computers in one particular room rarely connect at speeds above 11 Mbps. Which of the following might be the cause of the problem?

        1. The computers in the problematic room are configured to use a different wireless encryption protocol than the AP.
        2. The computers in the problematic room are experiencing an SSID mismatch.
        3. The network adapters in the problematic computers support IEEE 802.11a, not 802.11g.
        4. The RSSI of the problematic computers might be low, due to excessive distance from the AP.

        Answer:

        D. As wireless computers move farther away from the AP, their signals attenuate (weaken), their Received Signal Strength Indicators (RSSIs) go down, and the maximum speed of their connections drops. If the computers were using a different encryption protocol than the AP, there would be no connection at all, not a diminished connection speed. A SSID mismatch would cause the computers to connect to a different network, not necessarily connect at a slower speed. If the computers had 802.11a adapters, they would fail to connect to the AP at all, because 802.11a requires the use of the 5 GHz frequency band, and 802.11g uses 2.4 GHz.
156.    Which of the following is not a potential solution for an IEEE 802.11g wireless computer that has intermittent problems connecting to an IEEE 802.11b/g Access Point (AP)?

        1. Install a higher gain antenna on the AP
        2. Replace the AP with a model that supports 802.11n
        3. Move the computer closer to the AP
        4. Change the channel used by the AP

        Answer:

        B. Replacing the AP with an 802.11n model is not going to have any effect at all unless you upgrade the computer's network adapter as well. Installing a higher gain antenna on the AP can improve its range, enabling the computer to connect more readily. Moving the computer closer to the AP can strengthen the signal and raise its Received Signal Strength Indicator (RSSI), enabling it to connect more reliably. Changing the channel on the AP to a lesser used one can enable the computer to connect more easily.
157.    Ed has installed a separate 802.11n wireless network for guest users working in his company's offices. The guest network is unsecured, and Ed has recently become aware that people outside the building are able to access it. It is not possible to move the Access Point (AP), and it must run at maximum power to reach the entire building. Which of the following is the most convenient way to prevent users outside the building from accessing the guest network while leaving it available to users inside the building?

        1. Change the passphrase daily
        2. Switch the network frequency
        3. Disable SSID broadcasting
        4. Implement MAC filtering

        Answer:

        C. Disabling Service Set Identifier (SSID) broadcasts will not defeat dedicated attackers, but it can prevent casual intruders from accessing the network. Media Access Control (MAC) filtering would require Ed to configure the AP with the MAC addresses of all devices that will access the network, which would be impractical in this case. The network is unsecured, so there is no passphrase to change, and a frequency change will have no effect on the problem.
158.    Alice is trying to provide users in a warehouse with wireless network connectivity for their tablets. The warehouse is a huge concrete structure with many internal cinderblock walls. Which of the following types of signal interference are inhibiting Alice's efforts?

        1. Refraction
        2. Reflection
        3. Diffraction
        4. Absorption

        Answer:

        D. Absorption is a type of interference that occurs when radio signals have to pass through barriers made of dense materials, such as concrete or cinderblock walls. The density of the material's molecular structure causes the radio signals to be partially converted to heat, which weakens them. Reflection is when signals bounce off of certain surfaces, such as metal. Refraction is when signals bend as they pass through certain barriers, such as glass or water. Diffraction is when signals have to pass around barriers to reach a particular destination. All of these phenomena can weaken the radio signals used in wireless networking, but absorption is the primary problem for Alice in this case.
159.    Ralph is having trouble providing satisfactory wireless network performance to some executive offices at the far end of the building. The wireless Access Point (AP) is based on the 802.11g standard. The offices have heavy doors and insulated walls for sound dampening, and the occupants typically leave their doors closed during work hours. Which of the following actions can Ralph take to provide the users in these offices with better wireless network performance?

        1. Install an additional AP nearer to the offices.
        2. Modify the AP to use higher number channels.
        3. Upgrade the AP to a model based on the 802.11n standard.
        4. Configure the AP to disable SSID broadcasting.

        Answer:

        A. The closer the users are to the AP, the stronger the signals will be. Installing an additional AP nearer to the executive offices will likely enable the signals to pass through the barriers more efficiently. The channel used by the AP, the standard on which the AP is based, and the broadcasting of Service Set Identifier (SSID) signals have no effect on the strength of the signals reaching the executive offices and will not resolve Ralph's problem.
160.    Ralph is having trouble providing satisfactory wireless network performance to some executive offices at the far end of the building. The offices have heavy doors and insulated walls for sound dampening, and the occupants typically leave their doors closed during work hours. Which of the following types of radio signal interference is Ralph trying to overcome?

        1. Reflection
        2. Refraction
        3. Diffraction
        4. Absorption

        Answer:

        D. Absorption is a type of interference that occurs when radio signals have to pass through barriers made of dense materials, such as walls and doors. In this case, the construction of the barriers has made them more formidable. Reflection is when signals bounce off of certain surfaces, such as metal. Refraction is when signals bend as they pass through certain barriers, such as glass or water. Diffraction is when signals have to pass around barriers to reach a particular destination. All of these phenomena can weaken the radio signals used in wireless networking, but absorption is the primary problem for Ralph in this case.
161.    Ralph is having trouble providing satisfactory wireless network performance to a row of glass-walled conference rooms at the far end of the building. The doors to the conference rooms are also made of glass and are always closed when meetings are in progress. Which of the following types of radio signal interference are likely to be the main issues that Ralph is trying to overcome? (Choose all that apply.)

        1. Reflection
        2. Refraction
        3. Diffraction
        4. Attenuation

        Answer:

        B, D. Attenuation is the tendency of signals to weaken as they travel through a network medium. In the case of a wireless network, the medium is the air, and the farther away a wireless device is from the Access Point (AP), the weaker the signal will be. Refraction is when signals bend as they pass through certain types of barriers, such as the glass walls of conference rooms. The bending changes the direction of the signals, possibly causing them to weaken in the process. Reflection is when signals bounce off of certain surfaces, such as metal. Diffraction is when signals have to pass around barriers to reach a particular destination. All of these phenomena can weaken the radio signals used in wireless networking, but attenuation and refraction are likely to be the primary problems for Ralph in this case.
162.    Alice receives a call from a user who cannot connect to the company's 802.11g wireless network with a new laptop that has an 802.11ac network adapter. Other users working in the same area are able to connect to the network without difficulty. Which of the following are tasks that Alice can perform to resolve the problem? (Choose all that apply.)

        1. Install an 802.11ac wireless Access Point (AP) on the network
        2. Change the channel used by the Wireless Access Point (WAP)
        3. Install an 802.11g wireless network adapter in the user's laptop
        4. Move the user closer to the WAP

        Answer:

        A, C. The 802.11ac and 802.11g wireless networking standards are fundamentally incompatible. The 802.11g AP uses the 2.4 GHz band, and the user's 802.11ac laptop uses the 5 GHz band. Therefore, the only possible solutions are to install an 802.11ac AP or an 802.11g network adapter. Changing channels on the WAP and moving the user will have no effect on the problem.
163.    Several accounting consultants are working in Ed's office for the first time, and they are unable to connect to the 802.11g wireless network with their laptops. They are selecting the correct Service Set Identifier (SSID) from the Available Networks list, but they cannot connect, and there are no error messages of any kind. Which of the following tasks should Ed perform to try to resolve the problem?

        1. Check the network adapters in the laptops for channel overlap
        2. Change the frequency used by the Wireless Access Point (WAP) from 2.4 GHz to 5 GHz
        3. Examine the area where the consultants are working for possible sources of signal interference
        4. Make sure that the consultants' laptops are configured to use the correct wireless security protocol

        Answer:

        D. The use of an incorrect wireless security protocol is a well-known source of errorless connection failures, so checking this will most likely enable Ed to locate the source of the problem. Channel overlap is a problem that Ed would check and resolve at the Access Point (AP), not the users' workstations. It is not possible to change the frequency on the WAP because the 802.11g standard only supports the 2.4 GHz frequency. Although signal interference could conceivably be the cause for a connection failure, the users can see the network, so this is probably not the problem.
164.    Ed has installed a separate 802.11n wireless network for guest users working in his company's offices. The guest network uses no security protocol, and Ed has recently become aware that people outside the building are able to access it. Which of the following steps can Ed take to prevent users outside the building from accessing the guest network, while leaving it available to users inside the building? (Choose all that apply.)

        1. Move the Wireless Access Point (WAP) to the center of the building
        2. Lower the power level of the WAP
        3. Disable Service Set Identifier (SSID) broadcasting
        4. Implement Media Access Control (MAC) filtering
        5. Install a captive portal

        Answer:

        A, B, C. Moving the Wireless Access Point (WAP) to the center of the building will keep as much of its operational range inside the structure as possible. If the signals still reach outside the building, Ed can reduce the power level of the WAP until the network is only accessible inside. Disabling SSID broadcasts will not defeat dedicated attackers, but it can prevent casual intruders from accessing the network. MAC filtering would require Ed to configure the WAP with the MAC addresses of all devices that will access the network, which would be impractical in this case. Installing a captive portal would not block outside users unless Ed configures the portal to require user authentication, which defeats the purpose of the guest network.
165.    Alice receives a call from a user who cannot connect to the company's 802.11n wireless network with a laptop that has an 802.11g network adapter. Other users working in the same area are able to connect to the network without difficulty. Which of the following steps should Alice take first to try to resolve the problem? (Choose all that apply.)

        1. Change the channel used by the Wireless Access Point (WAP)
        2. Check whether the user is connecting to the correct Service Set Identifier (SSID)
        3. Check whether the wireless adapter in the user's laptop is enabled
        4. Provide the user with an 802.11n wireless network adapter

        Answer:

        B, C. The first steps Alice should take are the simplest ones: make sure that the wireless interface in the user's laptop is turned on and that she is attempting to connect to the correct SSID for the company network. Changing the channel would not be necessary unless other users in the area are also having problems due to interference. The 802.11n wireless networking standard is backward compatible with 802.11g, so it should not be necessary to provide the user with a new network adapter.
166.    Users on Ed's 802.11n wireless network are dropping their connections intermittently. Which of the following might help to resolve the problem?

        1. Restart the Wireless Access Point (WAP)
        2. Change the network's Service Set Identifier (SSID)
        3. Change the channel the devices are using
        4. Change the wireless security protocol

        Answer:

        C. If the users are losing their connections due to interference from other types of devices, changing the channel alters the frequency the network uses and can enable it to avoid the interference. The other options are not likely to affect any condition that would cause users to drop their connections.
167.    Several accounting consultants are working in Ed's office for the first time, and they are unable to connect to the 802.11n wireless network with their laptops. Which of the following tasks should Ed perform first to try to resolve the problem? (Choose all that apply.)

        1. Check the network adapters in the laptops for channel overlap
        2. Make sure that the consultants are attempting to connect to the correct SSID
        3. Examine the area where the consultants are working for possible sources of signal interference
        4. Make sure that the consultants' laptops are configured to use the correct wireless encryption protocol

        Answer:

        B, D. Of the options provided, the ones most likely to be causing the problem are the use of an incorrect Service Set Identifier (SSID) or encryption protocol. Although signal interference could possibly be a cause, it is more likely that the new users have devices that are incorrectly configured for Ed's network. Channel overlap is a problem that Ed would check and resolve at the Access Point (AP), not the users' workstations.
168.    Ralph is deploying an 802.11n wireless network for a client that calls for the best possible security without deploying additional servers. When setting up the Wireless Access Point (WAP), Ralph disables Service Set Identifier (SSID) broadcasts, selects WiFi Protected Access security with Pre-Shared Keys (WPA-PSKs), and configures Media Access Control (MAC) address filtering. Which of the following statements about the security of this arrangement is true?

        1. The configuration is as secure as Ralph can make it with the specified equipment.
        2. Ralph should not disable SSID broadcasts since this prevents users from connecting to the network.
        3. Ralph should not use MAC address filtering, because it exposes MAC addresses to possible attacks.
        4. Ralph should use WiFi Protected Access II (WPA2) instead of WPA, because it is more resistant to certain types of attacks.

        Answer:

        D. WPA has been found to be vulnerable, and WPA2 was designed to address those vulnerabilities, so Ralph should use WPA2 instead of WPA. Suppressing SSID broadcasts does not prevent users from connecting to the network, and MAC filtering strengthens security without exposing MAC addresses to undue risk.
169.    Ralph is experiencing long Access Point (AP) association times and generally poor performance on his home 802.11n wireless network. Ralph lives in a large apartment complex, and when he runs a WiFi analyzer, he sees many other nearby networks using the often-recommended channels 1, 6, and 11 on the 2.4 GHz frequency. Using the 5 GHz frequency is not an option for Ralph's equipment. What should Ralph do to improve his network performance?

        1. Configure his equipment to use channel 2
        2. Configure his equipment to use channel 5
        3. Configure his equipment to use channel 9
        4. Configure his equipment to use channel 10

        Answer:

        C. The 2.4 GHz band used by Wireless Local Area Networks (WLANs) consists of channels that are 20 (or 22) MHz wide. However, the channels are only 5 MHz apart, so there is channel overlap that can result in interference, possibly causing long AP association times and degraded performance. Channels 1, 6, and 11 are the only channels that are far enough apart from each other to avoid any overlap with the adjacent channels. This is why they are often recommended. However, in Ralph's case, these channels are too crowded with other networks. Ralph should therefore use a channel that is as far as possible from the crowded ones. Channels 2, 5, and 10 are all immediately adjacent to a crowded channel, but channel 9 is at least two channels away from the nearest crowded channel. Therefore, Ralph should configure his equipment to use channel 9.
170.    Which of the following is a power measurement of a specific transmitter and antenna combination, as used in a wireless access point?

        1. RSSI
        2. EIRP
        3. SSID
        4. MIMO

        Answer:

        B. Effective Isotropic Radiated Power (EIRP) is a measurement of the signal strength generated by an access point (or other radio transceiver) with a particular antenna. Received Signal Strength Indicator (RSSI) is a measurement of the strength of the signal received by a device from an access point. Service Set Identifier (SSID) is a designation assigned to a specific wireless network, which appears in the Available Networks list of a WiFi client. Multiple Input, Multiple Output (MIMO) is a technology used by some IEEE wireless networking standards to increase throughput by using multiple antennae.
171.    Ed is working the help desk at a local computer store, and he receives a call from a customer trying to set up a home network using Windows 10 and wired Ethernet equipment. The customer reports that, from her computer, she can see the two other computers in the house, but she cannot access the Internet. Ed asks her to run the `ipconfig /all` command and read the results to him. She says that her IP address is 172.16.41.2, her subnet mask is 255.255.255.0, and her default gateway is 172.16.43.1. Which of the following is most likely the cause of the customer's problem?

        1. The customer's network cable is unplugged.
        2. The customer has an incorrect subnet mask.
        3. The customer has an incorrect default gateway address.
        4. The computer's DNS record contains the wrong information.
        5. The computer is inhibited by a switching loop.

        Answer:

        C. Because the customer can access the other two computers in the house, Ed knows that her Internet Protocol (IP) address and subnet mask are properly configured, that the network cable is plugged in and functional, and that a switching loop is not preventing access to the Internet. Ed also knows that the computer's Domain Name System (DNS) record does not play a role in outgoing connections. The problem is most likely in the default gateway because the gateway address the customer specified is on another network, 172.16.43.0, rather than on her own network, 172.16.41.0.
172.    Ralph has a wired home network with three Windows computers, a switch, and a cable modem/router that provides access to the Internet. All three computers are able to access the Internet, but none of them can access filesystem shares on the others. Which of the following is the most likely cause of the problem on the three network computers?

        1. Incorrect IP addresses
        2. Incorrect subnet mask
        3. Incorrect default gateway address
        4. Incorrect ACL settings

        Answer:

        D. The problem is most likely incorrect Access Control List (ACL) settings. Because the computers are all able to access the Internet, their Transmission Control Protocol/Internet Protocol (TCP/IP) settings, including their IP addresses, subnet mask, and default gateway address, must be correct. However, if the users do not have the correct permissions in the ACLs of the filesystem shares, they will not be able to access the shares over the network.
173.    Alice has been asked to update an accounts receivable spreadsheet with information about the day's incoming payments, a task she has never performed before. After locating and opening the spreadsheet on the network server, she types in her new information, but when she attempts to save the changes, she receives an error message that directs her to save the file on her local drive instead of the network server. Which of the following is the probable cause of the problem?

        1. Blocked Transmission Control Protocol/User Datagram Protocol (TCP/UDP) ports
        2. Incorrect filesystem Access Control List (ACL) settings
        3. Incorrect firewall settings
        4. Untrusted Secure Sockets Layer (SSL) certificate

        Answer:

        B. Because Alice is able to access the server and open the spreadsheet file, the problem is not related to blocked ports, firewall settings, or an untrusted certificate. The problem is most likely that though she has the necessary filesystem ACL permissions to open and read the file, she does not have the permissions needed to modify it.
174.    Which of the following Internet Protocol (IP) address assignments indicates that a computer has been unable to communicate with a Dynamic Host Configuration Protocol (DHCP) server?

        1. 127.0.0.1
        2. 255.255.255.0
        3. 240.15.167.251
        4. 169.254.199.22

        Answer:

        D. The address 169.254.199.22 is from the 169.254.0.0/16 network address assigned to Automatic Private Internet Protocol Addressing (APIPA), a standard for the assignment of IP addresses to DHCP clients when they cannot obtain an address from a DHCP server. 127.0.0.1 is the standard IP loopback address. 240.15.167.251 is from the 240.0.0.0 network address, which is reserved for experimental use. Neither of these is ever assigned by DHCP. 255.255.255.0 is not an IP address at all; it is a subnet mask.
175.    A user reports to Ralph that he cannot access the Internet, although he is able to connect to computers on the local network. Ralph runs `ipconfig /all` on the user's workstation and examines the output. Which of the following is the most likely explanation for the user's problem, based on these `ipconfig` results?

        `Windows IP Configuration Host Name . . . . . . . . . . . . : Client12 Primary Dns Suffix . . . . . . . : Node Type . . . . . . . . . . . . : Hybrid IP Routing Enabled. . . . . . . . : No WINS Proxy Enabled. . . . . . . . : No Ethernet adapter Local Area Connection: Connection-specific DNS Suffix . : Description . . . . . . . . . . . : PCIe Family Controller Physical Address. . . . . . . . . : 60-EB-69-93-5E-E5 DHCP Enabled. . . . . . . . . . . : No Autoconfiguration Enabled . . . . : Yes Link-local IPv6 Address . . . . . : fe80::c955:c944:acdd:3fcb%2 IPv4 Address. . . . . . . . . . . : 192.168.4.24 Subnet Mask . . . . . . . . . . . : 255.255.255.0 Lease Obtained. . . . . . . . . . : Monday, October 23, 2017 6:23:47 PM Lease Expires . . . . . . . . . . : Saturday, November 18, 2017 9:49:24 PM Default Gateway . . . . . . . . . : 192.168.6.99 DHCPv6 IAID . . . . . . . . . . . : 241232745 DHCPv6 Client DUID. . . . . . . . : 00-01-00-01-18-10-22-0D-60-EB-69-93-5E-E5 DNS Servers . . . . . . . . . . . : 202.86.10.114 NetBIOS over Tcpip. . . . . . . . : Enabled`

        1. The Subnet Mask setting is incorrect.
        2. The Default Gateway setting is incorrect.
        3. The DNS Servers setting is located on another network.
        4. DHCP is not enabled.

        Answer:

        B. The Default Gateway setting should contain the address of a router on the local network that provides access to other networks, such as the Internet. In this case, therefore, the Default Gateway address should be on the 192.168.4.0 network, but it contains an address on the 192.18.6.0 network, which is not local. Therefore, the user can only access systems on the 192.168.4.0 network. The Subnet Mask setting must be correct, or the user would not be able to access any other systems. Unlike the default gateway, the Domain Name System (DNS) server does not have to be on the local network, so the address shown can be correct. Dynamic Host Configuration Protocol (DHCP) is not necessary to access the Internet.
176.    Ralph is troubleshooting a workstation that cannot access the network. The workstation is plugged into a wall plate that should provide it with access to a DHCP-equipped network using the 192.168.4.0/24 network address. No one else on that network is reporting a problem. Ralph checks that the patch cable is properly plugged into the workstation and the wall plate, which they are, and then runs `ipconfig /all` on the user's workstation and examines the output. Which of the following could be the explanation for the user's problem, based on these `ipconfig` results?

        `Windows IP Configuration Host Name . . . . . . . . . . . . : Client12 Primary Dns Suffix . . . . . . . : Node Type . . . . . . . . . . . . : Hybrid IP Routing Enabled. . . . . . . . : No WINS Proxy Enabled. . . . . . . . : No Ethernet adapter Local Area Connection: Connection-specific DNS Suffix . : Description . . . . . . . . . . . : PCIe Family Controller Physical Address. . . . . . . . . : 60-EB-69-93-5E-E5 DHCP Enabled. . . . . . . . . . . : Yes Autoconfiguration Enabled . . . . : Yes Link-local IPv6 Address . . . . . : fe80::c955:c944:acdd:3fcb%2 IPv4 Address. . . . . . . . . . . : 169.254.203.42 Subnet Mask . . . . . . . . . . . : 255.255.0.0 Lease Obtained. . . . . . . . . . : Monday, October 23, 2017 6:23:47 PM Lease Expires . . . . . . . . . . : Saturday, November 18, 2017 9:49:24 PM Default Gateway . . . . . . . . . : DHCPv6 IAID . . . . . . . . . . . : 241232745 DHCPv6 Client DUID. . . . . . . . : 00-01-00-01-18-10-22-0D-60-EB-69-93-5E-E5 DNS Servers . . . . . . . . . . . : fec0:0:0:ffff::1%1 fec0:0:0:ffff::2%1 fec0:0:0:ffff::3%1 NetBIOS over Tcpip. . . . . . . . : Enabled`

        1. The Subnet Mask is incorrect.
        2. The Default Gateway address is missing.
        3. The DHCPv4 scope is exhausted.
        4. The DNS server addresses are incorrect.

        Answer:

        C. The 169.254.203.42 address assigned to the workstation is from the 169.254.0.0/16 network address assigned to Automatic Private Internet Protocol Addressing (APIPA), a standard for the assignment of Internet Protocol (IP) addresses to Dynamic Host Configuration Protocol (DHCP) clients when they cannot obtain an address from a DHCP server. Since no one else is experiencing a problem, the DHCP server is presumably functioning. The Subnet Mask value is correct for an APIPA address, and APIPA does not provide Default Gateway or Domain Name System (DNS) server addresses. Therefore, an exhausted DHCP scope is the only one of the explanations provided that could be the cause of the problem.
177.    Ralph is troubleshooting a workstation that cannot access the network. The workstation is plugged into a wall plate that should provide it with access to a DHCP-equipped network using the 192.168.32.0/20 network address. Ralph checks that the patch cable is properly plugged into the workstation and the wall plate, which they are, and then runs `ipconfig /all` on the user's workstation and examines the output. Which of the following could be the explanation for the user's problem, based on these `ipconfig` results?

        `Windows IP Configuration Host Name . . . . . . . . . . . . : Client12 Primary Dns Suffix . . . . . . . : Node Type . . . . . . . . . . . . : Hybrid IP Routing Enabled. . . . . . . . : No WINS Proxy Enabled. . . . . . . . : No Ethernet adapter Local Area Connection: Connection-specific DNS Suffix . : Description . . . . . . . . . . . : PCIe Family Controller Physical Address. . . . . . . . . : 60-EB-69-93-5E-E5 DHCP Enabled. . . . . . . . . . . : No Autoconfiguration Enabled . . . . : Yes Link-local IPv6 Address . . . . . : fe80::c955:c944:acdd:3fcb%2 IPv4 Address. . . . . . . . . . . : 192.168.42.24 Subnet Mask . . . . . . . . . . . : 255.255.255.0 Lease Obtained. . . . . . . . . . : Monday, October 23, 2017 6:23:47 PM Lease Expires . . . . . . . . . . : Saturday, November 18, 2017 9:49:24 PM Default Gateway . . . . . . . . . : 192.168.42.99 DHCPv6 IAID . . . . . . . . . . . : 241232745 DHCPv6 Client DUID. . . . . . . . : 00-01-00-01-18-10-22-0D-60-EB-69-93-5E-E5 DNS Servers . . . . . . . . . . . : 202.86.10.114 NetBIOS over Tcpip. . . . . . . . : Enabled`

        1. The IPv4 Address setting is incorrect.
        2. The Subnet Mask setting is incorrect.
        3. The Default Gateway setting is incorrect.
        4. The DNS Servers setting is located on another network.

        Answer:

        B. For a computer connected to the 192.168.32.0/20 network, the Subnet Mask value should be 255.255.240.0, not 255.255.255.0, as shown in the `ipconfig` output. The IPv4 Address, Default Gateway, and Domain Name System (DNS) Servers settings are appropriate for the network. The workstation apparently has Dynamic Host Configuration Protocol (DHCP) disabled, so it has not retrieved appropriate Internet Protocol (IP) address settings from the DHCP server.
178.    Ralph is troubleshooting a workstation that cannot access the network. The workstation is plugged into a wall plate that should provide it with access to a DHCP-equipped network using the 192.168.4.0/24 network address. Ralph checks that the patch cable is properly plugged into the workstation and the wall plate, which they are, and then runs `ipconfig /all` on the user's workstation and examines the output. Which of the following could be the explanation for the user's problem, based on these `ipconfig` results?

        `Windows IP Configuration Host Name . . . . . . . . . . . . : Client12 Primary Dns Suffix . . . . . . . : Node Type . . . . . . . . . . . . : Hybrid IP Routing Enabled. . . . . . . . : No WINS Proxy Enabled. . . . . . . . : No Ethernet adapter Local Area Connection: Connection-specific DNS Suffix . : Description . . . . . . . . . . . : PCIe Family Controller Physical Address. . . . . . . . . : 60-EB-69-93-5E-E5 DHCP Enabled. . . . . . . . . . . : Yes Autoconfiguration Enabled . . . . : Yes Link-local IPv6 Address . . . . . : fe80::c955:c944:acdd:3fcb%2 IPv4 Address. . . . . . . . . . . : 10.124.16.8 Subnet Mask . . . . . . . . . . . : 255.0.0.0 Lease Obtained. . . . . . . . . . : Monday, October 23, 2017 6:23:47 PM Lease Expires . . . . . . . . . . . : Saturday, November 18, 2017 9:49:24 PM Default Gateway . . . . . . . . . : DHCPv6 IAID . . . . . . . . . . . : 241232745 DHCPv6 Client DUID. . . . . . . . . .: 00-01-00-01-18-10-22-0D-60-EB-69-93-5E-E5 DNS Servers . . . . . . . . . . . : fec0:0:0:ffff::1%1 fec0:0:0:ffff::2%1 fec0:0:0:ffff::3%1 NetBIOS over Tcpip. . . . . . . . : Enabled`

        1. The workstation could not connect to a DHCP server.
        2. There is a rogue DHCP server on the network.
        3. The workstation is not configured to use DHCP.
        4. The IP address assigned by the DHCP server has expired.

        Answer:

        B. The Dynamic Host Configuration Protocol (DHCP) client on the workstation is enabled, but the Internet Protocol (IP) address assigned to the workstation is not from the 192.168.4.0/24 network. The assigned address is not an Automatic Private Internet Protocol Addressing (APIPA) address, nor is it expired, so the only conclusion is that there is a rogue DHCP server on the network assigning addresses from a wholly different subnet.
179.    Ralph is responsible for the network installation in a new building purchased by his company, and he has elected to have Category 6 (Cat 6) Unshielded Twisted Pair (UTP) cable installed. The company president has asked him if it is possible to run their Gigabit Ethernet network using two of the wire pairs in the cable, while using the other two pairs for telephone connections. Ralph is not sure, so he sets up a lab network using cables with only two pairs connected. When he plugs computers into the switch and turns them on, the Light-Emitting Diodes (LEDs) labeled 1000 light up, indicating that a Gigabit Ethernet connection has been established. Ralph gets excited at the thought of how much money he might save the company by using the same cable for both telephone and data. However, while the LED is lit, he cannot seem to connect to another system over his test network. Which of the following describes what he must do to correct the problem?

        1. Ralph must manually configure the network adapters to use Gigabit Ethernet, rather than let them autonegotiate.
        2. Ralph is using the wrong two wire pairs for the Gigabit Ethernet connection. He must rewire the connectors.
        3. Ralph is using the wrong pinout standard on his lab network. He must use T568A.
        4. Ralph must use all four wire pairs for a Gigabit Ethernet connection.

        Answer:

        D. The autonegotiation mechanism is not the problem, nor is the pinout standard or Ralph's wire pair selection. The speed autonegotiation mechanism in Gigabit Ethernet uses only two wire pairs, so although the Light-Emitting Diodes (LEDs) do light up successfully, a functional Gigabit Ethernet data connection requires all four wire pairs.
180.    Ed is inspecting the cable runs recently installed for some new Gigabit Ethernet systems on his network. Looking at the patch panel connections, he notices that they are wired using the T568B pinout standard. However, when he examines the wall plate connections, he sees that they are wired using the T568A standard. What is the best way for Ed to resolve the problem?

        1. Call the contractor and have all of the wall plate connectors rewired using the T568B standard.
        2. Purchase crossover patch cables for all of the connections between the patch panel and the switches.
        3. Configure the switches to not use a crossover circuit for all of the ports connected to the patch panel.
        4. Do nothing. The cable runs will function properly as is.

        Answer:

        D. Cable runs are traditionally wired “straight through”; that is, with the transmit pins at one end wired to the transmit pins at the other end. It is the switch that is supposed to implement the crossover circuit that connects the transmit pins to the receive pins. Cable runs wired using T568A at one end and T568B at the other end create a crossover circuit in the cable run. At one time, this would have been a serious problem, but today's switches automatically configure crossover circuits as needed, so they will adjust themselves to adapt to the cable runs. All of the other options would correct the problem, but doing nothing is certainly the easiest and best option.
181.    Ralph has two computers that he long ago networked together by plugging one end of an Ethernet cable into each machine. He recently bought an old Ethernet hub at a garage sale and wants to use it to expand his network. The hub has four numbered ports and a fifth port marked with an X. Ralph plugs one computer into port 1 using his existing cable and buys a new cable to plug the other computer into port 4. The two computers cannot communicate, however. Which of the following solutions will not enable his computers to communicate?

        1. Move the port 4 cable to port 2
        2. Replace the old cable with a second new one
        3. Plug the computer with the old cable into the X port
        4. Plug the computer with the new cable into the X port

        Answer:

        A. The problem is unlikely to be a bad hub port or a bad cable, so moving the cable from port 4 to port 2 will not help. The problem is the crossover circuit between the two computers. The two systems were once connected directly together, which means that Ralph was using a crossover cable. The hub also provides a crossover circuit (except in the X port), and old hubs often do not autonegotiate crossovers. Therefore, the connection has two crossovers, which is the equivalent of wiring transmit pins to transmit pins, instead of transmit pins to receive pins. All of the other options eliminate one of the crossover circuits, enabling the computers to be wired correctly.
182.    Ralph recently bought an old Ethernet hub and some twisted-pair cables at a garage sale and wants to use them to build a home network. He plugs two computers into the hub using the cables but finds that the computers are unable to communicate. Then he notices that one of the ports in the hub is labeled with an X. He tries plugging one of the computers into the X port, and now they can communicate. Which of the following statements is the most likely explanation for this behavior?

        1. The hub has a bad port.
        2. One of the cables is a crossover cable.
        3. Both of the cables are crossover cables.
        4. The X port provides extra strength to the signals.

        Answer:

        B. Older Ethernet hubs do not autonegotiate crossovers. Instead, they have an X (or uplink) port that provides a connection without a crossover circuit, so you can connect one hub to another. If both of the cables had been standard straight-through Ethernet cables or if both had been crossover cables, then plugging them into two regular ports should have worked. Because plugging one cable into the X port worked, this means that only one of the cables must be a crossover cable. The problem, therefore, was the cable, not the port. The X port does not provide extra strength to the signals.
183.    Alice is a consultant who has been hired to move a client's old 20-node coaxial Ethernet network to a new location. She disassembles all of the network cabling and other components and packs them for shipping. At the new site, she sets up all of the computers, plugs a T-connector into each network adapter, and connects the cables, running them from one computer to the next to form the bus. When Alice is finished, she starts the computers and tests their network connectivity. She finds that 12 consecutive computers can communicate with each other, and the other 8 can communicate with each other, but the 12 cannot communicate with the 8. She makes sure that all of the connectors are securely tightened, especially the ones on the 12th computer, but the problem persists. Which of the following is the most likely cause of the difficulty?

        1. Alice has forgotten to terminate the computers at each end of the bus.
        2. One of the connectors on the 12th computer has a bent pin.
        3. Alice has forgotten to ground the network.
        4. The transmit and receive pins are reversed on the 12th computer.

        Answer:

        B. A bent pin on one of the 12th computer's connections would cause a break in the bus, essentially forming two networks that operate independently. The failure to terminate or ground the network would not produce this type of fault. Reversing the transmit and receive pins is not possible on a coaxial connection, due to the architecture of the cable.
184.    Ed is troubleshooting some network performance problems. After exhausting many other possibilities, he is examining the twisted-pair cable runs in the office's drop ceiling. He finds that some cables have been damaged, apparently by electricians working in that space. In some cases, the cable sheath has been split along its length, and some of the insulation on the wires inside has been scraped off as well. Which of the following types of faults might be caused by this damage? (Choose all that apply.)

        1. Open circuits
        2. Short circuits
        3. Split pairs
        4. Transposed wires

        Answer:

        A, B. An open circuit is caused either by a break in the wire somewhere inside the cable or a bad connection with the pin in one or both connectors. A short is when a wire is connected to two or more pins at one end of the cable or when the conductors of two or more wires are touching inside the cable. In this instance, the damage to the cables could have resulted in either condition. A split pair is a connection in which two wires are incorrectly mapped in exactly the same way on both ends of the cable. Having transposed pairs is a fault in which both of the wires in a pair are connected to the wrong pins at one end of the cable. Both of these faults are the result of incorrect wiring during installation; they are not caused by damaged cables.
185.    Which of the following types of interference on a twisted-pair network are designed to be prevented by the twists in the wire pairs inside the cable?

        1. Crosstalk
        2. EMI
        3. Attenuation
        4. Latency

        Answer:

        A. Crosstalk is a type of interference that occurs on copper-based networks when a signal transmitted on one conductor bleeds over onto another nearby conductor. Twisted-pair cables, which have eight or more conductors compressed together inside one sheath, are particularly susceptible to crosstalk. Twisting each of the separate wire pairs tends to reduce the amount of crosstalk to manageable levels. Twisting the wire pairs does not prevent signals from being affected by electromagnetic interference (EMI) or attenuation. Latency is a measurement of the time it takes for a signal to travel from its source to its destination.
186.    Ralph has been asked to create some new patch cables that will be used to connect patch panel ports to the network switches. He has been told that the patch panel connectors are all wired using the T568A pinout standard. Which of the following instructions should Ralph use when creating the patch cables?

        1. Use T568A at both ends
        2. Use T567B at both ends
        3. Use T568A at one end and T568B at the other end
        4. Use either standard, as long as both ends are the same

        Answer:

        D. Either the T568A or the T568B pinout standard is acceptable. The patch cables will function properly as long as both ends are wired using the same pinout standard.
187.    Ed has discovered that, on some of his newly installed twisted-pair cable runs, the installer has stripped away nearly a foot of the cable sheath at each end and has untwisted the wire pairs before attaching them to the connectors. Which of the following problems is the network more likely to experience due to the untwisted wires?

        1. Jitter
        2. Attenuation
        3. Crosstalk
        4. EMI

        Answer:

        C. Crosstalk is a type of interference that occurs on copper-based networks when in a signal transmitted on one conductor bleeds over onto another nearby conductor. Twisted-pair cables, which have eight or more conductors compressed together inside one sheath, are particularly susceptible to crosstalk. Twisting each of the separate wire pairs tends to reduce the amount of crosstalk to manageable levels. Untwisting the pairs leaves them more susceptible to crosstalk. Jitter, attenuation, and electromagnetic interference (EMI) are all conditions that can affect the performance of a wired network, but they are not directly related to untwisted wire pairs.
188.    Ed is the administrator of his small company's network. A user calls the help desk and reports that she cannot connect to the network. She has never had any problems connecting before now, and she says that nothing on her computer has changed. Ed goes to the user's location to investigate and notices that the link pulse Light-Emitting Diode (LED) on the switch port for the user's computer is not lit. What should Ed do next to isolate and fix the problem? (Choose all that apply.)

        1. Verify that the cable is securely connected to the switch
        2. Verify that the patch cable is pinned and paired properly
        3. Replace the existing patch cable with a straight-through cable that is known to be good
        4. Replace the existing patch cable with a crossover cable that is known to be good

        Answer:

        A, C. In this scenario, the user was previously able to connect to the network. There have been no hardware or software changes to the computer. These factors indicate that there is possibly a physical layer problem, such as a loose cable, a faulty cable, a bad switch port, or a bad network interface adapter in the computer. Since the user's cable previously worked, there is no need to verify that it is pinned and paired properly, and crossover cables are not used to connect workstations to switches. The first thing Ed should do is verify that all cable connections are secure. If he finds a loose cable and the link pulse LED lights up when he reseats it, then the cable was the problem. If the link pulse LED does not light, Ed should replace the existing cable with a straight-through cable that is known to be good. If the LED lights up, the existing cable was probably faulty. If the LED does not light up, Ed should suspect a faulty network interface adapter or switch port and try moving the cable to a port on the switch that is known to function. If the connection works, the problem is probably a failed switch port. If the connection still does not work, then the fault is probably the network interface adapter in the user's computer.
189.    Ed is examining some twisted-pair cable runs that were recently installed in his office by an outside contractor. Looking at the connectors, he sees a variety of pinout combinations. Which of the following pinouts must Ed have rewired because they are incorrect? (Choose all that apply.)

        1. White/orange, orange, white/green, blue, white/blue, green, white/brown, brown
        2. White/green, green, white/orange, blue, white/blue, orange, white/brown, brown
        3. White/orange, orange, white/green, green, white/blue, blue, white/brown, brown
        4. White/brown, white/green, white/orange, blue, white/blue, orange, green, brown

        Answer:

        C, D. Option A is the T568B pinout, and option B is the T568A pinout. Both of these are correct and may be used. Options C and D are both incorrect and can result in excessive amounts of crosstalk.
190.    You have three Virtual LANs (VLAN2, VLAN3, and VLAN4) with each implemented on three switches. A single router provides routing among the VLANs. All of the VLAN2 users connected to a common switch are complaining that they cannot access resources on other hosts within their own VLAN or on VLAN3 and VLAN4. Before today, they could connect to local and remote resources with no problem. What is the likeliest cause of the service interruption?

        1. The router is malfunctioning and not routing among the VLANs.
        2. VLAN2 is misconfigured.
        3. The common switch to which the VLAN2 users are connected is not functioning.
        4. VLAN3 and VLAN4 are misconfigured.

        Answer:

        C. In this scenario, some, but not all, users on VLAN2 cannot connect to local and remote resources. Since users connected to other switches within the same VLAN and on other VLANs are not reporting any problems, the router is not the issue. This also excludes a VLAN2 configuration problem because this would affect the VLAN2 users on all of the switches. VLAN3 and VLAN4 users can communicate through the router, so they are also not the problem. The likeliest problem is the common component, which is the switch to which the VLAN2 users experiencing the outage are connected.
191.    Alice is supporting a network that consists of four internal Local Area Networks (LANs) with 50 users each. Each internal LAN uses twisted-pair Gigabit Ethernet links that connect the users to a switch. Each of the four switches connects to a backbone router. All of the routers connect to the same backbone network, which has a single additional router to connect the company's network to the Internet, using a T-1 link. Users on one of the internal LANs are complaining that, when they came in this morning, they could not access the Internet or the other internal LANs, although they could access local resources with no problems. Which network component is the likeliest source of the problem in this scenario?

        1. The router connecting the problem LAN to the backbone
        2. The Internet router
        3. The switch on the problem LAN
        4. The cable on the backbone network

        Answer:

        A. In this scenario, only users on one LAN are experiencing problems connecting to the Internet and other internal LANs. This isolates the problem to a component within that LAN only. Since users can connect successfully to local resources, the problem does not lie within the individual computers, the switch that connects the users to the network, or the backbone network cable. The likeliest problem is in the router connecting problem LAN to the backbone network. Since users on the other internal LANs are not reporting problems connecting to the Internet, the problem most likely does not involve the Internet router.
192.    Alice is examining a captured sample of network traffic to create a network performance baseline for future reference. She notices that the sample contains a flood of multicast traffic, but she does not know why. After some investigation, she learns that there is video traffic on the network being transmitted as multicasts, but it is only intended for a particular group of users, not for everyone. However, since the multicast traffic is flooding the network, all of the hosts must process the packets, possibly resulting in performance degradation or even Denial-of-Service (DoS). Which of the following can Alice use to prevent the traffic from being processed by the unintended hosts?

        1. Asymmetric routing
        2. Flow control
        3. Multipathing
        4. IGMP snooping

        Answer:

        D. Internet Group Management Protocol (IGMP) snooping is a switching technique that prevents network hosts from receiving multicast packets when they are not members of the multicast group. The multicast traffic will still appear on the network, but only the members of the multicast group will process the packets. Asymmetric routing and multipathing all affect the route that the packets take through the network, and flow control only affects the speed at which transmitting systems send packets. None of these can control which hosts process the incoming packets.
193.    Alice is supporting a network that consists of four internal Local Area Networks (LANs) with 50 users each. Each internal LAN uses twisted-pair Gigabit Ethernet links that connect the users to a switch. Each of the four switches connects to a backbone router. All of the routers connect to the same backbone network, which has a single additional router to connect the company's network to the Internet. Users on all of the internal LANs are complaining that, when they came in this morning, they could not access the Internet, although they could access resources on all of the LANs with no problems. Which network component is the likeliest source of the problem in this scenario?

        1. The router connecting the problem LAN to the backbone
        2. The Internet router
        3. The switch on the problem LAN
        4. The cable on the backbone network

        Answer:

        B. In this scenario, all of the internal users are experiencing problems connecting to the Internet, so the router that provides access to the Internet is the suspected component. Since users can connect to resources on the internal LANs, the problem probably is not in any of the routers connecting the LANs to the backbone or the backbone cable itself. This also eliminates the probability that the switches on the LANs are the problem.
194.    Ed is implementing a web server farm on his company's network and has installed a router to create a screened subnet (or perimeter network) on which the web servers will be located. However, Ed now cannot access the web servers from his workstation on the internal network. Which of the following tasks will Ed have to complete before he can access the perimeter network from the internal network? (Choose all that apply.)

        1. Change IP addresses
        2. Change default gateway addresses
        3. Update the DNS records
        4. Change MAC addresses

        Answer:

        A, B, C. Ed will first have to change the Internet Protocol (IP) addresses. This is because the computers on the other side of the router, on the screened subnet, must use an IP network address that is different from the internal network's address. Next, Ed will have to change the default gateway address setting on the internal network computers to the address of the router so that traffic can be directed to the screened subnet. Finally, Ed will have to update the resource records on the Domain Name System (DNS) server to reflect the IP address changes. Media Access Control (MAC) addresses are hard-coded into network interface adapters and are not easily changed.
195.    Ralph has a wired home network with three Windows computers, a switch, and a cable modem/router that provides access to the Internet. One of the computers is able to connect to the other two, but it cannot connect to the Internet. Which of the following configuration parameters on the malfunctioning computer will Ralph most likely have to change to resolve this problem?

        1. IP address
        2. Subnet mask
        3. Default gateway
        4. MAC address

        Answer:

        C. The problem is most likely the default gateway address, which directs all traffic intended for the Internet to the cable modem/router. If that address is incorrect, the traffic will never reach the router. Because the computer can access the other two systems on the local network, the Internet Protocol (IP) address and subnet mask are not the problem. It is not necessary (and not always possible) to change the Media Access Control (MAC) address on a Windows workstation.
196.    Ralph is a network administrator attempting to use his workstation to remote into a web server called WebServ1 on the screened subnet (perimeter network). However, the remote desktop client software is unable to establish a connection to the server. Ralph can see all of the computers on his local network and on the screened subnet. He tries using the ping utility to test WebServ1's Transmission Control Protocol/Internet Protocol (TCP/IP) functionality, and the ping test is successful. Ralph then calls his colleague Ed and has him try to connect to WebServ1 using the same remote access tool. Ed connects successfully. Which of the following could be the cause of the problem Ralph is experiencing?

        1. Name resolution failure
        2. Unresponsive service on the web server
        3. Blocked TCP/UDP ports on the web server
        4. Incorrect firewall settings on Ralph's workstation

        Answer:

        D. Because Ed can connect to WebServ1 successfully, the problem is not an unresponsive service or blocked ports on the server. The problem is not a name resolution failure because Ralph can successfully ping WebServ1 by name. Therefore, of the options listed, the only possible problem must be that the firewall on Ralph's workstation is not configured to allow the remote desktop client's traffic out.
197.    A user calls the company's IT help desk to report that she has received an error message on her Windows workstation. The error states that her computer has an IP address that is duplicated on the network. Ralph is concerned that there might be a configuration problem with the DHCP servers on the network. He suspects that there are DHCP servers configured with scopes that overlap, resulting in two DHCP servers assigning the same IP addresses to different clients. He is worried that they are about to receive a flood of calls reporting the same problem. Alice reassures Ralph, telling him that it cannot be a DHCP problem, and that there must be two computers that are manually configured with the same IP address. How does Alice know this?

        1. Because Windows computers check the routing table before accepting an IP address from a DHCP server
        2. Because DHCP servers use DNS queries to check for duplicate IP addresses
        3. Because DHCP clients use ARP broadcasts to check for duplicate IP addresses
        4. Because it is only possible to have one DHCP server on a given subnet

        Answer:

        C. When a Dynamic Host Configuration Protocol (DHCP) client is offered an Internal Protocol (IP) address by a DHCP server, the client broadcasts Address Resolution Protocol (ARP) requests using that address before accepting it. If another computer on the local network is using the offered address, the computer responds to the ARP request, and the DHCP client declines the address. The DHCP server then offers another address. Domain Name Service (DNS) queries and routing table checks are not reliable means of checking for duplicate IP addresses. It is possible to have two DHCP servers on the same local network, but they must be configured with scopes that do not overlap.
198.    A user, Ed, is reporting what appear to be intermittent traffic interruptions on his workstation. Sometimes he receives responses to his server requests, and sometimes not. It does not seem to be an Internet issue, because the problem also occurs with local server requests. While troubleshooting the problem, Ralph performs a series of packet captures and analyzes the network traffic. He discovers that all of the request messages generated by Ed's workstation have responses on the network, but in some cases, the responses are going to a workstation other than Ed's. Which of the following conditions could be causing this to happen?

        1. Duplicate IP addresses
        2. Blocked TCP/UDP ports
        3. Duplicate MAC addresses
        4. Incorrect host firewall settings
        5. Multicast flood

        Answer:

        C. If someone on the network is spoofing the Media Access Control (MAC) address of Ed's workstation, the MAC address table in the switch handing the network traffic might be continually changing as packets from each computer reach the switch. This could cause some of the response packets to be forwarded to Ed's workstation and some to the spoofer's workstation. Duplicate IP addresses would not cause this problem, because they would be detected by the operating system. Blocked Transmission Control Protocol/User Datagram Protocol (TCP/UDP) ports, incorrect firewall settings, or a flood of multicast transmissions could prevent Ed from receiving responses, but they would not be sent to another workstation.
199.    A user calls Alice at the IT help desk and reports that she is having intermittent problems accessing both local servers and Internet websites. Which of the following potential problems can Alice rule out immediately?

        1. Duplicate Media Access Control (MAC) addresses
        2. Duplicate Internet Protocol (IP) addresses
        3. Malfunctioning router
        4. Malfunctioning Domain Name System (DNS) server

        Answer:

        B. Operating systems detect duplicate IP addresses immediately and display error messages or notifications on the computers involved. Therefore, the user with the problem would have been informed immediately if another system were using her IP address. All of the other options are possible causes of the problem that are more difficult to troubleshoot.
200.    The entire network at Adatum Corp. is unable to access the Internet. All of the users throughout the network are complaining that their browsers are displaying Domain Name System (DNS) failure messages. The company does not have an in-house network administrator, so they call Ralph at his consulting firm. Which of the following should be the first question that Ralph asks in his attempt to pinpoint the location of the malfunction?

        1. What browser are the users running?
        2. Where is the DNS server located?
        3. What technology is used to provide access to the Internet?
        4. What sites are the users attempting to access?

        Answer:

        B. The users' browsers are failing to resolve the hostnames of the requested websites into Internet Protocol (IP) addresses, which they must do before they can connect to the web servers. By asking where the company's DNS server is located, Ralph can determine if the problem is the DNS server itself or the router that provides access to the Internet. If the DNS server is located on Adatum's company network, then the DNS server could be failing to resolve the website names. However, the DNS server could be located on the Internet Service Provider's (ISP's) network, in which case the problem might be in the router that provides access to the ISP's network.
201.    To save the company money and to provide some new hires with Gigabit Ethernet connectivity, Ralph has installed some new Category 5e (Cat 5e) cable runs, connecting his company's datacenter with a newly rented office at the far end of the building. However, the new users are complaining of intermittent connectivity problems. The company brings in a cabling contractor to investigate, and his diagnosis is attenuation. Which of the following will most likely be a sure solution to the problem?

        1. Repull the runs using Category 6 cable
        2. Shorten the cable runs
        3. Configure the hardware to run at a slower speed
        4. Install high-end network adapters in the workstations

        Answer:

        B. Attenuation is the weakening of the signals as they traverse the network medium. In this case, the problem is most likely the result of cable runs that exceed the 100 meter maximum defined in the Ethernet twisted-pair specification. Therefore, shortening the cable runs will be likely to solve the problem. All of the Ethernet twisted-pair specifications have a 100 meter maximum length, so running the network at a slower speed, installing a higher grade cable, and installing higher end network adapters might have no effect if the runs are overly long.
202.    Alice's network has been experiencing intermittent service slowdowns and outages ever since the company moved into their new building. She has tried every troubleshooting procedure she can think of and has not been able to determine the cause. One particular user, hoping to be the squeaky wheel that gets the grease, has taken to calling Alice every time he experiences a problem. One day, as she is working in the datacenter, Alice notices that the user calls her every time she hears an additional humming noise begin. After examining the doors in the hallway, Alice realizes that the racks containing her switches are located right next to the building's elevator machinery room. Which of the following conditions is probably causing the network communication problem?

        1. EMI
        2. NEXT
        3. FEXT
        4. Attenuation

        Answer:

        A. Elevator machinery, fluorescent light fixtures, and other electrical devices in an office environment can generate magnetic fields, resulting in electromagnetic interference (EMI). When copper-based data cables are located too near to such a device, the magnetic fields can generate an electric current on the cable that interferes with the signals exchanged by network devices. If the network users experience a problem every time the elevator machinery switches on, EMI is a likely cause of the problem. Near-end crosstalk (NEXT), far-end crosstalk (FEXT), and attenuation can all cause intermittent network communication problems, but they cannot be caused by elevator machinery.
203.    Ralph is setting up a workstation for the company's new vice president. He has installed the computer in the VP's office and plugged the data cable into the wall plate. Then, back in the datacenter, he uses a patch cable to connect the corresponding port in the patch panel to a port in the network switch. However, the computer is unable to access the network. There are no complaints from other users. Which of the following could be the source of the problem? (Choose all that apply.)

        1. The DNS server is malfunctioning.
        2. The switch port is disabled.
        3. The NAT server is not functioning.
        4. The switch is configured to use port security.

        Answer:

        B, D. It is common practice on many networks to disable switch ports that are not in use so that unauthorized individuals cannot plug devices into them. Some networks also use port security, in which switches are configured with Access Control Lists (ACLs) that specify the Media Access Control (MAC) addresses of devices that are permitted to use them. Either of these could be the source of Ralph's problem. Because there are no other network users reporting problems, malfunctioning services such as Network Address Translation (NAT) and Domain Name System (DNS) are not likely to be the cause.
204.    Ralph is setting up a network connection for a new vice president, who is supplying his own laptop under the company's Bring Your Own Device (BYOD) policy. He plugs the computer into the wall plate, and the link pulse Light-Emitting Diode (LED) lights up. Then, back in the datacenter, he uses a patch cable to connect the corresponding port in the patch panel to a port in the network switch. Later, the VP calls Ralph to report that data transfers between his laptop and the network servers are extremely slow. Which of the following could explain the problem?

        1. There is a duplex mismatch between the laptop and the network switch.
        2. Ralph used a crossover cable to connect the laptop to the wall plate.
        3. The switch port is disabled.
        4. The network adapter drivers on the laptop are outdated.

        Answer:

        A. A duplex mismatch is the most likely of the options. Ethernet running over twisted-pair cable, in its original half-duplex mode, detects collisions by looking for data on the transmit and receive pins at the same time. In full-duplex mode, data is supposed to be transmitted and received at the same time. When one side of a connection is configured to use full duplex and the other end is configured to use half duplex, the full-duplex communications on the one side look like collisions to the half-duplex side. The half-duplex adapter transmits a jam signal as a result of each collision, which causes the full-duplex side to receive an incomplete frame. Both sides then start to retransmit frames in a continuing cycle, causing network performance to diminish drastically. If the problem were a crossover cable or a disabled switch port, the link pulse LED would not light. Outdated drivers would not be likely to slow network performance, and if they did, the slowdown would be minor.
205.    While working in her company's datacenter, Alice notices that the Light-Emitting Diodes (LEDs) on most of the network switch ports are green, but there are some that are orange. Alice asks several people why this is so and receives a different answer from each one. Which one of the following answers is correct?

        1. The orange LEDs indicate that no device is connected to the switch port.
        2. The orange LEDs indicate that the connected device is experiencing an excessive number of collisions.
        3. The orange LEDs indicate that the device is connected to the switch at a relatively slow speed.
        4. The orange LEDs indicate that the connected devices are other switches, rather than workstations.

        Answer:

        C. Green LEDs indicate the device is running at the full speed supported by the switch, whereas orange LEDs indicate that the device is running at a reduced speed. If no device is connected, the LED does not illuminate at all. The LED does not indicate the occurrence of collisions or the type of device connected to the port.
206.    Alice's company is opening a new branch office, and Alice is responsible for building the domain controller for that office. She installs a new Windows server and configures it as a domain controller, and then ships it to the new office site. However, once it arrives and is connected to the home office network, the new domain controller fails to synchronize with the existing ones at the home office. Which of the following could be the cause of the problem?

        1. Incorrect time
        2. Server hardware failure
        3. Duplicate IP addresses
        4. Incorrect default gateway address

        Answer:

        A. If the time on the domain controller at the new office is more than five minutes off of the time held by domain controller at the home office, then the new domain controller will not sync. Duplicate Internet Protocol (IP) addresses or an incorrect default gateway address would prevent the new domain controller from connecting to the home office network. A server hardware failure would manifest as an outage far more serious than a domain controller synchronization issue.
207.    Ralph recently bought an old 10Base-T Ethernet hub at a garage sale and wants to use it to connect his various computers into a home network. He plugs three computers into the hub and finds that although two of his older computers can communicate with each other, his newest computer cannot connect to the network. Which of the following tasks will most likely resolve the problem?

        1. Configure the hub to run at 10 Mbps
        2. Configure the hub to run at 100 Mbps
        3. Configure the computer's network adapter to run at 10 Mbps
        4. Configure the computer's network adapter to run at 100 Mbps

        Answer:

        C. Ralph's new computer is probably equipped with a network adapter that supports at least Fast Ethernet (100Base-TX). Fast Ethernet and newer network adapters support autonegotiation of the connection speed, but 10Base-T does not. Therefore, if the computer tries to negotiate a connection speed with the 10Base-T hub, it will fail and run at its default speed, which the hub does not support. By manually configuring the adapter in the computer to run at 10 Mbps, it should be able to communicate with the network. Setting the computer's adapter to run at 100 Mbps will not change anything. It is not possible to change the speed of a 10Base-T hub.
208.    Alice is troubleshooting a problem that some users are having connecting to an application server on the local network. While testing connectivity using the ping tool, she discovers that she can ping the server successfully using its computer name, but pinging the computer's fully qualified domain name (FQDN) fails. Which of the following is most likely the source of the problem?

        1. DNS
        2. DHCP
        3. EMI
        4. ACL

        Answer:

        A. Only Domain Name System (DNS) servers perform FQDN resolutions, so that is likely to be the source of the problem. It is possible to ping a device on the local network using its computer name without the use of DNS. Electromagnetic interference (EMI) would inhibit all network communication, and Access Control Lists (ACLs) have no effect on ping tests. Dynamic Host Configuration Protocol (DHCP) assigns IP addresses to clients; it does not resolve FQDNs.
209.    Alice is working on an older network with a Windows Internet Name Service (WINS) server, a Domain Name System (DNS) server, and an Internet router. A user is complaining that he suddenly cannot connect to hosts on other internal networks. The user is not having problems connecting to resources on his local network or the Internet. Alice asks the user whether anything is new or has been changed on the computer and discovers that he recently changed some Internet Protocol (IP) parameters. What should Alice do next?

        1. Verify that the router is up and running and properly configured
        2. Verify that the WINS server is up and running and properly configured
        3. Verify that the DNS server is up and running and properly configured
        4. Verify that the user's IP configuration settings are correct

        Answer:

        D. Since only one user is reporting the problem, the user's computer is the likeliest source of the problem. The user has probably changed or removed the WINS server address. If the user is working with an incorrect WINS address, he can access local network resources but not resources on another internal LAN. Also, he can access resources on the Internet, which means the Internet router and the DNS server are not the problem.
210.    Ralph has begun to receive calls from users reporting that they cannot access the local network or the Internet. Ralph checks their computers and discovers that all of the users with a problem have IP addresses in the 169.254.0.0/16 network, which is not the address used on Ralph's network. Which of the following might be the cause of the problem?

        1. The users have tried to modify their IP configuration settings.
        2. There is a rogue DHCP server somewhere on the network.
        3. The IP address leases assigned by the DHCP server have expired.
        4. The users' workstations have been infected by a form of malware.

        Answer:

        C. The 169.254.0.0/16 network is used by Automatic Private Internet Protocol Addressing (APIPA), a standard that provides Dynamic Host Configuration Protocol (DHCP) clients with an Internet Protocol (IP) address when they cannot contact a DHCP server. Unknown to Ralph, the DHCP server on his network has been down for over a week, and the users' IP address leases have begun to expire. This causes them to revert to APIPA addresses. Multiple users changing their IP addresses would not result in them all using the same network address. A rogue DHCP would not be likely to deploy APIPA addresses to clients. Malware infections that modify IP addresses are rare.
211.    Ralph has installed a new Category 5e (Cat 5e) cable run himself. He has attached keystone connectors to both ends of the cable, mounted the office-side connector to a wall plate, and mounted the datacenter connector into a patch panel. Then he took a patch cord and connected the patch panel port to an open port in one of the network switches. However, the Light-Emitting Diode (LED) on the switch port does not light. What should Ralph do?

        1. Repull the cable run using Category 6 cable
        2. Check the cable run for wiring faults
        3. Make sure the switch port is not disabled
        4. Plug a computer into the wall plate

        Answer:

        D. For the link pulse LED on the switch port to light up, there must be a completed connection between the switch and a computer at the other end. None of the other options will cause the LED to light.
212.    A user calls Ed at the help desk to report that his computer is displaying a Duplicate IP Address error message. This puzzles Ed because all of the network workstations should be configured to obtain their Internet Protocol (IP) addresses from Dynamic Host Configuration Protocol (DHCP) servers. Ed asks the user if he has changed the Transmission Control Protocol/Internet Protocol (TCP/IP) configuration settings on the computer recently. The user says no. Ed then asks of anybody else uses the workstation. The user says no. However, when Ed runs the `ipconfig /all` command on the user's workstation, he sees that the DHCP Enabled setting reads No. What should Ed do next?

        1. Accuse the user of changing the TCP/IP settings and then lying about it
        2. Activate the DHCP client on the workstation and close the trouble ticket
        3. Begin an investigation into the possibility of a rogue DHCP server on the network
        4. Change the IP address on the workstation to one that is not already in use

        Answer:

        B. Because Ed knows that the network workstations should be using DHCP to obtain their IP addresses, the best thing to do is to enable the DHCP client and close the ticket rather than configure the system with another static address. There is no indication that there is a rogue DHCP server on the network since the workstation's DHCP client is disabled. This is not the first time that Ed has had a user lie to him, nor will it be the last. He should just let it go and work on addressing the problem.
213.    Ralph is working with an Asymmetric Digital Subscriber Line (ADSL) router that has a switch module containing four Ethernet ports, all of which are assigned to the default VLAN1. Ralph can plug a laptop into one of the router's ports and access the Internet with no problems. Ralph now needs to connect the ADSL router to the company network, so that the wireless access points on the network can provide users with Internet access through the ADSL router. However, when Ralph plugs the router into a network switch port in VLAN4, the switch starts generating “Native VLAN mismatch detected” errors every minute. Which of the following steps should be part of the solution Ralph implements to stop the error messages? (Choose all that apply.)

        1. Create a VLAN1 on the network switch
        2. Create a VLAN4 on the ADSL router's switch module
        3. Configure the network switch port connected to the router to use VLAN1
        4. Configure the router port connected to the network switch to use VLAN4

        Answer:

        B, D. The solution should call for Ralph to create a VLAN on the ADSL router that matches the Virtual Local Area Network (VLAN) that the network switch port is using. Therefore, he should create a VLAN4 on the router and assign a port to it, which will be the port Ralph uses to connect the router to the network switch. There is no need to create a VLAN1 on the network switch, because all switches have a default VLAN called VLAN1. Modifying the VLAN assignments on the network switch is not a good idea, because it might interfere with the existing VLAN strategy in place.
214.    Ralph is working with an Asymmetric Digital Subscriber Line (ADSL) router that has a switch module containing four Ethernet ports, all of which are assigned to VLAN2. Ralph can plug a laptop into one of the router's ports and access the Internet with no problems. Ralph now needs to connect the ADSL router to the company network. However, when Ralph plugs the router into a network switch port in VLAN4, the switch starts generating “Native VLAN mismatch detected” errors every minute. To correct the problem, Ralph attempts to create a VLAN4 on the router, but he receives a “Feature not licensed” error. Which of the following actions can Ralph take to resolve the problem? (Choose all that apply.)

        1. Purchase a feature upgrade for the router
        2. Create a VLAN2 on the switch
        3. Configure the router to use VLAN1
        4. Configure the switch to use VLAN1

        Answer:

        A, B. Ralph could purchase a license upgrade for the router that would enable him to create a VLAN4. However, the simpler and less expensive solution would be to create a VLAN2 on the switch. As long as both ends of the cable are plugged into ports using the same Virtual Local Area Network (VLAN), the router should be able to service the network. Configuring the devices to use the default VLAN1 might interfere with the existing VLAN strategy.
215.    Clients of Ralph's company are calling to complain that, when they try to access the company's website, they see an error message stating that the website has an untrusted security certificate. They are afraid that they are connecting to an unprotected site or that the site has been taken over by hackers. What must Ralph due to address this problem?

        1. Obtain an SSL certificate from a trusted third-party company
        2. Configure the web servers to generate a self-signed certificate
        3. Install a certification authority on one of the network servers
        4. Explain to the clients that it is safe to bypass the error message and proceed to the website

        Answer:

        A. For the website's Secure Socket Layer (SSL) certificate to be trusted, it must be signed by a source that both parties in the transaction trust. Many security firms are in the business of providing SSL certificates to companies that have provided them with confirmation of their identities. This is what Ralph must do to prevent the error message from appearing to the company's clients. Creating a self-signed certificate or installing a certification authority in-house are not sufficient and are probably already the cause of the problem. Users are not likely to be convinced that everything is all right.
216.    Ralph is a network administrator who has had a Windows user report difficulties accessing certain other computers on the network. Ralph determines that the user is only experiencing problems when trying to connect to a system on the far side of a router. Ralph therefore decides to inspect the routing table on the user's computer. Which of the following tools can he use to do this? (Choose all that apply.)

        1. `nbtstat`
        2. `route`
        3. `nslookup`
        4. `netstat`

        Answer:

        B, D. The `route` tool, with the `print` parameter, displays the contents of the routing table on a Windows computer. So does the `netstat -r` command. The `nbtstat` and `nslookup` tools cannot display the routing table.
217.    A user calls Alice at the help desk to report that he cannot access the Internet. He can access systems on the local network, however. Alice examines the routing table on the user's workstation and sees the following. Which of the following commands must Alice run to correct the user's problem?

        `IPv4 Route Table =========================================================================== Active Routes: Network Destination Netmask Gateway Interface Metric 127.0.0.0 255.0.0.0 On-link 127.0.0.1 331 127.0.0.1 255.255.255.255 On-link 127.0.0.1 331 127.255.255.255 255.255.255.255 On-link 127.0.0.1 331 192.168.2.0 255.255.255.0 On-link 192.168.2.37 281 192.168.2.37 255.255.255.255 On-link 192.168.2.37 281 192.168.2.255 255.255.255.255 On-link 192.168.2.37 281 224.0.0.0 240.0.0.0 On-link 127.0.0.1 331 224.0.0.0 240.0.0.0 On-link 192.168.2.37 281 255.255.255.255 255.255.255.255 On-link 127.0.0.1 331 255.255.255.255 255.255.255.255 On-link 192.168.2.37 281 =========================================================================== Persistent Routes: None`

        1. `route add 0.0.0.0 MASK 0.0.0.0 192.168.2.37 METRIC 25 IF 192.168.2.99`
        2. `route add 0.0.0.0 MASK 255.255.255.0 192.168.2.99 METRIC 25 IF 192.168.2.37`
        3. `route add 192.168.2.0 MASK 255.255.255.0 192.168.2.99 METRIC 25 IF 192.168.2.37`
        4. `route add 0.0.0.0 MASK 0.0.0.0 192.168.2.99 METRIC 25 IF 192.168.2.37`

        Answer:

        D. To access the Internet, the workstation's routing table must include a default gateway entry. To create a default gateway entry in the routing table, you use the `route add` command with a Network Destination value of 0.0.0.0, a MASK value of 0.0.0.0, and the address of a router on the local network (in this case, 192.168.2.99). The entry must also have a `METRIC` value that is lower than the other entries in the table so that it will be used first.
218.    Alice is working the IT help desk at her company, which has 500 inside salespeople who start work at 9:00 a.m. The users are running Windows 10 and obtaining their Internet Protocol (IP) address configuration settings from Dynamic Host Configuration Protocol (DHCP) servers. Every morning, Alice receives many trouble calls from users that are experiencing extremely slow performance after they first turn their computers on. Their performance gradually improves within an hour. Which of the following is the most likely cause of the slowdown?

        1. Broadcast storm
        2. Routing loop
        3. Rogue DHCP server
        4. Switching loop
        5. Asymmetric routing

        Answer:

        A. The most likely cause for the slowdown is a broadcast storm. DHCP relies on broadcast messages to assign IP addresses to users, so 500 users all turning on their computers at 9:00 a.m. can generate an abnormally high number of broadcast packets. This can degrade network performance until all of the users have completed their DHCP address assignments. Routing loops, switching loops, and asymmetric routing can degrade network performance, but the degradation would not be limited to the early morning hours. A rogue DHCP server can cause problems but not the one described here.
219.    Alice is having trouble with a new fiber-optic cable run that has just been installed between two buildings on her company's campus. To confirm that there is a problem with the cables, Alice consults the wiring diagram provided by the cable installer and begins to calculate the optical power loss resulting from cable installation factors such as the type of cable used, the attenuation resulting from the length of the cable runs, and the number and type of splices. Which of the following terms describes the calculations that Alice is performing?

        1. Protocol analysis
        2. Routing loop
        3. Optical link budget
        4. Received Signal Strength Indication (RSSI)

        Answer:

        C. Alice's calculations are called an optical link budget. By adding up the various loss factors in decibels (dB), she can determine whether the budget is low, resulting in communication problems over the link. Protocol analysis is an examination of network packet contents. A routing loop is a condition in which packets are circulating endlessly around a network. RSSI is a wireless networking statistic that does not apply to fiber-optic connections.
220.    Ralph is a network administrator for a company with several branch offices, each of which has a Windows domain controller. There have been problems lately with the domain controllers synchronizing their data, and Ralph suspects that the problem is related to the Network Time Protocol (NTP) settings on the servers. Examining the server logs on the various domain controllers, he sees multiple errors saying, “Server NTP service not synchronized.” All of the other server functions are running normally. Which of the following could be the cause of the problem Ralph is experiencing?

        1. Name resolution failure
        2. Unresponsive database service on the servers
        3. Incorrect TCP/IP settings on the servers
        4. Incorrect firewall settings on the servers

        Answer:

        D. On all of the servers, NTP uses the well-known User Datagram Protocol (UDP) port 123 for its communications with a Coordinated Universal Time (UTC) server. If a server's firewall is blocking that port, it cannot synchronize its clock time. If the domain controllers have clocks that are not synchronized, their data synchronization processes can be affected. The problem is not a name resolution failure, an unresponsive database service, or incorrect Transmission Control Protocol/Internet Protocol (TCP/IP) settings because other server functions are not affected.
