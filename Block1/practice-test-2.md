# Block 1 — Practice Test 2

> 35 multiple-choice questions covering all Block 1 units.
> Each question targets one of three cognitive levels: **Rote Definition**, **Conceptual Knowledge**, or **Application**.

---

## Unit 2: Client Basics

**1. Which type of memory is volatile and requires power to retain data?**
*(Rote Definition)*

- A) ROM
- B) SSD
- C) RAM
- D) HDD

**Answer: C**

---

**2. Which statement best describes the relationship between an operating system and the hardware it runs on?**
*(Conceptual Knowledge)*

- A) The OS replaces hardware functions with software emulations
- B) The OS acts as a bridge between the user and the hardware, managing both hardware and software resources
- C) The OS communicates directly with all hardware without the use of drivers
- D) The OS is only responsible for running user applications and has no role in resource management

**Answer: B**

---

**3. A cybersecurity analyst observes that a piece of malware has gained unrestricted access to hardware and is modifying driver behavior. In which CPU mode is this malware most likely executing?**
*(Application)*

- A) User Mode
- B) Application Mode
- C) Kernel Mode
- D) Restricted Mode

**Answer: C**

---

## Unit 3: Virtualization

**4. Which of the following is a security risk specifically associated with virtualization?**
*(Rote Definition)*

- A) Increased power consumption from multiple physical servers
- B) VM escape, where an attacker breaks out of a VM to the host
- C) Inability to run more than one operating system at a time
- D) Loss of data caused by volatile memory in the hypervisor

**Answer: B**

---

**5. Which of the following best explains why disabling copy-paste between the host and VM is a recommended hardening measure?**
*(Conceptual Knowledge)*

- A) It prevents the VM from consuming excessive host memory during clipboard operations
- B) It reduces the attack surface by eliminating a data transfer path that could be exploited to move malicious content between environments
- C) It ensures that the host OS and guest OS use the same file system format
- D) It prevents unauthorized users from logging into the hypervisor management console

**Answer: B**

---

**6. A company deploys a Type 2 hypervisor on employee workstations so analysts can run isolated malware samples. An analyst reports that the host workstation has slowed significantly when three VMs run simultaneously. What is the most likely cause?**
*(Application)*

- A) The guest OS inside each VM is incompatible with the Type 2 hypervisor
- B) The malware samples have already escaped the VMs and infected the host
- C) The host workstation lacks sufficient CPU and RAM to support three concurrent VMs plus the host OS and hypervisor overhead
- D) Type 2 hypervisors cannot run more than one VM at a time on a workstation

**Answer: C**

---

## Unit 4: Server

**7. In the DHCP process, what is the correct order of steps a client follows to obtain an IP address?**
*(Rote Definition)*

- A) Request → Discover → Acknowledge → Offer
- B) Offer → Discover → Request → Acknowledge
- C) Discover → Offer → Request → Acknowledge
- D) Discover → Request → Offer → Acknowledge

**Answer: C**

---

**8. Why would an organization use DNS instead of requiring users to type IP addresses directly?**
*(Conceptual Knowledge)*

- A) DNS encrypts all network traffic between the client and server
- B) DNS eliminates the need for IP addresses on the network entirely
- C) DNS resolves human-readable domain names to IP addresses, making network resources easier to access
- D) DNS assigns dynamic IP addresses to clients so they do not need static configurations

**Answer: C**

---

**9. A security technician is hardening a newly deployed server in a secure facility. Which combination of measures best aligns with server security best practices?**
*(Application)*

- A) Enable all USB ports for easy patching, create multiple admin accounts, and connect the server to the public internet
- B) Disable external device ports, implement a man-trap for physical access, use a single admin account with rotating passwords, and isolate the server on the network
- C) Install the server in an unlocked closet, assign a shared admin password, and connect it to the guest Wi-Fi
- D) Place the server behind a man-trap but enable all services and use a default admin password for convenience

**Answer: B**

---

**10. Which physical security measure controls access to a server room through a dual-door entry system that prevents unauthorized tailgating?**
*(Rote Definition)*

- A) Global Catalog Server
- B) Man-trap
- C) Network isolation zone
- D) Domain Controller checkpoint

**Answer: B**

---

## Unit 6: Cyber Hygiene

**11. According to Air Force policy, which publication governs software anti-piracy rules?**
*(Rote Definition)*

- A) NIST SP 800-53
- B) AFI 33-200
- C) DAFMAN 17-1203
- D) DoD Directive 8570

