Unit 2

1. **Identify basic facts and terms about major components of a client**   
   1. Hardware   
      1. Physical part of the system  
      2. Motherboard   
         1. **Allows the components of computer to communicate**   
         2. Contains multiple paths of electrical circuits running through to form routes of communication   
            1. Allows the communication between   
         3. Example: Motherboard are the nerves that connect everything, while the CPU is the brain itself   
      3. CPU  
         1. **Communicating with all the other components**  
         2. Registers \= storage locations for the CPU   
         3. Clock Speed \= determines how much instructions the CPU can execute   
      4. GPU   
         1. To handle rendering graphics/generate output images to a monitor   
      5. ROM (Read Only Memory)  
         1. Non volatile   
            1. Can or cant hold its memory without power supply   
            2. Even without power applied to it, it can still hold memory tings like hard disks, cd are non-volatile   
         2. Needs to store permanently for the device to run   
         3. Contains read only memory   
         4. Relationship between ROM and RAM   
            1.   
      6. RAM   
         1. **Volatile**   
            1. Needs to have power applied to run data   
         2. What good is RAM?   
            1. Extra chunk of memory to juggle tasks   
         3. **Temporary storage**  
         4. Example:   
      7. Storage  
         1. Allows you to store digital data   
         2. Two types of drives   
            1. SSD (Solid State Drives)  
               1. Faster, less power, **flash memory chips**,   
            2. HDD (Hard Disk Drives)   
               1. Slower, requires more power, individual **magnetic disks**   
               2. Moving parts   
            3. Differences   
         3. Has sectors (smallest unit on the device)  
         4. Has partitions (section of the drive that logically separated from the other segments)   
      8. PSU (Power Supply Unit)   
         1. Converts power from the main output into low voltage for the computer to use   
         2. You need a switch to change between voltages, conditions the power   
   2. Software   
      1. Coding and instructions to tell the computer how to work   
      2.   
2. **Identify  relationship of basic facts and state general principles about Theory of operations**   
   1. Theory of Operations   
      1. System boot up instructions are stored in the **ROM (Read only Memory)**   
      2. Sequence   
         1. BIOS   
            1. Performs POST   
               1. Runs built in diagnostic and report back the result   
            2. Looks for a bootable device from the boot sequence (order)   
               1. Where to BOOT?   
         2. Boot Loader   
            1. Provides instructions from the Master Boot to the CPU   
               1. MBR \= tells BIOS where to find the OS so system can boot up   
            2. Loads OS instructions into the RAM   
         3. Kernel   
            1. Registry is loaded first, then drivers   
               1. Register that has information   
            2. Control is handed over to the user   
   2. CPU Modes  
      1. User Mode  
         1. **Not just for humans, but also for applications as well**, where an app ask for permission to do certain things such as asking for your location   
         2. Restricted/unprivileged   
            1. You don't automatically have elevated privileges   
            2. By default, its restricted   
         3. Applications run at this level   
         4. **Doesn't have direct access to hardware resources, it needs to go through a level of software which might cause a delay**   
            1. Level of abstraction   
      2. Kernel Mode  
         1. You can directly access the hardware, unrestricted/privileged   
            1. Meaning it’s lockdown   
         2. Core operating systems/hardware run at this level

         

3. **Identify basic facts and terms about client software**   
   1. **Operating System**   
      1. Bridge between the human user and the computer hardware  
         2. Applications run off of the OS    
         3. Manages hardware and software resources for a computer   
      2. **Windows Operating System**  
         1. Components   
            1. Interface  
               1. Command Prompt. Power shell, Search, Action center, start menu   
               2. GUIs   
            2. Drivers  
               1. Lets OS and device communicate with each other   
               2. Basically like a translator   
            3. Registry  
               1. Central hierarchical Database that stores necessary configuration information  
                  1. Record that has a list of all your settings   
            4. Security  
               1. Uses password protection, file encryption, and limited privileges to control access to data and prevent unauthorized configuration changes   
            5. File Management   
               1. FAT-32   
                  1. Used to be a fat kid   
                  2. 4GB max file size  
               2. NTFS   
                  1. Complex  
                  2. 16 TB file size   
                  3. encrypted   
                  4. Automatic troubleshooting is present   
                  5. Supports file compression   
                  6. User level disk space is present   
            6. Client Applications  
               1. Application software that do real work for users  
               2. Unable to run without OS platform  
   2. Desktop vs Laptop   
      1. Difference is the main form factors, where laptops are to be a lot more compact   
