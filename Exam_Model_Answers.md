## Model Answers for "Computer Forensics - PRACTICE" Exam Paper

### **Section A**

**Answer ALL of the Four questions listed.**

---

**1. Network monitoring is an important aspect in network forensics, why are traffic (packet) capturing an effective approach to gathering information to be used in a legal investigation? (10 marks)**

**Model Answer:**

Traffic (packet) capturing is an effective approach to gathering information for a legal investigation in network forensics for several key reasons:

*   **Real-time Evidence of Activity (2 marks):** Packet capture provides a direct, contemporaneous record of network communications as they occur. This can be crucial for understanding live attacks, intrusions, or illicit data transfers, offering a snapshot of events in progress.
*   **Identification of Source and Destination (2 marks):** Captured packets contain IP addresses, MAC addresses, and port numbers for both the source and destination of the communication. This is fundamental for identifying involved parties, tracing attack origins, or determining where compromised data is being exfiltrated.
*   **Content Analysis (Payload) (2 marks):** Depending on whether the traffic is encrypted, the payload of packets can be reconstructed to reveal the actual data transmitted. This could include emails, chat messages, transferred files, commands issued, or web pages visited, providing direct evidence of an activity.
*   **Reconstruction of Events and Timelines (2 marks):** Sequences of captured packets can be used to reconstruct the timeline of network events, understand the methods used by an attacker (e.g., reconnaissance, exploitation, exfiltration), and determine the scope of an incident. Timestamps on packets are vital for this.
*   **Detection of Anomalies and Malicious Signatures (1 mark):** Packet analysis can reveal traffic patterns that deviate from normal behavior, or match known signatures of malware, exploits, or specific attack tools (e.g., port scanning, DDoS patterns).
*   **Independent Corroboration (1 mark):** Network traffic data can corroborate or refute claims made by individuals or evidence found on end-host systems. It provides an objective record of what traversed the network.

For these reasons, packet capture is a powerful tool, providing rich, detailed, and often irrefutable evidence of network activities that can be critical in legal investigations.

---

**2. What is the purpose of the SHA–1 hash when applied to a computer forensic examination? (15 marks)**

**Model Answer:**

The Secure Hash Algorithm 1 (SHA-1) is a cryptographic hash function that produces a 160-bit (20-byte) hash value, typically rendered as a 40-digit hexadecimal number. In a computer forensic examination, the primary purposes of applying a SHA-1 hash are:

*   **Integrity Verification (5 marks):**
    *   **Concept:** SHA-1 is used to create a unique digital "fingerprint" of a piece of digital evidence (e.g., a file, a disk image, or a partition) at a specific point in time.
    *   **Application:** A hash value is calculated for the original evidence before acquisition or at the time of seizure. After creating a forensic image (copy), the hash of the image is calculated. If the hash values of the original and the copy match, it provides strong assurance that the copy is an exact, unaltered duplicate of the original. This process is repeated at various stages (e.g., before and after analysis) to demonstrate that the evidence has not been tampered with or corrupted throughout the investigation.
    *   **Importance:** This is crucial for admissibility in court, as it demonstrates that the evidence presented is the same as what was originally collected.

*   **Authentication (5 marks):**
    *   **Concept:** Hashing helps to authenticate that a piece of data is what it purports to be and has not been modified since it was last hashed.
    *   **Application:** If an investigator analyzes a file and later needs to present it, recalculating its hash and comparing it to the original hash value recorded in the case notes authenticates that the file being presented is the same unaltered file that was analyzed. It confirms the evidence's authenticity.

*   **Identification (Known File Filtering/Comparison) (3 marks):**
    *   **Concept:** SHA-1 hashes can be used to identify known files.
    *   **Application:** Investigators can compare the hash values of files on a suspect system against databases of known file hashes.
        *   **Known Good Files:** Hashes of standard operating system files or legitimate application files can be used to filter out irrelevant data, allowing the investigator to focus on unique or suspicious files (e.g., NIST National Software Reference Library - NSRL).
        *   **Known Bad Files:** Hashes of known malware, child exploitation material, or other contraband can quickly identify illicit files on a system.
    *   **Importance:** This significantly speeds up the examination process by reducing the volume of data that needs manual review.

*   **Uniqueness (Implicit) (2 marks):**
    *   While SHA-1 has known theoretical collision weaknesses (meaning two different inputs *could* produce the same hash, though practically rare for distinct large files), for most forensic purposes, it's assumed that a specific SHA-1 hash value corresponds to a unique piece of data. A change of even a single bit in the input data will result in a drastically different hash value.

**Note on SHA-1 Weaknesses:** While SHA-1 serves these purposes, it's important to acknowledge that due to discovered collision vulnerabilities, for high-security applications or where absolute collision resistance is paramount, stronger hash functions like SHA-256 or SHA-512 are now preferred. However, SHA-1 is still widely encountered in digital forensics for legacy systems and for general integrity checking where the risk of deliberate collision attacks is considered low for the specific context.

---

**3. Evidence integrity is essential in order for digital evidence to be admissible in court and to carry weight as evidence.**
    *   **What is CoC (Chain of Custody) and why is it important for evidence integrity?**
    *   **Assuming that a forensic team follows the right steps for preserving evidence integrity and for keeping an unbroken CoC, what must they do in order to convince the court that they have done so?**
    *   **What is OOV (order of volatility), and how does it influence decisions regarding which evidence should be preserved first?**
    *   **List various data storage media as a function of their OOV.**
    **(12 marks)**

**Model Answer:**

