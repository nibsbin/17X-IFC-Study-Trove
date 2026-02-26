# Block 1 — Practice Test

> 100 multiple-choice questions across all Block 1 units.
> Each question targets one of three cognitive levels: **Rote Definition**, **Conceptual Knowledge**, or **Application**.

---

## Unit 2: Client Basics

**1. What is the primary function of the motherboard in a computer system?**
*(Rote Definition)*

- A) Converting AC power to DC power
- B) Rendering graphics and generating display output
- C) Allowing components to communicate via electrical circuit paths
- D) Storing permanent boot instructions

**Answer: C**

---

**2. Which type of memory is volatile and requires power to retain data?**
*(Rote Definition)*

- A) ROM
- B) SSD
- C) RAM
- D) HDD

**Answer: C**

---

**3. What does the BIOS perform immediately after the system is powered on?**
*(Rote Definition)*

- A) Loads the registry and hardware drivers
- B) Reads the Master Boot Record to locate the OS
- C) Runs a Power-On Self-Test (POST) and identifies bootable devices
- D) Converts AC voltage to DC voltage for internal components

**Answer: C**

---

**4. A technician notices that an application cannot directly access hardware and must go through an intermediary layer, sometimes causing a slight delay. Which CPU mode is the application running in?**
*(Conceptual Knowledge)*

- A) Kernel Mode
- B) User Mode
- C) Safe Mode
- D) Privileged Mode

**Answer: B**

---

**5. How does the NTFS file system differ from FAT-32 in terms of capabilities?**
*(Conceptual Knowledge)*

- A) FAT-32 supports encryption and disk quotas, while NTFS does not
- B) FAT-32 supports a maximum file size of 16 TB, while NTFS supports only 4 GB
- C) NTFS supports encryption, compression, and disk quotas, while FAT-32 does not
- D) NTFS and FAT-32 have identical feature sets but differ only in maximum partition size

**Answer: C**

---

**6. Which statement best describes the relationship between an operating system and the hardware it runs on?**
*(Conceptual Knowledge)*

- A) The OS replaces hardware functions with software emulations
- B) The OS acts as a bridge between the user and the hardware, managing both hardware and software resources
- C) The OS communicates directly with all hardware without the use of drivers
- D) The OS is only responsible for running user applications and has no role in resource management

**Answer: B**

---

**7. Why does the boot loader need to load the operating system into RAM rather than running it directly from storage?**
*(Conceptual Knowledge)*

- A) Storage devices cannot be accessed after POST completes
- B) RAM is non-volatile and preserves the OS between reboots
- C) RAM provides much faster read/write speeds needed for active OS execution
- D) The BIOS requires the OS to reside in RAM before it can run POST

**Answer: C**

---

**8. A system administrator is building a file server that will store video files regularly exceeding 6 GB each. Which file system must the administrator choose, and why?**
*(Application)*

- A) FAT-32, because it supports larger partition sizes
- B) NTFS, because FAT-32 has a maximum file size limit of 4 GB
- C) FAT-32, because it offers better encryption for large media files
- D) Either file system, because both support files up to 16 TB

**Answer: B**

---

**9. A user powers on a new PC but the system boots to the hard drive instead of the USB installation media. Which step in the OS installation process did the user most likely skip?**
*(Application)*

- A) Entering the Windows activation key before booting
- B) Changing the boot order in the BIOS/CMOS settings
- C) Replacing the CMOS battery to reset default settings
- D) Installing hardware drivers before inserting the USB

**Answer: B**

---

**10. A cybersecurity analyst observes that a piece of malware has gained unrestricted access to hardware and is modifying driver behavior. In which CPU mode is this malware most likely executing?**
*(Application)*

- A) User Mode
- B) Application Mode
- C) Kernel Mode
- D) Restricted Mode

**Answer: C**

---

## Unit 3: Virtualization

**11. What is the role of a hypervisor in a virtualized environment?**
*(Rote Definition)*

- A) It provides the physical hardware for the host server
- B) It is the operating system installed inside a virtual machine
- C) It is the software layer that creates and runs virtual machines
- D) It allocates network bandwidth between physical servers

**Answer: C**

---

**12. Which of the following is a security risk specifically associated with virtualization?**
*(Rote Definition)*

- A) Increased power consumption from multiple physical servers
- B) VM escape, where an attacker breaks out of a VM to the host
- C) Inability to run more than one operating system at a time
- D) Loss of data caused by volatile memory in the hypervisor

**Answer: B**

---

**13. According to DISA, what are STIGs used for in the context of virtualization security?**
*(Rote Definition)*

- A) Allocating CPU and RAM resources to each virtual machine
- B) Providing standardized guidance for patching and hardening the OS
- C) Monitoring network bandwidth between the host and guest OS
- D) Backing up virtual machine images to external storage