4. **Identify basic facts and terms about client OS installation**   
   1. OS Installation \- Windows   
      1. Steps  
         1. PC   
            1. Find a access to a device   
         2. BIOS CMOS   
            1. Change the CMOS boot order, so your installation media is the first boot device   
               1. Whether that is a USB drive or USB C drive   
            2. CMOS is the battery that goes on the motherboard, stores hardware settings  
            3. Gives user control over PC hardware. Security settings, boot device order, internal device options   
         3. Windows installation media   
            1. Insert commercial, purchased media   
         4. Windows activation key   
            1. Active using the activation key 

Unit 3 (Virtualization)

1. **Identify basic facts and terms about tech and applications**   
   1. Virtualization \= creates an abstraction layer   
      1. Extra space and gap between hardware and users   
      2. Ex: within your OS, you can create a separate OS which acts like a different computer   
      3. Components   
         1. Host Server (machine that hosts that VM)  
            1. Computer on which virtualized environment resides   
         2. Virtual Machine (emulation itself)  
            1. Emulation of computer system using the host’s hardware  
            2. Not the actual physical machine   
         3. Hypervisor (runs the VM)  
            1. Software layer that creates and runs VMs. Interfaces between VM and Hardware   
            2. Creates and runs the VMs   
         4. Guest OS   
            1. Installed on a VM that allows for ender user interaction that is indistinguishable form a standard physical computer  
      4. Hypervisor Types   
         1. Bare Metal   
            1. Installed on hardware   
         2. Hosted   
            1. Installed on OS like most applications   
2. **Identify basic facts and terms about the benefits of virtualization**  
   1. Advantages of Virtualization   
      1. Reduces operational costs   
         1. Less hardware and maintenance of hardware   
      2. Minimizes/eliminate downtime   
         1. You got fewer points of failure, less hardware involved as long as you have the hardware   
      3. Productivity and Efficiency increase 	  
         1. Sharing resources, multiple OSs  
      4. Offers flexibility and scalability  
         1. Re-allocation for workload, can be customizdd to fit needs of organization   
   2. Disadvantages   
      1. Physical hardware performance   
         1. You need higher end hardware or you will see an impact   
         2. Hypervisors run on the physical hardware of device   
      2. Security Risk   
         1. Volatility of virtual servers, requires good security program (VM escapes)  
      3. Additional Training Requirements   
         1. New processes and methodologies,   
3. **Identify basic facts and terms about virtualization security**  
   1. Prevention   
      1. Hardening   
         1. Securing a system by reducing its surface of vulnerability  
      2. Examples  
         1. Removing unnecessary hardware   
         2. Disable copy paste between system and VM   
         3. Patch the OS   
            1. DISA is the ISP   
            2. List of patches, STIGs  
         4. Disable unused services   
            1.   
         5. Prevent further allocation of hardware   
            1. Limit what the VM is allowed to access   
4. **Identify basic facts and terms about host server hardware**   
   1. Hardware requirements for host device are dependent upon the number and roles of virtual machines managed   
      1. CPU and RAM \- how many VMs can be supported   
         2. Storage \- ensures allotted space for VMs stored on host   
         3. Network Interface Card \- bandwidth and speed   
         4. input/Output \- to interact with each other 

Units 4 (Server)

1. Identify basic facts and state general principles about server types   
   1. Server \= providing services and functionality to other computers on the network, can also manage resources on a network, which include but are not limited to data users, security   
   2. Network Models   
      1. Peer to Peer   
         1. Everyone acts as a both to client and a server, can request and respond to services   
         2. Airdrop is peer to peer   
      2. Client Server   
         1. Client makes requests and server respond with services   
         2. Client vs. Server  
            1. Server needs more security, holds more information, and supports many users, can both host firewalls and similar hardware   
            2. Client needs less security, hold less info, makes requests  
      3.   
2. Identify relationship of basic facts and terms about server security processes and concepts   
   1. Server Security   
      1. Best practices   
         1. Disable devices from being plugged in   
         2. Man-traps, key into the server room   
            1. Outer door and inner door   
         3. One admin account, rotating passwords   
            1. People think its insecure to have one admin account, same login and passwords but the passwords rotate   
            2. Every elevated account is another attack vector, gives a hacker gives more attack vectors   
         4. Disconnect from network   
            1. Prevent any traffic from traveling to anyone connected to server  
      2. Server Types   
         1. Web Proxy   
