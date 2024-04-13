# Questions

1.  Kyong manages the vulnerability scans for his organization. The senior director that oversees Kyong's group provides a report to the CIO on a monthly basis on operational activity, and he includes the number of open critical vulnerabilities. He would like to provide this information to his director in as simple a manner as possible each month. What should Kyong do?

    1. Provide the director with access to the scanning system.
    2. Check the system each month for the correct number and email it to the director.
    3. Configure a report that provides the information to automatically send to the director's email at the proper time each month.
    4. Ask an administrative assistant to check the system and provide the director with the information.

    Answer:

    C. Although all of these options are viable, the simplest solution is to design a report that provides the information and then configure the system to automatically send this report to the director each month.
2.  Carla is designing a vulnerability scanning workflow and has been tasked with selecting the person responsible for remediating vulnerabilities. Which one of the following people would normally be in the _best_ position to remediate a server vulnerability?

    1. Cybersecurity analyst
    2. System administrator
    3. Network engineer
    4. IT manager

    Answer:

    B. System administrators are normally in the best position to remediate vulnerabilities because they are responsible for maintaining the server configuration. Network engineers, security analysts, and managers may provide input, but they often lack either the privileges or the knowledge to successfully remediate a server.
3.  During a vulnerability scan, Patrick discovered that the configuration management agent installed on all of his organization's Windows servers contains a serious vulnerability. The manufacturer is aware of this issue, and a patch is available. What process should Patrick follow to correct this issue?

    1. Immediately deploy the patch to all affected systems.
    2. Deploy the patch to a single production server for testing and then deploy to all servers if that test is successful.
    3. Deploy the patch in a test environment and then conduct a staged rollout in production.
    4. Disable all external access to systems until the patch is deployed.

    Answer:

    C. Patrick should be extremely careful with this patch. If the patch causes services to fail, it has the potential to disable all of his organization's Windows servers. This is a serious risk and requires testing prior to patch deployment. Patrick's best course of action is to deploy the patch in a test environment and then roll it out into production on a staged basis if that test is successful. Options that involve deploying the patch to production systems prior to testing may cause those services to fail. Disabling all external access to systems is likely an overreaction that would have critical business impact.
4.  Ben is preparing to conduct a vulnerability scan for a new client of his security consulting organization. Which one of the following steps should Ben perform first?

    1. Conduct penetration testing.
    2. Run a vulnerability evaluation scan.
    3. Run a discovery scan.
    4. Obtain permission for the scans.

    Answer:

    D. Ben should obtain permission from the client to perform scans before engaging in any other activities. Failure to do so may violate the law and/or anger the client.
5.  Katherine coordinates the remediation of security vulnerabilities in her organization and is attempting to work with a system engineer on the patching of a server to correct a moderate impact vulnerability. The engineer is refusing to patch the server because of the potential interruption to a critical business process that runs on the server. What would be the most reasonable course of action for Katherine to take?

    1. Schedule the patching to occur during a regular maintenance cycle.
    2. Exempt the server from patching because of the critical business impact.
    3. Demand that the server be patched immediately to correct the vulnerability.
    4. Inform the engineer that if he does not apply the patch within a week that Katherine will file a complaint with his manager.

    Answer:

    A. The fact that the server runs a critical business process should increase the importance of the patch, rather than deferring it indefinitely. Katherine should work with the engineer to schedule the patch to occur during a regular maintenance window. It is reasonable to wait until that scheduled window because of the relatively low impact of the vulnerability.
6.  Grace ran a vulnerability scan and detected an urgent vulnerability in a public-facing web server. This vulnerability is easily exploitable and could result in the complete compromise of the server. Grace wants to follow best practices regarding change control while also mitigating this threat as quickly as possible. What would be Grace's best course of action?

    1. Initiate a high-priority change through her organization's change management process and wait for the change to be approved.
    2. Implement a fix immediately and document the change after the fact.
    3. Schedule a change for the next quarterly patch cycle.
    4. Initiate a standard change through her organization's change management process.

    Answer:

    B. In this situation, Grace is facing a true emergency. Her web server has a critical vulnerability that is exposed to the outside world and may be easily exploited. Grace should correct the issue immediately, informing all relevant stakeholders of the actions that she is taking. She can then follow up by documenting the change as an emergency action in her organization's change management process. All of the other approaches in this question introduce an unacceptable delay.
7.  Joe discovered a critical vulnerability in his organization's database server and received permission from his supervisor to implement an emergency change after the close of business. He has eight hours before the planned change window. In addition to planning the technical aspects of the change, what else should Joe do to prepare for the change?

    1. Ensure that all stakeholders are informed of the planned outage.
    2. Document the change in his organization's change management system.
    3. Identify any potential risks associated with the change.
    4. All of the above.

    Answer:

    D. Joe has time to conduct some communication and change management before making the change. Even though this change is urgent, Joe should take advantage of that time to communicate with stakeholders, conduct a risk assessment, and initiate change management processes. These tasks will likely be abbreviated forms of what Joe would do if he had time to plan a change normally, but he should make every effort to complete them.
8.  Sally discovered during a vulnerability scan that a system she manages has a high-priority vulnerability that requires a patch. The system is behind a firewall and there is no imminent threat, but Sally wants to get the situation resolved as quickly as possible. What would be her best course of action?

    1. Initiate a high-priority change through her organization's change management process.
    2. Implement a fix immediately and then document the change after the fact.
    3. Implement a fix immediately and then inform her supervisor of her action and the rationale.
    4. Schedule a change for the next quarterly patch cycle.

    Answer:

    A. In this situation, Sally recognizes that there is no imminent threat, so it is not necessary to follow an emergency change process that would allow her to implement the change before conducting any change management. That said, the change should be made without waiting up to three months for a scheduled patch cycle. Therefore, Sally's best option is to initiate a high-priority change through her organization's change management process.
9.  Gene runs a vulnerability scan of his organization's datacenter and produces a summary report to share with his management team. The report includes the chart shown here. When Gene's manager reads the report, she points out that the report is burying important details because it is highlighting too many unimportant issues. What should Gene do to resolve this issue?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c04uf001.jpg)

    1. Tell his manager that all vulnerabilities are important and should appear on the report.
    2. Create a revised version of the chart using Excel.
    3. Modify the sensitivity level of the scan.
    4. Stop sharing reports with the management team.

    Answer:

    C. Gene's best option is to alter the sensitivity level of the scan so that it excludes low-importance vulnerabilities. The fact that his manager is telling him that many of the details are unimportant is his cue that the report contains superfluous information. Although he could edit the chart manually, he should instead alter the scan settings so that he does not need to make those manual edits each time he runs the report.