**Answer: B**

---

**14. How does a Type 1 (Bare Metal) hypervisor differ from a Type 2 (Hosted) hypervisor?**
*(Conceptual Knowledge)*

- A) Type 1 runs on top of an existing OS, while Type 2 is installed directly on hardware
- B) Type 1 is installed directly on hardware, while Type 2 runs on top of an existing OS
- C) Type 1 can only run one VM at a time, while Type 2 supports multiple VMs
- D) Type 1 is used exclusively for desktop virtualization, while Type 2 is used for servers

**Answer: B**

---

**15. Why does running multiple virtual machines on a single host server require high-end physical hardware?**
*(Conceptual Knowledge)*

- A) Each VM requires its own dedicated physical NIC and cannot share bandwidth
- B) The hypervisor adds performance overhead, and each VM consumes CPU, RAM, and storage from the host
- C) Virtual machines cannot use shared storage and each needs a separate physical disk
- D) The host OS must be reinstalled each time a new VM is added

**Answer: B**

---

**16. Which of the following best explains why disabling copy-paste between the host and VM is a recommended hardening measure?**
*(Conceptual Knowledge)*

- A) It prevents the VM from consuming excessive host memory during clipboard operations
- B) It reduces the attack surface by eliminating a data transfer path that could be exploited to move malicious content between environments
- C) It ensures that the host OS and guest OS use the same file system format
- D) It prevents unauthorized users from logging into the hypervisor management console

**Answer: B**

---

**17. An organization wants to minimize downtime and reduce physical hardware costs while running multiple operating systems simultaneously. Which technology best addresses all of these requirements?**
*(Conceptual Knowledge)*

- A) RAID array configuration
- B) Upgrading to faster SSDs across all workstations
- C) Virtualization
- D) Deploying a dedicated physical server for each operating system

**Answer: C**

---

**18. A system administrator is planning host server hardware for an environment that will run 15 VMs, each serving web applications with heavy network traffic. Which hardware component should the administrator prioritize upgrading to prevent a bottleneck?**
*(Application)*

- A) GPU, to handle graphical rendering for each VM
- B) PSU, to ensure adequate power for the hypervisor
- C) NIC, to provide sufficient network bandwidth for the VMs
- D) ROM, to store additional boot instructions for each VM

**Answer: C**

---

**19. During a security audit, an analyst discovers that several unused services are running inside a production VM and the guest OS has not been patched in six months. Which combination of hardening actions should the analyst recommend first?**
*(Application)*

- A) Increase the VM's allocated RAM and install a second hypervisor
- B) Disable the unused services and apply current OS patches using DISA STIGs
- C) Enable copy-paste between the host and VM and add more storage
- D) Remove the VM's network adapter and replace the host server hardware

**Answer: B**

---

**20. A company deploys a Type 2 hypervisor on employee workstations so analysts can run isolated malware samples. An analyst reports that the host workstation has slowed significantly when three VMs run simultaneously. What is the most likely cause?**
*(Application)*

- A) The guest OS inside each VM is incompatible with the Type 2 hypervisor
- B) The malware samples have already escaped the VMs and infected the host
- C) The host workstation lacks sufficient CPU and RAM to support three concurrent VMs plus the host OS and hypervisor overhead
- D) Type 2 hypervisors cannot run more than one VM at a time on a workstation

**Answer: C**

---

## Unit 4: Server

**21. What is the primary function of a server in a network?**
*(Rote Definition)*

- A) Rendering graphics for connected clients
- B) Providing services and managing resources on a network
- C) Converting domain names to IP addresses
- D) Assigning MAC addresses to network devices

**Answer: B**

---

**22. In the DHCP process, what is the correct order of steps a client follows to obtain an IP address?**
*(Rote Definition)*

- A) Request → Discover → Acknowledge → Offer
- B) Offer → Discover → Request → Acknowledge
- C) Discover → Offer → Request → Acknowledge
- D) Discover → Request → Offer → Acknowledge

**Answer: C**

---

**23. What is the top-level container in the Active Directory logical hierarchy?**
*(Rote Definition)*

- A) Domain
- B) Organizational Unit (OU)
- C) Tree
- D) Forest

**Answer: D**

---

**24. How does a client-server model differ from a peer-to-peer model in terms of security?**
*(Conceptual Knowledge)*

- A) Peer-to-peer networks provide stronger centralized security than client-server networks
- B) Client-server networks offer higher security because the server centralizes control, whereas peer-to-peer nodes each act as both client and server
- C) Both models provide identical security since they use the same authentication protocols
- D) Client-server networks are less secure because they rely on a single point of failure

**Answer: B**

---

**25. Why would an organization use DNS instead of requiring users to type IP addresses directly?**
*(Conceptual Knowledge)*