3. Identify relationship of basic facts and state general principles about active directory   
   1. Regular directory vs active directory  
      1. List of organizing resources versus used for managing permissions and user/group access to network resources   
   2. Types of Server Roles  
      1. Active Directory Domain Services (ADDS)   
         1. A list **organizing resources** and associates their characteristics; similar to a telephone directory   
         2. **Manage provisions**   
         3. Logical Structure Partition   
            1. Forrest   
               1. Set of one or more domain trees   
               2. Contains multiple subnetworks that have security domains, but they have a common namespace  
               3. Ex: 81st training wing is a host domain, and subdomains are the groups with squadrons   
            2. Tree  
            3. Domains   
               1. A security or admin boundary   
            4. Organizational Units (OU)  
               1. Container within a domain where you can place users, groups, computers, and other organizational units   
            5. Objects   
               1. User, group, computer, application, etc  
         4. Active Directory Physical Structure   
            1. Sites   
               1. Where is it set up  
               2. Maps the physical structure of the network  
            2. Domain Controller   
               1. Manages the domain security policy   
            3. Global Catalog Server  
               1. Allows access to network resources in other domains within a tree or forest   
               2. Allow you to move between domains  
               3. Gotta go through a   
            4. Member Servers  
            5. Domain Clients  
4. Identify the relationship of basic facts and state general principles about DNS and DHCP  
   1. Domain Name System (DNS)  
      1. Resolves domain names to IP addresses   
      2. Path  
         1. /filepath  
      3. Top level domain   
         1. .com, .net, .mil, .us, .ul, .ip  
      4. Domain Name   
      5. Subdomain   
      6. Ex: www. Google .com/ login   
         1. ^ subdomain ^domain ^ top level ^ path   
   2. Dynamic Host Configuration Protocol (DHCP)   
      1. Standardized protocol that enable clients to be dynamically assigned an IP with various configuration parameters   
      2. DORA   
         1. Discover  
            1. Client Sends out a DHCP discover messages to identify DHCP servers  
            2. Switch has to realize new client,  
         2. Offer   
            1. Server Offers an address  
         3. Request   
            1. But client needs to request an address from the server  
         4. Acknowledge   
            1. Server ack the IP request and completes initiation cycle 

Units 6 Cyber Hygiene

1. Identify basic facts and terms pertaining to network user habits   
   1. **Cyber Hygiene**   
      1. Set of practices that maintain system health and improve online security   
   2. Good User Habits  
      1. Using firewalls   
         1. On both personal and   
      2. Update Virus Definitions (antivirus software)   
         1. Enable automatic updates   
      3. Running Security Scans   
      4. Select and maintain passwords   
         1. Long is better  
         2. Mix of characters  
         3. Dont use dictionary words   
         4. No obvious substiutitons   
      5. Update software   
         1. Enable auto updates   
      6. Back up data   
         1. Multiple locations   
   3. Securing Personal Data   
      1. Read Privacy Policies   
         1. Tells you how sites maintain, security, and control, of the personal info it collects  
      2. Device Disposal   
         1. Always wipe devices memory before discarding   
         2. Use a wipe utility program to overwrite hard drives  
2. Identify basic facts and terms pertaining to anti-piracy and ethics   
   1. Anti Piracy   
      1. Unauthorized copying downloading or installing of copyrighted software  
      2. Control Measures  
         1. DAFMAN 17-1203   
      3. Penalities  
         1. Can have civil or criminal penalties   
            1. Monetary pay back to owner or jail time and paying a fine   
      4. Computer Ethics   
         1. Use Gov Systems responsibility   
         2. Protect Information   
         3. Respect Intellectual Property   
         4. Be Professional Online   
         5. Monitoring  
            1. By using this system, you are consenting to monitoring  
            2. SItes you visit, keys be logged, sharedrive, everything you access is monitored 

Units 7 Security Programs

