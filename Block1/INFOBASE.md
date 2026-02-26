## Unit 2: Client Basics

### Hardware

* **Motherboard** — allows components to communicate via electrical circuit paths; the "nervous system" connecting everything
* **CPU** — communicates with all components; contains *registers* (storage locations) and runs at a *clock speed* (instructions per cycle)
* **GPU** — renders graphics and generates display output
* **ROM** (Read-Only Memory) — non-volatile; retains data without power; stores permanent boot instructions
* **RAM** (Random Access Memory) — volatile; requires power; temporary storage for active tasks
* **Storage** — persists digital data
  * **SSD** — faster, lower power, uses flash memory chips
  * **HDD** — slower, higher power, uses magnetic disks with moving parts
  * Both use *sectors* (smallest storage unit) and *partitions* (logical drive segments)
* **PSU** (Power Supply Unit) — converts AC mains voltage to low DC voltage for components

### Theory of Operations

Boot sequence stored in ROM:

1. **BIOS** — runs POST (power-on self-test); identifies bootable device per boot order
2. **Boot Loader** — reads MBR to locate OS; loads OS into RAM
3. **Kernel** — loads registry then drivers; hands control to user

#### CPU Modes

* **User Mode** — restricted/unprivileged; used by applications; no direct hardware access (goes through abstraction layer, may cause delay)
* **Kernel Mode** — unrestricted/privileged; used by core OS and hardware drivers

### Client Software

#### Operating System

* Bridge between user and hardware; manages hardware and software resources
* Applications run on top of the OS

#### Windows OS Components

* **Interface** — GUI, Command Prompt, PowerShell, Start Menu, Action Center
* **Drivers** — translate between OS and hardware devices
* **Registry** — central hierarchical database storing system configuration settings
* **Security** — password protection, file encryption, limited privileges
* **File Systems**
  * **FAT-32** — max 4 GB file size; older/simpler
  * **NTFS** — max 16 TB; supports encryption, compression, user disk quotas, auto troubleshooting
* **Client Applications** — user-facing software; requires OS to run

### OS Installation — Windows

1. Access a PC
2. **BIOS/CMOS** — change boot order so installation media boots first; CMOS battery stores hardware settings
3. Insert Windows installation media (USB)
4. Activate with Windows activation key

---

## Unit 3: Virtualization

### Virtualization Basics

**Virtualization** — creates an abstraction layer between hardware and users, enabling multiple OSs on one machine

#### Components

* **Host Server** — physical machine that hosts the VM
* **Virtual Machine (VM)** — software emulation of a computer system using host hardware
* **Hypervisor** — software layer that creates and runs VMs; interfaces between VM and hardware
* **Guest OS** — OS installed on a VM; appears identical to a physical machine to the end user

#### Hypervisor Types

* **Bare Metal (Type 1)** — installed directly on hardware
* **Hosted (Type 2)** — installed on top of an existing OS like a regular application

### Benefits of Virtualization

#### Advantages

* **Reduced operational costs** — less physical hardware and maintenance
* **Minimized downtime** — fewer points of failure
* **Increased efficiency** — share resources across multiple OSs simultaneously
* **Flexibility and scalability** — reallocate workloads; customizable to org needs

#### Disadvantages

* **Hardware overhead** — requires high-end physical hardware; hypervisor adds performance cost
* **Security risk** — VM escape vulnerabilities; requires strong security program
* **Training requirements** — new processes and methodologies

### Virtualization Security

**Hardening** — reduce attack surface by:

* Removing unnecessary hardware
* Disabling copy-paste between host and VM
* Patching the OS (using STIGs from DISA)
* Disabling unused services
* Limiting VM hardware resource allocation

### Host Server Hardware Requirements

Dependent on number and roles of VMs:

* **CPU & RAM** — determines how many VMs run simultaneously
* **Storage** — space allocated for VM images
* **NIC** — bandwidth and network speed
* **I/O** — interaction between host and VM components

---

## Unit 4: Server

### Server Types

**Server** — provides services and manages resources (data, users, security) on a network

#### Network Models

* **Peer-to-Peer** — every node acts as both client and server (e.g., AirDrop)
* **Client-Server** — clients make requests; server responds
  * Server: higher security, more data, supports many users
  * Client: lower security, less data, makes requests

### Server Security

#### Best Practices

* Disable external device ports
* **Man-traps** — dual-door entry system controlling physical server room access
* Single admin account with rotating passwords — fewer accounts = fewer attack vectors
* Network isolation — disconnect to prevent traffic spread

