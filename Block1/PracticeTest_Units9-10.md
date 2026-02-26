# Block 1 — Practice Test: Units 9 & 10

### Unit 9: Network Security

**1. What does NAC stand for?**
*(Rote Definition)*

- A) Network Authentication Control
- B) Network Access Control
- C) Network Application Controller
- D) Node Access Configuration

**Answer: B**

---

**2. In the AAA framework, which step involves recording a user's actions after they have been granted access?**
*(Rote Definition)*

- A) Identification
- B) Authentication
- C) Authorization
- D) Accounting

**Answer: D**

---

**3. Which authentication factor does a fingerprint scanner represent?**
*(Rote Definition)*

- A) Something you know
- B) Something you have
- C) Something you are
- D) Something you do

**Answer: C**

---

**4. How does an IPS differ from an IDS?**
*(Conceptual Knowledge)*

- A) An IPS only monitors host-level activity, while an IDS monitors network traffic
- B) An IPS detects threats and takes corrective action automatically, while an IDS only detects and alerts
- C) An IPS uses signature-based detection, while an IDS uses anomaly-based detection
- D) An IPS replaces the need for a firewall, while an IDS supplements it

**Answer: B**

---

**5. Why is RADIUS considered less reliable than DIAMETER for AAA services?**
*(Conceptual Knowledge)*

- A) RADIUS uses TCP, which has higher overhead and slower connection setup
- B) RADIUS uses UDP, which does not guarantee delivery of packets
- C) RADIUS cannot perform accounting functions, only authentication
- D) RADIUS requires a permanent agent installed on every endpoint

**Answer: B**

---

**6. What is the relationship between TPM and BitLocker?**
*(Conceptual Knowledge)*

- A) BitLocker is a physical chip that stores encryption keys for TPM software
- B) TPM is a hardware chip that stores cryptographic keys and powers BitLocker's full-disk encryption
- C) TPM and BitLocker are competing encryption standards that cannot be used together
- D) BitLocker replaces TPM by performing all cryptographic operations in software

**Answer: B**

---

**7. Why does Single Sign-On (SSO) present both a security benefit and a potential risk?**
*(Conceptual Knowledge)*

- A) SSO encrypts all passwords but stores them in plaintext on a central server
- B) SSO reduces password fatigue and repeated logins, but a single compromised credential can grant access to multiple systems
- C) SSO eliminates the need for multifactor authentication entirely
- D) SSO only works with biometric authentication, which limits its adoption

**Answer: B**

---

**8. A security administrator discovers that a user's laptop connected to the network despite having outdated antivirus definitions and missing OS patches. Which NAC component most likely failed?**
*(Application)*

- A) IEEE 802.1X port-based authentication
- B) Host health checks
- C) Terms of usage acceptance
- D) RADIUS server configuration

**Answer: B**

---

**9. A contractor needs temporary network access at a military facility. The security team wants to verify the contractor's device compliance without installing any persistent software. Which NAC agent type should they use?**
*(Application)*

- A) Permanent agent
- B) Dissolvable agent
- C) Agentless
- D) Host-based agent

**Answer: B**

---

**10. A cybersecurity analyst notices that a popular internal web application is displaying unexpected pop-up messages containing scripts that redirect users to a credential-harvesting page. Which type of attack is most likely occurring?**
*(Application)*

- A) Peer-to-peer file sharing exploit
- B) Cross-site scripting (XSS)
- C) Cross-site request forgery (CSRF)
- D) Brute-force authentication attack

**Answer: B**

---

### Unit 10: Firewalls

**11. What is the default behavior of an allowlisting firewall policy?**
*(Rote Definition)*

- A) Allow all traffic by default, then block specific entries
- B) Deny all traffic by default, then permit only explicitly approved entries
- C) Inspect packet payloads and allow traffic based on application type
- D) Log all traffic without blocking or allowing anything

**Answer: B**

---

**12. What is a DMZ in network architecture?**
*(Rote Definition)*

- A) A virtual private network tunnel between two remote sites
- B) An encrypted segment of the internal LAN for classified traffic
- C) An area situated between two firewalls that separates internal and external networks
- D) A backup firewall that activates when the primary firewall fails

**Answer: C**

---

**13. Which firewall type is considered the simplest, filtering traffic based only on IP addresses and port numbers?**
*(Rote Definition)*

- A) Stateful inspection firewall
- B) Application layer firewall
- C) Next-generation firewall
- D) Packet filtering firewall

**Answer: D**

---

**14. How does a stateful inspection firewall improve upon basic packet filtering?**
*(Conceptual Knowledge)*

- A) It inspects the full application-layer payload of every packet
- B) It tracks the state of active connections and only allows inbound traffic that corresponds to an outbound-initiated session
- C) It replaces the need for both IDS and IPS by performing deep packet inspection
- D) It filters traffic based solely on source and destination MAC addresses

**Answer: B**

---

**15. Why are hardware firewalls generally preferred over software firewalls for protecting medium-to-large enterprise networks?**
*(Conceptual Knowledge)*

- A) Hardware firewalls are easier to configure and require no specialized knowledge
- B) Hardware firewalls are less expensive to purchase and maintain than software alternatives
- C) Hardware firewalls funnel all traffic through a single dedicated appliance, providing more efficient perimeter protection for many hosts
- D) Hardware firewalls can only protect individual hosts, making them more granular

**Answer: C**

---

**16. What is the key difference between an allowlisting and a denylisting approach to firewall policy?**
*(Conceptual Knowledge)*

- A) Allowlisting is used for hardware firewalls; denylisting is used for software firewalls
- B) Allowlisting permits only explicitly approved traffic and blocks everything else; denylisting blocks only specified traffic and permits everything else
- C) Allowlisting applies to inbound traffic only; denylisting applies to outbound traffic only
- D) Allowlisting requires deep packet inspection; denylisting requires only port filtering

**Answer: B**

---

**17. Why would an organization choose an application layer / next-generation firewall over a stateful inspection firewall?**
*(Conceptual Knowledge)*

- A) It is simpler to configure and has lower hardware requirements
- B) It provides deep packet inspection, IDS/IPS capabilities, and can analyze traffic at the application level for more advanced threat detection
- C) It only filters by IP address and port, reducing processing overhead
- D) It eliminates the need for a DMZ by combining internal and external network segments

**Answer: B**

---

**18. A small business owner wants to protect a single workstation used for online transactions. The business has no dedicated IT staff and needs a low-cost solution. Which firewall solution is most appropriate?**
*(Application)*

- A) A hardware firewall appliance deployed at the network perimeter
- B) A next-generation firewall with deep packet inspection
- C) A software firewall installed on the workstation, such as Windows Firewall
- D) A packet filtering router placed between the workstation and the modem

**Answer: C**

---

**19. A network administrator is designing the security architecture for a public-facing web server that must be accessible from the internet but must not expose the internal corporate network. Where should the web server be placed?**
*(Application)*

- A) On the internal LAN behind a single firewall
- B) Directly on the internet with no firewall protection
- C) In the DMZ, between two firewalls
- D) On the same subnet as the organization's domain controller

**Answer: C**

---

**20. An organization's firewall is configured to deny all traffic by default. A new cloud-based collaboration tool stops working because its traffic is being blocked. An administrator adds a rule to explicitly permit the tool's specific IP addresses and ports. Which firewall policy model is this organization using?**
*(Application)*

- A) Denylisting
- B) Stateful inspection
- C) Allowlisting
- D) Application layer filtering

**Answer: C**
