### Unit 2: Client Basics

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

### Unit 3: Virtualization

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