1. Provide appropriate instructional materials, identify basic facts pertaining to   
   1. **COMPUSEC**   
      1. Computer Security and is implement of measures to **protect info systems resources and information**   
         1. Really broad term   
         2. Employs countermeasures for Confidentiality, Integrity, and Availability   
      2. Confidentiality   
         1. Unauthorized access  
         2. Access control/permission  
            1. Only appropriate user can access the files   
         3. Encryption   
            1. Taking a readable product and use a mathematical algorithm to make it unreadable   
            2. In storage and in transit   
         4. Steganography   
         5. Physical protections  
            1. Locked doors, fences, security cameras, etc all help ensure only authorized   
      3. Integrity   
         1. Hashing,  
            1. Was the data changed? Or manipulating?  
            2. Sends data through hashing algorithm, and generates a hash value and sends it with a file, thne receive system chck for matching hash value   
         2.  digital signatures   
            1. Signs message with seneder’s private key, proving it from the sender   
         3. digital certificate  
            1. Electronic file used to transport encryption/signature keys  
         4. Non-repudiation   
            1. Can’t deny that you sent something because you have some sort of fingerprint on it   
         5. Data is not altered or deleted   
      4. Availability   
         1. Permission   
            1. Can limit who can delete data, maintaining availability   
         2. Backups  
            1. Performing regular backups allows restoral if data is corrupted    
         3. Fault tolerance   
            1. Data redundancy using multiple storage drives such as RAID   
         4. Clustering   
            1. Multiple servers acts as one unit so if one fails, others take   
            2. Failover   
         5. Patching   
            1. Reduces vulnerabilities for attacks   
      5. COMPUSEC Threats and Vulnerabilities  
         1. Unauthorized access   
            1. Person gaining access to computer hardware, software or information is a failure of COMPUSEC   
            2. Can occur remotely or covertly   
               1. Covertly is physical access to the location  
         2. MAlicious Logic   
            1. Viruses,   
               1. Requires human interaction   
            2. Worm  
               1. Like a virus and can self-replicate and doesnt need to have human interaction   
            3. Trojan	  
               1. Looks like a program that is legit or safe, but it has malware   
            4. RAnsomware/Steal-ware   
               1. Malware infects the system and encrypts the data drives and then sends them a ransom   
            5. Spyware  
         3. Fraud Waste and Abuse (FWA)  
            1. Deception to unlawfully deprive USAF of something of value, or for an individual to secure an unentitled benefit   
            2. Examples include:  
               1. Unauthorized printing   
               2. Unauthorized internet use   
            3. Waste \-\> Abuse \-\> Fraud   
   2. TEMPEST  
      1. Program to ID vulnerabilities in information systems processing national security information   
      2. **UNINTENTIONIAL EMANATIONS,** Leads to compromising emanations   
      3. Unintentionally emitted signals   
         1. If it escapes the facilities   
         2. Electromagnetic interference   
            1. Every electronic device emits electromagnetic interference to some degree. They can radiate strongly enough to interfere with or compromise comms   
      4. Counter Measures   
         1. Product Distribution Systems (PDS)  
            1. Wired telecom system with safeguards to allow transmission   
         2. HDS (Hardened Distribution system)  
            1. Hardened conduit material, typically metal   
         3. Simple Distribution SDS   
            1. Reduced level such as wood or plastic   
         4. Red/Black Separation  
            1. Red Signal  
               1. Plaintext   
               2. sensitive /classified plain text   
            2. Black SIgnal  
               1. Encrypted (cipher text)   
   3. INFOSEC  
      1. To protect **classified national security information and controlled unclassified information (CLASSIFIED AND CUI)**   
      2. 3 Disciplines  
         1. Personnel Security   
            1. Determines military, civilian, to access classified   
         2. Industrial Security   
            1. Civilian workforce   
            2. External third party   
            3. Industry outside the military complex   
         3. Information Security   
            1. Protects classified/CUI in general   
      3. FOIA   
         1. Provides public the right to request records from Federal Agencies  
         2. Exemptions fall under:   
            1. Personal privacy  
            2. National Security  
            3. Law Enforcement   
      4. Information Designations   
         1. Controlled Unclassified Information (CUI)  
            1. Unclass info that requires access and distribution controls and protective measure to keep it secure  
            2. Privacy act information (1974)  
               1. How long we have to keep records for   
               2. Examples include social security numbers, age, address, etc   
         2. Classified Information (CI)  
            1. Require protection against unauthorized is in the interest of national defense  
            2. Disclosure of classified material could cause damage to national security   
            3. Confidential   
               1. Can cause some damage  
               2. USPS **certified mail or first class mail** to DoD contractors   
            4. Secret  
               1. Can cause serious damage  
               2. USPS **registered mail** within the US   
            5. TS   
               1. Can cause exceptionally grace damager   
               2. Dept of State carrier   
   4. **OPSEC**  
      1. Reduce mission vulnerabilities by reducing adversary collection of **critical information**   
         1. Whatever can help the enemy or hurt us   
         2. Ex: Not talking about deployments, when your gonna take off etc   
      2. Critical information   
         1. Specific facts about activities and capabilities needed by adversaries to plan and act effectively   
      3. Indicator   
         1. Anything that adversary can collect by watching the new, like planning an exercise or planning for a deployments   
         2. Open source information   
         3. A unit getting ready for a deployment vs knowing exactly when it is   
      4. OPSEC Vulnerabilities   
         1. Social MEdia  
         2. Open Conversations   
         3. Critical Information   
         4. Private Messaging and Text Messaging   
         5. Family and friends   
   5. **COMSEC**  
      1. Measures and controls **to deny unauthorized information** derived from government systems   
      2. Ex: Classified information systems, radios, encryption keys  
      3. Encryption   
         1. Conversion of data into a form that is not easily deciphered   
      4. Decryption  
         1. Restoration of  encrypted data to its original readability   
      5. Cryptography   
         1. Use of coding system to encrypt and decrypt info   
      6. Crypto analysis:  
         1. Science of trying to break a coding system so that their information can be revealed to an unauthorized user   
      7. COmponents of COMSEC  
         1. Cryptosecurity   
            1. Protection from cryptographic systems   
         2. Transmission Security (TRANSEC)  
            1. Intentionally transmitted signals  
            2. All measures designed to protect **intentional transmissions and exploitations**   
            3.  **Sending classified materials over an unclassified network would be a TRANSEC failure**   
         3. Physical Security   
            1. Protection that results from physically protecting against vulnerabilities   
            2. Vulnerabilities  
               1. Improper destruction of waste  
               2. Improper handling   
            3. Safeguards  
               1. Physical barriers  
               2. Sharing COMSEC in GSA approved safe   
                  1. Must of appropriate classification or higher 	  
               3. Limiting COMSEC access 