*   **What is CoC (Chain of Custody) and why is it important for evidence integrity? (3 marks)**
    *   **Definition (1 mark):** Chain of Custody (CoC) is a chronological documented record of the sequence of custody, control, transfer, analysis, and disposition of physical or electronic evidence. It details who handled the evidence, when, where, why, and how.
    *   **Importance for Evidence Integrity (2 marks):** CoC is crucial for evidence integrity because it demonstrates that the evidence has been handled properly and has not been tampered with, altered, or substituted from the moment it was seized until it is presented in court. An unbroken and well-documented CoC helps to establish the authenticity and reliability of the evidence, making it more likely to be admissible and carry weight in legal proceedings. It answers potential challenges about how the evidence was managed.

*   **Assuming that a forensic team follows the right steps for preserving evidence integrity and for keeping an unbroken CoC, what must they do in order to convince the court that they have done so? (3 marks)**
    To convince the court, the forensic team must:
    *   **Meticulous Documentation (1 mark):** Provide comprehensive and contemporaneous documentation for every step taken. This includes detailed evidence logs, acquisition forms, analysis notes, photographs/videos of the scene and evidence, and a complete CoC form.
    *   **Adherence to Standards and Best Practices (1 mark):** Demonstrate that the investigation followed established guidelines and best practices (e.g., ACPO principles in the UK). This includes using validated tools and techniques.
    *   **Expert Testimony (1 mark):** Have a qualified forensic examiner clearly and confidently explain the procedures followed, the tools used, how integrity was maintained (e.g., use of write-blockers, hashing), and how the CoC was managed. The examiner must be able to withstand cross-examination regarding their methods.

*   **What is OOV (order of volatility), and how does it influence decisions regarding which evidence should be preserved first? (3 marks)**
    *   **Definition (1 mark):** Order of Volatility (OOV) refers to the sequence in which digital evidence should be collected based on how quickly it can be lost, altered, or destroyed. Data ranges from highly volatile (disappears quickly when power is lost or system state changes) to non-volatile (persists after power-off).
    *   **Influence on Decisions (2 marks):** OOV dictates that the most volatile evidence must be collected first. For example, data in CPU registers and RAM is extremely volatile and will be lost if a system is powered down. Therefore, live acquisition techniques to capture RAM and running processes should be prioritized over imaging a hard drive if both are options and the system is live. This ensures that transient but potentially crucial evidence is not inadvertently destroyed.