10. Glenda routinely runs vulnerability scans of servers in her organization. She is having difficulty with one system administrator who refuses to correct vulnerabilities on a server used as a jump box by other IT staff. The server has had dozens of vulnerabilities for weeks and would require downtime to repair. One morning, her scan reports that all of the vulnerabilities suddenly disappeared overnight, while other systems in the same scan are reporting issues. She checks the service status dashboard, and the service appears to be running properly with no outages reported in the past week. What is the most likely cause of this result?

    1. The system administrator corrected the vulnerabilities.
    2. The server is down.
    3. The system administrator blocked the scanner.
    4. The scan did not run.

    Answer:

    C. Although any of these reasons are possible, the most likely cause of this result is that the system administrator blocked the scanner with a host firewall rule. It is unlikely that the administrator completed the lengthy, time-consuming work overnight and without causing a service disruption. If the server were down, other IT staff would have reported the issue. If the scan did not run, Glenda would not see any entries in the scanner's logs.
11. Tom is planning a series of vulnerability scans and wants to ensure that the organization is meeting its customer commitments with respect to the scans' performance impact. What two documents should Tom consult to find these obligations?

    1. SLAs and MOUs
    2. SLAs and DRPs
    3. DRPs and BIAs
    4. BIAs and MOUs

    Answer:

    A. Tom should consult service level agreements (SLAs) and memorandums of understanding (MOUs). These documents should contain all commitments made to customers related to performance. Disaster recovery plans (DRPs) and business impact assessments (BIAs) should not contain this type of information.
12. Zhang Wei is evaluating the success of his vulnerability management program and would like to include some metrics. Which one of the following would be the _least_ useful metric?

    1. Time to resolve critical vulnerabilities
    2. Number of open critical vulnerabilities over time
    3. Total number of vulnerabilities reported
    4. Number of systems containing critical vulnerabilities

    Answer:

    C. Zhang Wei should likely focus his efforts on high-priority vulnerabilities, as vulnerability scanners will report results for almost any system scanned. The time to resolve critical vulnerabilities, the number of open critical vulnerabilities over time, and the number of systems containing critical vulnerabilities are all useful metrics. The total number of reported vulnerabilities is less useful because it does not include any severity information.
13. Donna is working with a system engineer who wants to remediate vulnerabilities in a server that he manages. Of the report templates shown here, which would be most useful to the engineer?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c04uf002.jpg)

    1. Qualys Top 20 Report
    2. PCI Technical Report
    3. Executive Report
    4. Technical Report

    Answer:

    D. The Technical Report will contain detailed information on a specific host and is designed for an engineer seeking to remediate the system. The PCI Technical Report would focus on credit card compliance issues, and there is no indication that this server is used for credit card processing. The Qualys Top 20 Report and Executive Report would contain summary information more appropriate for a management audience and cover an entire network, rather than provide detailed information on a single system.
14. Abdul received the vulnerability report shown here for a server in his organization. The server runs a legacy application that cannot easily be updated. What risks does this vulnerability present?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c04uf003.jpg)

    1. Unauthorized access to files stored on the server
    2. Theft of credentials
    3. Eavesdropping on communications
    4. All of the above

    Answer:

    D. The use of FTP is not considered a good security practice. Unless tunneled through a secure protocol, FTP is unencrypted, allowing an attacker to eavesdrop on communications and steal credentials that may be transmitted over FTP links. Additionally, this vulnerability indicates that an attacker can gain access to the server without even providing valid credentials.
15. William is preparing a legal agreement for his organization to purchase services from a vendor. He would like to document the requirements for system availability, including the vendor's allowable downtime for patching. What type of agreement should William use to incorporate this requirement?

    1. MOU
    2. SLA
    3. BPA
    4. BIA

    Answer:

    B. Service level agreements (SLAs) specify the technical parameters of a vendor relationship and should include coverage of service availability as well as remedies for failure to meet the agreed-on targets. Memorandums of understanding (MOUs) are less formal documents that outline the relationship between two organizations. Business partnership agreements (BPAs) typically cover business, rather than technical, issues and would not normally include availability commitments. Business impact analysis (BIA) documents are risk assessments and are not legal agreements.
16. Raul is replacing his organization's existing vulnerability scanner with a new product that will fulfill that functionality moving forward. As Raul begins to build the policy, he notices some conflicts in the scanning settings between different documents. Which one of the following document sources should Raul give the highest priority when resolving these conflicts?

    1. NIST guidance documents
    2. Vendor best practices
    3. Corporate policy
    4. Configuration settings from the prior system

    Answer:

    C. Of the documents listed, only corporate policy is binding on Raul, and he should ensure that his new system's configuration complies with those requirements. The other sources may provide valuable information to inform Raul's work, but compliance with them is not mandatory.
17. Pietro is responsible for distributing vulnerability scan reports to system engineers who will remediate the vulnerabilities. What would be the most effective and secure way for Pietro to distribute the reports?

    1. Pietro should configure the reports to generate automatically and provide immediate, automated notification to administrators of the results.
    2. Pietro should run the reports manually and send automated notifications after he reviews them for security purposes.
    3. Pietro should run the reports on an automated basis and then manually notify administrators of the results after he reviews them.
    4. Pietro should run the reports manually and then manually notify administrators of the results after he reviews them.

    Answer:

    A. There is no reasonable justification for Pietro reviewing the reports prior to providing them to the administrators responsible for the systems. In the interests of transparency and efficiency, he should configure the scans to run automatically and send automated notifications to administrators as soon as they are generated. This allows immediate remediation. There is nothing preventing Pietro from performing a review of the scan results, but he should not filter them before providing them to the responsible engineers.