Unit 8 Risk Threats and Vulnerabilities

Computer Network Attack Types

1. Threat Framework  
   1. Spoofing  
      1. Pretending to be something other than yourself   
   2. Tampering  
      1. Malicious modification of data   
   3. Repudiation   
      1. Claiming you did not do something or were not responsible   
   4. Information Disclosure   
      1. Providing info to someone not authorized to access it   
   5. Denial of Service   
      1. Exhausting resources needed to provide service   
      2. The goal is to exhaust resource   
         1. DDOS   
            1. Flood the switch with requests   
   6. Elevation of Privilege   
      1. Unprivileged user gains privileged access   
2. Threat Agents   
   1. Inside Attack  
      1. Malicious insider   
      2. Initiated by entity inside the security perimeter   
         1. Granted access but misused   
      3. Human error   
   2. OUtside Attack   
      1. Initiated by entity outside the security perimeter   
      2. Gains unauthorized or illegitimate access   
      3. Threat actors ranging from  
         1. Competitors   
         2. Script kiddies   
            1. Can buy it and buy pre made tools and scripts   
         3. Criminal syndicates   
         4. State actors   
3. Computer Network Attack  
   1. Intentional act by which a threat attempts to evade security   
   2. Characterized by   
      1. Intent   
      2. Point of initiation   
         1. Attack vector, weak point in your security   
      3. Method of delivery  
         1. Some type of malware   
         2. STUXNET  
            1. Virus of damaging physical equipments  
   3. Types of Computer Network Attacks  
      1. Denial of Service   
         1. Sends more requests to a machine than it can handle   
         2. **Toolkit**  
            1. Used to make DoS attacks easier to execute   
            2. Runs a prebuilt program to overwhelm a host with requests   
      2. DDOS   
         1. Using multiple bots working in multiple coordination   
         2. Multiple systems orchestrate a synchronized DoS attack to a single target   
         3. DDOS prevention   
            1. Run servers before capacity  
               1.    
            2. Packet filtering   
            3. Security patches   
      3. Unauthorized Access  
         1. Most likely trying to steal data   
         2. Allows an attacker access to info they should not have   
      4. Executing commands illicitly   
         1. Unknown and untrusted person executes commands on a server  
      5. Destructive behavior   
         1. Data diddling   
            1. Attacker changes entries in record   
            2. Very dangerous   
            3. Usually not obvious   
               1. **Extremely hard to detect**   
         2. Data destruction   
            1. Attacker deletes files   
            2. Can impact computing capability 

Social Engineering

4. Social Engineering   
   1. People are the weakest link in cybersecurity   
   2. Psychological manipulation   
   3. Types of Social Engineering  
      1. Phishing   
         1. Attempts to acquire sensitive data   
         2. **Sphear Phishing**  
            1. Targets a specific individual   
            2. Utilizing message that appeals to that person   
         3. **Whaling**  
            1. For high value targets  
      2. Baiting   
         1. **Preys on curiosity or greed**   
            1. Ex: leaving an infected flash drive in a public place   
            2. If you give me $500, then i’ll give you a 1000   
      3. Piggybacking or Tailgating   
         1. Piggybacking   
            1. Lying about losing a badge   
         2. Tailgating   
            1. Literally following someone through access points   
      4. Impersonation   
      5. Dumpster Diving   
         1. Digging through the garbage   
   4. Targeted Phishing  
      1. Spear Phishing   
         1. Target specific individual  
      2. Whaling   
         1. Targeting high value individuals liek CEO CFOs   
   5. Mitigating Social Engineering  
      1. User Training and Awareness  
      2. Not opening emails or attachments from suspicious sources   
      3. Enabling multifactor authentication   
      4. Regularly update anti-virus/anti-malware programs 