### Active Directory

**Active Directory (AD)** — manages permissions and user/group access to network resources (vs. a regular directory which just organizes/lists resources)

#### Logical Structure

* **Forest** — top-level container; set of domain trees sharing a common namespace
* **Tree** — collection of domains in a hierarchy
* **Domain** — security/administrative boundary
* **Organizational Unit (OU)** — container within a domain for users, groups, computers, etc.
* **Objects** — users, groups, computers, applications

#### Physical Structure

* **Sites** — maps physical network topology
* **Domain Controller** — manages domain security policy
* **Global Catalog Server** — enables access to resources across domains/trees
* **Member Servers** — servers joined to the domain
* **Domain Clients** — end-user machines in the domain

### DNS and DHCP

#### Domain Name System (DNS)

Resolves domain names to IP addresses

Structure: `subdomain.domain.tld/path`
Example: `www.google.com/login` → subdomain . domain . top-level . path

* Top-level domains: `.com`, `.net`, `.mil`, `.us`

#### Dynamic Host Configuration Protocol (DHCP)

Dynamically assigns IP addresses to clients — **DORA** process:

1. **Discover** — client broadcasts to find DHCP server
2. **Offer** — server offers an IP address
3. **Request** — client requests the offered address
4. **Acknowledge** — server confirms; IP assignment complete

---

## Unit 6: Cyber Hygiene

### Network User Habits

**Cyber Hygiene** — practices that maintain system health and improve online security

#### Good User Habits

* Use firewalls (personal and organizational)
* Enable automatic antivirus definition updates
* Run regular security scans
* Strong passwords — long, mixed characters, no dictionary words, no obvious substitutions
* Enable automatic software updates
* Back up data to multiple locations

#### Securing Personal Data

* Read privacy policies — explains how sites collect, secure, and use your data
* **Device disposal** — wipe memory before discarding; use overwrite utility on hard drives

### Anti-Piracy and Ethics

#### Anti-Piracy

**Piracy** — unauthorized copying, downloading, or installing of copyrighted software

* Governed by **DAFMAN 17-1203**
* Penalties: civil or criminal (monetary damages, jail time, or fines)

#### Computer Ethics

* Use government systems responsibly
* Protect information
* Respect intellectual property
* Be professional online
* **Monitoring** — by using government systems, you consent to monitoring (sites visited, keystrokes, shared drives, all access is logged)

---

## Unit 7: Security Programs

### COMPUSEC

**COMPUSEC** — Computer Security; broad set of measures to protect information systems resources

#### CIA Triad

**Confidentiality** — prevent unauthorized access
* Access controls and permissions
* **Encryption** — algorithm converts readable data to unreadable form (at rest and in transit)
* Steganography
* Physical protections (locks, fences, cameras)

**Integrity** — ensure data is not altered or deleted
* **Hashing** — generates hash value sent with data; receiver verifies match to detect tampering
* **Digital signatures** — signed with sender's private key; proves origin
* **Digital certificates** — electronic file transporting encryption/signature keys
* **Non-repudiation** — sender cannot deny sending; digital fingerprint

**Availability** — ensure data is accessible when needed
* Permissions — limit who can delete data
* Backups — regular backups enable restoration
* **Fault tolerance** — RAID; redundant storage
* **Clustering** — multiple servers act as one unit; failover if one fails
* Patching — reduces exploitable vulnerabilities

#### COMPUSEC Threats

* **Unauthorized Access** — remote or physical (covert) access to systems
* **Malicious Logic**
  * **Virus** — requires user interaction; replicates across network
  * **Worm** — self-replicates without user interaction
  * **Trojan** — disguised as legitimate software; contains malware
  * **Ransomware** — encrypts data; demands ransom for decryption
  * **Spyware** — silently monitors and collects user info
* **Fraud, Waste, and Abuse (FWA)** — unauthorized printing/internet use; Waste → Abuse → Fraud

### TEMPEST

Program to identify vulnerabilities from **unintentional electromagnetic emanations** that could compromise national security information

#### Countermeasures

* **PDS (Protected Distribution System)** — wired telecom with safeguards
* **HDS (Hardened Distribution System)** — hardened metal conduit
* **SDS (Simple Distribution System)** — reduced protection (wood/plastic conduit)
* **Red/Black Separation**
  * **Red** — plaintext/sensitive unencrypted signals
  * **Black** — encrypted (ciphertext) signals

### INFOSEC

Protects **classified national security information and Controlled Unclassified Information (CUI)**

#### Three Disciplines