18. Nitesh would like to identify any systems on his network that are not registered with his asset management system because he is concerned that they might not be remediated to his organization's current security configuration baseline. He looks at the reporting console of his vulnerability scanner and sees the options shown here. Which of the following report types would be his best likely starting point?

    ![](https://cdn2.percipio.com/1713091581.af3c25110d5be87c964ff1f58db3e061c5d018ae/eod/books/165333/images/c04uf004.jpg)

    1. Technical Report
    2. High Severity Report
    3. Qualys Patch Report
    4. Unknown Device Report

    Answer:

    D. The Unknown Device Report will focus on systems detected during the scan that are not registered with the organization's asset management system. The High Severity Report will provide a summary of critical security issues across all systems. The Technical Report will likely contain too much detail and may not call out unknown systems. The Patch Report will indicate systems and applications that are missing patches but not necessarily identify unknown devices.
19. Nabil is the vulnerability manager for his organization and is responsible for tracking vulnerability remediation. There is a critical vulnerability in a network device that Nabil has handed off to the device's administrator, but it has not been resolved after repeated reminders to the engineer. What should Nabil do next?

    1. Threaten the engineer with disciplinary action.
    2. Correct the vulnerability himself.
    3. Mark the vulnerability as an exception.
    4. Escalate the issue to the network administrator's manager.

    Answer:

    D. The scenario does not indicate that Nabil has any operational or managerial control over the device or the administrator, so his next step should be to escalate the issue to an appropriate manager for resolution. Nabil should not threaten the engineer because there is no indication that he has the authority to do so. Nabil cannot correct the vulnerability himself because he should not have administrative access to network devices as a vulnerability manager. He should not mark the vulnerability as an exception because there is no indication that it was accepted through a formal exception process.
20. Maria discovered an operating system vulnerability on a system on her network. After tracing the IP address, she discovered that the vulnerability is on a proprietary search appliance installed on her network. She consulted with the responsible engineer who informed her that he has no access to the underlying operating system. What is the best course of action for Maria?

    1. Contact the vendor to obtain a patch.
    2. Try to gain access to the underlying operating system and install the patch.
    3. Mark the vulnerability as a false positive.
    4. Wait 30 days and rerun the scan to see whether the vendor corrected the vulnerability.

    Answer:

    A. Maria should contact the vendor to determine whether a patch is available for the appliance. She should not attempt to modify the appliance herself, as this may cause operational issues. Maria has no evidence to indicate that this is a false positive report, and there is no reason to wait 30 days to see whether the problem resolves itself.
21. Trevor is working with an application team on the remediation of a critical SQL injection vulnerability in a public-facing service. The team is concerned that deploying the fix will require several hours of downtime and will block customer transactions from completing. What is the most reasonable course of action for Trevor to suggest?

    1. Wait until the next scheduled maintenance window.
    2. Demand that the vulnerability be remediated immediately.
    3. Schedule an emergency maintenance for an off-peak time later in the day.
    4. Convene a working group to assess the situation.

    Answer:

    C. This is a critical vulnerability in a public-facing service and should be patched urgently. However, it is reasonable to schedule an emergency maintenance for the evening and inform customers of the outage several hours in advance. Therefore, Trevor should immediately begin monitoring affected systems for signs of compromise and work with the team to schedule maintenance for as soon as possible.
22. Thomas discovers a vulnerability in a web application that is part of a proprietary system developed by a third-party vendor, and he does not have access to the source code. Which one of the following actions can he take to mitigate the vulnerability without involving the vendor?

    1. Apply a patch.
    2. Update the source code.
    3. Deploy a web application firewall.
    4. Conduct dynamic testing.

    Answer:

    C. Thomas can deploy a web application firewall to block attempts to exploit the vulnerability. Applying a patch or updating the source code may also resolve the issue, but Thomas cannot do this himself because he does not have access to the source code. Dynamic testing identifies vulnerabilities but does not correct them.
23. Walt is designing his organization's vulnerability management program and is working to identify potential inhibitors to vulnerability remediation. He has heard concern from functional leaders that remediating vulnerabilities will impact the ability of a new system to fulfill user requests. Which one of the following inhibitors does not apply to this situation?

    1. Degrading functionality
    2. Organizational governance
    3. Legacy systems
    4. Business process interruption

    Answer:

    C. Walt finds himself in a very common situation, with business leaders worried about the impact of vulnerability remediation on their activities. The business leaders are concerned about business process interruption and degrading functionality. This could be best resolved with a robust organizational governance process. The system in question is newly deployed, so it is not an example of a legacy system.
24. The company that Brian works for processes credit cards and is required to be compliant with PCI DSS. If Brian's company experiences a breach of card data, what type of disclosure will they be required to provide?

    1. Notification to local law enforcement
    2. Notification to their acquiring bank
    3. Notification to federal law enforcement
    4. Notification to Visa and MasterCard

    Answer:

    B. Organizations that process credit cards work with acquiring banks to handle their card processing, rather than directly with the card providers. Notification to the bank is part of this type of response effort. Requiring notification of law enforcement is unlikely, and the card provider listing specifies only two of the major card vendors, none of which are specified in the question.
25. As Lauren prepares her organization's security practices and policies, she wants to address as many threat vectors as she can using an awareness program. Which of the following threats can be most effectively dealt with via awareness?

    1. Attrition
    2. Impersonation
    3. Improper usage
    4. Web

    Answer:

    C. Improper usage, which results from violations of an organization's acceptable use policies by authorized users, can be reduced by implementing a strong awareness program. This will help ensure users know what they are permitted to do and what is prohibited. Attrition attacks focus on brute-force methods of attacking services. Impersonation attacks include spoofing, man-in-the-middle attacks, and similar threats. Finally, web-based attacks focus on websites or web applications. Awareness may help with some specific web-based attacks like fake login sites, but many others would not be limited by Lauren's awareness efforts.
26. Laura wants to ensure that her team can communicate during an incident. Which of the following should the team prepare to be ready for an incident?

    1. A second, enterprise authenticated messaging system
    2. An enterprise VoIP system using encryption
    3. Enterprise email with TLS enabled
    4. A messaging capability that can function if enterprise authentication is unavailable

    Answer:

    D. A distinct messaging system that can work if enterprise services are unavailable due to an incident can be a critical factor for IR teams. Whether it's a phone tree, a collaboration system that also allows distinct logins that are not part of enterprise authentication, or another solution, IR teams often need a system that is separate during wide-ranging incidents.
27. Which of the following is not an important part of the incident response communication process?

    1. Limiting communication to trusted parties
    2. Disclosure based on public feedback
    3. Using a secure method of communication
    4. Preventing accidental release of incident-related information

    Answer:

    B. Disclosure based on regulatory or legislative requirements is commonly part of an incident response process; however, public feedback is typically a guiding element of information release. Limiting communication to trusted parties and ensuring that data and communications about the incident are properly secured are both critical to the security of the incident response process. This also means that responders should work to limit the potential for accidental release of incident-related information.
28. After law enforcement was called because of potential criminal activity discovered as part of a forensic investigation, the officers on the scene seized three servers. When can Joe expect his servers to be returned?

    1. After 30 days, which provides enough time for a reasonable imaging process
    2. After 6 months, as required by law
    3. After 1 year, as most cases resolve in that amount of time
    4. Joe should not plan on a timeframe for return

    Answer:

    D. Criminal investigations can take very long periods of time to resolve. In most cases, Joe should ensure that he can continue to operate without the servers for the foreseeable future.
29. NIST SP 800-61 identifies six outside parties that an incident response team will typically communicate with. Which of the following is not one of those parties?

    1. Customers, constituents, and media
    2. Internet service providers
    3. Law enforcement agencies
    4. Legal counsel

    Answer:

    D. NIST identifies customers, constituents, media, other incident response teams, Internet service providers, incident reporters, law enforcement agencies, and software and support vendors as outside parties that an IR team will communicate with.
30. Ben works at a U.S. federal agency that has experienced a data breach. Under FISMA, which organization does he have to report this incident to?

    1. US-CERT
    2. The National Cyber Security Authority
    3. The National Cyber Security Centre
    4. CERT/CC

    Answer:

    A. FISMA requires that U.S. federal agencies report incidents to US-CERT. CERT/CC is the coordination center of the Software Engineering Institute and researches software and Internet security flaws as well as works to improve software and Internet security. The National Cyber Security Authority is Israel's CERT, whereas the National Cyber Security Centre is the UK's CERT.
31. Which of the following organizations is not typically involved in post-incident communications?

    1. Developers
    2. Marketing
    3. Public relations
    4. Legal

    Answer:

    A. Post-incident communication often involves marketing and public relations staff who focus on consumer sentiment and improving the organization's image, whereas legal often reviews statements to limit liability or other issues. Developers are typically not directly involved in post-incident communications and are instead working on ensuring the security of the applications or systems they are responsible for.
32. Tom is building his incident response team and is concerned about how the organization will address insider threats. Which business function would be most capable of assisting with the development of disciplinary policies?

    1. Information security
    2. Human resources
    3. Legal counsel
    4. Senior management

    Answer:

    B. Although all of these functions are likely able to provide important advice on disciplinary policies, the human resources team has primary responsibility for employee relations and would be the best team to include for this purpose.
33. Craig is revising his organization's incident response plan and wants to ensure that the plan includes coordination with all relevant internal and external entities. Which one of the following stakeholders should he be most cautious about coordinating with?

    1. Regulatory bodies
    2. Senior leadership
    3. Legal
    4. Human resources

    Answer:

    A. All of these stakeholders should be included in the planning for an incident response program. However, Craig should be most careful about coordinating with external entities, such as regulatory bodies, because of their enforcement role. He should plan to coordinate more freely with internal entities, such as senior leadership, legal, and human resources.
34. The vulnerability management action plan that was sent to Jacinda notes that a critical application that her organization uses relies on an insecure version of a software package because of a long-standing workflow requirement. Jacinda's organization's best practices state that the organization will select the most secure option that also permits business to be conducted. What should Jacinda do?

    1. Mark the vulnerability as “ignored.”
    2. Change the business requirements to enable the vulnerability to be handled.
    3. Disable the service.
    4. Install a third-party patch for the service.

    Answer:

    B. Jacinda knows that reviewing business processes to see if they can be changed to use a secure version of the software package may require some business process changes but is often a possible solution. Ignoring the vulnerability isn't secure, turning off the service will disrupt the business itself, and third party patches rarely exist and are seldom a preferred solution.
35. What section of an incident response report provides a brief, clear summary of the incident, response activities, and current state of the incident?

    1. The timeline
    2. The scope statement
    3. The executive summary
    4. The documentation of evidence

    Answer:

    C. Executive summaries are brief, clear, and focused on conveying the important elements of the IR report. They are typically found at the beginning of the report and are intended to allow leaders and others who read the report to quickly grasp and understand the content of the report.
36. Ian wants to prepare his organization for communications with the media as part of incident related public relations. What should he recommend that his organization do to prepare?

    1. Build a list of phrases and topics to avoid.
    2. Hire a reputation defense firm.
    3. Engage legal counsel.
    4. Conduct media training.

    Answer:

    D. Ian knows that media training is a common preparedness item for organizations that may have to respond to the media in the event of an incident. Building a list of phrases and topics to avoid is difficult before an incident and can be problematic if it becomes public. Engaging either legal counsel or a reputation defense firm does not prepare the organization itself for engaging with the media but may be part of post or during the incident activities if the organization feels it to be necessary.
37. Jason is required to notify the company that provides credit card processing services to his organization if an incident impacting credit card data occurs. What type of communications does he need to perform?

    1. Regulatory reporting
    2. Customer communications
    3. Law enforcement communications
    4. None of the above

    Answer:

    D. Payment card industry requirements are contractual, not regulatory. Jason's organization is the customer, and law enforcement communication is not required by PCI.
38. The incident response report that Kathleen has prepared includes the following statement:

    “Unnecessary services including HTTP and FTP should be disabled on all devices of this type that are deployed.”

    What incident response reporting component will most commonly include this type of statement?

    1. Scope
    2. Executive summary
    3. Recommendations
    4. Timeline

    Answer:

    C. The recommendations section of an incident response report will have specific suggestions for changes that will help prevent or limit the impact of future incidents. This statement provides more detail than would typically be found in an executive summary. Timelines specify when something happened but don't make recommendations, and scope detail provides information about the scale and impacted systems or services from an incident.
39. What common score is used to help with prioritization of vulnerability remediation in many organizations?

    1. CVE
    2. ATT\&CK
    3. CVSS
    4. PASTA

    Answer:

    C. The common vulnerabilities scoring system (CVSS) score provides a numerical score that reflects the severity of a vulnerability and is thus useful for prioritization. Common vulnerabilities and exposure (CVE) provides a way to identify and catalog vulnerabilities. ATT\&CK is a framework used to define adversarial tactics and techniques, and PASTA is a threat modeling process.
40. Olivia has been notified that a vulnerability has recurred on a server after being marked as remediated through a compensating control by an administrator. Which of the following is the most likely reason that a vulnerability may recur in this circumstance?

    1. An attacker has removed the patch to expose the vulnerability.
    2. The system has been reinstalled by the administrator.
    3. A patch has caused the compensating control to fail.
    4. The service has been re-enabled by a user.

    Answer:

    C. A common scenario for compensating controls and work-arounds is that a follow-up patch causes the fix to no longer work. This may be because settings are changed or because the service or system has been modified in ways the compensating control did not anticipate. It is less likely that an attacker would remove a patch, or that the system would be reinstalled without re-applying the remediation, and in most environments, users should not be able to change server configurations.
41. The incident response report that Brian is reading includes a statement that says “Impacted systems were limited to those in the organization's AWS VPC.” What part of an incident response report will typically contain this type of information?

    1. The timeline
    2. The evidence statement
    3. The impact statement
    4. The scope statement

    Answer:

    D. Scope statements are used to explain and define which systems, services, or infrastructure components were part of an incident. Timelines are used to show when events occurred in relation to each other. Evidence is provided as part of a report to show what was found and how it was interpreted. Impact statements describe what the incident's results or outcome was for the organization.
42. Nila's incident response team has discovered evidence of an employee who may have been engaged in criminal activity while they were conducting an incident investigation. The team has suggested that law enforcement should be contacted. What significant concern should Nila raise about this potential communication?

    1. Law enforcement can't enforce organizational policy.
    2. Law enforcement engagement may hinder the organization's ability to respond or operate.
    3. Law enforcement involvement may create communications issues.
    4. Law enforcement may arrest a critical employee.

    Answer:

    B. Since the violation is only an organizational policy, Nila should note that law enforcement engagement may hinder the organization's ability to respond or operate. Law enforcement isn't being asked to enforce organizational policy, the more pressing issue is interruption of business instead of communications issues, and if the employee violated the law an arrest may happen anyway.
43. Sameer wants to establish and track a metric for his organization that will help him know if his IoC monitoring processes are working well. Which of the following metrics is best suited to determining if IoCs are being effectively captured and analyzed?

    1. Mean time to detect
    2. Mean time to respond
    3. Mean time to remediate
    4. Mean time to compromise

    Answer:

    A. Sameer knows that mean time to detect should be lower if IoCs are being effectively captured, correlated, and analyzed. Mean time to respond measures the time from detection to assessing the event as an incident and activating the process. Mean time to remediate is a much more complex measure to provide a metric for since each incident's size, scope, and complexity will all influence the mean time to remediate. This metric requires more nuanced communication and explanation than a simple number on a report in many cases and may benefit from granular reporting describing types of incidents as well as their impact and scope. Mean time to compromise is not a metric defenders will typically track.
44. Sameer is continuing to improve his metrics to report to his organization's board of directors. The board has requested that he include alert volumes in his reporting. What issue should Sameer discuss with the board after receiving this request?

    1. High-alert volumes indicate poor incident response processes.
    2. Low-alert volumes indicate effective incident response processes.
    3. Alert volume is not an effective security metric.
    4. Alert volume requires other measures like number of patches installed to be an effective security metric.

    Answer:

    C. Alert volume is not an effective security metric because it is highly impacted by tuning as well as external factors like the number of probes and attacks. High-alert volumes don't indicate a poor incident response process but may indicate poor tuning or a high number of events. Low-alert volumes may similarly indicate poor tuning or events that are not being detected. Correlating the number of patches with alert volume does not produce a useful metric.
45. What important incident response report section relies heavily on NTP to be successful?

    1. The executive summary
    2. The recommendations
    3. The timeline
    4. The scope statement

    Answer:

    C. Network Time Protocol (NTP) is used to synchronize clocks and thus keeps log entries set to the proper time. Without synchronized time between systems, log entries can be extremely difficult to correlate, and timelines are difficult to build properly.
46. What type of agreement between two organizations is a common inhibitor to remediation because of uptime requirements?

    1. An NDA
    2. An SLA
    3. A TLA
    4. A KPI

    Answer:

    B. Service level agreements often have uptime requirements included in their metrics and measures. Since patching may require systems or services to be offline, an SLA is a common inhibitor to remediation. Nondisclosure agreements (NDAs) and key performance indicators (KPIs) are not common inhibitors to remediation, and a TLA is a three-letter acronym!
47. Valerie needs to explain CVSS score metrics to her team. Which of the following is not part of the basic metric group for CVSS scores?

    1. The attack vector
    2. The maturity of the exploit code
    3. The attack complexity
    4. The privileges required

    Answer:

    B. The base metric group for CVSS includes the attack vector, the attack complexity, the privileges required, user interaction, and four impact metrics: confidentiality, integrity, availability, and scope. The maturity of exploit code is part of the temporal metric group, not the basic metric group.
48. The scientific instrument that Chas is responsible for has multiple critical severity vulnerabilities in its operating system and services. The device cannot be patched according to instructions from the vendor who provides it. Which of the following is not an appropriate compensating control in this scenario?

    1. Place a network security device configured to prevent access to the system between the instrument and the network.
    2. Install vendor patches against recommendations.
    3. Disable network connectivity to the device.
    4. Place the device on a protected network segment.

    Answer:

    B. Patching against vendor recommendations is the only control on this list that does not meet business requirements. Using a firewall device, disabling network connectivity, and moving the device to an isolated and secure network segment are all common compensating controls in this type of scenario.
49. Hui's incident response report includes log entries showing that a user logged in from another country, despite living and working in the country that the company Hui works for is located in. What incident response report section is most likely to contain this type of information?

    1. The impact section
    2. The scope section
    3. The evidence section
    4. The timeline section

    Answer:

    C. Log entries showing logins from a country where the employee does not work or reside are an example of evidence that may be included in an incident response report.
50. Melissa is conducting a root-cause analysis. Which of the following is not a common step in RCA processes?

    1. Identify problems and events.
    2. Establish a timeline.
    3. Differentiate causal factors and the root cause.
    4. Implement compensating controls.

    Answer:

    D. The four stages of RCA are identifying problems and events that occurred as part of the incident, establishing a timeline of events, differentiating causal factors and the root cause, and documenting the root-cause analysis. Root-cause analyses result in a report, which may then be used as part of preparation processes where compensating controls may be employed. Implementing compensating controls isn't typically part of the RCA process itself.
51. What information is typically included in a list of affected hosts in a vulnerability management report?

    1. Hostname and IP address
    2. IP address and MAC address
    3. Hostname and MAC address
    4. Hostname and subnet mask

    Answer:

    A. The hostname and IP address are commonly used to identify each vulnerable host in a vulnerability report. The hardware (MAC) address is not typically listed, and subnet masks are also not typically listed.
52. Hannah wants to establish a metric that will help her organization determine if their response process completes in a timely manner. Which common metric should she select to help assess this?

    1. Mean time to detect
    2. Mean time to report
    3. Mean time to respond
    4. Mean time to remediate

    Answer:

    D. Assessing whether incidents are remediated in a timely manner can help Hannah determine if IR completion is happening in a timely manner since remediation is the last nonreporting stage in the process and reporting is not typically a process where time to complete is critical to an organization.
53. Mikayla's team has determined that a previously remediated vulnerability has re-appeared after installation of a vendor supplied patch. What type of vulnerability management issue is this?

    1. Risk scoring
    2. Prioritization
    3. Mitigation
    4. Recurrence

    Answer:

    D. This is an example of recurrence and is something that should be reported on as part of Mikalya's ongoing vulnerability reporting and exception management process. No risk scoring or prioritization is mentioned, and while mitigation was performed, re-appearing vulnerabilities are recurrence, not mitigation.
54. Gurvinder wants to consider impact metrics like the integrity impact, availability impact, and compatibility impact of a vulnerability that is scored using CVSS. What metric group includes this information?

    1. Basic
    2. Environmental
    3. Temporal
    4. Residual

    Answer:

    A. The Base Metric Group for CVSS includes both exploitability metrics and impact metrics. The impact metric is made up of components covering confidentiality, integrity, and availability impact as well as scope.
55. Which of the following is not a type of stakeholder that will frequently need to understand an organization's overall vulnerability stance or status?

    1. Security practitioners
    2. Legal counsel
    3. Auditors
    4. Compliance stakeholders

    Answer:

    B. Legal counsel rarely needs to know an organization's vulnerability management status or stance. Security, audit, and compliance stakeholders do.
56. Which of the following CVSS scores indicates the highest impact to an organization?

    1. 9.6
    2. 7.5
    3. 3.2
    4. 1.3

    Answer:

    A. CVSS scores range from 0–10, with higher scores having greater impact, exploitability, temporal, and environmental factors. Without more context, the highest number will generally indicate the highest impact.
57. Expectations of time to remediate and time to patch by a vendor are both examples of what in a vulnerability management program?

    1. Service level objectives
    2. Risks
    3. Vulnerabilities
    4. Internal policies

    Answer:

    A. Service level objectives (SLOs) are part of a service level agreement (SLA) with a vendor. Time to remediate and time to patch are not risks or vulnerabilities, and internal policies do not determine vendor expectations without a contract or agreement in place.
58. What issue is organizational governance likely to cause in a vulnerability management program?

    1. It may prevent vulnerabilities from being patched or compensating controls being used.
    2. It may increase the number of vulnerabilities that need patched.
    3. It may slow down patching.
    4. It may limit the vulnerabilities that will be patched.

    Answer:

    C. Governance processes are most likely to lead to slower patching processes because of approval requirements. They typically do not prevent patches from being installed or the use of compensating controls, although it may take some time to identify which option will be put in place. It typically doesn't increase the number of vulnerabilities that need to be patched nor do they typically limit what vulnerabilities will be patched.
59. Jacob has initiated the incident response process in his organization. IoCs have been identified, and Jacob is ready to take the next step in the process. What typically happens next?

    1. Legal counsel is notified.
    2. Incident responders collect forensic data.
    3. Law enforcement is notified.
    4. Incident responders determine if it is a real incident.

    Answer:

    D. Just because IoCs exist doesn't mean that an incident has occurred. Instead, responders need to analyze the data available and to look for additional information that will tell if the incident is a real incident or a false positive. Notifying counsel or law enforcement happens after an incident is verified and only if needed. Collecting forensic data happens once the organization determines that an incident has occurred and wants to investigate it.
60. Asha wants to reduce the alert volumes her team are dealing with due to the numbers of emails and SMS alerts they are receiving. Which of the following is most likely to help reduce the volume of alerts?

    1. Tune alerting thresholds.
    2. Subscribe to more IoC feeds.
    3. Create additional IoCs.
    4. Set work hours to avoid after hours alerts.

    Answer:

    A. Asha knows that alert volumes need to be tuned to be useful and will spend her time tuning alerts to ensure that only the important alerts escalate. Disabling alerts outside of working hours is a terrible idea and might cause her team to miss a critical alert. Subscribing to more IoC feeds or creating additional IoCs are both likely to increase alert volume.
61. What NIST standard provides information on incident handling practices?

    1. NIST SP 800-61
    2. ISO 27001
    3. NIST SP 800-53
    4. SOC 2

    Answer:

    A. NIST SP 800-61 is NIST's Computer Security Incident Handling guide and provides information on incident handling standards. NIST SP 800-53 describes security and privacy controls for information systems and organizations. ISO 27001 and SOC 2 are not NIST standards.
62. Jaime want to consider critical components of public relations as part of her incident communications plan. What two topics are best aligned to this?

    1. Customer and law enforcement communications
    2. Customer and executive communications
    3. Customer and media communications
    4. Customer and legal counsel communications

    Answer:

    C. Jessica knows that communicating with customers and the media are both critical parts of public relations. Law enforcement, executive communications, and legal counsel communications are part of incident response communications but not necessarily part of public relations.
63. Annie's organization makes divisional administrators responsible for patching vulnerabilities after they are notified of them using a ticketing system. Annie has noticed that the administrators are not promptly patching systems. What should she do to most effectively address this issue?

    1. Switch notification to automated emails.
    2. Invest in an awareness and training campaign.
    3. Use the vulnerabilities to compromise the systems to prove a point.
    4. Involve HR due to a lack of job performance.

    Answer:

    B. Awareness and training programs are an important part of vulnerability management practices, and Annie can expect that if administrators understand their roles, job requirements, and the importance of patching that they will more promptly patch systems they are responsible for. Switching notification styles is unlikely to have a major impact, attacking systems is not a common or typically acceptable practice in most organizations, and escalating to HR may lead to resentment and shouldn't be her first option.
64. Henry's organization handles credit card data as part of their operations. What type of vulnerability management report is Henry most likely to need to run due to this?

    1. PCI compliance reporting
    2. GLBA compliance reporting
    3. A list of compromised systems
    4. A list of unpatched systems

    Answer:

    A. Henry's organization is most likely to need to be compliant with the Payment Card Industry (PCI) standards and thus will need to run reports that will help prove PCI compliance. A list of compromised or unpatched systems is not required for PCI-DSS.
65. Jen has discovered that many systems in her organization are being deployed with a vulnerable service active. What solution is best suited to addressing this type of issue in a large organization?

    1. An awareness program
    2. Compensating controls
    3. Changing business requirements
    4. Configuration management

    Answer:

    D. Jen knows that configuration management is an appropriate solution to ensure that organization wide standards are met and that it can help with this type of issue. She may also need to implement an awareness program to ensure that admins are appropriately configuring systems before deployment, but configuration management is the more complete fix. Compensating controls aren't indicated by the question, and changing business requirements isn't a demonstrated need either.
66. An incident report should indicate the individuals involved, as well as which of the following items?

    1. The hardware addresses of the systems involved
    2. The time frame the event or incident occurred
    3. A written statement from each individual interviewed
    4. A police report

    Answer:

    B. Incident reports typically need to include who, what, when, where, and why. Hardware addresses, written statements from those involved, and police reports are rarely included.
67. Jason has defined the problem as part of a root-cause analysis effort. What step typically comes next in RCA?

    1. Collecting data about the problem
    2. Determining the root cause of the problem
    3. Determining potential causal factors
    4. Analyzing the causes

    Answer:

    A. Root-cause analysis requires data to proceed, and Jason knows that his next step is to collect data. Then he will proceed to determining causal factors, identifying the root cause, and prioritizing causes.
68. Mean time to respond is an example of what?

    1. An incident response report target
    2. An industry standard SOW
    3. An industry standard SLA
    4. An incident response KPI

    Answer:

    D. Mean time to respond is a key performance indicator (KPI) for incident response.
69. What information is gathered as part of a lessons learned exercise conducted at the end of an incident response process?

    1. Issues that will positively impact future incident response processes
    2. Both positive and negative lessons learned during the process
    3. Issues that will negatively impact future incident response processes
    4. Root causes of the incident

    Answer:

    B. Lessons learned should include both positive and negative lessons learned. This ensures that organizations reinforce what goes well and improve what goes badly. Root causes are identified as part of a root-cause analysis, not as part of lessons learned.
70. Jason wants to quickly understand the content of an incident report. What should he read?

    1. The scope statement
    2. The timeline
    3. The executive summary
    4. The evidence

    Answer:

    C. Executive summaries should be short and to the point and are intended to allow readers to quickly understand the content of the report without reading the full report. Scope statements describe the scale and impacted systems or services, timelines list when events happened, and evidence provides detailed information about the incident that support analysis or theories.
71. What important role does criticality and impact information play in organizational use of CVSS scores?

    1. It helps with prioritization.
    2. It determines if a patch should be installed.
    3. It determines if a compensating control should be used.
    4. It helps prevent recurrence.

    Answer:

    A. Combining criticality and impact information organizations can determine both how dangerous the issue is and how likely it is to impact them. That means that CVSS can provide a useful rating to prioritize their efforts given limited resources and time. Recurrence is not impacted by criticality or impact, and instead tends to point to technical or procedural issues. Compensating controls are used when a patch is not available or the fix does not meet the business needs of an organization. Patch installation is determined by administrators based on testing and organizational policies which may be influenced by criticality and impact for prioritization.
72. Natalie has signed a service level agreement with a customer that specifies performance requirements for a service that her company provides. How is this most likely to impact her ability to remediate vulnerabilities on the underlying containerized services that provide the service?

    1. It will require Natalie to seek customer approval for each patch that is deployed via their governance process.
    2. It will require Natalie to ensure that the service is not disrupted when new, patched containers are deployed and vulnerable containers are disabled.
    3. It will allow as much downtime as needed as patches are deployed to the containerized services.
    4. It will prevent Natalie from upgrading the legacy systems the customer relies on.

    Answer:

    B. The fact that Natalie's organization uses containers will likely help her to avoid unexpected or unwanted downtime, but Natalie still needs to ensure the service is not interrupted as she deployed patched containers and removes the old vulnerable containers. An SLA does not require external governance; instead, it determines key aspects of the performance of the service like uptime, and downtime is rarely unlimited. Otherwise, an SLA wouldn't be in use. Finally, there is no mention of legacy systems in this question.
73. Angela's organization has discovered that their Windows workstations have a vulnerability that was discovered more than a year ago. What solution is best suited to handling this known vulnerability?

    1. Patching
    2. Awareness, education, and training
    3. Changing business requirements
    4. Compensating controls

    Answer:

    A. Angela knows that simply patching it is likely the best option. A well-known Windows vulnerability will typically have an available patch. She should find out why her organization has failed to patch it and address the issue. That may require awareness or training once she figures out why the patching isn't happening! Compensating controls are typically not necessary for an older, known vulnerability in a supported product because patches usually exist, and there's no indication in the question of a business process change that would help.
74. Jacob wants to update mitigation notes for a vulnerability on a server. Which of the following is not a common mitigation option?

    1. Installing a patch
    2. Deploying a compensating control
    3. Disabling a service or software
    4. Turning the system off

    Answer:

    D. Simply turning a system off is not a common mitigation since systems typically have a purpose for running, and turning them off will create a business disruption. While turning systems off may be done in exigent circumstances, patching, deploying a compensating control, or disabling a vulnerable service are far more common.
75. Which of the following is the most critical to have involved in incident escalation processes?

    1. End users
    2. Legal
    3. Management
    4. Law enforcement

    Answer:

    C. It is critical to involve management in incident escalation processes to allow for proper escalation and response. Legal and law enforcement experts are engaged on an as-needed basis, and end users are not typically required to be involved in escalation.
76. Gurvinder's organization is required to report breaches within 24 hours of the breach being detected, regardless of how far into the investigation the organization is. What type of requirement is most likely to drive this type of communication?

    1. Contractual requirements
    2. Social media requirements
    3. Regulatory requirements
    4. Reputational requirements

    Answer:

    C. Regulatory requirements often have specific timeframes for communication, regardless of the state of the incident response process. Contractual requirements tend to offer the organization more flexibility in reporting. Social media does not create requirements, and reputation may benefit from timely notification but does not result in requirements either.
77. Xuan's organization uses an old, no longer updated or sold software package that has an embedded web server that it exposes on every workstation that runs the software allowing file transfer between workstations. During a vulnerability scan the web browser was highlighted as a critical vulnerability. Which of the following solutions should Xuan recommend to best resolve the issue?

    1. An awareness program
    2. Compensating controls
    3. Changing business requirements
    4. Configuration management

    Answer:

    C. Xuan should recommend that the organization change business practices. There are many other ways to exchange files that do not require a vulnerable software package, and change in process would resolve this. Awareness, compensating controls, and configuration management do not address the business need.
78. Jackie is reviewing the risk scores round in a vulnerability report and notes that the risk she is reviewing scores a 1.0. What recommendation should Jackie make about the vulnerability?

    1. It should be patched immediately because the risk score is high.
    2. The risk is very low and can likely be ignored.
    3. The risk is low and should be patched in the next patch cycle.
    4. It should be patched immediately because it is in the top 10 percent of risks.

    Answer:

    C. While a risk as low as 1.0 on the CVSS scale is unlikely to cause immediate harm, if a patch is available and does not introduce additional risk, it should still be installed at the next patch window.
79. Log entries are commonly found in what part of an incident response report?

    1. Recommendations
    2. Executive summary
    3. Evidence
    4. Timeline

    Answer:

    C. The evidence section of an incident response report often includes information like log entries. Log files typically don't show up in the executive summary, the timeline, or the recommendations section of the report.
80. Kathleen wants to build a prioritized list of vulnerabilities for her organization. What part of the CVSS metric will help her adjust the score to best match her organization's availability requirements?

    1. The base metric group
    2. The advanced metric group
    3. The temporal metric group
    4. The environmental metric group

    Answer:

    D. The environmental group includes information that takes an organization's specific requirements into account including availability requirements the organization itself establishes. Even if you're not familiar with the CVSS scoring system's three groupings (base, temporal, and environmental), you can likely answer a question like this by considering the likely meaning of each of these options.
81. Derek is the lead of his organization's finance and accounting team and has expressed concerns about installing patches because his team relies on the service that is being patched. Derek noted that the team is at a critical time because of annual financial reports. What type of inhibitor to remediation is this?

    1. A potential MOU violation
    2. A legacy system issue
    3. A business process interruption issue
    4. A potential SLA violation

    Answer:

    C. This is an example of a business process interruption issue. Organizations are often sensitive to downtime and outages that could be caused by patching and vulnerability remediation during sensitive or busy parts of their business cycle. This often drives “freezes” or other windows where patching may be paused or delayed. There is no mention of a MOU or SLA that would be breached, and the system is not described as being a legacy system, making these less likely choices.
82. What part of an incident response report describes detailed ways to avoid similar issues in the future?

    1. The executive summary
    2. Lessons learned
    3. The scope
    4. Evidence

    Answer:

    B. Incident response reports should include a lessons learned listing that describes ways to improve as well as how to avoid similar issues in the future. The executive summary is brief, and while it may point to lessons learned, it will not typically cover them in depth. The scope statement for an incident describes what systems, services, or other elements and assets of the organizations were impacted. Evidence provides information about how the incident was detected.
83. Potential compensating controls can be found in what section of a vulnerability management report?

    1. The mitigations section
    2. The risk scores
    3. The recurrence section
    4. The affected hosts list

    Answer:

    A. Compensating controls are an example of a mitigation technique and can be found as part of the mitigation recommendations.
84. The company that Amari works for uses an embedded system as part of a manufacturing process. The system relies on an operating system created by the machine's vendor and Amari's team has identified vulnerabilities during a network scan. What type of system should Amari identify this device as?

    1. A proprietary system
    2. A legacy system
    3. A primary system
    4. A secondary system

    Answer:

    A. This is an example of a proprietary system that may not use commonly available and supported operating systems or software. Legacy systems are out-of-date, often unsupported systems. Primary and secondary systems are not terms typically used to categorize vulnerable systems.
85. Amari wants to ensure that her team can meet her organization's service level agreement for the embedded system that has been identified as vulnerable. Which of the following compensating controls would be the most appropriate solution to allow the system to stay online while remaining secure?

    1. Install a hardware-based IDS between the system and the network.
    2. Place a hardware firewall between the system and the network.
    3. Disable the device's network connection.
    4. Install a nonproprietary operating system on the embedded system.

    Answer:

    B. A hardware firewall will prevent the system from being remotely accessed if configured properly, protecting it from network-based attacks and acting as an appropriate compensating control. An IDS will only detect attacks and won't stop them. Disabling the network connection for the device entirely is likely to impact the service level agreement for the device, and installing another OS is like impossible.
86. Amari has deployed a compensating control to protect the vulnerable embedded system that she is responsible for. What step should she take next?

    1. Create an incident report and distribute it to appropriate recipients.
    2. Remove the device from the vulnerability scanning process to avoid continued false positives.
    3. Note the compensating control and flag the device for follow-up to see if patches become available.
    4. Flag the vulnerabilities previously discovered as false positives.

    Answer:

    C. Amari should note the compensating control and ensure that periodic review is done to determine if new patches are required or any additional compensating controls or maintenance of the firewall device is required. No incident occurred, meaning an incident report is not necessary. The device should not be removed from the vulnerability scanning system because it remains on the network. The vulnerabilities were not false positives and should not be treated as such.
87. NIST provides recommendations for communication with the media as part of incident response. Which of the following is a NIST recommended preparation for working with the media?

    1. Pre-writing all incident communications before incident occur
    2. Holding media practice sessions for incident responders as part of IR exercises
    3. Creating procedures on media avoidance as part of incident response planning
    4. Contacting law enforcement to prepare for media concerns

    Answer:

    B. Holding media practice sessions for incident responders as part of IR exercises is a NIST-recommended practice. Incident communication examples and templates can be prepared, but all incident communications cannot be written before incidents occur. Avoiding the media or contacting law enforcement to help with media concerns is also not NIST-recommended procedures.
88. Michele's root-cause analysis has determined a number of events that contributed to the problem but were not the root cause. What has she identified?

    1. Compensating controls
    2. Causal factors
    3. Branch causes
    4. Nonroot causes

    Answer:

    B. Causal factors are events that contribute to an incident but that are not the root cause.
89. What three groups of metrics make up a CVSS score?

    1. The Core Metric Group, the Impact Metric Group, and the Organizational Metric Group
    2. The Core Metric Group, the Temporal Metric Group, and the Organizational Metric Group
    3. The Basic Metric Group, the Impact Metric Group, and the Environmental Metric Group
    4. The Basic Metric Group, the Temporal Metric Group, and the Environmental Metric Group

    Answer:

    D. CVSS scores are based on three sets of metrics: the Base, Temporal, and Environmental groups.
90. Which of the following questions is not typically answered as part of an incident response report?

    1. Who?
    2. When?
    3. What?
    4. With whom?

    Answer:

    D. It may seem like common sense, but answering the five Ws (who, what, when, where, and why) is common in incident response reports. With whom, however, is not one of the five Ws.