Malicious Code

5. Malicious Code   
   1.  Designed to infiltrate or damage a computer system through email and internet   
   2. Computer Viruses   
      1. Code that infects a host   
      2. Requires user executions, replicates across the network   
   3. Worms   
      1. Once activated, they can self-replicate throughout the network   
      2. Worm does not require user execution   
   4. Boot Sector Malware   
      1. Resides in the first sector of a disk  
      2. Controls the boot sequence  
      3. Even if you clean it off, you can still have that on that   
   5. Polymorphic Malware   
      1. Shape shifting   
      2. Virus changes every it runs   
   6. Macro Malware  
      1. Code that uses macro language to perform a malicious action   
      2. Supported by most applications, automate tasks within applications   
   7. Logic Bomb   
      1. Software acts normally until predefined event occurs   
   8. Trojan horses   
      1. Tricked into installing something that looks like a legitimate application or program  
   9. Rootkits   
      1. Hidden software that gives hacker privilege/root access to a computer system   
   10. Spyware   
       1. Hidden software that monitors and collects info  
   11. Adware  
       1. That automatically loads ads on the screen  
6. Symptoms of Infection  
   1. If system is acting abnormal,  
      1.  computer will not boot   
      2. Computer will not boot,   
      3. a partition is lost,   
      4. hard drive is reformatted   
      5. Programs close and open without input   
      6. Warning and error messages   
7. Mitigation Mechanisms   
   1. It has already happened, prevention measures that stop unauthorized users from accessing par  
      1. Vulnerability Scanning   
         1. Mimic malicious network that hosts could encounter   
      2. Software Patching  
         1. Repairing a vulnerability or a flaw that is ID’d after the release of an applicaiton or software   
      3. User Awareness   
         1. Training informs users of common pitfalls and what they can do to mitigate them   
      4. Firewall  
         1. Restricts communications to and from the network   
         2. Protects network resources against threats   
         3. Packet filtering   
            1. Inspecting the traffic in the network   
         4. Why is it called a firewall?   
            1.   
      5. Anti-Spyware   
         1. Prevents spyware from collecting information about the user   
      6. Mail Gateway   
         1. Server within an organization's demilitarized zones that sends and receives email   
            1. **DMZ is the area between two firewalls**   
            2. Mail servers are placed in the DMZ   
         2. Server within an organization's demilitarized DMZ that sends and receives  
   2. Detection  
      1. Use to determine if someone attempted to break into a system,   
      2. Anti-Virus   
      3. Monitor Logs 

Supply Chain

8. Supply Chain   
   1. Entities such as third party vendors or small businesses coordinating to get products to a final destination   
   2. Vulnerabiltiies  
      1. **Third Party**  
         1. Middleman or subcontractor that provides a product or a service in support of the primary of an organization  
      2. Supply Management   
         1. Sourcing, supply chain continuity and quality   
      3. Third Party Data Storage   
         1. Cloud computing relies on a third party to handle your data, which could   
         2. Moving in house services off site and putting them in the hands of a third party   
         3. **Ensuring how the third party is securing data is an important prerequisite when considering cloud computing**   
   3. Solutions  
      1. Talk to your resource advisor, **BECO**, and or the contracting squadron   
      2. When purchasing IT equipment for the AF network, always make sure it’s on **approved product list** (not a guarantee just because its an AF Way) 

## Unit 9 Network Security

### Identify basic facts pertaining to NAC 