**Answer: C**

---

**12. What is the relationship between using a government system and consent to monitoring?**
*(Conceptual Knowledge)*

- A) Monitoring only begins after a user is suspected of a policy violation
- B) Users must opt in to monitoring by signing a separate agreement each session
- C) By using a government system, users automatically consent to monitoring of sites visited, keystrokes, shared drives, and all access
- D) Government systems are only monitored during scheduled audit windows

**Answer: C**

---

**13. A government employee receives an email with an attachment claiming to be a required software update. The email does not come from an official IT channel. Applying good cyber hygiene practices, what should the employee do?**
*(Application)*

- A) Open the attachment immediately since it claims to be a required update
- B) Forward the email to all coworkers so they can also install the update
- C) Avoid opening the attachment, report the suspicious email through proper channels, and rely on automatic software updates from authorized sources
- D) Download the attachment to a personal USB drive and scan it at home

**Answer: C**

---

## Unit 7: Security Programs

**14. What is the primary purpose of OPSEC?**
*(Rote Definition)*

- A) To encrypt all government communications end-to-end
- B) To reduce mission vulnerabilities by limiting adversary collection of critical information
- C) To classify national security documents at the appropriate level
- D) To detect unintentional electromagnetic emanations from equipment

**Answer: B**

---

**15. How does a worm fundamentally differ from a virus?**
*(Conceptual Knowledge)*

- A) A worm encrypts data and demands ransom; a virus does not
- B) A worm self-replicates without user interaction; a virus requires user interaction to spread
- C) A worm disguises itself as legitimate software; a virus attaches to boot sectors
- D) A worm monitors user activity; a virus modifies system files

**Answer: B**

---

**16. An administrator needs to send a Top Secret document to a cleared recipient at another installation. Which method of transmission is authorized?**
*(Application)*

- A) USPS registered mail within the United States
- B) USPS certified or first-class mail to DoD contractors
- C) Department of State courier
- D) Encrypted email over an unclassified network

**Answer: C**

---

**17. Which classification level applies to information whose unauthorized disclosure could cause "serious damage" to national security?**
*(Rote Definition)*

- A) Confidential
- B) Secret
- C) Top Secret
- D) Controlled Unclassified Information (CUI)

**Answer: B**

---

## Unit 8: Risk, Threats, and Vulnerabilities

**18. What type of malware remains dormant until a predefined event triggers its execution?**
*(Rote Definition)*

- A) Rootkit
- B) Polymorphic malware
- C) Logic bomb
- D) Adware

**Answer: C**

---

**19. Why is polymorphic malware particularly difficult for traditional antivirus software to detect?**
*(Conceptual Knowledge)*

- A) It hides in the boot sector and loads before the antivirus starts
- B) It changes its code signature with each execution, evading signature-based detection
- C) It encrypts the entire hard drive, preventing the antivirus from scanning files
- D) It disables the network adapter so the antivirus cannot download updated definitions

**Answer: B**

---

**20. A system administrator notices that programs on a server are opening and closing without user input, the system has rebooted unexpectedly, and unfamiliar error messages are appearing. Based on these symptoms, what should the administrator suspect?**
*(Application)*

- A) A DHCP address conflict
- B) A malware infection
- C) A routine operating system update
- D) A misconfigured firewall rule

**Answer: B**

---

**21. What is the defining characteristic of a rootkit?**
*(Rote Definition)*

- A) It displays unwanted advertisements without user consent
- B) It encrypts the victim's files and demands payment for decryption
- C) It grants an attacker hidden, privileged access to a compromised system
- D) It changes its code signature on every execution to evade detection

**Answer: C**

---

## Unit 9: Network Security

**22. In the AAA framework, which step involves recording a user's actions after they have been granted access?**
*(Rote Definition)*

- A) Identification
- B) Authentication
- C) Authorization
- D) Accounting

**Answer: D**

---

**23. Why is RADIUS considered less reliable than DIAMETER for AAA services?**
*(Conceptual Knowledge)*

- A) RADIUS uses TCP, which has higher overhead and slower connection setup
- B) RADIUS uses UDP, which does not guarantee delivery of packets
- C) RADIUS cannot perform accounting functions, only authentication
- D) RADIUS requires a permanent agent installed on every endpoint

**Answer: B**

---

**24. A contractor needs temporary network access at a military facility. The security team wants to verify the contractor's device compliance without installing any persistent software. Which NAC agent type should they use?**
*(Application)*

