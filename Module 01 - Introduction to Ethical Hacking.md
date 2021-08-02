# **Module 01: Introduction to Ethical Hacking**

## **Information Security Overview**
Information security refers to the protection or safeguarding of information and information systems that use, store and trasmit information from unauthorized access, disclosure, alteration and destruction.

### 🔷 **Elements of Information Security**

* **Confidentiality**
    * Confidentiality is the assurance that the information is accessible only to authorized.
        * Confidentiality breaches may occur due to improper data handling or a hacking attempt.

* **Integrity**
    * Integrity is the trustworthiness of data or resources in the prevention of improper and unauthorized changes - the assurance that information is sufficiently accurate for its purpose.
        * Measures to maintain data integrity may include a checksum (a number produced by a mathematical function to verify that a given block of data is not changed) and access control.

* **Availability**
    * Availability is the assurance that the systems responsible for delivering, storing, and processing information are accessible when required by authorized users.
        * Measures to maintain data availability can include disk arrays for redundant systems and clustered machines, antivirus software to combat malware, ...

* **Authenticity**
    * Authenticity refers to the characteristic of communication, documents, or any data that ensures the quality of being genuine or uncorrupted.
        * The major role of authentication is to confirm that the user is genuine.

* **Non-Repudiation**
    * Non-Repudiation is a way to guarantee that the sender of a message cannot later deny having sent the message and that the recipient cannot deny having received the message.

### 🔷 **Motives, Goals & Objectives of Information Security Attacks**

**```Attacks = Motive (Goal) + Method + Vulnerability```**

#### **Motives behind information security attacks**
* Disrupt business continuity
* Perform information theft
* Manipulation data
* Create fear and chaos by disruption ciritcal infrastructures
* Bring financial loss to the target
* etc.

### 🔷 **Classification of Attacks**
* **Passive Attacks**
    * Intercepting and monitoring network traffic and data flow on the target network and do not tamper with the data.
        * Footprinting
        * Sniffing and eavesdropping
        * Network traffic analyses
        * Decryption of weakly encrypted traffic

* **Active Attacks**
    * Tamper with the data in transit or disrupt communication or services between the systems to bypass or break into secured systems.
        * Denial-of-Service (DoS) Attack
        * Bypassing protection mechanisms
        * Malware attacks
        * Spoofing attacks
        * DNS & ARP poisoning
        * Privilege escalation
        * etc.

* **Close-in Attacks**
    * Close physical proximity with the target system or network
        * Social engineering (eavesdropping, shoulder surfing, dumpster diving, ...)

* **Insider Attack**
    * Performed by trusted persons who have physical access to critical assets of the target.
        * Eavesdropping and wiretapping
        * Theft of physical devices
        * Social engineering
        * Data theft and spoliation
        * Planting keyloggers, backdoors or malware

* **Distribution Attacks**
    * Tamper with hardware or software prior to installation.
        * Modification of software or hardware during production
        * Modification of software or hardware during distribution


### 🔷 **Information Warfare**
The term information Warfare or InfoWar refers to the use of information and communication technologies (ICT) for competitive advantages over an opponent. (viruses, worms, Trojan Horses, ...)

* **Command and control warfare (C2 Warfare)**
    * Refers to the impact an attacker possesses over a compromised system or network that they control.

* **Intelligence-based warfare**
    * Senior-based technology that directly corrupts technology systems.

* **Electronic warfare**
    * Uses radio-electronic and cryptographic techniques to degrade communication.

* **Psychological warfare**
    * The use of various techniques such as propaganda and terror to demoralize one's adversary in an attempt to succeed in battle.

* **Hacker warfare**
    * Shutdown of systems, data errors, theft of information, theft of services, false messaging, etc.

* **Economic warfare**
    * Effects the economy of a business or nation by blocking the flow of information.

* **Cyberwarfare**
    * Use of information systems against the virtual personas of individuals or groups.

* **Defensive information warfare**
    * Involves all strategies and actions to defend against attacks on ICT assets.

* **Offensive information warfare**
    * Involves attacks against the ICT assets of an opponent.

<br>

## **Cyber Kill Chain Concepts**
The cyber kill chain is an efficient and effective way of illustrating how an adversary can attack the target organization. This model helps organizations understand the various possible threats at every stage of an attack and the necessary countermeasures to defend against such attacks.

<br>

### 🔷 **Cyber Kill Chain Methodology**