* **Personnel Security** — determines eligibility for classified access
* **Industrial Security** — covers civilian workforce and external third parties
* **Information Security** — protects classified/CUI generally

#### Information Designations

**CUI (Controlled Unclassified Information)**
* Unclassified but requires access controls and protective measures
* Includes Privacy Act information (e.g., SSN, age, address)

**Classified Information**
* **Confidential** — causes *some* damage; USPS certified/first-class mail to DoD contractors
* **Secret** — causes *serious* damage; USPS registered mail within US
* **Top Secret (TS)** — causes *exceptionally grave* damage; Department of State carrier

**FOIA** — public right to request federal records; exemptions: personal privacy, national security, law enforcement

### OPSEC

Reduces mission vulnerabilities by limiting adversary collection of **critical information**

* **Critical Information** — specific facts about activities/capabilities adversaries need to act effectively
* **Indicator** — observable info an adversary can collect (e.g., unit preparing for deployment vs. exact departure time)

#### OPSEC Vulnerabilities

* Social media
* Open conversations
* Private messaging and texts
* Family and friends

### COMSEC

Measures and controls to **deny unauthorized access** to information derived from government communications

#### Key Terms

* **Encryption** — converting data into an unreadable form
* **Decryption** — restoring encrypted data to readable form
* **Cryptography** — use of coding systems to encrypt/decrypt
* **Cryptanalysis** — science of breaking coding systems to reveal information

#### Components

* **Cryptosecurity** — protection via cryptographic systems
* **TRANSEC (Transmission Security)** — protects intentional transmissions from exploitation; sending classified over unclassified network = TRANSEC failure
* **Physical Security** — safeguards against improper destruction or handling
  * Physical barriers
  * GSA-approved safes (must match or exceed classification level)
  * Limited COMSEC access

---

## Unit 8: Risk, Threats, and Vulnerabilities

### Threat Framework (STRIDE)

* **Spoofing** — impersonating another entity
* **Tampering** — malicious modification of data
* **Repudiation** — denying responsibility for an action
* **Information Disclosure** — exposing data to unauthorized parties
* **Denial of Service** — exhausting resources to disrupt service
* **Elevation of Privilege** — unprivileged user gains privileged access

### Threat Agents

* **Inside Attack** — malicious insider or human error; initiated within the security perimeter with granted access
* **Outside Attack** — initiated externally; unauthorized access
  * Threat actors: competitors, script kiddies, criminal syndicates, state actors

### Computer Network Attacks

Characterized by **intent**, **attack vector** (point of initiation), and **method of delivery**

#### Attack Types

* **DoS** — floods a machine with more requests than it can handle; toolkits automate execution
* **DDoS** — multiple bots coordinate a synchronized DoS on one target
  * Prevention: over-provision capacity, packet filtering, security patches
* **Unauthorized Access** — attacker gains data they shouldn't have; usually aimed at theft
* **Illicit Command Execution** — untrusted person executes commands on a server
* **Destructive Behavior**
  * **Data diddling** — subtle record manipulation; extremely hard to detect
  * **Data destruction** — attacker deletes files; impacts computing capability

### Social Engineering

People are the weakest link; attacks use **psychological manipulation**

#### Types

* **Phishing** — acquires sensitive data via deceptive messages
  * **Spear Phishing** — targets a specific individual with tailored messaging
  * **Whaling** — targets high-value individuals (CEO, CFO)
* **Baiting** — preys on curiosity or greed (e.g., infected USB left in public)
* **Piggybacking/Tailgating** — gaining physical access by lying about credentials (piggybacking) or physically following someone through an access point (tailgating)
* **Impersonation** — posing as someone else
* **Dumpster Diving** — retrieving sensitive info from discarded materials

#### Mitigation

* User training and awareness
* Don't open suspicious emails or attachments
* Enable multi-factor authentication
* Keep antivirus/anti-malware updated

### Malicious Code

#### Malware Types

* **Virus** — requires user execution; replicates across network
* **Worm** — self-replicates without user interaction
* **Boot Sector Malware** — resides in first disk sector; controls boot sequence; persists through OS reinstall
* **Polymorphic Malware** — changes its signature every execution; evades signature-based detection
* **Macro Malware** — uses macro language to perform malicious actions within applications
* **Logic Bomb** — dormant until a predefined event triggers execution
* **Trojan Horse** — disguised as legitimate software
* **Rootkit** — hidden software granting attacker root/privileged access
* **Spyware** — silently monitors and collects user info
* **Adware** — automatically displays ads

#### Symptoms of Infection