- A) DNS encrypts all network traffic between the client and server
- B) DNS eliminates the need for IP addresses on the network entirely
- C) DNS resolves human-readable domain names to IP addresses, making network resources easier to access
- D) DNS assigns dynamic IP addresses to clients so they do not need static configurations

**Answer: C**

---

**26. Which of the following correctly describes the relationship between a Domain Controller and a Global Catalog Server in Active Directory?**
*(Conceptual Knowledge)*

- A) A Domain Controller manages security within a single domain, while a Global Catalog Server enables cross-domain resource access
- B) A Global Catalog Server replaces the Domain Controller when the network expands beyond one site
- C) A Domain Controller handles DNS resolution, while a Global Catalog Server manages DHCP leases
- D) Both perform identical functions but are named differently depending on the operating system version

**Answer: A**

---

**27. In the URL structure "mail.example.mil/inbox", which component represents the Top-Level Domain (TLD)?**
*(Conceptual Knowledge)*

- A) mail
- B) example
- C) .mil
- D) /inbox

**Answer: C**

---

**28. A network administrator notices that new employees can connect to the network but are unable to access shared department folders. Which Active Directory component should the administrator check first?**
*(Application)*

- A) DNS records for the department file server
- B) DHCP lease assignments for the new employees' workstations
- C) Organizational Unit (OU) and group permissions for the new user accounts
- D) The Global Catalog Server's replication schedule

**Answer: C**

---

**29. A security technician is hardening a newly deployed server in a secure facility. Which combination of measures best aligns with server security best practices?**
*(Application)*

- A) Enable all USB ports for easy patching, create multiple admin accounts, and connect the server to the public internet
- B) Disable external device ports, implement a man-trap for physical access, use a single admin account with rotating passwords, and isolate the server on the network
- C) Install the server in an unlocked closet, assign a shared admin password, and connect it to the guest Wi-Fi
- D) Place the server behind a man-trap but enable all services and use a default admin password for convenience

**Answer: B**

---

**30. A user reports that their laptop receives a different IP address every time it reconnects to the office network, yet they can still access all resources normally. Which service is responsible for this behavior?**
*(Application)*

- A) Active Directory, which reassigns user credentials on each login
- B) DNS, which rotates IP addresses to balance network traffic
- C) DHCP, which dynamically assigns an available IP address each time the client connects
- D) The Global Catalog Server, which distributes IP pools across domains

**Answer: C**

---

## Unit 6: Cyber Hygiene

**31. What is the definition of cyber hygiene?**
*(Rote Definition)*

- A) The process of encrypting all files on a government network
- B) Practices that maintain system health and improve online security
- C) A federal regulation requiring annual cybersecurity audits
- D) Software that automatically removes viruses from a network

**Answer: B**

---

**32. According to Air Force policy, which publication governs software anti-piracy rules?**
*(Rote Definition)*

- A) NIST SP 800-53
- B) AFI 33-200
- C) DAFMAN 17-1203
- D) DoD Directive 8570

**Answer: C**

---

**33. Which of the following is considered a strong password practice?**
*(Rote Definition)*

- A) Using a short, memorable dictionary word for easy recall
- B) Reusing the same password across multiple accounts for consistency
- C) Creating a long password with mixed characters that avoids dictionary words
- D) Writing the password on a sticky note and attaching it to the monitor

**Answer: C**

---

**34. Why should users enable automatic antivirus updates rather than relying on manual updates?**
*(Conceptual Knowledge)*

- A) Automatic updates prevent all forms of cyberattack, including zero-day exploits
- B) Automatic updates ensure virus definitions stay current without relying on the user to remember, reducing the window of vulnerability
- C) Manual updates are faster and more thorough than automatic updates
- D) Automatic updates replace the need for a firewall on the system

**Answer: B**

---

**35. How does backing up data to multiple locations improve security compared to a single backup?**
*(Conceptual Knowledge)*

- A) Multiple backups encrypt data more effectively than a single backup
- B) Multiple backups guarantee that no data will ever be lost under any circumstances
- C) If one backup location is compromised or fails, data can still be restored from an alternate location, providing redundancy
- D) Multiple backups eliminate the need for antivirus software on the primary system

**Answer: C**

---

**36. What is the relationship between using a government system and consent to monitoring?**
*(Conceptual Knowledge)*

- A) Monitoring only begins after a user is suspected of a policy violation
- B) Users must opt in to monitoring by signing a separate agreement each session
- C) By using a government system, users automatically consent to monitoring of sites visited, keystrokes, shared drives, and all access
- D) Government systems are only monitored during scheduled audit windows

**Answer: C**

---

**37. Why is overwriting a hard drive with a utility recommended over simply deleting files when disposing of a device?**
*(Conceptual Knowledge)*