1. NAC \= allows control of access based on predefined conditions that system must meet prior to being granted onto a network,   
   1. Looking for system patches, seeing if system is up to date before granting access  
   2. Agent-Based   
      1. Installed on the clients   
      2. Permanent Agents  
         1. Installed on the system and doesn’t go away  
      3. Dissolvable Agents  
         1. Install and uninstall after authentication   
   3. Agentless  
      1. Does not require agent software to be installed on agent   
   4. **Authentication**  
      1. Verification process where secured system access requires individuals to identify themselves and for a system to verify that they are who they say they are   
      2. Popular approach for hardening the network ensure that anyone who connects suppliers before   
      3. **Factors**  
         1. Something you know   
            1. Password   
            2. pin  
         2. Something you have   
            1. Physical tokens   
            2. Codes sent via text   
         3. Something you are   
            1. Biometrics   
            2. Facial Recognition   
         4. Somewhere you are   
            1. GPS location   
            2. IP address   
         5. Something you do   
            1. Based on habits   
            2. Typing patterns   
      4. Single Sign On (SSO)  
         1. Authenticate once, and then those credentials are shared across the multiple websites and systems without needing to provide additional credentials   
      5. Network Security Enforcement   
         1. IEEE  
            1. 802.1X   
               1. Must present valid credentials on a system with agent based NAC   
            2. Host Health Checks   
               1. Scans a system attempting to connect to the network for operating system updates, antivirus software and host-based firewalls   
            3. Terms of Usage   
               1. Users may be required to accept terms of usage before permitting them access to a network 

### Identify basic facts pertaining to networking authentication, authorization, and accounting 

5. Authentication, Authorization, and Accounting   
   1. Authentication (verifying who they claim to be )  
      2. Authorization (what are they allowed to access)  
      3. Accounting (Logging what people do and documenting actions)   
   6. Identification  
      1. Presenting info about yourself, identification is not PROOF  
      2. Also typing a username is a form of identification   
      3. Just making a claim  
   7. Authentication  
      1. Verification process requires individuals and for a system to verify that they are who they say they are   
   8. Authorization  
      1. Determines what a user has authority to do and what they have acces to   
   9. Accounting  
      1. Tracks and records user access time, bandwidth usage, and   
   10. RADIUS   
       1. Allows clients to access a **network remotely** through UDP to a RADIUS server   
   11. DIAMETER   
       1. Newer AAA protocol that gives a more reliable and secure communication service through TCP   
   12. TCP \= protocol that guarantees delivery of data   
       1. Forcing the host that its sending data to ack and sends a receipt   
       2. But takes more bandwidth   
       3. 3 way handshake   
   13. UDP \= lightweight, doesn't require ack of receipt of data, just streams the data 

### State general principles pertaining to Application Security

1. Peer to Peer (P2P) File Sharing: file can be shared online between users through peer to peer file sharing applications. Common method of transmitting malicious code   
   2. Scripting: executing a list of commands to be performed by a program, it can make modifications to a system without user input   
      3. Cross Site Scripting: injects malicious code into a website,   
      4. Vulnerability Prevention:   
         1. Apply software updates  
         2. Application Configuration Baseline  
            1. Process of   
         3. Application hardening   
            1. Disable unnecessary application features   
         4. Cross site request forgery prevention  
            1. Remember me should be disabled in the browser   
            2. Tracks ur sesssion, and steals your identity   
   14. Host Instruction Control  
       1. Intrusion Detection System  
          1. Detects suspicious activity on host or network and then alerts system   
       2. Intrusion Prevention System  
          1. Monitors hosts or networks for suspicious activity and takes corrective actions   
       3. Host based or network based (HHIDS/HIPS) NIDS/NIPS) 

### State general principles pertaining to Hardware Security 

15. Vulnerability protection that comes in form of a physical device   
    16. Hardware Security Threats  
        1. Boot Sequence Threats   
           1. **Enable secure boot or trusted boot t**o prevent malware and corrupted components from loading as windows is starting up   
        2. Removable Storage Threats   
           1. **USB data ports** are disabled on DoD computers to prevent data theft and to prevent worms from spreading  
           2. Plugging a USB drive will trigger Host Based Security System   
           3. Can also physically disable ports or restrict physical access  
    17. Theft   
        1. Devices are investments. So susceptible to people stealing it   
    18. Theft Prevention  
        1. Protect through limited physical access  
           1. Access to server rooms should be controlled   
           2. Portable devices with lockdown cables and secured to desks   
    19. Hardware Encryption  
        1. Uses chips physically in the system and applies very complex encryption more quickly than software encryption   
        2. Usually faster than software   
        3. TPM (trusted platform module)   
           1. Stores cryptography keys used to encrypt the data   
           2. Bitlocker   
        4. HSM(hardware security module)   
           1. External service or device that stores multiple crypto processors, installed on a system   
           2. Stores crypto processors on a separate card installed on a system

## Unit 10: Firewalls

### Firewalls

Hard/soft-ware to protect IT from outside systems

* **Allowlisting** \- explicit allow; deny by default  
* **Dentylisting** \- explicit deny; allow by default

#### Software Firewall

* Installed in single system (e.g. ur computer)  
* Block in/out traffic  
* Notification for potentially bad connections  
* Can **Create Rules** to customize permitted traffic  
* E.g. Windows Firewall