![CyberKillChain](https://nucleon-security.com/wp-content/uploads/2020/07/Cyber_Kill_Chain.jpg)

* **Reconnaissance**
    * Collecting as much information as possible about the target to probe for weak points before actually attacking. Such as publicly available information, network information, etc. This kind of information can help gaining backdoor access to the target network.

* **Weaponization**
    * Analyse the gathered data to identify the vulnerabilities and techniques that can exploit and gain unauthorized access to the target organization

* **Delivery**
    * The payload created in the previous step is being transmitted to the indented victim(s) as an email attachment, via a malicious link on websites, etc.

* **Exploitation**
    * After the "weapon" is transmitted to the inteded victim, exploitation triggers the adversary's malicious code to exploit a vulnerability in the operating system, application or server on a target system

* **Installation**
    * Downloads and installs more malicious software on the target system to maintain access to the target network for an extended period. They may use the weapon to install a backdoor to gain remote access.

* **Command and Control**
    * Creates a command and control channel, which established two-way communication between the victim's system and adversary-controlled server to communicate and pass data back and forth.

* **Exfiltration**
    * Victim's system is controllable from a remote location and finally accomplishes their inteded goals. The adversary gains access to confidential data, disrupts the services or network, etc.

<br>

### 🔷 **Tactics, Techniques & Procedures (TTPs)**

The terms "tactics, techniques & procedures" refer to the patterns of activities and methods associated with the specific threat actors or groups of theat actors.

* **Tactics**
    * Tactics describe the way the threat actor operates during different phases of an attack

* **Techniques**
    * To launch an attack successfully, theat actors use several techniques during its execution. These techniques include initial exploitation, setting up and maintaining command and control channels, etc.

* **Procedures**
    * Procedures involve a sequence of actions performed by the threat actors to execute different steps of an attack life cycle.

<br>

### 🔷 **Adversary Behavioral Identification**
Adversary behavioral identification involves the identification of the common methods or techniques followed by an adversary to launch attacks to penetrate on organization's network.

* **Internal Reconnaissance**
    * Once adversary is inside the target network, they follow various techniques and methods to carry out internal reconnaissance. (Enumeration of systems, hosts, processes, etc.)

* **Use of PowerShell**
    * PowerShell can be used by an adversary as a tool for automating data exfiltration and launching further attacks

* **Unspecified Proxy Activities**
    * Create and configure multiple domains pointing to the same host, thus, allowing an adversary to switch quickly between the domains to avoid detection

* **Use of Command-Line Interface**
    * On gaining access to a system an adversary can use the CLI to interact with the target system.

* **HTTP User Agent**
    * In HTTP-based communication, the server identifies the connected HTTP client using the user agent field. An adversary modifies the content of this field to communicate with the compromised system.

* **Command & Control Server**
    * Command & Control server are being used to communicate remotely with compromised systems through encrypted sessions.

* **Use of DNS Tunneling**
    * DNS tunneling can be used to obfuscate malicious traffic in the legitement traffic carried by common protocols used in the network.

* **Use of Web Shell**
    * An adversary uses a web shell to manipulate the web server by creating a shell within a website, it allows an adversary to gain remote access to the functionalities of a server.

* **Data Staging**
    * After successful penetration into a target's network, the adversary uses data staging techniques to collect and combine as much data as possible.

### 🔷 **Indicators of Compromise (IoCs)**
Cyber threats are continuously evolving with the newer TTPs adapted based on the vulnerabilities of the target organization. Security professionals must perform continious monitoring of IoCs to effectively and efficienttly detect and respond to evolving cyber threats.

* **Email Indicators**
    * Attackers usually prefer email services to send malicious data to the target organization or individual. Such socially engineered emails are preferred due to their ease of use and comparative anonymity.

* **Network Indicators**
    * Network indicators are useful for command and control, malware delivery, and identifying details about the operating system, browser typen and other computer-specific information.

* **Host-Based Indicators**
    * Host-Based indicators are found by performing an analysis of the infected system within the organizational network.

* **Behavioral Indicators**
    * Generally, typical IoCs are useful for identifying indicators of intrusion, such as malicious IP addresses, virus signatures, etc.

<br>

## **Hacking Concepts**

### 🔷 **What is Hacking?**

Hacking in the field of computer security refers to exploiting system vulnerabilities and compromising security controls to gain unauthorized or inappropriate access to system resources. It involves a modifying system or application features to achieve a goal outside its creator's original purpose.

<br>

### 🔷 **Who is a Hacker?**
A hacker is a person who breaks into a system or network without authorization to destroy, steal sensitive data or perform malicious attacks.

* Intelligent individual
* Exelent computer skills
* Ability to create and explore computer software and hardware

<br>

### 🔷 **Hacker Classes**
* **Black Hats**
    * Uses there extraordinary computer skills for illegal or malicious purposes.

* **White Hats**
    * Also known as penetration testers, using there skills for defensive purposes.

* **Gray Hats**
    * These people work both offensively and defensively at various times.

* **Suicide Hackers**
    * Suicide hackers are individuals who aim to bring down critical infrastructure and are not worried about facing jail terms of any other punishment.

* **Script Kiddies**
    * Unskilled hackers who compromise systems by running scripts, tools and software developed by real hackers.

* **Cyber Terrorists**
    * Wide range of skills, motivated by religious or political beliefs, to create fear of large-scale disruption of computer networks.

* **State-Sponsored Hackers**
    * Employed by the government to penetrate, gain top-level information from, and damage the information systems of other governments.

* **Hacktivists**
    * Hacktivism is when hackers break into government or corporate computer systems as an act of protest.

<br>

### 🔷 **Hacking Phases**

* **Reconnaissance**
    * As mentioned before, in this phase the hacker gathers as much information as possible of the target before launching an attack

* **Scanning**
    * In this phase the hacker uses the information gathered in the previous phase to scan the network for specific information for example open ports, network IP addresses, services, etc.

* **Gaining Access**
    * This phases is the phases where the real hacking occurs, the hacker uses the gathered information out of the scanning phase to search for vulnerabilities to exploit.

* **Maintaining Access**
    * After a hacker got access to the system with admin or root-level privileges, he/she can use both the system and the system resources at will. Therefor the hacker installs a backdoor or Trojan Horse to keep a way to access the system on a later moment.

* **Clearing Tracks**
    * A hacker will usually attempt to erase all evidence of their action to remain undetected but still maintaining access to the compromised system or network.

<br>

## **Ethical Hacking Concepts**

### 🔷 **What is Ethical Hacking?**
Ethical hacking is the practice of employing computer and network skills in order to assist organizations in testing their network security for possible loopholes and vulnerabilities.

<br>

### 🔷 **Why is Ethical Hacking Necessary?**
As technology is growing at a faster pace, so is the growth in the risks associated with it. To beat a hacker, it is necessary to think like one!

<br>

### 🔷 **Scope and Limitations of Ethical Hacking**
Ethical hackers determine the scope of the security assessment according to the client's security concerns.

*An ethical hacker should know the penalties of unauthorized hacking into a system. No ethical hacking activities associated with a network-penetration test or security audit should begin before receiving a signed legal document giving the ethical hacker express permission to perform the hacking activities form the target organization.*

<br>

### 🔷 **Skills of an Ethical Hacker**
* **Technical Skills**
    * In-depth knowledge of operation systems
    * In-depth knowledge of networking concepts
    * Knowledge of security areas
    * High technical knowledge on how to launch such attacks

<br>

* **Non-Technical Skills**
    * The ability to quickly learn and adapt new technologies
    * A strong work ethic and good problem solving and communication skills
    * An awareness of local standards and laws

<br>

## **Information Security Controls**
Information security controls prevent the occurance of unwanted events and reduce risk to the organization's information assets.

* **Information Assurance (IA)**
    * IA refers to the assurace of Integrity, Availability, Confidentiality and Authenticity of information and information system during usage, processing, storage and transmission.

* **Defence-in-Depth**
    * This is a security strategy in which security professionals use several protection layers throughout an information system.
    
    <br>

    ![DiD](https://img-blog.csdnimg.cn/20201129155053952.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3Rhb2YyMTE=,size_16,color_FFFFFF,t_70)

<br>

### 🔷 **What is Risk?**

* The probability of the occurance of a threat or an event that will damage, cause loss to, or have other negative impacts on the organization.

* The possibility of a threat acting upon an internal or external vulnerability and causing harm to a resource

* The product of the likelihood that an event will occur and the impact that the event might have on an information technology asset.

Relation between Risk, Threats, Vulnerabilities and Impact:<br>
**```RISK = Threats x Vulnerabilities x Impact```**

<br>

The impact of an event on an information asset is the product of vulnerability in the asset and the asset's value to its stakeholders:<br>
**```RISK = Threat x Vulnerability x Asset Value```**

<br> 

### 🔷 **Risk Level**
Risk level is an assessment of the resulted impact on the network.<br>
**```Level of Risk = Consequence x Likelihood```** 

### 🔷 **Risk Matrix**
The risk matrix scales the risk occurance or likelihood probability, along with its consequences or impact.<br>

![RiskMatrix](https://www.programmersought.com/images/459/209b2e55809ed8192372be0a58cd051b.png)

<br>

### 🔷 **Risk Management**
Risk management is the process of identifying, assessing, responding to, and implementing the activities that control how the organization manages the potential effects of risk.

* **Risk Identification**
    * Identifies the sources, causes, consequences of the internal and external risks.

* **Risk Assessment**
    * Assesses the org. risk and provides an estimate on the likelihood and impact of the risk

* **Risk Treatment**
    * Selects and implements appropriate controls on the identified risks

* **Risk Tracking**
    * Ensures appropriate control are implemented to handle risks and identifies the chance of a new risk occurring

* **Risk Review**
    * Evaluates the performance of the implemented risk management strategies

<br>

### 🔷 **Threat Modelling**
Is a risk assessment approach for analyzing the security of an application by capturing, organizing and analyzing all the information that affects the security of an application.

* **Identify Objectives**
    * Helps to determine how much effort needs to be put on subsequent steps

* **Application Overview**
    * Identify the components, data flows, and trust boundaries

* **Decompose Application**
    * Find more relevant details on threats

* **Identify Threats**
    * Identify threats relevant to your control scenario and context using the information obtained in steps 2 and 3

* **Identify Vulnerabilities**
    * Identify weaknesses related to the threats found using vulnerability categories

<br>

> **Go To [Module 02 - Footprinting & Reconnaissance]()**
