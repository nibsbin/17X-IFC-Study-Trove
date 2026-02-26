### Unit 4: Server

**1. What is the primary function of a server in a network?**
*(Rote Definition)*

- A) Rendering graphics for connected clients
- B) Providing services and managing resources on a network
- C) Converting domain names to IP addresses
- D) Assigning MAC addresses to network devices

**Answer: B**

---

**2. In the DHCP process, what is the correct order of steps a client follows to obtain an IP address?**
*(Rote Definition)*

- A) Request → Discover → Acknowledge → Offer
- B) Offer → Discover → Request → Acknowledge
- C) Discover → Offer → Request → Acknowledge
- D) Discover → Request → Offer → Acknowledge

**Answer: C**

---

**3. What is the top-level container in the Active Directory logical hierarchy?**
*(Rote Definition)*

- A) Domain
- B) Organizational Unit (OU)
- C) Tree
- D) Forest

**Answer: D**

---

**4. How does a client-server model differ from a peer-to-peer model in terms of security?**
*(Conceptual Knowledge)*

- A) Peer-to-peer networks provide stronger centralized security than client-server networks
- B) Client-server networks offer higher security because the server centralizes control, whereas peer-to-peer nodes each act as both client and server
- C) Both models provide identical security since they use the same authentication protocols
- D) Client-server networks are less secure because they rely on a single point of failure

**Answer: B**

---

**5. Why would an organization use DNS instead of requiring users to type IP addresses directly?**
*(Conceptual Knowledge)*

- A) DNS encrypts all network traffic between the client and server
- B) DNS eliminates the need for IP addresses on the network entirely
- C) DNS resolves human-readable domain names to IP addresses, making network resources easier to access
- D) DNS assigns dynamic IP addresses to clients so they do not need static configurations

**Answer: C**

---

**6. Which of the following correctly describes the relationship between a Domain Controller and a Global Catalog Server in Active Directory?**
*(Conceptual Knowledge)*

- A) A Domain Controller manages security within a single domain, while a Global Catalog Server enables cross-domain resource access
- B) A Global Catalog Server replaces the Domain Controller when the network expands beyond one site
- C) A Domain Controller handles DNS resolution, while a Global Catalog Server manages DHCP leases
- D) Both perform identical functions but are named differently depending on the operating system version

**Answer: A**

---

**7. In the URL structure "mail.example.mil/inbox", which component represents the Top-Level Domain (TLD)?**
*(Conceptual Knowledge)*

- A) mail
- B) example
- C) .mil
- D) /inbox

**Answer: C**

---

**8. A network administrator notices that new employees can connect to the network but are unable to access shared department folders. Which Active Directory component should the administrator check first?**
*(Application)*

- A) DNS records for the department file server
- B) DHCP lease assignments for the new employees' workstations
- C) Organizational Unit (OU) and group permissions for the new user accounts
- D) The Global Catalog Server's replication schedule

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

**10. A user reports that their laptop receives a different IP address every time it reconnects to the office network, yet they can still access all resources normally. Which service is responsible for this behavior?**
*(Application)*

- A) Active Directory, which reassigns user credentials on each login
- B) DNS, which rotates IP addresses to balance network traffic
- C) DHCP, which dynamically assigns an available IP address each time the client connects
- D) The Global Catalog Server, which distributes IP pools across domains

**Answer: C**

---

### Unit 6: Cyber Hygiene

**11. What is the definition of cyber hygiene?**
*(Rote Definition)*

- A) The process of encrypting all files on a government network
- B) Practices that maintain system health and improve online security
- C) A federal regulation requiring annual cybersecurity audits
- D) Software that automatically removes viruses from a network

**Answer: B**

---

**12. According to Air Force policy, which publication governs software anti-piracy rules?**
*(Rote Definition)*

- A) NIST SP 800-53
- B) AFI 33-200
- C) DAFMAN 17-1203
- D) DoD Directive 8570

**Answer: C**

---

**13. Which of the following is considered a strong password practice?**
*(Rote Definition)*

- A) Using a short, memorable dictionary word for easy recall
- B) Reusing the same password across multiple accounts for consistency
- C) Creating a long password with mixed characters that avoids dictionary words
- D) Writing the password on a sticky note and attaching it to the monitor

**Answer: C**

---

**14. Why should users enable automatic antivirus updates rather than relying on manual updates?**
*(Conceptual Knowledge)*

- A) Automatic updates prevent all forms of cyberattack, including zero-day exploits
- B) Automatic updates ensure virus definitions stay current without relying on the user to remember, reducing the window of vulnerability
- C) Manual updates are faster and more thorough than automatic updates
- D) Automatic updates replace the need for a firewall on the system

**Answer: B**

---

**15. How does backing up data to multiple locations improve security compared to a single backup?**
*(Conceptual Knowledge)*

- A) Multiple backups encrypt data more effectively than a single backup
- B) Multiple backups guarantee that no data will ever be lost under any circumstances
- C) If one backup location is compromised or fails, data can still be restored from an alternate location, providing redundancy
- D) Multiple backups eliminate the need for antivirus software on the primary system

**Answer: C**

---

**16. What is the relationship between using a government system and consent to monitoring?**
*(Conceptual Knowledge)*

- A) Monitoring only begins after a user is suspected of a policy violation
- B) Users must opt in to monitoring by signing a separate agreement each session
- C) By using a government system, users automatically consent to monitoring of sites visited, keystrokes, shared drives, and all access
- D) Government systems are only monitored during scheduled audit windows

**Answer: C**

---

**17. Why is overwriting a hard drive with a utility recommended over simply deleting files when disposing of a device?**
*(Conceptual Knowledge)*

- A) Deleting files permanently erases them from the disk surface, so overwriting is only an extra precaution
- B) Overwriting replaces data on the disk with random patterns, making recovery far more difficult, whereas deleting files only removes file system pointers and leaves data recoverable
- C) Overwriting is faster than deleting, which is why it is preferred
- D) Deleting files triggers an automatic backup to a cloud server, creating a security risk

**Answer: B**

---

**18. An airman downloads a popular commercial application from an unauthorized website and installs it on their government workstation without a valid license. Which of the following best describes the potential consequences?**
*(Application)*

- A) No consequences, because the software was freely available on the website
- B) A verbal warning from the unit's IT help desk with no further action
- C) Civil or criminal penalties for software piracy under DAFMAN 17-1203
- D) The software will simply be uninstalled automatically by the network firewall

**Answer: C**

---

**19. A cybersecurity analyst discovers that a departing employee's government laptop is being reassigned to a new hire. The laptop's hard drive contains sensitive project files. What is the most appropriate action before reassignment?**
*(Application)*

- A) Delete the departing employee's user profile and hand the laptop to the new hire
- B) Move all files to the Recycle Bin, empty it, and reimage the desktop background
- C) Wipe the device's memory and use an overwrite utility on the hard drive before reconfiguring it for the new user
- D) Remove the laptop from the network and store it in a closet indefinitely

**Answer: C**

---

**20. A government employee receives an email with an attachment claiming to be a required software update. The email does not come from an official IT channel. Applying good cyber hygiene practices, what should the employee do?**
*(Application)*

- A) Open the attachment immediately since it claims to be a required update
- B) Forward the email to all coworkers so they can also install the update
- C) Avoid opening the attachment, report the suspicious email through proper channels, and rely on automatic software updates from authorized sources
- D) Download the attachment to a personal USB drive and scan it at home

**Answer: C**