*   **List various data storage media as a function of their OOV. (3 marks)**
    Listed from most volatile to least volatile:
    1.  **CPU Registers, Cache (L1, L2, L3)** (Extremely volatile, lost almost instantly)
    2.  **RAM (Main Memory)**, including routing tables, ARP cache, process tables, running applications, open network connections, encryption keys. (Volatile, lost on power-off)
    3.  **Paging File / Swap Space** (Less volatile than RAM, but frequently changing; resides on persistent storage)
    4.  **Hard Disk Drives (HDD) / Solid State Drives (SSD)** (Non-volatile, data persists after power-off, but can be overwritten)
    5.  **Logs stored on remote systems** (e.g., syslog server, cloud storage) (Non-volatile, persistence depends on remote system's configuration)
    6.  **Archive Media** (e.g., backup tapes, DVDs, external HDDs used for backup) (Non-volatile, designed for long-term storage)

---

**4. Computer forensics have various types of acquisition methods,**
    *   **Explain the difference between “live acquisition” and “post mortem acquisition”.**
    *   **What are the advantages and disadvantages of live and post mortem acquisition?**
    *   **Give an example when “live acquisition” is necessary**
    **(15 marks)**

**Model Answer:**

*   **Explain the difference between “live acquisition” and “post mortem acquisition”. (4 marks)**
    *   **Live Acquisition (2 marks):** This refers to the process of acquiring data from a computer system while it is still running and powered on. The primary goal is to capture volatile data that would be lost if the system were shut down, such as the contents of RAM, running processes, active network connections, and logged-on users. It often involves running trusted forensic tools directly on the live system or from a trusted external device.
    *   **Post Mortem Acquisition (Dead Box Forensics) (2 marks):** This involves acquiring data from a computer system after it has been powered off. The focus is typically on non-volatile storage media like hard drives or SSDs. The storage device is often removed from the suspect system and connected to a forensic workstation via a write-blocker to create a bit-for-bit forensic image.

*   **What are the advantages and disadvantages of live and post mortem acquisition? (8 marks)**

    **Live Acquisition:**
    *   **Advantages (2 marks):**
        *   **Captures Volatile Data:** Access to RAM contents, running processes, network state, encryption keys in memory, which are lost upon shutdown.
        *   **Insight into Active State:** Can reveal active malware, established malicious connections, or user activity at the time of acquisition.
        *   **Overcomes Full Disk Encryption (FDE):** If the system is running and the disk is decrypted, live acquisition can capture data from the decrypted volume.
    *   **Disadvantages (2 marks):**
        *   **Risk of Altering System State:** Running tools on a live system inherently makes minor changes (e.g., loading tools into memory, creating log entries). This must be minimized and documented.
        *   **Malware Interference:** Active malware (e.g., rootkits) on the system could interfere with acquisition tools, hide data, or even attack the forensic tools.
        *   **Complexity and Skill Required:** Requires more specialized knowledge and tools, and careful execution to maintain forensic soundness.

    **Post Mortem Acquisition:**
    *   **Advantages (2 marks):**
        *   **Forensically Sounder for Static Data:** When performed correctly with a write-blocker, it provides a verifiable, unaltered image of non-volatile storage.
        *   **Reduced Risk of System Alteration:** The system is off, so no active processes are changing data on the storage device being imaged.
        *   **More Established Tools and Procedures:** A wider range of mature tools and well-defined procedures exist for imaging powered-off devices.
    *   **Disadvantages (2 marks):**
        *   **Loss of Volatile Data:** All data in RAM, active processes, etc., is lost.
        *   **Full Disk Encryption (FDE) Challenges:** If the disk is encrypted and the system is off, the data will be inaccessible without the decryption key/password or specialized decryption techniques.
        *   **May Miss Context:** Doesn't show what was actively happening on the system at a specific moment.

*   **Give an example when “live acquisition” is necessary (3 marks)**
    Live acquisition is necessary in several scenarios, for example:
    *   **Investigating an Active Network Intrusion or Malware Infection:** If a system is suspected of being actively compromised (e.g., by ransomware encrypting files, or a Remote Access Trojan (RAT) communicating with an attacker), live acquisition is crucial. It can capture the malicious processes in RAM, identify active network connections to command-and-control servers, and potentially recover encryption keys or other transient indicators of compromise that would be lost if the system were immediately shut down. For instance, if investigating a system actively participating in a DDoS attack, live acquisition could identify the malware responsible and its network targets.

---

### **Section B**

**Answer any Two out of Three questions listed.**

*(Model answers will be provided for all three for completeness, but in an exam, you would only choose two.)*

---

**1. The ACPO guidelines outline the process that UK law enforcement follows for forensic operations, the guidelines contain 4 key principles. Outline each principle and give an example to demonstrate how this principle can be implemented. (10 marks)**

**Model Answer:**

The Association of Chief Police Officers (ACPO) Good Practice Guide for Digital Evidence outlines four key principles for handling digital evidence in the UK. These are:

*   **Principle 1: No action taken by law enforcement agencies or their agents should change data held on a computer or storage media which may subsequently be relied upon in court. (1 mark for outlining)**
    *   **Explanation:** This principle emphasizes the paramount importance of preserving the original state of digital evidence. Any alteration could compromise its integrity and admissibility.
    *   **Example of Implementation (1.5 marks):** When seizing a computer hard drive, a forensic investigator uses a hardware or software write-blocker. This device physically prevents any write operations from reaching the original drive while a forensic image (a bit-for-bit copy) is being created. The original drive is then stored securely, and all analysis is performed on the verified forensic image.

*   **Principle 2: In circumstances where a person finds it necessary to access original data held on a computer or on storage media, that person must be competent to do so and be able to give evidence explaining the relevance and implications of their actions. (1 mark for outlining)**
    *   **Explanation:** This acknowledges that sometimes, direct interaction with original evidence might be unavoidable (e.g., some live acquisitions, or accessing specific data on a complex server setup before full imaging is feasible). However, this must only be done by trained personnel who understand the risks and can justify their actions.
    *   **Example of Implementation (1.5 marks):** During a live acquisition of a server suspected of running active malware, a trained forensic examiner might need to run a trusted tool from a USB drive to capture RAM content. The examiner must be able to explain why this was necessary (e.g., to capture volatile data that would be lost on shutdown), what tool was used, how it was used, and what potential (minimal) changes their actions might have made to the system, and why these were unavoidable and do not compromise the key evidence sought.

*   **Principle 3: An audit trail or other record of all processes applied to computer-based evidence should be created and preserved. An independent third party should be able to examine those processes and achieve the same results. (1 mark for outlining)**
    *   **Explanation:** This principle mandates thorough documentation of every action taken during the forensic process. This ensures transparency, accountability, and allows the process to be repeatable and verifiable by another independent expert.
    *   **Example of Implementation (1.5 marks):** An investigator meticulously records every step in their case notes: the date/time of evidence seizure, details of the hardware/software used for imaging (including version numbers), hash values calculated before and after imaging, tools used for analysis, search terms used, and findings. This detailed log forms part of the chain of custody and allows another examiner to understand and potentially replicate the steps taken.

*   **Principle 4: The person in charge of the investigation (the case officer) has overall responsibility for ensuring that the law and these principles are adhered to. (1 mark for outlining)**
    *   **Explanation:** This assigns ultimate responsibility for the forensic integrity of the investigation to a designated individual, typically the Senior Investigating Officer (SIO) or case officer. They must ensure that all personnel involved are aware of and comply with legal requirements and forensic best practices.
    *   **Example of Implementation (1.5 marks):** The case officer ensures that all forensic examiners are properly trained and certified, that appropriate warrants are obtained before search and seizure, that resources (like validated tools and secure storage) are available, and that all ACPO principles are followed throughout the investigation. They would review case files and reports to ensure compliance.

---

**2. The UK Legislation ’Computer misuse act 1990’ outlines several offences directly related to forensic investigations,**
    *   **S1 Unauthorised Access To Computer Material,**
    *   **S2 Unauthorised Access With Intent to Commit Other Offence,**
    *   **S3 Unauthorised Acts with Intent to Impair Operation,**
    *   **S3A Making, Supplying or Obtaining Article for Use in S1 or S3 offences.**
**Give a brief description of each offence S1, S2, S3 and S3A, give an example of such an offence that a forensic investigator may encounter. (10 marks)**

**Model Answer:**

The UK Computer Misuse Act 1990 (CMA) outlines several key offences relevant to forensic investigations:

*   **S1 Unauthorised Access To Computer Material (1 mark for description, 1 mark for example):**
    *   **Description:** This offence makes it illegal to intentionally cause a computer to perform any function with intent to secure access to any program or data held in any computer, or to enable any such access to be secured, when the access is unauthorised, and the person knows at the time that it is unauthorised. It's often referred to as "basic hacking."
    *   **Example Encountered:** An investigator examining a suspect's computer might find logs or browser history indicating the suspect guessed or used stolen credentials to log into someone else's social media account or email without permission, purely to view their private messages or files.

*   **S2 Unauthorised Access With Intent to Commit Other Offence (1 mark for description, 1 mark for example):**
    *   **Description:** This is an aggravated offence. It involves committing an S1 offence (unauthorised access) with the further intent to commit or facilitate the commission of another, more serious offence (e.g., fraud, blackmail, or offences under S3 of the CMA).
    *   **Example Encountered:** An investigator finds evidence that a suspect gained unauthorised access to a company's financial database (S1 offence) with the clear intention of subsequently transferring funds to their own account (facilitating fraud). Email drafts or search history might indicate this intent.

*   **S3 Unauthorised Acts with Intent to Impair Operation (or hinder access) (1 mark for description, 1 mark for example):**
    *   **Description:** This offence covers acts done to a computer that are unauthorised and are carried out with the intent to impair the operation of any computer, prevent or hinder access to any program or data, or impair the operation of any such program or the reliability of such data. This includes modifying, corrupting, or deleting data or programs.
    *   **Example Encountered:** A disgruntled ex-employee is suspected of remotely accessing the company server after termination and deleting critical customer databases or deploying ransomware. The investigator would look for evidence of the unauthorised access and the subsequent data deletion/encryption.

*   **S3A Making, Supplying or Obtaining Article for Use in S1 or S3 offences (1 mark for description, 1 mark for example):**
    *   **Description:** This offence makes it illegal to make, adapt, supply, or offer to supply any article (including any program or data held in electronic form) intending it to be used to commit, or to assist in the commission of, an offence under S1 or S3. It also covers obtaining such an article with such intent.
    *   **Example Encountered:** During an investigation, a suspect's computer is found to contain malware creation kits (e.g., tools to build custom viruses or phishing website templates), or a collection of stolen usernames and passwords, along with evidence (like forum posts or chat logs) that they intend to use or supply these for hacking (S1) or disruptive (S3) activities.

*(Note: For full marks, ensure the description captures the essence of "unauthorised" and "intent/knowledge" where specified in the Act for each section.)*

---

**3. The monitoring and logging of user activities have tangible benefits to a forensic investigator. Discuss these benefits and provide reasoning as to why this practice of excessive logging may or may not be ethical. (10 marks)**

**Model Answer:**

**Benefits of Monitoring and Logging User Activities for a Forensic Investigator (4 marks):**

The monitoring and logging of user activities provide significant tangible benefits to a forensic investigator:

1.  **Audit Trail and Event Reconstruction:** Logs create a chronological record of user actions (e.g., file access, program execution, login attempts, network connections). This allows investigators to reconstruct the sequence of events leading up to, during, and after an incident, which is crucial for understanding how an incident occurred. (1 mark)
2.  **Attribution and Identification:** Detailed logs can help identify which user account was involved in suspicious activity, potentially leading to the individual responsible. IP address logs, MAC addresses, and user login correlations can pinpoint the source of actions. (1 mark)
3.  **Detection of Anomalies and Unauthorized Access:** By establishing a baseline of normal activity, logs can help investigators identify deviations that may indicate unauthorized access, malware activity, or policy violations. For instance, logins at unusual times or from unexpected locations. (1 mark)
4.  **Evidence for Investigation and Prosecution:** Logs can provide direct evidence of wrongdoing, such as unauthorized data access, deletion of files, or attempts to cover tracks. This evidence is often critical in both internal investigations and legal proceedings. (1 mark)

**Ethical Considerations of Excessive Logging (6 marks):**

The practice of excessive logging, while beneficial for forensics, raises significant ethical concerns, but can also be justified in certain contexts.

**Arguments for why excessive logging MAY BE UNETHICAL (3 marks):**

1.  **Invasion of Privacy:** Extensive logging can capture a vast amount of personal information about users, including their browsing habits, personal communications (if company systems are used for personal reasons), and other sensitive activities. This can be seen as a disproportionate intrusion into employee privacy if not properly justified and managed. (1 mark)
2.  **Potential for Misuse and Chilling Effect:** The collected data, if not securely stored and access-controlled, could be misused by employers or malicious insiders. Furthermore, the knowledge of constant, detailed monitoring can create a "chilling effect," discouraging legitimate communication or making employees feel untrusted. (1 mark)
3.  **Lack of Transparency and Consent:** If employees are not fully aware of the extent and nature of logging, or if consent is not appropriately obtained (especially for personal data), the practice can be ethically questionable. Data protection laws (like GDPR) emphasize transparency and lawful basis for processing. (1 mark)

**Arguments for why excessive logging MAY NOT BE UNETHICAL (or may be justified) (3 marks):**

1.  **Legitimate Security Interest and Duty of Care:** Organizations have a legitimate interest in protecting their assets, data, and systems, and a duty of care to protect customer/employee data. Logging can be essential for detecting and responding to security incidents, thereby fulfilling these responsibilities. (1 mark)
2.  **Compliance and Legal Requirements:** Certain industries or regulations may mandate specific levels of logging for compliance purposes (e.g., financial services, healthcare). Failure to log adequately could lead to legal or regulatory penalties. (1 mark)
3.  **Clear Policies, Consent, and Proportionality:** If logging practices are clearly communicated to employees through acceptable use policies, if consent is obtained where necessary, if data collected is minimized to what is necessary (proportionality), and if strict access controls and retention policies are in place, the ethical concerns can be mitigated. The focus should be on business-related activities on company systems. (1 mark)

**Conclusion:** The ethicality of logging hinges on a balance between the legitimate needs of the organization for security and investigation, and the privacy rights of individuals. Transparency, clear policies, consent, proportionality, and robust data protection measures are key to ethically implementing logging practices.

---

## Model Answers for "Computer Forensics" (Actual Past Paper) Exam Paper

### **Section A**

**Answer ALL of the Four questions listed.**

---

**1. Explain what a forensic methodology is and what the benefits of such a method are in forensic computing? - you should outline the difference between a legal investigation and an internal forensic investigation (10 marks)**

**Model Answer:**

**Forensic Methodology (3 marks):**
A forensic methodology is a systematic, standardized, and documented set of procedures and principles followed during a digital forensic investigation. It provides a structured framework for handling digital evidence from its initial identification and collection through to its analysis and presentation. The goal is to ensure that the investigation is conducted in a consistent, reliable, repeatable, and legally defensible manner, preserving the integrity of the evidence at all stages. Examples include models like CFSAP or the processes outlined in the ACPO guidelines.

**Benefits of a Forensic Methodology (3 marks):**
The benefits of using a defined forensic methodology in forensic computing are numerous:
*   **Consistency and Reliability:** Ensures that investigations are conducted in a uniform way, leading to more reliable and predictable outcomes.
*   **Admissibility of Evidence:** Following a recognized methodology increases the likelihood that evidence will be admissible in court, as it demonstrates due diligence and adherence to best practices.
*   **Reproducibility:** A well-documented methodology allows another qualified examiner to repeat the steps taken and, ideally, arrive at the same conclusions, verifying the findings.
*   **Defensibility:** Provides a strong basis for defending the investigative process and findings against legal challenges or scrutiny.
*   **Minimizes Errors and Contamination:** Reduces the risk of errors, evidence alteration, or contamination by providing clear guidelines for each stage.
*   **Efficiency:** While initially seeming more time-consuming, a structured approach can improve efficiency by streamlining processes and ensuring all necessary steps are covered.

**Difference between a Legal Investigation and an Internal Forensic Investigation (4 marks):**

| Feature                 | Legal Investigation (e.g., Law Enforcement, Civil Litigation) | Internal Forensic Investigation (e.g., Corporate)            |
| :---------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| **Primary Goal**        | Gather evidence for prosecution in criminal cases or for resolution in civil disputes. (1 mark) | Investigate policy violations, security incidents, employee misconduct, or gather intelligence for the organization. (1 mark) |
| **Legal Authority**     | Requires legal authority (e.g., warrants, subpoenas) for search, seizure, and access to data. Bound by strict rules of evidence and criminal/civil procedure. (0.5 mark) | Typically operates under company policy, employment contracts, and acceptable use policies. May not require external legal authority for internal systems but must respect privacy laws. (0.5 mark) |
| **Scope & Constraints** | Scope often defined by legal warrants. Subject to greater scrutiny and legal challenges regarding methodology and evidence handling. (0.5 mark) | Scope defined by internal needs and policies. May have more flexibility but still needs to be ethically sound and potentially defensible if it leads to legal action. (0.5 mark) |
| **Outcome/Reporting**   | Evidence presented in court, leading to potential criminal convictions, civil judgments, or acquittals. Reports are formal and geared towards legal standards. (0.5 mark) | Outcomes can include disciplinary action, termination of employment, system remediation, policy changes, or, if criminal activity is found, referral to law enforcement. Reports may be less formal initially. (0.5 mark) |

Essentially, legal investigations are driven by the requirements of the justice system and have a higher burden of proof, while internal investigations are primarily focused on organizational concerns, though they must still be conducted with integrity as they might escalate to legal matters.

---

**2. The CFSAP (Computer forensics - Secure, analyse, present) principles outline four key elements in computer forensics. With relation to stage one Secure, discuss two different potential sources of computer information and describe a suitable process for securing each of these sources. (25 marks)**

**Model Answer:**

The CFSAP (Computer Forensics - Secure, Analyse, Present) model outlines a high-level framework for conducting computer forensic investigations. The first stage, "Secure," encompasses the crucial initial steps of identifying potential sources of digital evidence and then preserving (securing) that evidence to maintain its integrity.

**Stage One: Secure**
This stage involves:
*   **Identification:** Recognizing and locating potential sources of digital evidence relevant to the investigation.
*   **Preservation:** Taking steps to protect the identified evidence from alteration, damage, or destruction. This is fundamental for ensuring the evidence's admissibility and reliability.

**Discussion of Two Different Potential Sources of Computer Information and Suitable Securing Processes:**

**Source 1: Hard Disk Drive (HDD) from a Desktop Computer (Suspect's primary workstation)**

*   **Why it's a potential source (4 marks):**
    *   HDDs are the primary non-volatile storage for most traditional desktop computers.
    *   They can contain a vast amount of information, including the operating system, installed applications, user-created files (documents, images, videos), internet browsing history, emails, chat logs, deleted files (in unallocated space or slack space), system logs, and various other digital artifacts that can provide evidence of user activity, intent, or criminal conduct.
    *   Even if files are deleted, remnants often remain recoverable until overwritten.

*   **Suitable process for securing an HDD (6 marks):**
    1.  **Documentation:** Photograph the computer system in situ, noting all connections, the state of the machine (on/off), and any on-screen information if it's live. Record the make, model, and serial number of the computer and the HDD.
    2.  **Power Down (if live and appropriate):** If the system is live and a decision is made not to perform a live RAM capture first (or if it's already off), power down the system correctly. For most forensic purposes, pulling the power cord is preferred for Windows systems to prevent shutdown scripts from running and altering data, while a graceful shutdown might be considered for some server systems (after careful consideration of OOV).
    3.  **Physical Removal and Write-Blocking:** Carefully remove the HDD from the suspect computer. Connect the original HDD to a forensic workstation via a validated hardware write-blocker. This device prevents any data from being written to or altering the original evidence drive during the imaging process.
    4.  **Forensic Imaging:** Create a bit-for-bit (sector-by-sector) forensic image of the entire original HDD onto a forensically sterile target drive. Use validated forensic imaging software (e.g., FTK Imager, EnCase Imager, `dd` with appropriate options).
    5.  **Hashing:** Calculate cryptographic hash values (e.g., SHA-256) of both the original source drive and the created forensic image. Verify that the hash values match to confirm the image is an exact and unaltered copy. Record these hash values.
    6.  **Chain of Custody:** Document the seizure of the HDD, its details, who handled it, when, where, and the details of the imaging process on the Chain of Custody form. Securely store the original HDD as evidence. All subsequent analysis will be performed on the verified forensic image(s).

**Source 2: Volatile Memory (RAM) from a Live Server experiencing a suspected ongoing network attack**

*   **Why it's a potential source (4 marks):**
    *   RAM is volatile memory, meaning its contents are lost when the system loses power.
    *   It contains a snapshot of the system's current operational state, including: running processes (legitimate and potentially malicious), active network connections (which could identify C&C servers for malware), loaded kernel modules, open files, recently typed commands, cryptographic keys, unencrypted data being processed, and other transient artifacts.
    *   For an ongoing network attack, RAM is often the primary location for evidence of the attacker's tools, techniques, and current activities.

*   **Suitable process for securing (capturing) RAM (6 marks):**
    1.  **Prioritization (OOV):** RAM is highly volatile, so its capture must be prioritized before any action that might alter its state or power down the system.
    2.  **Minimize Interaction:** Interact with the live system as minimally as possible to avoid overwriting valuable data in RAM.
    3.  **Use Trusted Tools:** Employ validated live RAM acquisition tools (e.g., FTK Imager Lite, DumpIt, Belkasoft Live RAM Capturer, Volatility Framework's imagecopy plugin if running from a trusted USB). These tools are designed to copy the contents of physical memory to a file.
    4.  **Capture to External Sterile Media:** The RAM dump file should be saved directly to an external, forensically sterile storage device (e.g., a USB drive connected to the live server, or over a trusted network connection to a forensic collection server if direct connection is risky). Do not save the RAM dump to the server's own hard drive.
    5.  **Documentation:** Meticulously document the command used, the tool version, the exact time of capture, the output file name and location, and any observations made during the capture. Photograph the screen if relevant.
    6.  **Hashing:** Once the RAM dump file is created, calculate its cryptographic hash value and record it. This allows for integrity verification if the file is copied or moved later.
    7.  **Chain of Custody:** Document the RAM capture process and the resulting dump file in the Chain of Custody.

*(For a 25-mark question, ensure each point is well-elaborated with clear reasoning and detailed steps, emphasizing forensic principles like integrity and documentation throughout.)*

---

**3. Modern computers have moved away from traditional magnetic storage media, this change brings many challenges for forensic investigations. Discuss the similarities and differences between magnetic drive investigations and those involving SSD. How will these differences influence your approach to a forensic investigation? (25 marks)**

**Model Answer:**

The shift from traditional magnetic Hard Disk Drives (HDDs) to Solid State Drives (SSDs) presents significant challenges and necessitates adaptations in digital forensic investigations.

**Similarities between Magnetic Drive (HDD) and SSD Investigations (5 marks):**

Despite their differences, some fundamental aspects of forensic investigation remain similar:
1.  **Data Storage:** Both are non-volatile storage media designed to store the operating system, applications, and user data.
2.  **Forensic Imaging Goal:** The primary goal of acquiring a bit-for-bit forensic image to preserve evidence remains the same, though the methods might differ slightly.
3.  **Evidence Types:** Both can contain similar types of digital evidence: file system structures, user files, deleted data remnants, system artifacts, logs, etc.
4.  **Chain of Custody:** The requirement for meticulous chain of custody documentation applies equally to both HDD and SSD investigations.
5.  **Analysis Tools:** Many existing forensic analysis tools can process images from both HDDs and SSDs to analyze file systems and recover artifacts, although SSD-specific features are becoming more important.

**Differences between Magnetic Drive (HDD) and SSD Investigations (10 marks):**

| Feature                    | Magnetic Drive (HDD)                                         | Solid State Drive (SSD)                                      |
| :------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| **Storage Mechanism**      | Data stored magnetically on rotating platters with read/write heads. (1 mark) | Data stored in NAND flash memory chips using floating gate transistors; no moving parts. (1 mark) |
| **Data Deletion/Recovery** | Deleted data remains physically present until overwritten by new data. Recovery from unallocated space is often successful. (1 mark) | **TRIM Command & Garbage Collection:** OS informs SSD of deleted blocks, which the SSD controller can then internally erase during idle time. This makes deleted data recovery very difficult or impossible. (1 mark) |
| **Wear Leveling**          | Not a primary concern for data layout in the same way. Data tends to be more static once written. | Actively redistributes data across flash cells to evenly distribute wear and extend drive life. This means logical data might not correspond to a fixed physical location over time, and old data fragments can be scattered. (1 mark) |
| **Write Blocking**         | Hardware write-blockers are generally effective at preventing writes to the drive. (0.5 mark) | Hardware write-blockers may not always prevent internal SSD controller operations (like garbage collection or wear leveling) that could alter data, especially on live power-on. Software write-blocking or specialized SSD blockers might be needed. (0.5 mark) |
| **Performance/Access**     | Slower access times due to mechanical movement.              | Significantly faster access times.                           |
| **Data Remanence**         | Magnetic traces can sometimes remain even after overwriting (though difficult to recover). | Less data remanence after proper erasure/TRIM due to the nature of flash memory cells being erased in blocks. (1 mark) |
| **Self-Encryption (SED)**  | Less common as a default feature.                            | Increasingly common for SSDs to have built-in hardware encryption, always on, sometimes transparent to the user until a password is set. (1 mark) |
| **Firmware/Controller**    | Simpler controller logic.                                    | Complex controller (Flash Translation Layer - FTL) manages data placement, wear leveling, garbage collection, making the internal workings opaque to the OS and forensic tools. (1 mark) |
| **Volatility**             | Primarily non-volatile.                                      | Has volatile DRAM cache on the controller which can hold important transient data. (1 mark) |
| **Failure Modes**          | Often mechanical failure with potential for data recovery.   | Electronic failure; data recovery can be more complex or impossible if chips are damaged or controller fails catastrophically. (1 mark) |

**How these differences influence the approach to a forensic investigation (10 marks):**

1.  **Prioritization of Live Acquisition (2 marks):** Due to TRIM, garbage collection, and volatile controller caches on SSDs, live acquisition (capturing RAM and potentially a live image of the disk if decrypted) becomes even more critical than with HDDs if the system is found running. This is to capture data before the SSD's internal processes permanently erase it or before encryption locks it down on power-off.
2.  **Challenges in Deleted Data Recovery (2 marks):** Investigators must be aware that traditional unallocated space carving techniques may yield limited results on SSDs with active TRIM/GC. Focus may shift to other artifacts like file system journals, shadow copies, or application-level logs that might retain information about deleted files.
3.  **Understanding SSD-Specific Artifacts (1 mark):** Investigators need to understand the FTL, over-provisioned space, and how wear-leveling and garbage collection operate to interpret the data found and understand potential areas where remnants might exist (though often inaccessible without specialized techniques).
4.  **Write-Blocking Considerations (1 mark):** While still best practice, the effectiveness of traditional hardware write-blockers on SSDs needs careful consideration. Some SSDs might continue internal operations. Using a forensically sound boot environment that mounts the SSD as read-only at the OS level is crucial.
5.  **Encryption Challenges (2 marks):** If an SSD is self-encrypting or uses OS-level FDE (like BitLocker), obtaining the decryption key/password is paramount. If the system is live and decrypted, capturing RAM might yield keys. If off, decryption becomes a major hurdle.
6.  **Tool and Technique Adaptation (1 mark):** Forensic tools are evolving to better handle SSDs, including features to disable TRIM (if possible via specific interfaces before imaging) or to interpret SSD controller data (though this is often proprietary and difficult).
7.  **Time Sensitivity (1 mark):** The window of opportunity to recover certain types of data from SSDs (especially deleted data) can be much shorter than with HDDs due to the drive's internal management processes. Rapid response and acquisition are key.

In summary, while core forensic principles remain, investigating SSDs requires a greater emphasis on live data capture, an understanding of the drive's internal architecture and data management processes, and an awareness of the increased difficulty in recovering deleted data due to features like TRIM and garbage collection.

---

**4. The use of full drive encryption highlights the strength of modern cryptography, making the discovery of potential target files difficult. Another method to prevent forensic investigation is Steganography. Give a detailed comparison and discussion on the similarities and differences of these counter forensic methods. (20 marks)**

**Model Answer:**

Full Drive Encryption (FDE) and Steganography are both methods that can be used to protect data and can act as counter-forensic techniques, making it difficult for investigators to access or discover information. However, they operate on fundamentally different principles.

**Full Drive Encryption (FDE) (3 marks for definition/purpose):**
*   **Definition:** FDE is a cryptographic method that encrypts all data on a storage device (e.g., hard drive, SSD), including the operating system, application files, and user data.
*   **Purpose:** Its primary purpose is to ensure **confidentiality** of data at rest. If the storage device is lost, stolen, or seized, the data remains unreadable without the correct decryption key (e.g., password, passphrase, or recovery key).
*   **How it works as counter-forensic:** If an investigator seizes an FDE-protected drive that is powered off, they cannot access the plaintext data without the decryption key. This makes discovery of target files impossible unless the key is obtained or the encryption is brute-forced (which is often computationally infeasible for strong encryption).

**Steganography (3 marks for definition/purpose):**
*   **Definition:** Steganography is the art and science of concealing the very existence of a message or data within another, seemingly innocuous, file or medium (the "carrier" file, e.g., an image, audio file, or even network packet).
*   **Purpose:** Its primary purpose is to achieve **covert communication** or **data hiding** by making the hidden data undetectable to an observer who is not aware of its presence or the method used to hide it.
*   **How it works as counter-forensic:** Steganography aims to prevent an investigator from even suspecting that hidden data exists. If successful, the investigator might overlook the carrier file or not realize it contains concealed information, thus preventing the discovery of potential target files.

**Similarities between FDE and Steganography as Counter-Forensic Methods (5 marks):**

1.  **Goal of Obscuring Data:** Both methods aim to make sensitive information inaccessible or undiscoverable to unauthorized parties, including forensic investigators.
2.  **Reliance on Secrecy:** FDE relies on the secrecy of the decryption key. Effective steganography often relies on the secrecy of the steganographic method/tool and/or a stegokey (password) used to embed or extract the hidden data.
3.  **Can Hinder Investigation:** Both can significantly hinder or completely prevent a forensic investigation if the investigator cannot overcome the protection mechanism (i.e., decrypt the data or detect and extract the hidden message).
4.  **Intentional Use for Evasion:** Both can be intentionally employed by individuals wishing to evade detection or hide illicit activities.
5.  **Layering Possible:** They can be used in conjunction; for example, an encrypted file can be hidden using steganography within an image on an encrypted drive, creating multiple layers of protection.

**Differences between FDE and Steganography as Counter-Forensic Methods (9 marks):**

| Feature                       | Full Drive Encryption (FDE)                                  | Steganography                                                |
| :---------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| **Primary Objective**         | **Confidentiality** of data (protecting content). (1 mark)   | **Obscurity/Covertness** of communication (hiding the existence of data). (1 mark) |
| **Visibility of Protection**  | The fact that the drive is encrypted is often apparent (e.g., password prompt at boot, unreadable raw disk data). (1 mark) | The presence of hidden data is ideally undetectable; the carrier file should appear normal and innocuous. (1 mark) |
| **Impact on Data**            | Transforms the entire dataset into an unreadable (ciphertext) form. (1 mark) | The hidden message is embedded within a carrier file, subtly altering the carrier. The original data of the hidden message is not changed before embedding (though it might be encrypted first). (1 mark) |
| **Detection Method**          | Detection is usually straightforward (system prompts for key, or raw data is clearly encrypted). The challenge is decryption. (1 mark) | Detection (steganalysis) is the primary challenge; involves looking for statistical anomalies, tool signatures, or subtle alterations in the carrier file. (1 mark) |
| **Capacity**                  | Encrypts the entire volume of data on the drive. (0.5 mark)  | Limited by the capacity of the carrier file and the steganographic technique's ability to hide data without causing noticeable distortion. (0.5 mark) |
| **Tools Required for Access** | Decryption software/hardware and the correct key/password. (0.5 mark) | Steganalysis tools to detect, and then potentially the original steganography tool and stegokey to extract the hidden message. (0.5 mark) |
| **Legal Status of Use**       | Generally legal for personal data protection. Mandated in many corporate/government environments. (0.5 mark) | Use itself is not inherently illegal, but often associated with illicit activities due to its covert nature. Can raise suspicion. (0.5 mark) |

**Discussion:**
FDE is a widely accepted and often encouraged security measure for protecting data confidentiality. From a forensic perspective, if a drive is encrypted and powered off, and the key is unavailable, accessing the data is a major roadblock. Live acquisition before shutdown or obtaining the key (through legal means or suspect cooperation) are primary strategies.

Steganography, on the other hand, aims for "security through obscurity." Its success as a counter-forensic method depends on the investigator not detecting the hidden data. If detected, and if the hidden data is also encrypted, then the investigator faces a secondary challenge similar to FDE. Steganalysis techniques are constantly evolving to detect subtle changes introduced by steganographic tools.

Both methods pose significant challenges. FDE makes data unreadable, while steganography attempts to make it invisible. An investigator needs different skill sets and tools to tackle each: cryptanalysis and key recovery for FDE, and steganalysis for steganography. The choice of method by a user depends on their goal: if it's simply to protect data from unauthorized eyes, FDE is common. If it's to hide the fact that secret communication is even occurring, steganography is chosen.

---

### **Section B**

**Answer any Two out of Three questions listed.**

*(Model answers provided for all three for completeness.)*

---

**1. The ACPO guidelines outline the process that UK law enforcement follows for forensic operations, the guidelines contain 4 key principles. Outline each principle and give an example to demonstrate how this principle can be implemented. (10 marks)**

*(This question is identical to question B1 in the "PRACTICE" paper. Please refer to the model answer provided above for that question. The key is to clearly outline each of the four principles and provide a distinct, practical example for each, demonstrating understanding of its implementation.)*

---

**2. The UK Legislation ’Computer misuse act 1990’ outlines several offences directly related to forensic investigations,**
    *   **S1 Unauthorised Access To Computer Material,**
    *   **S2 Unauthorised Access With Intent to Commit Other Offence,**
    *   **S3 Unauthorised Acts with Intent to Impair Operation,**
    *   **S3A Making, Supplying or Obtaining Article for Use in S1 or S3 offences.**
**Give a brief description of each offence S1, S2, S3 and S3A, give an example of such an offence that a forensic investigator may encounter. (10 marks)**

*(This question is identical to question B2 in the "PRACTICE" paper. Please refer to the model answer provided above for that question. The key is to accurately describe each section and provide a relevant forensic scenario for each.)*

---

**3. The monitoring and logging of user activities have tangible benefits to a forensic investigator. Discuss these benefits and provide reasoning as to why this practice of excessive logging may or may not be ethical. (10 marks)**

*(This question is identical to question B3 in the "PRACTICE" paper. Please refer to the model answer provided above for that question. The key is to discuss both the forensic benefits and the ethical implications (pros and cons) of excessive logging, providing reasoned arguments.)*