- A) Deleting files permanently erases them from the disk surface, so overwriting is only an extra precaution
- B) Overwriting replaces data on the disk with random patterns, making recovery far more difficult, whereas deleting files only removes file system pointers and leaves data recoverable
- C) Overwriting is faster than deleting, which is why it is preferred
- D) Deleting files triggers an automatic backup to a cloud server, creating a security risk

**Answer: B**

---

**38. An airman downloads a popular commercial application from an unauthorized website and installs it on their government workstation without a valid license. Which of the following best describes the potential consequences?**
*(Application)*

- A) No consequences, because the software was freely available on the website
- B) A verbal warning from the unit's IT help desk with no further action
- C) Civil or criminal penalties for software piracy under DAFMAN 17-1203
- D) The software will simply be uninstalled automatically by the network firewall

**Answer: C**

---

**39. A cybersecurity analyst discovers that a departing employee's government laptop is being reassigned to a new hire. The laptop's hard drive contains sensitive project files. What is the most appropriate action before reassignment?**
*(Application)*

- A) Delete the departing employee's user profile and hand the laptop to the new hire
- B) Move all files to the Recycle Bin, empty it, and reimage the desktop background
- C) Wipe the device's memory and use an overwrite utility on the hard drive before reconfiguring it for the new user
- D) Remove the laptop from the network and store it in a closet indefinitely

**Answer: C**

---

**40. A government employee receives an email with an attachment claiming to be a required software update. The email does not come from an official IT channel. Applying good cyber hygiene practices, what should the employee do?**
*(Application)*

- A) Open the attachment immediately since it claims to be a required update
- B) Forward the email to all coworkers so they can also install the update
- C) Avoid opening the attachment, report the suspicious email through proper channels, and rely on automatic software updates from authorized sources
- D) Download the attachment to a personal USB drive and scan it at home

**Answer: C**

---

## Unit 7: Security Programs

**41. In the TEMPEST program, what does "Red" signify in the Red/Black concept?**
*(Rote Definition)*

- A) Encrypted ciphertext signals
- B) Plaintext or sensitive unencrypted signals
- C) Signals requiring COMSEC physical barriers
- D) Electromagnetic emanations from shielded cables

**Answer: B**

---

**42. What is the primary purpose of OPSEC?**
*(Rote Definition)*

- A) To encrypt all government communications end-to-end
- B) To reduce mission vulnerabilities by limiting adversary collection of critical information
- C) To classify national security documents at the appropriate level
- D) To detect unintentional electromagnetic emanations from equipment

**Answer: B**

---

**43. Which three disciplines fall under INFOSEC?**
*(Rote Definition)*

- A) Cryptosecurity, TRANSEC, Physical Security
- B) Confidentiality, Integrity, Availability
- C) Personnel Security, Industrial Security, Information Security
- D) COMPUSEC, OPSEC, COMSEC

**Answer: C**

---

**44. A security analyst discovers that someone altered a financial database record without authorization. Which element of the CIA Triad was primarily violated?**
*(Conceptual Knowledge)*

- A) Availability
- B) Confidentiality
- C) Non-repudiation
- D) Integrity

**Answer: D**

---

**45. How does a worm fundamentally differ from a virus?**
*(Conceptual Knowledge)*

- A) A worm encrypts data and demands ransom; a virus does not
- B) A worm self-replicates without user interaction; a virus requires user interaction to spread
- C) A worm disguises itself as legitimate software; a virus attaches to boot sectors
- D) A worm monitors user activity; a virus modifies system files

**Answer: B**

---

**46. Why does INFOSEC distinguish between CUI and classified information?**
*(Conceptual Knowledge)*

- A) CUI can be freely distributed to the public, while classified information cannot
- B) CUI requires no protective measures, while classified information requires encryption
- C) CUI is unclassified but still requires access controls, while classified information is protected based on potential damage to national security
- D) CUI applies only to military systems, while classified information covers civilian data

**Answer: C**

---

**47. What is the relationship between an OPSEC "indicator" and "critical information"?**
*(Conceptual Knowledge)*

- A) Indicators are the classified details adversaries seek; critical information is publicly available context
- B) They are interchangeable terms for the same concept
- C) Critical information is the specific facts adversaries need, while indicators are observable pieces of information an adversary can collect that may reveal critical information
- D) Critical information applies only to COMSEC, while indicators apply only to TEMPEST

**Answer: C**

---

**48. A member of a unit posts a photo on social media showing a deployment preparation area with unit identifiers and aircraft tail numbers visible. Which security program is most directly compromised?**
*(Application)*

- A) TEMPEST
- B) COMSEC
- C) OPSEC
- D) COMPUSEC

**Answer: C**

---

**49. An administrator needs to send a Top Secret document to a cleared recipient at another installation. Which method of transmission is authorized?**
*(Application)*

