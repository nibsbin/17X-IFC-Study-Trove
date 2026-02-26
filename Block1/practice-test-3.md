# Block 1 — Practice Test 3

> 35 multiple-choice questions covering all Block 1 units.
> Each question targets one of three cognitive levels: **Rote Definition**, **Conceptual Knowledge**, or **Application**.

---

## Unit 2: Client Basics

**1. What does the BIOS perform immediately after the system is powered on?**
*(Rote Definition)*

- A) Loads the registry and hardware drivers
- B) Reads the Master Boot Record to locate the OS
- C) Runs a Power-On Self-Test (POST) and identifies bootable devices
- D) Converts AC voltage to DC voltage for internal components

**Answer: C**

---

**2. A technician notices that an application cannot directly access hardware and must go through an intermediary layer, sometimes causing a slight delay. Which CPU mode is the application running in?**
*(Conceptual Knowledge)*

- A) Kernel Mode
- B) User Mode
- C) Safe Mode
- D) Privileged Mode

**Answer: B**

---

**3. Why does the boot loader need to load the operating system into RAM rather than running it directly from storage?**
*(Conceptual Knowledge)*

- A) Storage devices cannot be accessed after POST completes
- B) RAM is non-volatile and preserves the OS between reboots
- C) RAM provides much faster read/write speeds needed for active OS execution
- D) The BIOS requires the OS to reside in RAM before it can run POST

**Answer: C**

---

**4. A system administrator is building a file server that will store video files regularly exceeding 6 GB each. Which file system must the administrator choose, and why?**
*(Application)*

- A) FAT-32, because it supports larger partition sizes
- B) NTFS, because FAT-32 has a maximum file size limit of 4 GB
- C) FAT-32, because it offers better encryption for large media files
- D) Either file system, because both support files up to 16 TB

**Answer: B**

---

## Unit 3: Virtualization

**5. According to DISA, what are STIGs used for in the context of virtualization security?**
*(Rote Definition)*

- A) Allocating CPU and RAM resources to each virtual machine
- B) Providing standardized guidance for patching and hardening the OS
- C) Monitoring network bandwidth between the host and guest OS
- D) Backing up virtual machine images to external storage

**Answer: B**

---

**6. Why does running multiple virtual machines on a single host server require high-end physical hardware?**
*(Conceptual Knowledge)*

- A) Each VM requires its own dedicated physical NIC and cannot share bandwidth
- B) The hypervisor adds performance overhead, and each VM consumes CPU, RAM, and storage from the host
- C) Virtual machines cannot use shared storage and each needs a separate physical disk
- D) The host OS must be reinstalled each time a new VM is added

**Answer: B**

---

**7. An organization wants to minimize downtime and reduce physical hardware costs while running multiple operating systems simultaneously. Which technology best addresses all of these requirements?**
*(Conceptual Knowledge)*

- A) RAID array configuration
- B) Upgrading to faster SSDs across all workstations
- C) Virtualization
- D) Deploying a dedicated physical server for each operating system

**Answer: C**

---

**8. During a security audit, an analyst discovers that several unused services are running inside a production VM and the guest OS has not been patched in six months. Which combination of hardening actions should the analyst recommend first?**
*(Application)*

- A) Increase the VM's allocated RAM and install a second hypervisor
- B) Disable the unused services and apply current OS patches using DISA STIGs
- C) Enable copy-paste between the host and VM and add more storage
- D) Remove the VM's network adapter and replace the host server hardware

**Answer: B**

---

## Unit 4: Server

**9. What is the top-level container in the Active Directory logical hierarchy?**
*(Rote Definition)*

- A) Domain
- B) Organizational Unit (OU)
- C) Tree
- D) Forest

**Answer: D**

---

**10. Which of the following correctly describes the relationship between a Domain Controller and a Global Catalog Server in Active Directory?**
*(Conceptual Knowledge)*

- A) A Domain Controller manages security within a single domain, while a Global Catalog Server enables cross-domain resource access
- B) A Global Catalog Server replaces the Domain Controller when the network expands beyond one site
- C) A Domain Controller handles DNS resolution, while a Global Catalog Server manages DHCP leases
- D) Both perform identical functions but are named differently depending on the operating system version

**Answer: A**

---

**11. A user reports that their laptop receives a different IP address every time it reconnects to the office network, yet they can still access all resources normally. Which service is responsible for this behavior?**
*(Application)*

- A) Active Directory, which reassigns user credentials on each login
- B) DNS, which rotates IP addresses to balance network traffic
- C) DHCP, which dynamically assigns an available IP address each time the client connects
- D) The Global Catalog Server, which distributes IP pools across domains

**Answer: C**

---

## Unit 6: Cyber Hygiene

**12. Which of the following is considered a strong password practice?**
*(Rote Definition)*