* System won't boot
* Lost partition or reformatted drive
* Programs open/close without user input
* Unexpected warnings or error messages

### Mitigation Mechanisms

#### Prevention

* **Vulnerability Scanning** — simulates attacks to find weaknesses before adversaries do
* **Software Patching** — repairs known flaws after software release
* **User Awareness** — training on common threats and mitigation
* **Firewall** — restricts inbound/outbound traffic; packet filtering inspects network traffic
* **Anti-Spyware** — blocks spyware from collecting data
* **Mail Gateway** — server in the **DMZ** (area between two firewalls) that filters inbound/outbound email

#### Detection

* Antivirus software
* Monitor system logs

### Supply Chain

Third-party vendors and subcontractors coordinating to deliver products to a final destination

#### Vulnerabilities

* **Third-Party risk** — middlemen/subcontractors introduce additional attack surface
* **Supply management** — sourcing, continuity, and quality risks
* **Third-Party Data Storage** — cloud computing hands data to external parties; must verify their security practices before adopting

#### Solutions

* Consult resource advisor, **BECO**, or contracting squadron
* When purchasing IT for AF network, verify equipment is on the **approved product list**

---

## Unit 9: Network Security

### NAC (Network Access Control)

Controls network access based on predefined conditions a system must meet before connecting (e.g., patch level, AV status)

#### Agent Types

* **Permanent Agent** — installed on client; persists after authentication
* **Dissolvable Agent** — installs temporarily; uninstalls after authentication
* **Agentless** — no client software required

### Authentication

**Verification process** confirming a user is who they claim to be

#### Authentication Factors

* **Something you know** — password, PIN
* **Something you have** — physical token, SMS code
* **Something you are** — biometrics, facial recognition
* **Somewhere you are** — GPS, IP address
* **Something you do** — typing patterns, behavioral habits

**SSO (Single Sign-On)** — authenticate once; credentials shared across multiple systems without re-authentication

#### Network Enforcement

* **IEEE 802.1X** — requires valid credentials before granting network access
* **Host Health Checks** — scans for OS updates, AV software, host firewall before allowing connection
* **Terms of Usage** — users accept terms before network access is granted

### AAA (Authentication, Authorization, Accounting)

* **Identification** — presenting a claim (e.g., username); not proof
* **Authentication** — verifying the claim
* **Authorization** — determining what the verified user can access
* **Accounting** — logging and recording user actions, access time, bandwidth

#### Protocols

* **RADIUS** — remote network access authentication via UDP
* **DIAMETER** — newer AAA protocol; more reliable/secure via TCP
* **TCP** — guarantees delivery via 3-way handshake; higher bandwidth overhead
* **UDP** — lightweight; no delivery acknowledgment; streams data

### Application Security

* **P2P File Sharing** — common vector for malicious code distribution
* **Scripting** — executes commands without user input; can modify systems
* **Cross-Site Scripting (XSS)** — injects malicious code into a website

#### Vulnerability Prevention

* Apply software updates
* Application configuration baseline
* **Application hardening** — disable unnecessary features
* **CSRF prevention** — disable "remember me" in browser to prevent session hijacking

#### Intrusion Systems

* **IDS (Intrusion Detection System)** — detects suspicious activity; alerts administrators
* **IPS (Intrusion Prevention System)** — detects and takes corrective action automatically
* Types: Host-based (HIDS/HIPS) and Network-based (NIDS/NIPS)

### Hardware Security

#### Threats

* **Boot Sequence** — enable **Secure Boot / Trusted Boot** to prevent malware from loading during startup
* **Removable Storage** — USB ports disabled on DoD systems; plugging USB triggers HBSS

#### Theft Prevention

* Limit physical access to server rooms
* Lock portable devices with cable locks

#### Hardware Encryption

* **TPM (Trusted Platform Module)** — chip storing cryptographic keys; powers BitLocker; faster than software encryption
* **HSM (Hardware Security Module)** — external device with multiple crypto processors installed on a system

---

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
  * Doesn't fall into cats
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
4. Coordinate \- with victim's system & support agency
5. Determ reporting reqs \- within **one hour** if incident meets Commander's **Critical Information Requirements (CCIR)**

#### Concluding CoA's

* **Postmortem**: Provides **Post-Incident Analysis** recommendations to affected units for corrective actions
* **Cyber Incident Report (CIR)** \- analysis of affected system, attacker, attack vector, & technical \+ operational impact
* **Network Intel Report (NIR)** \- analysis of incident, multiple incidents, or network activity of threat actor