- A) USPS registered mail within the United States
- B) USPS certified or first-class mail to DoD contractors
- C) Department of State courier
- D) Encrypted email over an unclassified network

**Answer: C**

---

**50. A technician accidentally transmits a classified briefing over an unclassified network. Which COMSEC component has failed?**
*(Application)*

- A) Cryptosecurity
- B) Physical Security
- C) Cryptanalysis
- D) TRANSEC

**Answer: D**

---

## Unit 8: Risk, Threats, and Vulnerabilities

**51. In the STRIDE threat model, what does the "R" stand for?**
*(Rote Definition)*

- A) Rootkit
- B) Ransomware
- C) Repudiation
- D) Reconnaissance

**Answer: C**

---

**52. What type of malware remains dormant until a predefined event triggers its execution?**
*(Rote Definition)*

- A) Rootkit
- B) Polymorphic malware
- C) Logic bomb
- D) Adware

**Answer: C**

---

**53. Where is a mail gateway server typically deployed within a network architecture?**
*(Rote Definition)*

- A) On the internal LAN behind all firewalls
- B) On the end-user workstation
- C) In the DMZ, between two firewalls
- D) Directly on the domain controller

**Answer: C**

---

**54. How does a DDoS attack differ from a standard DoS attack?**
*(Conceptual Knowledge)*

- A) A DDoS attack targets data integrity, while a DoS attack targets availability
- B) A DoS attack uses social engineering, while a DDoS attack uses malware
- C) A DDoS attack uses multiple coordinated bots to flood a target, while a DoS attack originates from a single source
- D) A DDoS attack only targets web applications, while a DoS attack targets all network services

**Answer: C**

---

**55. Why is polymorphic malware particularly difficult for traditional antivirus software to detect?**
*(Conceptual Knowledge)*

- A) It hides in the boot sector and loads before the antivirus starts
- B) It changes its code signature with each execution, evading signature-based detection
- C) It encrypts the entire hard drive, preventing the antivirus from scanning files
- D) It disables the network adapter so the antivirus cannot download updated definitions

**Answer: B**

---

**56. What makes data diddling especially dangerous compared to other destructive attacks?**
*(Conceptual Knowledge)*

- A) It immediately crashes the target system, causing maximum disruption
- B) It involves subtle record manipulation that is extremely difficult to detect
- C) It requires physical access to the target machine to execute
- D) It only affects backup systems, leaving production data intact

**Answer: B**

---

**57. Why are people often considered the weakest link in an organization's security posture?**
*(Conceptual Knowledge)*

- A) People are unable to learn new security protocols regardless of training
- B) Technical controls like firewalls are always bypassed before human error occurs
- C) People are susceptible to psychological manipulation, making social engineering attacks effective even when strong technical controls exist
- D) People always have administrative access to all systems on the network

**Answer: C**

---

**58. An employee finds a USB drive labeled "Salary Data 2025" in the office parking lot and plugs it into their workstation. The drive installs a keylogger. Which social engineering technique was used?**
*(Application)*

- A) Phishing
- B) Tailgating
- C) Baiting
- D) Impersonation

**Answer: C**

---

**59. A system administrator notices that programs on a server are opening and closing without user input, the system has rebooted unexpectedly, and unfamiliar error messages are appearing. Based on these symptoms, what should the administrator suspect?**
*(Application)*

- A) A DHCP address conflict
- B) A malware infection
- C) A routine operating system update
- D) A misconfigured firewall rule

**Answer: B**

---

**60. A wing cybersecurity office needs to procure new networking equipment from an outside vendor for installation on the Air Force network. Which action should they take to mitigate supply chain risk?**
*(Application)*

- A) Purchase the cheapest available equipment to reduce budget impact
- B) Allow the vendor to self-certify the security of their products
- C) Verify the equipment is on the approved product list and consult the resource advisor or BECO
- D) Install the equipment immediately and scan for vulnerabilities afterward

**Answer: C**

---

## Unit 9: Network Security

**61. What does NAC stand for?**
*(Rote Definition)*

- A) Network Authentication Control
- B) Network Access Control
- C) Network Application Controller
- D) Node Access Configuration

**Answer: B**

---

**62. In the AAA framework, which step involves recording a user's actions after they have been granted access?**
*(Rote Definition)*

- A) Identification
- B) Authentication
- C) Authorization
- D) Accounting

**Answer: D**

---

**63. Which authentication factor does a fingerprint scanner represent?**
*(Rote Definition)*

- A) Something you know
- B) Something you have
- C) Something you are
- D) Something you do

**Answer: C**

---

**64. How does an IPS differ from an IDS?**
*(Conceptual Knowledge)*

- A) An IPS only monitors host-level activity, while an IDS monitors network traffic
- B) An IPS detects threats and takes corrective action automatically, while an IDS only detects and alerts
- C) An IPS uses signature-based detection, while an IDS uses anomaly-based detection
- D) An IPS replaces the need for a firewall, while an IDS supplements it