#### Hardware Firewall

* Standalone appliance, acts as **secure gateway for network perimeter**  
* \+More Efficient \- funnel traffic thru single point; ideal for medium-large networks  
* \-More Complex \- require more knowledge to configure

#### Types of Firewalls

* **Packet Filtering** (simplest) \- Filter based on IP/PORT  
* **Stateful Inspection** \- check connection state; e.g. only allow inbound packets for outbound-initiated connection  
* **Application Layer/Next Gen** (most advanced)  
  * E.g. IDS, IPS  
  * **Deep packet inspection** \- understands service protocols and inspects contents

### Demilitarized Zone (DMZ)

## Unit 11: Publications and Personnel Security

### Personal and Equipment Protection

#### Personal Safety

* Electrostatic Discharge (ESD) \- electricity between two charged obj. Scary.  
* Grounding \- provides path for elect to flow safely into the ground  
* Bonding \- minimizes scary between conductive objects

#### Equipment Protection

* Active \- armed patrols, dogs, cameras, etc.  
* Passive \- Barriers, Bright lighting, limit entrances

### Publications and Directives

* **Pubs and Dirs** \- official documents for compliance, implementation, or information (AFMAN 33-361)  
* **DoDI** \- **establish** policy and general guidance  
* **DoDM** \- **Implement** policy from DoDI with details  
* **Air Force Instruction (AFI)** \- direct action, ensure compliance, or detailed guidance/procedures. Standardization  
* **Air Force Manual (AFMAN)** \- extension of instructions; does **not need to fall under AFI**; can stand **in place of AFI**  
* **Military Standards (MIL-STD)** \- DoD standardization for (fiber optic cabling requirements and measurements, etc.)  
* **STIG** \- DISA implementation guide for standardizing security and IT  
* **SOP** \- Step by step instructions for routine stuff  
* 

## Unit 12: Incident response

### IR facts and terms

* Computer Incident Respone Team (CIRT) \- handle, correct, document security incidents  
* IR Team  
  * Team Leader \- lead team, build relations with outside resources  
  * Tech Specialist \-  tech expertise to ID scale of incident and correct  
  * Doc specialist \- document incident/cause/solution  
  * Legal advisor \- Know laws and regs  
* Elements in IR plan  
  * Defined Incident Categories  
  * Roles and Responsibilities  
  * Reporting Requirements/Escalation  
  * CIRT  
  * Exercise Planning  
* Event \- Anything observable, can indicate incident  
* Incident \- Assessed occurence that jeapordizes CIA  
* IR Categories  
  * 0: Event	| Training/exercise  
  * 1: Incident 	| Root  
  * 2: Incident 	| User  
  * 3: Event 	| Unsucessful DOS  
  * 4: Incident 	| DOS  
  * 5: Event	| Non-compliance  
  * 6: Event	| Recon  
  * 7: Incident	| Malicious Logic  
  * 8: Event	| Under investigation  
  * 9: Event	| Explained anomaly  
* Classified Message Incident (CMI)  
  * Doesn’t fall into cats  
  * Transfer of confidential+ info  
  * Requires investigation and destroy unclass media  
* First Responder \- first user to ID and react to incident, trained for basic response

### IR principles and techniques

#### IR Handling Process

1. **Detect & Report Events** \- IDS, personnel reports; gather/report info; begin response  
2. **Prelim Analysis & ID** \- Categorize; gather info; classify; send notif messages  
3. **Prelim Response Actions** \- Contain Incident/threat; preserve data; begin chain of cust  
4. **Incident Analysis** \- technical details, root cause, potential impact  
5. **Response/Recovery** \- Prevent damage, Restore Integrity, Implement follow-up strats  
6. **Post-incident analysis \-** Review lessons learned, root cause, misc. problems

### Root Cause Analysis

#### Incident Analysis

Analsis steps to find out what happened \+ root cause; AFI 17-203

1. Gather Info  
2. Validate incident \- review, corroborate, update  
3. Determ ops impact  
4. Coordinate \- with victim’s system & support agency  
5. Determ reporting reqs \- within **one hour** if incident meets Commander’s **Critical Information Requirements (CCIR)**

#### Concluding CoA’s

* **Postmortem**: Provides **Post-Incident Analysis** recommendations to affected units for corrective actions  
* **Cyber Incident Report (CIR)** \- analysis of affected system, attacker, attack vector, & technical \+ operational impact  
* **Network Intel Report (NIR)** \- analysis of incident, multiple incidents, or network activity of threat actor