- A) Using a short, memorable dictionary word for easy recall
- B) Reusing the same password across multiple accounts for consistency
- C) Creating a long password with mixed characters that avoids dictionary words
- D) Writing the password on a sticky note and attaching it to the monitor

**Answer: C**

---

**13. How does backing up data to multiple locations improve security compared to a single backup?**
*(Conceptual Knowledge)*

- A) Multiple backups encrypt data more effectively than a single backup
- B) Multiple backups guarantee that no data will ever be lost under any circumstances
- C) If one backup location is compromised or fails, data can still be restored from an alternate location, providing redundancy
- D) Multiple backups eliminate the need for antivirus software on the primary system

**Answer: C**

---

**14. Why is overwriting a hard drive with a utility recommended over simply deleting files when disposing of a device?**
*(Conceptual Knowledge)*

- A) Deleting files permanently erases them from the disk surface, so overwriting is only an extra precaution
- B) Overwriting replaces data on the disk with random patterns, making recovery far more difficult, whereas deleting files only removes file system pointers and leaves data recoverable
- C) Overwriting is faster than deleting, which is why it is preferred
- D) Deleting files triggers an automatic backup to a cloud server, creating a security risk

**Answer: B**

---

**15. A cybersecurity analyst discovers that a departing employee's government laptop is being reassigned to a new hire. The laptop's hard drive contains sensitive project files. What is the most appropriate action before reassignment?**
*(Application)*

- A) Delete the departing employee's user profile and hand the laptop to the new hire
- B) Move all files to the Recycle Bin, empty it, and reimage the desktop background
- C) Wipe the device's memory and use an overwrite utility on the hard drive before reconfiguring it for the new user
- D) Remove the laptop from the network and store it in a closet indefinitely

**Answer: C**

---

## Unit 7: Security Programs

**16. Which three disciplines fall under INFOSEC?**
*(Rote Definition)*

- A) Cryptosecurity, TRANSEC, Physical Security
- B) Confidentiality, Integrity, Availability
- C) Personnel Security, Industrial Security, Information Security
- D) COMPUSEC, OPSEC, COMSEC

**Answer: C**

---

**17. Why does INFOSEC distinguish between CUI and classified information?**
*(Conceptual Knowledge)*

- A) CUI can be freely distributed to the public, while classified information cannot
- B) CUI requires no protective measures, while classified information requires encryption
- C) CUI is unclassified but still requires access controls, while classified information is protected based on potential damage to national security
- D) CUI applies only to military systems, while classified information covers civilian data

**Answer: C**

---

**18. A technician accidentally transmits a classified briefing over an unclassified network. Which COMSEC component has failed?**
*(Application)*

- A) Cryptosecurity
- B) Physical Security
- C) Cryptanalysis
- D) TRANSEC

**Answer: D**

---

## Unit 8: Risk, Threats, and Vulnerabilities

**19. Where is a mail gateway server typically deployed within a network architecture?**
*(Rote Definition)*

- A) On the internal LAN behind all firewalls
- B) On the end-user workstation
- C) In the DMZ, between two firewalls
- D) Directly on the domain controller

**Answer: C**

---

**20. Why are people often considered the weakest link in an organization's security posture?**
*(Conceptual Knowledge)*

- A) People are unable to learn new security protocols regardless of training
- B) Technical controls like firewalls are always bypassed before human error occurs
- C) People are susceptible to psychological manipulation, making social engineering attacks effective even when strong technical controls exist
- D) People always have administrative access to all systems on the network

**Answer: C**

---

**21. A wing cybersecurity office needs to procure new networking equipment from an outside vendor for installation on the Air Force network. Which action should they take to mitigate supply chain risk?**
*(Application)*

- A) Purchase the cheapest available equipment to reduce budget impact
- B) Allow the vendor to self-certify the security of their products
- C) Verify the equipment is on the approved product list and consult the resource advisor or BECO
- D) Install the equipment immediately and scan for vulnerabilities afterward

**Answer: C**

---

## Unit 9: Network Security

**22. Which authentication factor does a fingerprint scanner represent?**
*(Rote Definition)*

- A) Something you know
- B) Something you have
- C) Something you are
- D) Something you do

**Answer: C**

---

**23. Why does Single Sign-On (SSO) present both a security benefit and a potential risk?**
*(Conceptual Knowledge)*

- A) SSO encrypts all passwords but stores them in plaintext on a central server
- B) SSO reduces password fatigue and repeated logins, but a single compromised credential can grant access to multiple systems
- C) SSO eliminates the need for multifactor authentication entirely
- D) SSO only works with biometric authentication, which limits its adoption

**Answer: B**

---

**24. A cybersecurity analyst notices that a popular internal web application is displaying unexpected pop-up messages containing scripts that redirect users to a credential-harvesting page. Which type of attack is most likely occurring?**
*(Application)*