**Answer: B**

---

**65. Why is RADIUS considered less reliable than DIAMETER for AAA services?**
*(Conceptual Knowledge)*

- A) RADIUS uses TCP, which has higher overhead and slower connection setup
- B) RADIUS uses UDP, which does not guarantee delivery of packets
- C) RADIUS cannot perform accounting functions, only authentication
- D) RADIUS requires a permanent agent installed on every endpoint

**Answer: B**

---

**66. What is the relationship between TPM and BitLocker?**
*(Conceptual Knowledge)*

- A) BitLocker is a physical chip that stores encryption keys for TPM software
- B) TPM is a hardware chip that stores cryptographic keys and powers BitLocker's full-disk encryption
- C) TPM and BitLocker are competing encryption standards that cannot be used together
- D) BitLocker replaces TPM by performing all cryptographic operations in software

**Answer: B**

---

**67. Why does Single Sign-On (SSO) present both a security benefit and a potential risk?**
*(Conceptual Knowledge)*

- A) SSO encrypts all passwords but stores them in plaintext on a central server
- B) SSO reduces password fatigue and repeated logins, but a single compromised credential can grant access to multiple systems
- C) SSO eliminates the need for multifactor authentication entirely
- D) SSO only works with biometric authentication, which limits its adoption

**Answer: B**

---

**68. A security administrator discovers that a user's laptop connected to the network despite having outdated antivirus definitions and missing OS patches. Which NAC component most likely failed?**
*(Application)*

- A) IEEE 802.1X port-based authentication
- B) Host health checks
- C) Terms of usage acceptance
- D) RADIUS server configuration

**Answer: B**

---

**69. A contractor needs temporary network access at a military facility. The security team wants to verify the contractor's device compliance without installing any persistent software. Which NAC agent type should they use?**
*(Application)*

- A) Permanent agent
- B) Dissolvable agent
- C) Agentless
- D) Host-based agent

**Answer: B**

---

**70. A cybersecurity analyst notices that a popular internal web application is displaying unexpected pop-up messages containing scripts that redirect users to a credential-harvesting page. Which type of attack is most likely occurring?**
*(Application)*

- A) Peer-to-peer file sharing exploit
- B) Cross-site scripting (XSS)
- C) Cross-site request forgery (CSRF)
- D) Brute-force authentication attack

**Answer: B**

---

## Unit 10: Firewalls

**71. What is the default behavior of an allowlisting firewall policy?**
*(Rote Definition)*

- A) Allow all traffic by default, then block specific entries
- B) Deny all traffic by default, then permit only explicitly approved entries
- C) Inspect packet payloads and allow traffic based on application type
- D) Log all traffic without blocking or allowing anything

**Answer: B**

---

**72. What is a DMZ in network architecture?**
*(Rote Definition)*

- A) A virtual private network tunnel between two remote sites
- B) An encrypted segment of the internal LAN for classified traffic
- C) An area situated between two firewalls that separates internal and external networks
- D) A backup firewall that activates when the primary firewall fails

**Answer: C**

---

**73. Which firewall type is considered the simplest, filtering traffic based only on IP addresses and port numbers?**
*(Rote Definition)*

- A) Stateful inspection firewall
- B) Application layer firewall
- C) Next-generation firewall
- D) Packet filtering firewall

**Answer: D**

---

**74. How does a stateful inspection firewall improve upon basic packet filtering?**
*(Conceptual Knowledge)*

- A) It inspects the full application-layer payload of every packet
- B) It tracks the state of active connections and only allows inbound traffic that corresponds to an outbound-initiated session
- C) It replaces the need for both IDS and IPS by performing deep packet inspection
- D) It filters traffic based solely on source and destination MAC addresses

**Answer: B**

---

**75. Why are hardware firewalls generally preferred over software firewalls for protecting medium-to-large enterprise networks?**
*(Conceptual Knowledge)*

- A) Hardware firewalls are easier to configure and require no specialized knowledge
- B) Hardware firewalls are less expensive to purchase and maintain than software alternatives
- C) Hardware firewalls funnel all traffic through a single dedicated appliance, providing more efficient perimeter protection for many hosts
- D) Hardware firewalls can only protect individual hosts, making them more granular

**Answer: C**

---

**76. What is the key difference between an allowlisting and a denylisting approach to firewall policy?**
*(Conceptual Knowledge)*

- A) Allowlisting is used for hardware firewalls; denylisting is used for software firewalls
- B) Allowlisting permits only explicitly approved traffic and blocks everything else; denylisting blocks only specified traffic and permits everything else
- C) Allowlisting applies to inbound traffic only; denylisting applies to outbound traffic only
- D) Allowlisting requires deep packet inspection; denylisting requires only port filtering

