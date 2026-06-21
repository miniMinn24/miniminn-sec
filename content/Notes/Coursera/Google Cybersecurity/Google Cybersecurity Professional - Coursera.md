---
date: 2026-03-05
tags:
  - cybersecurity
  - course
  - frameworks
  - riskassessment
  - SIEM
author: miniMinn
category:
  - note
---
> **View all the Google Cybersecurity labs and walkthroughs here:** [[Activities & Labs]]

# Course 1 - Foundations of Security

## Module 1: Foundations of Cybersecurity

**Security analysts** - responsible for monitoring and protecting information and systems.

- Protecting computer and network systems
- Installing prevention software
- Conducting periodic security audits

Two basic parts of security:

- **Operations**: Responding to detections and doing investigations
- **Projects**: Working with other teams to build new detections or improve the current detection.

> [!quote]
> A **playbook** is a list of how to go through a certain detection, and what the analyst needs to look at in order to investigate those incidents.

## Module 2: The Evolution of Cybersecurity
#### Past Cybersecurity Attacks
**Computer Virus** is a Malicious code written to interfere with computer operations and cause damage to data and software. Now commonly referred to as **Malware**.  
- **Malware**: Software designed to harm devices or networks.

> [!quote] Morris Worm
> Created by Robert Morris In 1988. The program crawled the web and installed itself onto other computers to tally the number of computers that were connected to the internet. Failed to keep track of compromised computers and continued to re-install itself until the computers ran out of memory and crashed.  
> *About 6,000 computers were affected (10% of the internet at the time*

#### Attacks in Digital Age
The **LoveLetter** attack was an example of social engineering. Social engineering is a <mark style="background: #D2B3FFA6;">manipulation technique</mark> that exploits human error to gain private information, access, or valuables.

**Phishing** is the use of digital communications to trick people into revealing sensitive data or deploying malicious software.

> [!quote] Equifax Breach
> During the Equifax breach, over 143 million customer records were stolen, and the breach affected approximately 40% of all Americans.  
> ![[attachments/Pasted image 20260422201315.png]]

> [!INFO]- Identify: Methods of Attacks
> - **Malware**: A software designed to harm devices or networks.  
> - **Virus**: A malware program that modifies other computer programs by inserting its own code to damage and/or destroy data.  
> - **Worm**: Malware that self-replicates, spreading across the network and infecting computers.  
> - **Ransomware**: A malicious attack during which threat actors encrypt an organization's data and demand payment to restore access.  
> - **Spyware**: Malicious software installed on user's computer without their permission, which is used to spy on and steal user data.  
> - **Phishing**: The use of digital communications to trick people into revealing sensitive data or deploying malicious software.  
> - **Spear Phishing**: A malicious email attack targeting a specific user or group of users that appears to originate from a trusted source.  
> - **Whaling**: A form spear phishing during which threat actors target executive in order to gain access to sensitive data.  
> - **Business Email Compromise (BEC)**: An attack in which a threat actor impersonates a known source to obtain a financial advantage.  
> - **Vishing**: The exploitation of electronic voice communication to obtain sensitive information or to impersonate a known source.  
> - **Social Engineering**: A manipulation technique that exploits human error to gain unauthorized access to sensitive, private, and/or valuable data.  
> - **Social Media Phishing**: An attack in which a threat actor collects detailed information about their target on social media sites before initiating an attack.  
> - **Watering Hole Attack**: An attack in which a threat actor compromises a website frequently visited by a specific group of users.  
> - **Physical Social Engineering**: An attack in which a threat actor impersonates an employee, customer, or vendor to obtain unauthorized access to a physical location.  
> - **USB Baiting**: An attack in which a threat actor strategically leaves a malware USB stick for an employee to find and unknowingly infect a network.  

#### Intro to the eight CISSP security domains
![[attachments/Pasted image 20260423195514.png]]

1. **Security and Risk Management**
	Defines security goals and objectives, risk mitigation, compliance, business continuity, and the law.  
> Updating company policies related to private health info if a change is made to a federal compliance regulation.
2. **Asset Security**
	Secures digital and physical assets. It's also related to the storage, maintenance, retention, and destruction of data.
> Make sure confidential in that old equipment is properly disposed of and destroyed.
3. **Security architecture and engineering**
	Optimizes data security by ensuring effective tools, systems, and process are in place.
> Setting up firewalls
4. **Communication and network security**
	Manage and secure physical networks and wireless communications.
> Analyse user behaviors - users connecting to unsecure network.
5. **Identity and access management**
	Keeps data secure, by ensuring users follow established policies to control and manage physical assets, like office spaces, and logical assets, such as networks and applications.
> Setting up employee key cards access to building.
6. **Security assessment and testing**
	 Conducting security control testing, collecting and analyzing data, and conducting security audits to monitor for risks, threats and vulnerabilities.
> Limiting access to payroll information.
7. **Security operations**
	Conducting investigations and implementing preventative measures.
> When an unknown device is connected to your network, you stop it following company's policies.
8. **Software development security**
	Uses secure coding practices, which are a set of recommended guidelines that are used to create secure applications and services.
> Advising password policies or any other user data are secured when a new mobile app is being developed.

#### Understand Attackers
**Advanced Persistent Threats (APTs)**: Tends to research their targets in enterprise environments and can remain undetected. They can damage critical infrastructure and gaining access to intellectual property (trade secrets).  

**Insider Threats**: Abusing their authorized access to harm an organization (sabotage, corruption, leaks, espionage).  
**Hacktivists**: Driven by a political agenda (demonstrations, propaganda, social change campaigns, fame).  

##### Hacker types
- **Authorized hackers**: Follows a code of ethics, adhere to the law to conduct risk evaluations (safeguard from threat actors).
- **Semi-authorized hackers**: Researchers of vulnerabilities but doesn't take advantage of it.
- **Unauthorized hackers**: Doesn't follow or respect the law, just to collect and sell confidential data for their missions.

## Module 3: Protect against threats, risks, and vulnerabilities

#### Introduction to security frameworks and controls

**Security Frameworks**: Guidelines used for building plans to help mitigate risk and threats to data and privacy.  

**Purpose of Security Frameworks**
- Protecting PII
- Securing financial information
- Identifying security weaknesses
- Managing organizational risks
- Aligning security with business goals

##### Components of security frameworks

![[attachments/Pasted image 20260429115523.png]]
1. **Identifying and documenting security goals**
> ​For example, an organization may have a goal to ​align with the E.U.'s General Data Protection Regulation, ​also known as GDPR (a data protection law established to ​grant European citizens more control ​over their personal data)
2. **Setting guidelines to achieve security goals**
> For example, when implementing ​guidelines to achieve GDPR compliance, ​your organization may need to develop ​new policies for how to handle ​data requests from individual users.
3. **Implementing strong security processes**
> In the case of GDPR, ​a security analyst working for ​a social media company may help design ​procedures to ensure the organization ​complies with verified user data requests. 
4. **Monitoring and communicating results**
> As an example, you may monitor ​your organization's internal network and report ​a potential security issue affecting ​GDPR to your manager or regulatory compliance officer. 

**Security controls**: Safeguards designed to reduce specific security risks (like awareness training to employees).  

#### Secure design
**CIA Triad**: A foundational model that helps inform how organizations consider risk when setting up systems and security policies.  

![[attachments/Pasted image 20260429120737.png]]

- **Confidentiality**: Only authorized users can access specific assets or data.
> ​For example, strict access controls that ​define who should and should not have access to data, ​must be put in place to ensure ​confidential data remains safe.
- **Integrity**: Data is correct, authentic and reliable.
> To maintain integrity, ​security professionals can use a form of ​data protection like encryption ​to safeguard data from being tampered with.
- **Availability**: Data is accessible to those who are authorized to access it.

**Asset** is an item perceived as having value to an organization.

##### NIST Cybersecurity Framework (CSF)
National Institute of Standards and Technology (NIST) U.S.-based agency. A voluntary framework that consists of standards, guidelines, and best practices to manage cybersecurity risk.  
Important to be familiar with it as it is used by professionals as a **baseline.**  

#### Controls, Frameworks, and Compliance

##### The Federal Energy Regulatory Commission - North American Electric Reliability Corporation (FERC-NERC)
**FERC-NERC** is a regulation that applies to organizations that work with electricity or that are involved with the U.S. and North American power grid. These types of organizations have an obligation to prepare for, mitigate, and report any potential security incident that can negatively affect the power grid. They are also legally required to adhere to the Critical Infrastructure Protection (**CIP**) Reliability Standards defined by the FERC.

##### The Federal Risk and Authorization Management Program (FedRAMP®)
FedRAMP is a U.S. federal government program that standardizes security assessment, authorization, monitoring, and handling of cloud services and product offerings. Its purpose is to provide consistency across the government sector and third-party cloud providers.

##### Center for Internet Security (CIS®)
CIS is a nonprofit with multiple areas of emphasis. It provides a set of controls that can be used to safeguard systems and networks against attacks. Its purpose is to help organizations establish a better plan of defense. CIS also provides actionable controls that security professionals may follow if a security incident occurs.

##### General Data Protection Regulation (GDPR)
GDPR is European Union (E.U.) general data regulation that protects the processing of E.U. residents' data and their right to privacy in and out of E.U. territory. For example, if an organization is not being transparent about the data they are holding about an E.U. citizen and why they are holding that data, this is an infringement that can result in a fine to the organization. Additionally, if a breach occurs and an E.U. citizen's data is compromised, they must be informed. The affected organizations have 72 hours to notify the E.U. citizen about the breach.

##### Payment Card Industry Data Security Standard (PCI DSS)
PCI DSS is an international security standard meant to ensure that organizations storing, accepting, processing, and transmitting credit card information do so in a secure environment. The objective of this compliance standard is to reduce credit card fraud.

##### The Health Insurance Portability and Accountability Act (HIPAA)
HIPAA is a U.S. federal law established in 1996 to protect patients' health information. This law prohibits patient information from being shared without their consent. It is governed by three rules:
1. Privacy
2. Security
3. Breach notification

Organizations that store patient data have a legal obligation to inform patients of a breach because if patients' **Protected Health Information** (PHI) is exposed, it can lead to identify theft and insurance fraud. PHI relates to the past, present, or future physical or mental health or condition of an individual, whether it's a plan of care or payments for care. Along with understanding HIPAA as a law, security professionals also need to be familiar with the Health Information Trust Alliance (HITRUST®), which is a security framework and assurance program that helps institutions meet HIPAA compliance.

##### International Organization for Standardization (ISO)
ISO was created to establish international standards related to technology, manufacturing, and management across borders. It helps organizations improve their processes and procedures for staff retention, planning, waste, and services.

##### System and Organizations Controls (SOC type 1, SOC type 2)
The American Institute of Certified Public Accountants® (AICPA) auditing standards board developed this standard. The SOC1 and SOC2 are a series of reports that focus on an organization's user access policies at different organizational levels such as:
- Associate
- Supervisor
- Manager
- Executive
- Vendor
- Others

They are used to assess an organization's financial compliance and levels of risk. They also cover confidentiality, privacy, integrity, availability, security, and overall data safety. Control failures in these areas can lead to fraud.  

> Two suggestions to research: the **Gramm-Leach-Bliley Act** and the **Sarbanes-Oxley Act**


#### Heather: Protect sensitive data and information

> [!quote]
> We should make sure we're very deliberate about how it's handled and where it's stored, and that we understand where it's stored all the time.

#### Ethic in cybersecurity
**Security ethics**: Guidelines for making appropriate decisions as a security professional.  
- Privacy protection means safeguarding personal information from unauthorized use.
- Laws are rules that are recognized by a community and enforced by a governing entity.

##### United States standpoint on counterattacks 
In the U.S., deploying a counterattack on a threat actor is illegal because of laws like the Computer Fraud and Abuse Act of 1986 and the Cybersecurity Information Sharing Act of 2015, among others. You can only defend. The act of counterattacking in the U.S. is perceived as an act of vigilantism. A vigilante is a person who is not a member of law enforcement who decides to stop a crime on their own. And because threat actors are criminals, counterattacks can lead to further escalation of the attack, which can cause even more damage and harm. Lastly, if the threat actor in question is a state-sponsored hacktivist, a counterattack can lead to serious international implications. A hacktivist is a person who uses hacking to achieve a political goal. The political goal may be to promote social change or civil disobedience. 

##### International standpoint on counterattacks
The International Court of Justice (ICJ), which updates its guidance regularly, states that a person or group can counterattack if: 
- The counterattack will only affect the party that attacked first.
- The counterattack is a direct communication asking the initial attacker to stop.
- The counterattack does not escalate the situation.
- The counterattack effects can be reversed.

> [!quote]
> When you're faced with one of these difficult decisions, it's good to think about what would be the consequences of your decision."

## Module 4: Cybersecurity tools and programming languages
#### Common cybersecurity tools
**Log**: A record of events that occur within an organization's systems  
**Security Information and Event Management (SIEM) tool**: An application that collects and analyzes log data to monitor critical activities in an organization.
- [Splunk](https://www.splunk.com/): A mature, highly customizable platform known for its powerful Search Processing Language (SPL), extensive third-party integrations, and support for on-premises, cloud, and hybrid deployments.
- **Google's Chronicle**: cloud-native, serverless SIEM built on Google’s infrastructure, emphasizing automatic data normalization, massive scalability, and a flat-rate pricing model tied to data ingestion volume. 

**Playbook**: A manual that provides details about any operational action.  
**Network protocol analyzer (packet sniffer)**: A tool designed to capture and analyze data traffic within a network - `tcpdump` and `wireshark`.  

#### Introduction to Linux, SQL, and Python
**Programming**: Used to create a specific set of instructions for a computer to execute tasks.  
**Linux**: An open-source operating system (e.g., examining logs).  
**Structured Query Language (SQL)**: A programming language used to create, interact with, and request information from a database.  
**Database**: An organized collection of information or data.  
**Python**: Used to perform tasks that are repetitive and time-consuming, and that require a high level of detail and accuracy.  

---
# Course 2 - Play It Safe - Manage Security Risks

## Module 1: Security domains

#### CISSP security domains
**Security posture**: An organization's ability to manage its defense of critical assets and data, and react to change.  

![[attachments/Pasted image 20260430150833.png]]
#### 1. Security and risk management
Focused on defining security goals and objectives, risk mitigation, compliance, business continuity, and legal regulations.  
> Reducing risks to critical assets (like PII) by defining security goals and objectives.

**Risk mitigation**: The process of having the right procedures and rules in place to quickly reduce the impact of a risk like a breach.  
**Business continuity**: An organization's ability to maintain their everyday productivity by establishing risk and disaster recovery plans.  

#### 2. Asset security
Focused on securing digital and physical assets. It's also related to the storage, maintenance, retention, and destruction of data.  
> PII/SPII should be securely handled and protected, whether stored on a computer, transferred over a network or physically collected. **Following organization's policies**.

#### 3. Security architecture and engineering
Focused on optimizing data security by ensuring effective tools, systems, and processes are in place to protect an organization's assets and data.  
> Having policies that encourage users to recognize and report security concerns.

**Shared responsibility**: All individuals within an organization take an active role in lowering risk and maintaining both physical and virtual security.  

#### 4. Communication and network security
Focused on managing and securing physical networks and wireless communications.  
> Employees working remotely in public spaces need to be protected from vulnerabilities by having security team members remove access to those types of communication channels at the organization level.

#### 5. Identity and access management (IAM)
Focused on access and authorization to keep data secure, by making sure users follow established policies to control and manage assets.  
- Identification (username, biometric data, etc.)
- Authentication (password, pin, etc.)
- Authorization (level of access, takes place after Identification has been confirmed.)
> To reduce the overall risk to systems and data.

#### 6. Security assessment and testing
Focused on conducting security control testing, collecting and analyzing data, and conducting security audits to monitor for risks, threats, and vulnerabilities.  
> Examining organizational goals and objectives, testing evaluations and security assessment reports to improve existing controls or implement new controls.

#### 7. Security operations
Focused on conducting investigations and implementing preventative measures.  
> Once a security incident has been identified, a  heightened sense of urgency is required in order to minimize potential risks to the organization.

#### 8. Software development security
Focused on using secure coding practices.  
> Performing a secure design review during the design phase, secure code review and pentesting during deployment.

> [!quote]
> Cybersecurity path wasn't a linear path.

#### Threats, risks, and vulnerabilities

#### Threat
Any circumstance or event that can negatively impact assets (e.g., social engineering attacks).
- **Insider threats**: Staff members or vendors abuse their authorized access to obtain data the may harm an organization.
- **Advanced persistent threats (APTs)**: A threat actor maintains unauthorized access to a system for an extended period of time.  

#### Risk
Anything that can impact the confidentiality, integrity, or availability of an asset (e.g., lack of backup processes).  
- **External risk**: Anything outside the organization that has the potential to harm organizational assets, such as threat actors attempting to gain access to private information
- **Internal risk**: A current or former employee, vendor, or trusted partner who poses a security risk
- **Legacy systems**: Old systems that might not be accounted for or updated, but can still impact assets, such as workstations or old mainframe systems. For example, an organization might have an old vending machine that takes credit card payments or a workstation that is still connected to the legacy accounting system.
- **Multiparty risk**: Outsourcing work to third-party vendors can give them access to intellectual property, such as trade secrets, software designs, and inventions.
- **Software compliance/licensing**: Software that is not updated or in compliance, or patches that are not installed in a timely manner
![[attachments/Pasted image 20260430160742.png]]
- **Low-risk asset**: Information that would not harm the organization's reputation or ongoing operations, and would not cause financial damage if compromised (e.g., <mark style="background: #BBFABBA6;">public research data</mark>).
- **Medium-risk asset**: Information that's not available to the public and may cause some damage to the organization's finances, reputation, or ongoing operations (e.g., <mark style="background: #FFF3A3A6;">the early release of a company's quarterly earnings could impact the value of their stock</mark>).
- **High-risk asset**: Information protected by regulations or laws, which if compromised would have a severe negative impact on an organization's finances, ongoing operations, or reputation (e.g., <mark style="background: #FF5582A6;">leaked assets with SPII, PII or intellectual property</mark>).

#### Vulnerability
A weakness that can be exploited by a threat (e.g., outdated firewalls, software or apps; or unprotected confidential data).

#### Key impacts of threats, risks, and vulnerabilities
**Ransomware**: A malicious attack where threat actors encrypt an organization's data and demand payment to restore access.  
> Locked to confidential data, leave devices usable, etc.

#### Layers of the web
- Surface web (can be accessed by a usual web browser)
- Deep web (only authorized employees to access intranet)
- Dark web (by only specialized software)

> [!quote]
> My data to day consists of analyzing security risks and providing solutions to those risk.  
> One of the more common threats we come across is misconfigurations or requesting access for something that you don't really need.  


#### NIST's Risk Management Framework (RMF)
![[attachments/Pasted image 20260430163014.png]]
- Prepare
- Categorize
- Select
- Implement
- Assess
- Authorize
- Monitor

#### RMF Step 1: Prepare
Activities that are necessary to manage security and privacy risks before a breach occurs.
> To monitor for risks and identify controls that can be used to reduce those risks.

#### RMF Step 2: Categorize
Used to develop risk management processes and tasks.
> How the CIA of the systems and information can be impacted by risk. Understand how to follow processes established by your organization.

#### RMF Step 3: Select
Choose, customize, and capture documentation of the controls that protect an organization.
> Keeping a playbook up-to-date or helping to manage other docs that allows you and your team to address issues more efficiently.

#### RMF Step 4: Implement
Implement security and privacy plans for the organization.
> If you notice a pattern of employees constantly needing password resets, implementing a change to password requirements may help solve this issue.

#### RMF Step 5: Assess
Determine if established controls are implemented correctly.
> Analyzing whether the implemented protocols, procedures, and controls that are in place meets organizational needs.  
> Also identifies if anything should be changed to better manage potential risks.

#### RMF Step 6: Authorize
Being accountable for the security and privacy risks that may exist in an organization.
> Involves generating reports, developing plans of action, and establishing project milestones that are aligned to your organization's security goals.

#### RMF Step 7: Monitor
Be aware of how systems are operating.
> Assessing and maintaining technical operations are tasks that analysts complete daily.

#### Manage common threats, risks, and vulnerabilities
There are many resources, such as the NIST, that provide lists of [cybersecurity risks](https://www.nist.gov/itl/smallbusinesscyber/cybersecurity-basics/cybersecurity-risks). Additionally, the Open Web Application Security Project (OWASP) publishes a standard awareness document about the [top 10 most critical security risks](https://owasp.org/www-project-top-ten/) to web applications, which is updated regularly.  
![[attachments/Pasted image 20260430210530.png]]

#### Common Vulnerabilities
- **ProxyLogon**: A pre-authenticated vulnerability that affects the Microsoft Exchange server. This means a treat actor can complete a user authentication process to deploy malicious code from a remote location.
- **ZeroLogon**: A vulnerability in Microsoft's Netlogon authentication protocol. An authentication protocol is a way to verify a person's identity. Netlogon is a service that ensures a user's identity before allowing access to a website's location.
- **Log4Shell**: Allows attackers to run Java code on someone else's computer or leak sensitive information. It does this by enabling a remote attacker to take control of devices connected to the internet and run malicious code.
- **PetitPotam**: Affects Windows New Technology LAN Manager (NTLM). It is a theft technique that allows a LAN-based attacker to initiate an authentication request.
- **Security logging and monitoring failures**: Insufficient logging and monitoring capabilities that result in attackers exploiting vulnerabilities without the organization knowing it.
- **Server-side request forgery**: Allows attackers to manipulate a server-side application into accessing and updating backend resources. It can also allow threat actors to steal data.

## Module 2: Security frameworks and controls

#### About Frameworks and Controls
**Security frameworks**: Guidelines used for building plans to help mitigate risk and threats to data and privacy.  
> For example, the healthcare industry uses frameworks to comply with the United States’ Health Insurance Portability and Accountability Act (HIPAA), which requires that medical professionals keep patient information safe. 

**Security controls**: Safeguards designed to reduce specific security risks.  
- **Physical**: Gates, locks, guards, CCTV.
- **Technical**: Firewalls, MFA, Anti-virus software.
- **Administrative**: Separation of duties, Authorization, Asset classification. 
> Using a measure like MFA to validate someone’s identity is one way to help mitigate potential risks and threats to private data.

**Encryption**: The process of converting data from a readable format to an encoded format (ciphertext).  

**Biometrics**: Unique physical characteristics that can be used to verify a person's identity.  

**Vishing**: The exploitation of electronic voice communication to obtain sensitive information or to impersonate a known source.  

**Authorization**: The concept of granting access to specific resources within a system.  

#### Specific frameworks and controls

#### Cyber Threat Framework (CTF)
Developed by the U.S. government to provide "a common language for describing and communicating information about cyber threat activity".  
Helps professionals to analyze and share information more efficiently to improve their response to the cyber landscape.

#### International Organization for Standardization/International Electrotechnical Commission (ISO/IEC) 27001
An internationally recognized and used framework **ISO/IEC 27001**. Enables organizations of all sectors and sizes to manage the security of assets. Outlines requirements for a information security management system, best practices, and controls. Doesn't require specific controls, it does provide a collection of controls to improve security posture.  

#### NIST frameworks

#### NIST S.P. 800-53
A unified framework for protecting the security of information systems within the <mark style="background: #BBFABBA6;">federal government</mark>.  

#### NIST Cybersecurity Framework (CSF)
A voluntary framework that consists of standards, guidelines, and best practices to manage cybersecurity risk. 

![[attachments/Pasted image 20260501125313.png]]

#### 1. Identify
The management of cybersecurity risk and its effect on an organization's people and assets.
> As a security analyst, you may be asked to monitor systems and devices in your organization's internal network to identify potential security issues.

#### 2. Protect
The strategy used to protect an organization through the implementation of policies, procedures, training, and tools that help mitigate cybersecurity threats.
> You and your team might encounter new and unfamiliar threats and attacks. For this reason, studying historical data and making improvements to policies and procedures is essential.

#### 3. Detect
Identifying potential security incidents and improving monitoring capabilities to increase the speed and efficiency of detections.
> You might be asked to review a new security tool's setup to make sure it's flagging low, medium, or high risk, and then alerting the security team about any potential threats or incidents.

![[attachments/Pasted image 20260501130640.png]]

#### 4. Respond
Making sure that the proper procedures are used to contain, neutralize, and analyze security incidents, and implement improvements to the security process.  
> You could be working with a team to collect and organize data to document an incident and suggest improvements to process to prevent the incident from happening again.

#### 5. Recover
The process of returning affected systems back to normal operation.
> You might work with your security team to restore systems, data, and assets (financial or legal files), that have been affected by an incident like a breach.

#### 6. Govern (NIST CSF 2.0 update)
Emphasizes the importance of strong cybersecurity governance across all levels of the organization. Establishing and maintaining the structures and processes need to effectively manage risk.
> Setting clear cybersecurity objectives, ensuring leadership commitment, developing and implementing a comprehensive risk management strategy, and continuously improving cybersecurity performance.

#### OWASP (Open Web Application Security Project) principles

- **Minimize attack surface area** (e.g., phishing emails, weak passwords | restricting access, establish complex passwords)
- **Principle of least privilege** (e.g., you may have access to locked data, but can't be able to change permissions)
- **Defense in depth** (e.g., MFA setup)
- **Separation of duties** (e.g., the person in a company who sings the paychecks shouldn't also be the person who prepares them)
- **Keep security simple** (e.g., The more complex the security controls are, the harder it is for people to work collaboratively)
- **Fix security issues correctly** (e.g., Fixing a weak WiFi password that could lead to breach)

**Additional OWASP security principles**
- **Establish secure defaults**: Optimal security state of an application is also its default state for users.
- **Fail securely**: When a firewall fails it should simply close all connections and block all new ones, rather than start accepting everything.
- **Don't trust services**: If a third-party vendor tracks reward points for airline customers, the airline should ensure that the balance is accurate before sharing that information with their customers.
- **Avoid security by obscurity**: The security of an application should not rely on keeping the source code secret.

> [!quote]
> Don't be too overwhelmed with trying to understand every single specialization within cybersecurity.

#### Plan a security audit

**Security audit**: A review of an organization's security controls, policies, and procedures against a set of expectations (internal|external).  

#### Common elements of internal audits
- Establishing the scope and goals
- Conducting a risk assessment
- Completing a controls assessment
- Assessing compliance
- Communicating results

**Audit questions**
- What is the audit meant to achieve?
- Which assets are most at risk?
- Are current controls sufficient to protect those assets?
- What controls and compliance regulations need to be implemented?

**Stakeholder communication**
- Summarizes scope and goals
- Lists existing risks
- Notes how quickly those risks need to be addressed
- Identifies compliance regulations

![[attachments/o6XzbUnYRK6pwAtl0ME25Q_3c91489225e04f408952ba8a8595e0f1_Control-categories.pdf]]


## Module 3: Introduction to Cybersecurity Tools

#### Logs and SIEM Tools

**Log**: A record of events that occur within an organization's systems and networks.
- **Firewall logs**: A record of attempted or established connections for incoming traffic from the internet. It also includes outbound requests to the internet from within the network.
- **Network logs**: A record of all computers and devices that enter and leave the network. It also records connections between devices and services on the network.
- **Server logs**: A record of events related to services, such as websites, emails, or file shares. It includes actions: login, password, and username requests.

**Security Information and Event Management (SIEM)**: A application that collects and analyzes log data to monitor critical activities in an organization. They helps to inform only customized important logs/events, which saves time for better efficiency.

![[attachments/Pasted image 20260521162404.png|410]]

#### SIEM Dashboards

**Metrics**: Key technical attributes, such as response time, availability, and failure rate, which are used to assess the performance of a software application.

> [!quote] Parisa: The parallels of accessibility and security
> "I think of accessibility as making information, activities, or even environments meaningful, sensible, usable to as many people as possible."
> "Decisions we make based on our own abilities to enhance security can actually be ineffective."
> "For people who are new to the field of cybersecurity, it's just really important to remember that there's a range of abilities that you are wanting to serve."

#### Explore Common SIEM Tools

- **Self-hosted**: Used in the company/organization when control over confidential data is required.
- **Cloud-hosted**: Used by companies who doesn't want to maintain and invest for SIEM.

But **both** can be used as **Hybrid environments**

#### Splunk Enterprise
A self-hosted tool used to retain, analyze, and search an organization's log data to provide security information and alerts in real-time.

#### Splunk Cloud
A cloud-hosted tool used to collect, search, and monitor log data.

#### Chronicle
A cloud-native tool designed to retain, analyze, and search data.

#### Use SIEM tools to protect organizations

#### Splunk
- **Security posture dashboard**: SOCs, display last 24 hours of events and determine if performing as designed, in real time.
- **Executive summary dashboard**: Overall health over time to improve and reduce risk, provide high-level insights to stakeholders, summary of incidents and trends.
- **Incident review dashboard**: Identify suspicious patterns, highlights higher risk items that need immediate review by an analyst, visual timeline.
- **Risk analysis dashboard**: Identify risk for each risk object, specific user, logging in outside of normal working hours, vulnerabilities in critical assets.

#### Chronicle
A specific asset, a domain name, a user, an IP address.
- **Enterprise insights dashboard**: Indicators of compromise (IOCs), monitor login or data access attempts to critical asset.
- **Data ingestion and health dashboard**: Event logs, log sources, rates of data being processed. Ensuring log sources are correctly configured.
- **IOC matches dashboard**: Observe domain names, IP addresses, devices IOCs over time in order to identify trends. Used to search for activity associated with an alert.
- **Main dashboard**: Timeline of events, high-level summary of information, organization's data ingestion.
- **Rule detections dashboard**: Highest occurrences, severities and detections over time, (prevent user opening attachments), establish mitigation tactics to reduce level of risk.
- **User sign in overview dashboard**: Identify unusual user activity, mitigate threats, risks, and vulnerabilities.

## Module 4: Use playbooks to respond to incidents

#### Phases of an incident response playbook

**Playbook**: A manual that provides details about any operational action.  

**Incident Response**: An organization's quick attempt to identify an attack, contain the damage, and correct the effects of a security breach.  
1. **Preparation**: Outlining responsibility for each roles.
2. **Detection and Analysis**: Right tools and workflows.
3. **Containment**: Minimize damage on ongoing risks.
4. **Eradication and Recovery**: Mitigating vulnerabilities, removing affected malicious codes.
5. **Post incident activity**: Documenting and reporting to stakeholders.
6. **Coordination**: Meets compliance requirements.

#### 1. Preparation
Before incidents occur, mitigate potential impacts on the organization by documenting, establishing staffing plans, and educating users.

#### 2. Detection and Analysis
Detect and analyze events by implementing defined processes and appropriate technology.  

![[attachments/Pasted image 20260522151004.png]]

#### 3. Containment
Prevent further damage and reduce immediate impact of incidents.

#### 4. Eradication and Recovery
Completely remove artifacts of the incident so that an organization can return to normal operations.

#### 5. Post-incident Activity
Document the incident, inform organizational leadership, and apply lessons learned.

#### 6. Coordination
Report incidents and share information throughout the response process, based on established standards.  

![[attachments/Pasted image 20260522150853.png]]

> [!quote] Incident response and the value of playbooks.
> "You can use playbooks for: Open attacks, Privacy incidents, Data leaks, DoS attacks, Service alerts and others."
> "External search researchers also report vulnerabilities, so playbook can help as a guide to fix."
> "Some teams come in and out of fashion, but security is ever present."

#### Denial of Service (DoS) attacks

**Distributed Denial of service attack (DDoS)**: A type of denial of service attack that uses multiple devices or servers in different locations to flood the target network with unwanted traffic.  

**SYN (synchronize) flood attack**: A type of DoS attack that simulates a TCP connection and floods a server with SYN packets.  

**Internet Control Message Protocol (ICMP)**: An internet protocol used by devices to tell each other about data transmission error across the network.  
	- **ICMP flood**: A type of DoS attack performed by an attacker repeatedly sending ICMP packets to a network server.  

**Ping of death**: A type of DoS attack caused when a hacker pings a system by sending it an oversized ICMP packet that is bigger than 64 KB.   

#### Interpreting output by a network analyzer
**tcpdump** prints the output of the command as the sniffed packets in the command line, and optionally to a log file, after a command is executed. The output of a packet capture contains many pieces of important information about the network traffic. 

![[attachments/Pasted image 20260524223620.png]]

---
# Course 3 - Networks and Network Security

## Module 1 - Network Architecture

> [!quote] Chris: My path to cybersecurity
> "Despite this being a fairly technical field, the most important thing you're going to learn are the connections you're going to make other people."

#### Network Tools

- **Hub**: A network device that broadcasts information to every device on the network (**similar to a Radio tower**).
- **Switch**: A device that makes connections between specific devices on a network by sending and receiving data between them (**Passes data to only intended destination**).
- **Router**: A network device that connects multiple networks together (**sending info to other device in a different network**).
- **Modem**: A device that connects your router to the internet and brings interest access to the LAN (**sending info to other device in different geographic location**).
- **Virtualization tools**: Pieces of software that perform network operations (**like cloud services**).


#### Cloud Networks

**Cloud computing**: The practice of using remote servers, applications, and network services that are hosted on the internet instead of on local physical devices.

**Cloud network**: A collection of servers or computers that stores resources and data in remote data centers that can be accessed via the internet.  

#### Introduction to network communication

**Data packet**: A basic unit of information that travels form one device to another within a network.  

![[attachments/Pasted image 20260523162320.png|385]]

**Bandwidth**: The amount of data a device receives every second.  
**Speed**: The rate at which data packets are received or downloaded.  
**Packet sniffing**: The practice of capturing and inspecting data packets across a network.  

#### The TCP/IP model

**Transmission Control Protocol (TCP)**: An internet communication protocol that allows two devices to form a connection and stream data.  

**Internet Protocol (IP)**: A set of standards used for routing and addressing data packets as they travel between devices on a network.  

**Port**: A software-based location that organizes the sending and receiving of data between devices on a network.  
- **Port 25** - Email
- **Port 443** - Secure internet communication
- **Port 20** - Large file transfers

**TCP/IP model**: A framework used to visualize how data is organized and transmitted across the network.  

![[attachments/Pasted image 20260523163749.png]]

#### IP addresses and network communication

**Internet Protocol (IP) address**: A unique string of characters that identifies the location of a device on the internet.  
- IPv4 : `19.117.18.132`
- IPv6: `823D:1111:2222:3333:4444:5555:6:77`

**MAC address**: A unique alphanumeric identifier that is assigned to each physical device on a network.  

![[attachments/Pasted image 20260524123321.png]]


## Module 2 - Network Operations

#### Network Protocols
A set of rules used by two or more devices on a network to describe the order of delivery and the structure of the data.  
- **TCP**: An internet communications protocol that allows two devices to form a connection and stream data.
- **Address Resolution Protocol (ARP)**: A network protocol used to determine the MAC address of the next router or device on the path.
- **HTTPS (Secure)**: A network protocol that provides a secure method of communication between clients and website servers.
- **Domain Name System (DNS)**: A network protocol that translates internet domain names into IP addresses.
- **Simple Network Management Protocol (SNMP)**: a network protocol used for monitoring and managing devices on a network.

#### Additional Network Protocols

| Private IP Addresses                                                                                                                                                                                      | Public IP Addresses                                                                                                                                                                                                                                                                                    |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| - Assigned by the router<br>- Unique only within private network<br>- No cost to use<br>- Address ranges:<br>-- 10.0.0.0-10.255.255.255<br>-- 172.16.0.0-172.31.255.255<br>-- 192.168.0.0-192.168.255.255 | - Assigned by ISP and IANA<br>- Unique address in global internet<br>- Costs to lease a public IP address<br>- Assignable address ranges:<br>-- 1.0.0.0-9.255.255.255<br>-- 11.0.0.0-126.255.255.255<br>-- 128.0.0.0-172.15.255.255<br>-- 172.32.0.0-192.167.255.255<br>-- 192.169.0.0-233.255.255.255 |

| Protocol | Port                                                                  |
| -------- | --------------------------------------------------------------------- |
| DHCP     | UDP port 67 (servers), UDP port 68 (clients)                          |
| ARP      | none                                                                  |
| Telnet   | TCP port 23                                                           |
| SSH      | TCP port 22                                                           |
| POP3     | TCP/UDP port 110 (unencrypted), TCP/UDP port 995 (encrypted, SSL/TLS) |
| IMAP     | TCP port 143 (unencrypted), TCP port 993 (encrypted, SSL/TLS)         |
| SMTP     | TCP/UDP port 25 (unencrypted)                                         |
| SMTPS    | TCP/UDP port 587 (encrypted, TLS)                                     |

> [!quote] Antara: Working in network security
> "A typical day in the life of an entry-level network security engineer would start with solving a problem."
> "You might get your solution just by talking to people."

#### Wireless protocols

**IEEE 802.11 (WiFi)**: A set of standards that define communication for wireless LANs.  
**WiFi Protected Access (WPA)**: A wireless security protocol for devices to connect to the internet (now used WPA2/WPA3).  

#### Firewalls and network security measures

**Port filtering**: A firewall function that blocks or allows certain port numbers to limit unwanted communication.  

**Cloud-based firewalls**: Software firewalls that are hosted by a cloud service provider.  

#### Stateful vs Stateless Firewall
- **Stateful**: A class of firewall that keeps track of information passing through it and proactively filters out threats.
- **Stateless**: A class of firewall that operates based on predefined rules and does not keep track of information from data packets.

**Benefits of next generation firewalls (NGFWs)**
- Deep packet inspection
- Intrusion protection
- Threat intelligence

#### Virtual Private Networks (VPNs)
A network security service that changes your public IP address and hides your virtual location so that you can keep your data private when you are using a public network like the internet.

**Encapsulation**: A process performed by a VPN service that protects your data by wrapping sensitive data in other data packets.  

#### Security zones
A segment of a network that protects the internal network from the internet.  
- **Uncontrolled zone**: Any network outside of the organization's control.
- **Controlled zone**: A subnet that protects the internal network from the uncontrolled zone.
	- Demilitarized zone (DMZ)
	- Internal network
	- Restricted zone

![[attachments/Pasted image 20260524151946.png]]
**Subnetting** is the process of taking one large network and dividing it into several smaller, organized groups called subnets.  

**Classless Inter-Domain Routing (CIDR)** is a method of assigning subnet masks to IP addresses to create a subnet, replaced Classful from limited IPs. 

#### Proxy servers
A server that fulfills the requests of a client by forwarding them on to other servers.  

![[attachments/Pasted image 20260524155913.png]]

**Forward proxy server**: Regulates and restricts a person's access to the internet.  
**Reverse proxy server**: Regulates and restricts the internet's access to an internal server.  

## Module 3 - Secure against network intrusions

#### Malicious packet sniffing

**Passive packet sniffing**: A type of attack where data packets are read in transit.  
**Active packet sniffing**: A type of attack where data packets are manipulated in transit.  

Use **VPN** or **SSL/TLS (HTTPS, etc)** to prevent this attack. Even the attacker have access, they won't be able to read the data (which will be encrypted).  

#### IP Spoofing
A network attack performed when an attacker changes the source IP of a data packet to impersonate an authorized system and gain access to a network.  

#### 1. On-path attack
An attacker where a malicious actor places themselves in the middle of an authorized connection and intercepts or alters the data in transit.  

![[attachments/Pasted image 20260525121534.png]]

#### 2. Replay attack
A network attack performed when a malicious actor intercepts a data packet in transit and delays it or repeats it at another time.  

#### 3. Smurf attack
A network attack performed when an attacker sniffs an authorized user's IP address and floods it with packets.  

## Module 4 - Security hardening

#### Security Hardening
The practice of strengthening a system to reduce its vulnerability and attack surface.  
**Attack surface**: All the potential vulnerabilities that a threat actor could exploit.  

![[attachments/Pasted image 20260525151206.png]]

**Penetration test**: A simulated attack that helps identify vulnerabilities in systems, networks, websites, applications, and processes.  

#### OS hardening practices
**Operating system (OS)**: The interface between computer hardware and the user.  

**Baseline configuration (baseline image)**: A documented set of specifications within a system that is used as a basis for future builds, releases, and updates.  

**Multi-factor authentication (MFA)**: A security measure which requires a user to verify their identity in two or more ways to access a system or network.
- Something you know (password)
- Something you have (ID card)
- Something unique about you (finger print)

#### Assessing vulnerabilities
- **Virtual machines (VMs)**: An additional layer of security for an organization because they can be used to run code in an isolated environment, preventing malicious code from affecting the rest of the computer or system.
- **Sandbox environments**: Commonly used for testing patches, identifying and addressing bugs, or detecting cybersecurity vulnerabilities.  

**TCP Flag codes include:**
- **Flag `S`**: Connection Start
- **Flag `F`**: Connection Finish
- **Flag `P`**: Data Push
- **Flag `R`**: Connection Reset
- **Flag `.`**: Acknowledgement

#### Network hardening practices

#### Firewall
irewalls allow or block traffic based on a set of rules. As data packets enter a network, the packet header is inspected and allowed or denied based on its port number. NGFWs are also able to inspect packet payloads. Each system should have its own firewall, regardless of the network firewall.

![[attachments/Pasted image 20260525214233.png]]

#### Intrusion Detection System
The IDS is configured to detect known attacks. IDS systems often sniff data packets as they move across the network and analyze them for the characteristics of known attacks. Some IDS systems review not only for signatures of known attacks, but also for anomalies that could be the sign of malicious activity. When the IDS discovers an anomaly, it sends an alert to the network administrator who can then investigate further.

![[attachments/Pasted image 20260525214257.png]]

####  Intrusion Prevention System
An IPS searches for signatures of known attacks and data anomalies. An IPS reports the anomaly to security analysts and blocks a specific sender or drops network packets that seem suspect. 

![[attachments/Pasted image 20260525214326.png]]

#### Security Information and Event Management (SIEM)
An application that collects and analyzes log data to monitor critical activities in an organization. SIEM tools work in real time to report suspicious activity in a centralized dashboard. SIEM tools additionally analyze network log data sourced from IDSs, IPSs, firewalls, VPNs, proxies, and DNS logs.

![[attachments/Pasted image 20260525214420.png]]

> [!quote] Kelsey: Cloud security explained
> "As more and more companies move into cloud. You may just be the person who can help one of those organizations finally make that leap because they have a professional on their team."

#### Secure the cloud

- **Identity access management (IAM)**: is a collection of processes and technologies that helps organizations manage digital identities in their environment.
- **Configuration**: Each cloud service necessitates precise configuration to uphold security and compliance standards.
- **Attack surface**: Cloud service providers (CSPs) offer numerous applications and services for organizations at a low cost. Every service or application on a network carries its own set of risks and vulnerabilities and increases an organization’s overall attack surface.
- **Zero-day attacks**: Zero-day attacks are an important security consideration for organizations using cloud or traditional on-premise network solutions. A zero day attack is an exploit that was previously unknown.
- **Visibility and tracking**: CSPs take responsibility for security in the cloud, but they do not allow the organizations that use their infrastructure to monitor traffic on the CSP’s servers.
- **Share responsibility model**: CSP must take responsibility for security involving the cloud infrastructure, including physical data centers, hypervisors, and host operating systems.  

---
# Course 4 - Tools of The Trade - Linux and SQL

## Module 1: Introduction to operating systems

![[attachments/Pasted image 20260531195633.png]]

1. **User**: The user initiates the process by having something they want to accomplish on the computer.
2. **Application**: The application is the software program that users interact with to complete a task.
3. **Operating system**: The operating system receives the user’s request from the application. It’s the operating system’s job to interpret the request and direct its flow.
4. **Hardware**: The hardware is where all the processing is done to complete the tasks initiated by the user. 

After the work is done by the hardware, it sends the output back through the operating system to the application so that it can display the results to the user.

## Module 2: The Linux operating system

### Linux distribution

**Parent Distributions**
- Red Hat Enterprise Linux (CentOS)
- Slackware (SUSE)
- Debian (Ubuntu and KALI LINUX)

### KALI LINUX ™
**Pentesting tools**
- Metasploit
- Burp Suite
- John the Ripper

 **Digital forensics**: The practice of collecting and analyzing data to determine what has happened after an attack.  

**Digital forensics tools**
- tcpdump
- Wireshark
- Autopsy

### Package managers
**Advanced Package Tool (APT)**   
APT is a tool used with Debian-derived distributions. It is run from the command-line interface to manage, search, and install packages.

**Yellowdog Updater Modified (YUM)**  
YUM is a tool used with Red Hat-derived distributions. It is run from the command-line interface to manage, search, and install packages. YUM works with .rpm files.

## Module 3: Linux commands in the Bash shell

### Linux commands via the Bash shell

**Security analysts**
- work with server logs
- navigate, manage and analyze files remotely
- verify and configure users and group access
- give authorization and set file permissions

### Navigate Linux and read file content

### Filesystem Hierarchy Standard (FHS)
The component of Linux that organizes data. It defines how directories, directory contents, and other storage is organized in the operating system.  

![[attachments/Pasted image 20260601122428.png]]

### Standard FHS directories
- `/home`: Each user in the gets their own home directory.
- `/bin`:  Contains binary files and other executables. Executables are files that contain a series of commands a computer needs to follow to run programs and perform other functions.
- `/etc`: This directory stores the system’s configuration files.
- `/tmp`: This directory stores many temporary files. The `/tmp` directory is commonly used by attackers because anyone in the system can modify data in these files.
- `/mnt`: This directory stands for “mount” and stores media, such as USB drives and hard drives.

### -name and -iname
- `find /home/analyst/projects -name "*log*"` - Case-sensitive strings searching 
- `find /home/analyst/projects -iname "*log*"` - Not case-sensitive strings searching

### User & Group Management
**User Management** centers on the `useradd`, `usermod`, and `userdel` commands to create, modify, and remove accounts.
- `useradd -m username` to create a user with a home directory
- `usermod -aG groupname username` to add them to supplementary groups
- `userdel -r username` to delete the account and its files. 

**Group Management** utilizes `groupadd`, `groupmod`, `groupdel`, and `chgrp` to organize permissions.
- Create groups with `groupadd` `groupname`
- Modify group details with `groupmod`
- Delete empty groups with `groupdel`
- Assign group ownership to files using `chgrp groupname filename`

## Module 4: Databases and SQL

### WHERE 
To create a filter in SQL, you need to use the keyword `WHERE`. WHERE `indicates` the condition for a filter.
 
```sql
SELECT firstname, lastname, title, email
FROM employees
WHERE title = 'IT Staff';
```

| Pattern | Results that could be returned |
| ------- | ------------------------------ |
| `'a%'`    | `apple123, art, a`               |
| `'a_'`    | `as, an, a7`                     |
| `'a__'`   | `ant, add, a1c`                  |
| `'%a'`    | `pizza, Z6ra, a`                 |
| `'_a'`    | `ma, 1a, Ha`                     |
| `'%a%'`   | `Again, back, a`                 |
| `'_a_'`   | `Car, ban, ea7`                  |

### LIKE
To apply wildcards to the filter, you need to use the `LIKE` operator instead of an equals sign (`=`). `LIKE` is used with `WHERE` to search for a pattern in a column. 

```sql
SELECT lastname, firstname, title, email
FROM employees
WHERE title LIKE 'IT%';
```

### BETWEEN
Filter for login attempts made in a certain date range:

```sql
SELECT *
FROM log_in_attempts
WHERE login_date BETWEEN '2023-02-01' AND '2023-02-07';
```

### AND
As an example, a cybersecurity concern might affect only those customer accounts that meet both the condition of being handled by a support representative with an ID of 5 and the condition of being located in the USA. To find the names and emails of those specific customers, you should place the two conditions on either side of the `AND` operator in the `WHERE` clause:

```sql
SELECT firstname, lastname, email, country, supportrepid
FROM customers
WHERE supportrepid = 5 AND country = 'USA';
```

### OR 
For example, if you are responsible for finding all customers who are either in the USA or Canada so that you can communicate information about a security update, you can use an `OR` operator to find all the needed records. As the following query demonstrates, you should place the two conditions on either side of the `OR` operator in the `WHERE` clause:

```sql
SELECT firstname, lastname, email, country
FROM customers
WHERE country = 'Canada' OR country = 'USA';
```

### NOT
For example, if a cybersecurity issue doesn't affect customers in the USA but might affect those in other countries, you can return all customers who are not in the USA. This would be more efficient than creating individual conditions for all of the other countries. To use the `NOT` operator for this task, write the following query and place `NOT` directly after `WHERE`:

```sql
SELECT firstname, lastname, email, country
FROM customers
WHERE NOT country = 'USA';
```

### Combining logical operators

```sql
SELECT firstname, lastname, email, country
FROM customers
WHERE NOT country = 'Canada' AND NOT country = 'USA';
```

### Join tables in SQL

- **INNER JOIN**: Returns rows matching on a specified column that exists in more than one table.  

![[attachments/Pasted image 20260602154017.png]]

The first type of join that you might perform is an inner join. **INNER JOIN** returns rows matching on a specified column that exists in more than one table.  

![[attachments/Pasted image 20260602155057.png]]

```sql
SELECT *
FROM employees
INNER JOIN machines ON employees.device_id = machines.device_id;
```

### OUTER JOIN
- **LEFT JOIN**: Returns all of the records of the first table, but only returns rows of the second table that match on a specified column.

![[attachments/Pasted image 20260602154528.png]]

When joining two tables, **LEFT JOIN** returns all the records of the first table, but only returns rows of the second table that match on a specified column.  

![[attachments/Pasted image 20260602155300.png]]

```sql
SELECT *

FROM employees

LEFT JOIN machines ON employees.device_id = machines.device_id;
```

- **RIGHT JOIN**: Returns all of the records of the second table, but only returns rows from the first table that match on a specified column.

![[attachments/Pasted image 20260602154637.png]]

When joining two tables, **RIGHT JOIN** returns all of the records of the second table, but only returns rows from the first table that match on a specified column.  

![[attachments/Pasted image 20260602155346.png]]

```sql
SELECT *
FROM employees
RIGHT JOIN machines ON employees.device_id = machines.device_id;
```


- **Full outer joins**: `FULL OUTER JOIN` returns all records from both tables. You can think of it as a way of completely merging two tables.

![[attachments/Pasted image 20260602155452.png]]

```sql
SELECT *
FROM employees
FULL OUTER JOIN machines ON employees.device_id = machines.device_id;
```

### Aggregate functions
In SQL, **aggregate functions** are functions that perform a calculation over multiple data points and return the result of the calculation. The actual data is not returned. 

- **COUNT** returns a single number that represents the number of rows returned from your query.
- **AVG** returns a single number that represents the average of the numerical data in a column.
- **SUM** returns a single number that represents the sum of the numerical data in a column. 

```sql
SELECT COUNT(firstname)
FROM customers;
```

---
# Course 5 - Assets, Threats, and Vulnerabilities

## Module 1 - Introduction to asset security

### The what, why, and how of asset security

- **Risk**: Anything that can impact the confidentiality, integrity, or availability of an asset. `Likelihood x Impact = Risk`
- **Threat**: Any circumstance or event that can negatively impact assets
- **Vulnerability**: A weakness that can be exploited by a threat

### Security starts with asset classification

**Asset management**: The process of tracking assets and the risks that affect them.  
- Starts with **Asset inventory**: A catalog of assets that need to be protected.

**Asset classification**: The practice of labeling assets based on sensitivity and importance to an organization.
- Public
- Internal-only
- Confidential
- Restricted

### Elements of a Security Plan

- **Policies**: These are foundational rules that reduce risk and protect information, outlining the scope, objectives, and limitations of a security plan.
- **Standards**: These provide tactical guidance, acting as references that inform how policies are set, such as specifying password length requirements.
- **Procedures**: These are step-by-step instructions for performing specific security tasks, promoting accountability, consistency, and efficiency within an organization.

## Module 2 - Protect organizational assets

### Security controls
- Operational
- Technical
- Managerial

**Usage audits**: Reviewing which resources each account is accessing and what the user is doing with the resource.  
**Privilege audits**: Whether a user's role is in alignment with the resources they have access to.  
**Account change audits**: Account directory services keep records and logs associated with each user.  

### The data lifecycle
- **PII**: Personally identifiable information, any information used to infer an individual's identity.
- **PHI**: Protected health information, information that relates to the past, present, or future physical or mental health or condition of an individual.
- **SPII**: S for sensitive, a specific type of PII that falls under stricter handling guidelines.

![[attachments/Pasted image 20260610153543.png]]

- **Information privacy** refers to the protection from unauthorized access and distribution of data.
- **Information security** (InfoSec) refers to the practice of keeping data in all states away from unauthorized users.

### Fundamentals cryptography
**Cipher**: An algorithm that encrypts information.  

### Public key infrastructure (PKI)
 An encryption framework that secures the exchange of information online.  
 
- **Symmetric encryption** is the use of a single secret key to exchange information. Because it uses one key for encryption and decryption, the sender and receiver must know the secret key to lock or unlock the cipher.
- **Asymmetric encryption** is the use of a public and private key pair for encryption and decryption of data. It uses two separate keys: a public key and a private key. The public key is used to encrypt data, and the private key decrypts it. The private key is only given to users with authorized access.

### Non-repudiation and hashing

**Non-repudiation**: The concept that the authenticity of information can't be denied.  

**Hashing**: The hash function is an algorithm that produces a code that can't be decrypted (digesting).  

```bash
## Checking the hash of a particular file
$ sha256 <filename> 
```


**Salting** is an additional safeguard that's used to strengthen hash functions. A salt is a random string of characters that's added to data before it's hashed. The additional characters produce a more unique hash value, making salted data resilient to rainbow table attacks.  

![[attachments/Pasted image 20260611222601.png]]

### Access controls and authentication systems

**Authentication**:
1. **Knowledge**: something the user knows
2. **Ownership**: something the user possesses
3. **Characteristic**: something the user is

**Single sign-on (SSO)**: A technology that combines several different logins into one.  

**SSO** works by automating how trust is established between a user and a service provider. Rather than placing the responsibility on an employee or customer, SSO solutions use trusted third-parties to prove that a user is who they claim to be. This is done through the exchange of encrypted access tokens between the identity provider and the service provider.  

![[attachments/Pasted image 20260611223907.png]]

### Why we audit user activity
**Session**: A sequence of network HTTP basic auth requests and responses associated with the same user.  

**Session ID**: A unique token that identifies a user and their device while accessing the system.  

**Session cookie**: A token that websites use to validate a session and determine how long that session should last.  

### Authentication, Authorization, Accounting (AAA) Framework

1. **Authentication**: verifies the identity of a user or device attempting to access the network (<mark style="background: #ADCCFFA6;">passwords, biometrics, MFA</mark>, etc).
2. **Authorization**: determines what resources and actions the authenticated user is permitted to access (policies: <mark style="background: #ADCCFFA6;">Role-Based Access Control (RBAC) or the principle of least privilege</mark>).
3. **Accounting** (Auditing): tracks and logs user activities, including <mark style="background: #ADCCFFA6;">login times, data usage, and session details</mark>, to provide an audit trail for troubleshooting, billing, and forensic investigation.

**Identity and access management (IAM)** is a collection of processes and technologies that helps organizations manage digital identities in their environment. Both AAA and IAM systems are designed to authenticate users, determine their access privileges, and track their activities within a system.  

**User provisioning** is the process of creating and maintaining a user's digital identity.  

### Granting authorization
- Mandatory access control (MAC)
- Discretionary access control (DAC)
- Role-based access control (RBAC)

![[attachments/Pasted image 20260612111500.png]]

**MAC** is the strictest of the three frameworks. Authorization in this model is based on a strict need-to-know basis. Access to information must be granted manually by a central authority or system administrator.  
- Commonly applied in law enforcement, military, and other government agencies where users must request access through a chain of command. MAC is also known as non-discretionary control because access isn’t given at the discretion of the data owner.

![[attachments/Pasted image 20260612111615.png]]

**DAC** is typically applied when a data owner decides appropriate levels of access.
- One example of DAC is when the owner of a Google Drive folder shares editor, viewer, or commentor access with someone else.

![[attachments/Pasted image 20260612111644.png]]

**RBAC** is used when authorization is determined by a user's role within an organization.
- For example, a user in the marketing department may have access to user analytics but not network administration.

## Module 3 - Vulnerabilities in systems

### Vulnerability management
1. Identify vulnerabilities
2. Consider potential exploits
3. Prepare defense against threats

**Zero-day**: An exploit that was previously unknown.  

### Vulnerabilities of CI/CD

**Continuous Integration** (Building a solid foundation) is all about frequently merging code changes from different developers into a central location. This triggers automated processes like building the software and running tests. CI catches problems through an automated process: every time code is integrated, the system automatically builds and tests it. This immediate feedback loop reveals integration problems as soon as they occur. CI helps catch integration problems early, leading to higher quality code. Think of it as the foundation of the pipeline.  

**Continuous Delivery** (Ready to release) means your code is always ready to be released to users. After passing automated tests, code is automatically deployed to a staging environment (a practice environment) or prepared for final release. Typically, a manual approval step is still needed before going live to production, which provides a control point.  

**Continuous Deployment** (Fully automated releases) automates the entire release process. Changes that pass all automated checks are automatically deployed directly to the live production environment, with no manual approval. This is all about speed and efficiency.  

![[attachments/Pasted image 20260612161106.png]]

### Defense in depth strategy
1. **Perimeter layer**, like authentication systems that validate user access
2. **Network layer**, which is made up of technologies like network firewalls and others
3. **Endpoint layer**, which describes devices on a network, like laptops, desktops, or servers
4. **Application layer**, which involves the software that users interact with
5. **Data layer**, which includes any information that’s stored, in transit, or in use

### Common vulnerabilities and exposures

- **Common Vulnerabilities and Exposures list (CVE list)**: An openly accessible dictionary of known vulnerabilities and exposures.
	- **CVE list criteria**
	- Independent of other issues
	- Recognized as a potential security risk
	- Submitted with supporting evidence
	- Only affect one codebase
- **CVE Numbering Authority (CNA)**: An organization that volunteers to analyze and distribute information on eligible CVEs.
- **Common Vulnerability Scoring System (CVSS)**: A measurement system that scores the severity of a vulnerability.

**MITRE**: A collection of non-profit research and development centers.  

### The OWASP Top 10
**Open Worldwide Application Security Project** that security professionals from around the world use to share information, tools, and events that are focused on securing the web.  

### 1. Broken access control
Access controls limit what users can do in a web application. For example, a blog might allow visitors to post comments on a recent article but restricts them from deleting the article entirely. 

### 2. Cryptographic failures
Information is one of the most important assets businesses need to protect. Privacy laws such as General Data Protection Regulation (GDPR) require sensitive data to be protected by effective encryption methods. 

### 3. Injection
Injection occurs when malicious code is inserted into a vulnerable application. Although the app appears to work normally, it does things that it wasn’t intended to do. Injection attacks can give threat actors a backdoor into an organization’s information system (target: login forms).

### 4. Insecure design
Applications should be designed in such a way that makes them resilient to attack. Insecure design refers to a wide range of missing or poorly implemented security controls that should have been programmed into an application when it was being developed.

### 5. Security misconfiguration
Misconfigurations occur when security settings aren’t properly set or maintained. A common example is when businesses deploy equipment, like a network server, using default settings. 

### 6. Vulnerable and outdated components
Vulnerable and outdated components is a category that mainly relates to application development. Applications that use vulnerable components that have not been maintained are at greater risk of being exploited by threat actors.

### 7. Identification and authentication failures
When applications fail to recognize who should have access and what they’re authorized to do, it can lead to serious problems. For example, a home Wi-Fi router normally uses a simple login form to keep unwanted guests off the network.

### 8. Software and data integrity failures
Software and data integrity failures are instances when updates or patches are inadequately reviewed before implementation. A famous example of a supply chain attack is the [SolarWinds cyber attack (2020)](https://www.gao.gov/blog/solarwinds-cyberattack-demands-significant-federal-and-private-sector-response-infographic) where hackers injected malicious code into software updates that the company unknowingly released to their customers.

### 9. Security logging and monitoring failures
Having a record of events like user login attempts is critical to finding and fixing problems. Sufficient monitoring and incident response is equally important.

### 10. Server-side request forgery
Companies have public and private information stored on web servers. When you use a hyperlink or click a button on a website, a request is sent to a server that should validate who you are, fetch the appropriate data, and then return it to you.

![[attachments/Pasted image 20260612181726.png]]

### OSINT Tools
- VirusTotal is a service that allows anyone to analyze suspicious files, domains, URLs, and IP addresses for malicious content.
- MITRE ATT&CK® is a knowledge base of adversary tactics and techniques based on real-world observations.
- OSINT Framework is a web-based interface where you can find OSINT tools for almost any kind of source or platform.
- Have I been Pwned is a tool that can be used to search for breached email accounts.

### Vulnerability assessment process
1. Identification
2. Vulnerability analysis
3. Risk assessment
4. Remediation

### Penetration testing strategies
- **Open-box testing** is when the tester has the same privileged access that an internal developer would have—information like system architecture, data flow, and network diagrams. This strategy goes by several different names, including internal, full knowledge, white-box, and clear-box penetration testing.
- **Closed-box testing** is when the tester has little to no access to internal systems—similar to a malicious hacker. This strategy is sometimes referred to as external, black-box, or zero knowledge penetration testing.
- **Partial knowledge testing** is when the tester has limited access and knowledge of an internal system—for example, a customer service representative. This strategy is also known as gray-box testing.

