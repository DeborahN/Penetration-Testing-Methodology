# Penetration Testing Methodology #
----------

A **penetration testing/ pentest**, is a process that is followed to conduct an in-depth security assessment or audit.

A *penetration testing methodology* defines a roadmap with practical ideas and proven practices that can be followed to assess the true security posture of a network, application, system, or any combination thereof.

- Penetration testing can be carried out independently or as a part of an IT security risk management process.
- It can be conducted with or without prior knowledge of the targeted network or application.
- It may be used to assess all IT infrastructure components including applications, network devices, operating systems, communication medium, physical security, and human psychology.
- The output of penetration testing usually consists of a report divided into several sections that address the weaknesses found in the current state of the
target environment, followed by potential countermeasures and other remediation
recommendations.


##Types of penetration testing##

###Black box testing###
- The security auditor will not be aware of any internal technologies deployed by the targeted organization.
- Vulnerabilities may be revealed and potentially exploited using real-world hacker techniques and by following an organized test phases.
- Pentester should understand, classify, and prioritize these vulnerabilities according to their level of risk (low, medium, or high).
- Determine all attack vectors that could cause the target to be compromised.
- Once the testing process has been completed, a report should be prepared with all the necessary information regarding the targets' real-world security posture,
categorizing, and translating the identified risks into a business context.
- More expensive service.


###White box testing###
- The security auditor should be aware of all the internal and underlying technologies used by the target environment.
- Pentester can view and critically evaluate the security vulnerabilities with minimum possible efforts and highest accuracy.
- Eliminate any internal security issues.
- Can easily be integrated into a regular development life cycle.
- The time, cost, and knowledge level required to find and resolve the security vulnerabilities are comparably less than with the black box approach.


##Vulnerability assessment versus penetration testing##

A **Vulnerability assessment** is a process to assess the internal and external security controls by identifying the threats that pose serious exposure to the organizations' assets.

- The *penetration testing* goes beyond the level of identifying vulnerabilities and hooks into the process of exploitation, privilege escalation, and maintaining access to the target system(s).

- *Vulnerability assessment* provides you with a broad view of any existing flaws in the system without measuring the impact of these flaws to the system under consideration.

- The *penetration testing* is considerably more intrusive than the vulnerability assessment and aggressively applies all of the technical methods to exploit the live production environment.

- The *vulnerability assessment* process carefully identifies and quantifies all the known vulnerabilities.

- *Penetration testing* is ideal when there is doubt that mitigating controls such as firewalls, IDSs, file integrity monitoring.

- *Vulnerability scanning* will locate individual vulnerabilities.

- *Penetration testing* will actually attempt to verify that these vulnerabilities are exploitable within the target environment.

- *Penetration testing* is an expensive service in comparison to vulnerability assessment.


##Security Testing Methodologies##

####Open Source Security Testing Methodology Manual (OSSTMM) - (page 56-58)####

From a technical perspective, its methodology is divided into four key groups—*scope*, *channel*, *index*, and *vector*. Six standard security test types;

- **Blind**: Does not require any prior knowledge about the target system and the target is informed before the execution. e.g: *Ethical hacking* and *war gaming*.
- **Double blind**: An auditor neither requires any knowledge about the target system, nor is the target informed before the test execution. e.g: *Black box auditing* and *penetration testing*.
- **Gray box**: An auditor holds limited knowledge about the target system and the target is also informed before the test is executed. e.g.: *Vulnerability assessment*.
- **Double gray box**: Similar to gray box testing, except that the time frame for an audit is defined and there are no channels and vectors being tested. e.g.: *White box audit*.
- **Tandem**: The auditor holds minimum knowledge to assess the target system and the target is also notified in advance, before the test is executed. Note that tandem testing is conducted thoroughly. e.g.: *Crystal box* and *in-house audit*.
- **Reversal**: An auditor holds full knowledge of the target system and the target will never be informed of how and when the test will be conducted.


####Information Systems Security Assessment Framework (ISSAF) - (page 58-59)####

Its framework has been categorized into several domains to address the security
assessment in a logical order. Each of these domains assesses different parts of a target system and provides field inputs for the successful security engagement.

ISSAF was developed to focus on two areas of security testing—technical and managerial.

ISSAF contains a rich set of technical assessment baselines to test the number of different technologies and processes.


####Open Web Application Security Project (OWASP) - (page 60-61)####

OWASP can be used to increase the awareness of application security and to integrate security through secure coding principles and practices.

The OWASP top 10 mainly focuses on the high risk problem areas rather than addressing all the issues that surround the web application's security.


####Web Application Security Consortium Threat Classification (WASC-TC) - (page 61-63)####

Used to assess the security of web applications. The overall standard is presented in three different views to help developers and security auditors understand the vision of web application security threats:

- **Enumeration view**: This view is dedicated to providing the basis for web
application attacks and weaknesses. 
- **Development view**: The development view takes the developer's panorama forward by combining the set of attacks and weaknesses into vulnerabilities, which are likely to occur at any of three consecutive development phases. This could be a design, implementation, or deployment phase.
- **Taxonomy cross-reference view**: Referring to a cross-reference view of multiple web application security standards can help auditors and developers map the terminology presented in one standard with another.

####Penetration Testing Execution Standard (PTES) - (page 63-64)####

It consists of seven phases of penetration testing and can be used to perform an effective penetration test on any environment.

- Pre-engagement interactions
- Intelligence gathering
- Threat modeling
- Vulnerability analysis
- Exploitation
- Post-exploitation
- Reporting


##General penetration testing framework - (page 64-68)##
- **Target scoping**: Observe and understand the given scope of the target network environment. The scope can be defined for a single entity or set of entities.

- **Information gathering** (reconnaissance phase): A pentester uses a number of publicly available resources to learn more about his or her target, such as: Forums, Bulletin boards, Newsgroups, Articles, Blogs, Social networks, Commercial or non-commercial websites and search engines. Kali Linux tools can be used to extract the network information about a target. (Data mining techniques to collect information through DNS servers, trace routes, Whois database, e-mail addresses, phone numbers, personal information, and user accounts).

- **Target discovery**: A complete image of the interconnected current technologies or devices and may further help in enumerating various services that are running over the network. (Live network hosts, operating systems, and characterize each device according to its role in the network system).

- **Enumerating target**: Finds the open ports on the target systems and then enumerated for the running services for further investigating the vulnerabilities.

- **Vulnerability mapping**: Identify and analyze the vulnerabilities based on the disclosed ports and services.

- **Social engineering**: When there is no open gate available for an auditor to enter the target network, using a human attack vector, try to  penetrate the target system by tricking a user into executing malicious code that should give backdoor access to the auditor.

- **Target exploitation**: Penetrate the target system based on the types of exploits that are available. The process coordinates three core areas, which involve pre-exploitation, exploitation, and post-exploitation activities.

- **Privilege escalation**: Once the target is acquired privileges can also be escalated using any local exploits that match the system's environment to gain access super-user or system-level privileges.

- **Maintaining access**: Using tunneling methods, which make a use of protocol,
proxy, or end-to-end connection strategy that can lead to establishing a backdoor
access, can help an auditor maintain his or her footsteps into the target system as long as required.

- **Documentation and reporting**: Documenting, reporting, and presenting the vulnerabilities found, verified, and exploited will conclude your penetration testing activities.

**Reference**: L. Allen, T. Heriyanto, S. Ali. *Kali Linux – Assuring Security by Penetration Testing*. 2014.