**Answer: B**

---

**77. Why would an organization choose an application layer / next-generation firewall over a stateful inspection firewall?**
*(Conceptual Knowledge)*

- A) It is simpler to configure and has lower hardware requirements
- B) It provides deep packet inspection, IDS/IPS capabilities, and can analyze traffic at the application level for more advanced threat detection
- C) It only filters by IP address and port, reducing processing overhead
- D) It eliminates the need for a DMZ by combining internal and external network segments

**Answer: B**

---

**78. A small business owner wants to protect a single workstation used for online transactions. The business has no dedicated IT staff and needs a low-cost solution. Which firewall solution is most appropriate?**
*(Application)*

- A) A hardware firewall appliance deployed at the network perimeter
- B) A next-generation firewall with deep packet inspection
- C) A software firewall installed on the workstation, such as Windows Firewall
- D) A packet filtering router placed between the workstation and the modem

**Answer: C**

---

**79. A network administrator is designing the security architecture for a public-facing web server that must be accessible from the internet but must not expose the internal corporate network. Where should the web server be placed?**
*(Application)*

- A) On the internal LAN behind a single firewall
- B) Directly on the internet with no firewall protection
- C) In the DMZ, between two firewalls
- D) On the same subnet as the organization's domain controller

**Answer: C**

---

**80. An organization's firewall is configured to deny all traffic by default. A new cloud-based collaboration tool stops working because its traffic is being blocked. An administrator adds a rule to explicitly permit the tool's specific IP addresses and ports. Which firewall policy model is this organization using?**
*(Application)*

- A) Denylisting
- B) Stateful inspection
- C) Allowlisting
- D) Application layer filtering

**Answer: C**

---

## Unit 11: Publications and Personnel Security

**81. What is Electrostatic Discharge (ESD)?**
*(Rote Definition)*

- A) A method for safely grounding electrical equipment
- B) Electricity transferred between two charged objects
- C) A bonding technique used to connect conductive materials
- D) An electromagnetic pulse caused by power surges

**Answer: B**

---

**82. Which publication type provides step-by-step instructions for carrying out routine tasks?**
*(Rote Definition)*

- A) DoDI
- B) AFI
- C) STIG
- D) SOP

**Answer: D**

---

**83. What is the primary purpose of a STIG?**
*(Rote Definition)*

- A) To establish high-level DoD policy and general guidance
- B) To provide DISA implementation guidance for standardizing security and IT configurations
- C) To direct Air Force-specific compliance actions and procedures
- D) To define step-by-step instructions for routine operations

**Answer: B**

---

**84. How does bonding differ from grounding in the context of personal safety?**
*(Conceptual Knowledge)*

- A) Bonding provides a path for electricity to flow into the ground, while grounding minimizes discharge between objects
- B) Bonding minimizes electrostatic discharge between conductive objects, while grounding provides a safe path for electricity to flow into the earth
- C) Bonding and grounding are interchangeable terms for the same protective technique
- D) Bonding protects against lightning strikes, while grounding protects against ESD

**Answer: B**

---

**85. What is the relationship between a DoDI and a DoDM?**
*(Conceptual Knowledge)*

- A) A DoDI implements the detailed procedures outlined in a DoDM
- B) A DoDM establishes policy, while a DoDI provides the implementation details
- C) A DoDI establishes policy and general guidance, while a DoDM implements that policy with procedural details
- D) A DoDI and DoDM serve identical purposes but are issued by different authorities

**Answer: C**

---

**86. How does an AFMAN differ from an AFI?**
*(Conceptual Knowledge)*

- A) An AFMAN must always fall under a parent AFI, while an AFI can stand alone
- B) An AFMAN extends instructions and can stand in place of an AFI without needing to fall under one, while an AFI directs action and ensures compliance
- C) An AFI provides general guidance, while an AFMAN directs specific compliance actions
- D) An AFMAN is issued by DoD, while an AFI is issued by the Air Force

**Answer: B**

---

**87. Why are passive security measures considered a foundational layer of equipment protection rather than a complete solution?**
*(Conceptual Knowledge)*

- A) Passive measures such as barriers and limited entrances deter and delay threats but cannot detect or respond to active intrusions on their own
- B) Passive measures are more expensive than active measures and are only used for high-value assets
- C) Passive measures include cameras and patrols that require constant human monitoring
- D) Passive measures are temporary and must be replaced with active measures after installation

**Answer: A**

---

**88. A technician is about to replace a memory module in a server. Before touching the component, the technician clips a wrist strap to the metal chassis of the server. Which safety concept is the technician primarily applying?**
*(Application)*

- A) Bonding
- B) Active protection
- C) Grounding
- D) Passive protection

**Answer: C**

---