- A) Permanent agent
- B) Dissolvable agent
- C) Agentless
- D) Host-based agent

**Answer: B**

---

**25. Why is peer-to-peer (P2P) file sharing considered a security risk on organizational networks?**
*(Conceptual Knowledge)*

- A) P2P file sharing consumes more bandwidth than streaming services, degrading network performance
- B) P2P connections bypass NAC host health checks and allow direct peer authentication
- C) P2P file sharing is a common vector for malicious code distribution
- D) P2P applications require elevated privileges that trigger NAC alerts automatically

**Answer: C**

---

## Unit 10: Firewalls

**26. What is a DMZ in network architecture?**
*(Rote Definition)*

- A) A virtual private network tunnel between two remote sites
- B) An encrypted segment of the internal LAN for classified traffic
- C) An area situated between two firewalls that separates internal and external networks
- D) A backup firewall that activates when the primary firewall fails

**Answer: C**

---

**27. What is the key difference between an allowlisting and a denylisting approach to firewall policy?**
*(Conceptual Knowledge)*

- A) Allowlisting is used for hardware firewalls; denylisting is used for software firewalls
- B) Allowlisting permits only explicitly approved traffic and blocks everything else; denylisting blocks only specified traffic and permits everything else
- C) Allowlisting applies to inbound traffic only; denylisting applies to outbound traffic only
- D) Allowlisting requires deep packet inspection; denylisting requires only port filtering

**Answer: B**

---

**28. An organization's firewall is configured to deny all traffic by default. A new cloud-based collaboration tool stops working because its traffic is being blocked. An administrator adds a rule to explicitly permit the tool's specific IP addresses and ports. Which firewall policy model is this organization using?**
*(Application)*

- A) Denylisting
- B) Stateful inspection
- C) Allowlisting
- D) Application layer filtering

**Answer: C**

---

## Unit 11: Publications and Personnel Security

**29. Which publication type provides step-by-step instructions for carrying out routine tasks?**
*(Rote Definition)*

- A) DoDI
- B) AFI
- C) STIG
- D) SOP

**Answer: D**

---

**30. What is the relationship between a DoDI and a DoDM?**
*(Conceptual Knowledge)*

- A) A DoDI implements the detailed procedures outlined in a DoDM
- B) A DoDM establishes policy, while a DoDI provides the implementation details
- C) A DoDI establishes policy and general guidance, while a DoDM implements that policy with procedural details
- D) A DoDI and DoDM serve identical purposes but are issued by different authorities

**Answer: C**

---

**31. A cybersecurity team is configuring firewalls, hardening operating systems, and ensuring all devices meet a standardized security baseline across the enterprise. Which publication type should they reference for specific implementation guidance on these configurations?**
*(Application)*

- A) SOP
- B) MIL-STD
- C) STIG
- D) DoDI

**Answer: C**

---

## Unit 12: Incident Response

**32. Which Incident Response category is classified as an incident involving malicious logic?**
*(Rote Definition)*

- A) Cat 4
- B) Cat 5
- C) Cat 1
- D) Cat 7

**Answer: D**

---

**33. Why does a Classified Message Incident (CMI) fall outside the standard IR category framework?**
*(Conceptual Knowledge)*

- A) CMIs only affect unclassified networks and are handled by a separate team
- B) CMIs involve the transfer of confidential or higher information onto unauthorized media, requiring investigation and destruction of the unclassified media rather than fitting a standard numbered category
- C) CMIs are automatically resolved by automated systems and do not need human analysis
- D) CMIs are reclassified as Cat 0 training exercises once they are detected

**Answer: B**

---

**34. During an incident, the CIRT has completed its response and the affected systems are restored. The team now drafts a document analyzing the threat actor's tactics, techniques, and activity patterns observed during the incident. Which concluding course of action does this document represent?**
*(Application)*

- A) Postmortem
- B) Cyber Incident Report (CIR)
- C) Network Intel Report (NIR)
- D) Classified Message Incident (CMI)

**Answer: C**

---

**35. What is the role of a First Responder in an Incident Response scenario?**
*(Rote Definition)*

- A) To lead the CIRT team and maintain relationships with external agencies
- B) To document incident details, causes, and corrective actions for the record
- C) To be the first user to identify and react to a security incident, trained for basic response
- D) To advise the team on applicable laws and regulations governing the incident

**Answer: C**