- A) Peer-to-peer file sharing exploit
- B) Cross-site scripting (XSS)
- C) Cross-site request forgery (CSRF)
- D) Brute-force authentication attack

**Answer: B**

---

## Unit 10: Firewalls

**25. Which firewall type is considered the simplest, filtering traffic based only on IP addresses and port numbers?**
*(Rote Definition)*

- A) Stateful inspection firewall
- B) Application layer firewall
- C) Next-generation firewall
- D) Packet filtering firewall

**Answer: D**

---

**26. Why are hardware firewalls generally preferred over software firewalls for protecting medium-to-large enterprise networks?**
*(Conceptual Knowledge)*

- A) Hardware firewalls are easier to configure and require no specialized knowledge
- B) Hardware firewalls are less expensive to purchase and maintain than software alternatives
- C) Hardware firewalls funnel all traffic through a single dedicated appliance, providing more efficient perimeter protection for many hosts
- D) Hardware firewalls can only protect individual hosts, making them more granular

**Answer: C**

---

**27. Why would an organization choose an application layer / next-generation firewall over a stateful inspection firewall?**
*(Conceptual Knowledge)*

- A) It is simpler to configure and has lower hardware requirements
- B) It provides deep packet inspection, IDS/IPS capabilities, and can analyze traffic at the application level for more advanced threat detection
- C) It only filters by IP address and port, reducing processing overhead
- D) It eliminates the need for a DMZ by combining internal and external network segments

**Answer: B**

---

**28. A network administrator is designing the security architecture for a public-facing web server that must be accessible from the internet but must not expose the internal corporate network. Where should the web server be placed?**
*(Application)*

- A) On the internal LAN behind a single firewall
- B) Directly on the internet with no firewall protection
- C) In the DMZ, between two firewalls
- D) On the same subnet as the organization's domain controller

**Answer: C**

---

## Unit 11: Publications and Personnel Security

**29. What is the primary purpose of a STIG?**
*(Rote Definition)*

- A) To establish high-level DoD policy and general guidance
- B) To provide DISA implementation guidance for standardizing security and IT configurations
- C) To direct Air Force-specific compliance actions and procedures
- D) To define step-by-step instructions for routine operations

**Answer: B**

---

**30. How does an AFMAN differ from an AFI?**
*(Conceptual Knowledge)*

- A) An AFMAN must always fall under a parent AFI, while an AFI can stand alone
- B) An AFMAN extends instructions and can stand in place of an AFI without needing to fall under one, while an AFI directs action and ensures compliance
- C) An AFI provides general guidance, while an AFMAN directs specific compliance actions
- D) An AFMAN is issued by DoD, while an AFI is issued by the Air Force

**Answer: B**

---

**31. Why are passive security measures considered a foundational layer of equipment protection rather than a complete solution?**
*(Conceptual Knowledge)*

- A) Passive measures such as barriers and limited entrances deter and delay threats but cannot detect or respond to active intrusions on their own
- B) Passive measures are more expensive than active measures and are only used for high-value assets
- C) Passive measures include cameras and patrols that require constant human monitoring
- D) Passive measures are temporary and must be replaced with active measures after installation

**Answer: A**

---

**32. A base communications squadron needs to ensure that all fiber optic cabling installed across the installation meets a uniform DoD standard for quality and interoperability. Which publication type governs this requirement?**
*(Application)*

- A) AFI
- B) SOP
- C) STIG
- D) MIL-STD

**Answer: D**

---

## Unit 12: Incident Response

**33. In the IR handling process, which step comes immediately after "Detect & Report"?**
*(Rote Definition)*

- A) Response and Recovery
- B) Post-incident Analysis
- C) Preliminary Analysis and Identification
- D) Preliminary Response Actions

**Answer: C**

---

**34. How do the roles of the Technical Specialist and the Documentation Specialist complement each other during an incident?**
*(Conceptual Knowledge)*

- A) The Technical Specialist documents the incident while the Documentation Specialist identifies the root cause
- B) The Technical Specialist identifies the scale and corrects the issue, while the Documentation Specialist records the incident details, cause, and solution for future reference
- C) Both roles focus on correcting the incident, but the Documentation Specialist handles legal matters
- D) The Technical Specialist reports to external agencies, while the Documentation Specialist communicates with internal leadership

**Answer: B**

---

**35. A user discovers that a classified document was accidentally emailed to an unclassified distribution list. The user reports it immediately. Which type of incident has occurred, and what is a required action?**
*(Application)*

- A) Cat 1 — Root-level incident; isolate the email server from the network
- B) Cat 5 — Non-compliance event; retrain the user on email policy
- C) Classified Message Incident; investigate and destroy the unclassified media that received the information
- D) Cat 8 — Event under investigation; wait for further analysis before taking action

**Answer: C**