**89. A cybersecurity team is configuring firewalls, hardening operating systems, and ensuring all devices meet a standardized security baseline across the enterprise. Which publication type should they reference for specific implementation guidance on these configurations?**
*(Application)*

- A) SOP
- B) MIL-STD
- C) STIG
- D) DoDI

**Answer: C**

---

**90. A base communications squadron needs to ensure that all fiber optic cabling installed across the installation meets a uniform DoD standard for quality and interoperability. Which publication type governs this requirement?**
*(Application)*

- A) AFI
- B) SOP
- C) STIG
- D) MIL-STD

**Answer: D**

---

## Unit 12: Incident Response

**91. What is the primary mission of a Computer Incident Response Team (CIRT)?**
*(Rote Definition)*

- A) To prosecute cyber criminals and enforce federal cybersecurity laws
- B) To handle, correct, and document security incidents
- C) To design and deploy network infrastructure across an organization
- D) To develop cybersecurity training curricula for end users

**Answer: B**

---

**92. Which Incident Response category is classified as an incident involving malicious logic?**
*(Rote Definition)*

- A) Cat 4
- B) Cat 5
- C) Cat 1
- D) Cat 7

**Answer: D**

---

**93. In the IR handling process, which step comes immediately after "Detect & Report"?**
*(Rote Definition)*

- A) Response and Recovery
- B) Post-incident Analysis
- C) Preliminary Analysis and Identification
- D) Preliminary Response Actions

**Answer: C**

---

**94. What is the key distinction between an "event" and an "incident" in the context of Incident Response?**
*(Conceptual Knowledge)*

- A) An event is always malicious, while an incident may be benign
- B) An event is any observable occurrence that may indicate a problem, while an incident is an assessed occurrence that actually jeopardizes confidentiality, integrity, or availability
- C) An incident must involve physical damage, while an event is limited to digital systems
- D) Events require immediate escalation, while incidents are logged for future review

**Answer: B**

---

**95. Why does a Classified Message Incident (CMI) fall outside the standard IR category framework?**
*(Conceptual Knowledge)*

- A) CMIs only affect unclassified networks and are handled by a separate team
- B) CMIs involve the transfer of confidential or higher information onto unauthorized media, requiring investigation and destruction of the unclassified media rather than fitting a standard numbered category
- C) CMIs are automatically resolved by automated systems and do not need human analysis
- D) CMIs are reclassified as Cat 0 training exercises once they are detected

**Answer: B**

---

**96. How do the roles of the Technical Specialist and the Documentation Specialist complement each other during an incident?**
*(Conceptual Knowledge)*

- A) The Technical Specialist documents the incident while the Documentation Specialist identifies the root cause
- B) The Technical Specialist identifies the scale and corrects the issue, while the Documentation Specialist records the incident details, cause, and solution for future reference
- C) Both roles focus on correcting the incident, but the Documentation Specialist handles legal matters
- D) The Technical Specialist reports to external agencies, while the Documentation Specialist communicates with internal leadership

**Answer: B**

---

**97. Why must organizations report incidents that meet CCIR criteria within one hour according to root cause analysis guidance?**
*(Conceptual Knowledge)*

- A) One hour is the maximum time allotted before automated systems shut down the affected network segment
- B) Rapid reporting ensures leadership has timely situational awareness to assess operational impact and coordinate an appropriate response
- C) Federal law requires all cybersecurity incidents to be reported within one hour regardless of severity
- D) The one-hour window allows the CIRT to fully complete its post-incident analysis before reporting

**Answer: B**

---

**98. An analyst receives an alert indicating a large volume of SYN packets are flooding a web server, but the server remains operational and no service degradation is observed. How should this event be categorized?**
*(Application)*

- A) Cat 4 — Denial of Service (incident)
- B) Cat 7 — Malicious Logic
- C) Cat 3 — Unsuccessful Denial of Service Attempt (event)
- D) Cat 6 — Reconnaissance (event)

**Answer: C**

---

**99. During an incident, the CIRT has completed its response and the affected systems are restored. The team now drafts a document analyzing the threat actor's tactics, techniques, and activity patterns observed during the incident. Which concluding course of action does this document represent?**
*(Application)*

- A) Postmortem
- B) Cyber Incident Report (CIR)
- C) Network Intel Report (NIR)
- D) Classified Message Incident (CMI)

**Answer: C**

---

**100. A user discovers that a classified document was accidentally emailed to an unclassified distribution list. The user reports it immediately. Which type of incident has occurred, and what is a required action?**
*(Application)*

- A) Cat 1 — Root-level incident; isolate the email server from the network
- B) Cat 5 — Non-compliance event; retrain the user on email policy
- C) Classified Message Incident; investigate and destroy the unclassified media that received the information
- D) Cat 8 — Event under investigation; wait for further analysis before taking action

**Answer: C**
