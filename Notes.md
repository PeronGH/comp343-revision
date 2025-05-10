# COMP343 Computer Forensics - Exam Revision Notes

## Lecture 1: Forensic Computing

### What is Forensic Computing?
*   **Definition 1:** Application of investigation and analysis techniques to gather and preserve evidence from a particular computing device in a way that is suitable for presentation.
*   **Definition 2:** Building a clear and evidence-based report with regards to a computer system.

### Key Concepts
*   **IT Facilitation:** IT facilitates both the commission of crimes and the investigation into them.
*   **Internet as Arena:** The internet provides a major arena for new types of crime and offers means of potentially tracking criminal behavior.
*   **Two Main Themes of Forensics:**
    *   **Computer Forensics:** Focuses on the recovery and investigation of material found in digital devices, often in relation to computer crime.
    *   **Intrusion Forensics:** Focuses on identifying the source and method of unauthorized access or attacks on a system or network.

### Forensic Computing Process
Involves data:
1.  **Preservation:** Maintaining the integrity of the original evidence.
2.  **Identification:** Recognizing and determining what data is evidence.
3.  **Extraction:** Recovering the identified evidence.
4.  **Documentation:** Recording every step of the forensic process.
5.  **Interpretation:** Analyzing and drawing conclusions from the evidence.
*   Forensic computing is often considered more an "art" than a science due to the need for flexibility and interpretation, though specialists follow clear methodologies.

### Why Forensic Computing?
*   Not all computer misdeeds are criminal.
*   **Applications beyond criminal prosecution:**
    *   Determine root cause of an event to ensure no repeat.
    *   Identify responsibility.
    *   Internal investigation within an organization.
    *   Intelligence operations.
    *   Law enforcement.

### Global Impact of the Internet on Forensics
*   **Enhanced Interconnectedness:** Allows for rapid data discovery and sharing.
*   **Growing Scope:** Investigations can become global.
*   **Impact on Investigations:**
    *   **Clifford Stoll Example (1986):**
        *   Astronomer at LBNL tasked with resolving a 75-cent accounting error.
        *   Traced error to an unauthorized user (hacker from Germany) who exploited a vulnerability in GNU Emacs' movemail function.
        *   Monitored attacker via wiretap; hacker took encrypted password files, created early 'rainbow' tables.
        *   Demonstrated early network intrusion and the global nature of cybercrime.

### Human Behaviour and Cyber Crime
*   **Internet Users Distribution:** Statistics show global internet usage, highlighting the vast potential for online activity, both legitimate and illicit. (e.g., Asia 53.4%, Europe 14.3% in 2021).
*   **Cyber Concerns:**
    *   Paedophile activity and other abuses.
    *   Fraud (Phishing, Scam, Identity theft).
    *   Cyber warfare.
    *   Hate Crime, Harassment, Bullying, Stalking.
    *   Use of digital equipment for criminal activities (e.g., encrypted email/messaging like EncroChat/SkyCC).
    *   Monitoring and capture of network traffic for IDs, passwords.
    *   Hacking: Unauthorized access, disclosure, modification, destruction of resources.

### Cybercrime Classification (Not Mutually Exclusive)
*   **Computer as Target:** Crime targets the computer or its data (e.g., DDoS, malware damaging integrity/confidentiality/availability).
*   **Computer as Repository:** Computer stores information used or generated in the commission of a crime (e.g., storing illicit images, drug ledgers).
*   **Computer as Tool:** Computer is used as an instrument to commit a crime (e.g., using a computer for phishing, hacking other systems).

### Crime Examples
*   Child Pornography, Indecent solicitation of a child, Identity theft.
*   Criminal Threat, Computer Crimes (accessing, damaging, modifying, etc.), Unlawful Arranging Sale/Purchase of Controlled Substance.
*   Piracy Recordings, Conspiracy to Commit a Crime, Criminal Defamation.
*   Computer Trespass, Promoting Obscenity, Maliciously Circulating False Rumors.
*   Computer Password Disclosure, Eavesdropping, Breach of Privacy.
*   Assault, False Impersonation.

### Multiplicity of Crime
*   No "typical" computer crime. Examples:
    *   Demoted employee installing a time bomb.
    *   eBay fraud (payment received, goods not delivered).
    *   Ex-employee sending threatening emails.
    *   Law firm employee stealing trial plans.
    *   Website advertising fake IDs.
    *   Software piracy ring using a website.
    *   Hacker accessing bank records.

### What Cybercriminals Are After
*   **Personal Information:** Social security numbers, online payment logins, credit/debit card details, bank info, driver's licenses, loyalty accounts, diplomas, passports.
*   **Dark Web Prices (Examples):**
    *   Social Security Number: $1
    *   Online payment services login: $20-$200
    *   Credit/debit card with CVV: $5-$110 (Global $35, USA $17, UK $20)
    *   Cloned Mastercard with PIN: $25
    *   Stolen online banking logins ($2000+ on account): $120

### Cybercrime as a Service
*   **DDoS Attacks for Hire:**
    *   Unprotected website, 10-50k requests/sec, 1 hour: $10-$15
    *   Unprotected website, 10-50k requests/sec, 1 month: $800-$1,000
*   **Other Services:** Ransomware toolkits, Android banking trojans, credit cards, cloud service accounts, documents (passports, utility bills).

### Legal Considerations
*   **Search and Seizure:** Critical aspect of forensic investigations.
*   **Privacy Paradox:** Protecting privacy vs. solving computer-related crimes are often contradictory.
    *   **User Perspective:** Expectation of privacy.
    *   **Law Enforcement Perspective:** Need for access to investigate.
*   **Global Access Issues:** Banking, travel, email, phone data can cross borders, creating jurisdictional challenges.

### Challenges – Legal & Operational
*   **Legal Challenges:**
    *   Lack of boundaries on the Internet.
    *   Jurisdiction and applicable laws.
    *   Differences in crime classification and jurisprudence.
    *   Differences in legal systems: Accessing digital evidence, authority, human rights, ethics.
*   **Operational Challenges:**
    *   Technical and legal cooperation across countries.
    *   Harmonization of laws.
    *   Cooperative investigation.

### Protection from Cybercrime
*   **Prevent Cybercrime:**
    *   **Protection mechanisms in infrastructure:** Access controls, authorization.
        *   Leads to Data/Information Confidentiality, Privacy.
    *   **Best Practices for safe use:** Regulations, Standards.
    *   **Human Factor:** Conformance and behavior.
*   **Deter Criminal Activity:**
    *   **Penalties, Punishments:**
        *   Leads to Investigation and Forensics through Laws, Jurisprudence, Judiciary, Constabulary, Penitentiary.
    *   This forms part of **Regulations & Deterrents**.

### Computer Security (CompSec) vs. Forensic Computing
*   **Computer Security:** Preserve a system as it is meant to be (as per security policies).
    *   **Goals (CIA Triad):**
        *   **Confidentiality:** Preventing unauthorized disclosure of information.
        *   **Integrity:** Ensuring data is accurate and unaltered.
        *   **Availability:** Ensuring systems and data are accessible when needed.
    *   **Enforced through:** Preventative, Mitigating, Transferring, Recovery countermeasures.
*   **Forensic Computing (esp. Intrusion Forensics):** Set out to explain how a policy became violated.
*   **Discrepancy exists due to:** Historic reasons, security policies, technology changes.
*   **Relationship:** Complementary but distinct processes.
*   **Overlap & Conflict:**
    *   Degree of overlap in raw material used.
    *   Different, sometimes opposing aims (Security tries to prevent, Forensics investigates after an event).
    *   Security functions tend to implement minimal logging (to save resources), which can hinder forensics.
    *   Security countermeasures (e.g., encryption, data wiping) may work against forensic computing.

### Conclusion of Lecture 1
*   Forensic computing searches for electronic evidence of crime.
*   Computers can be targets, repositories, or tools for crime.
*   User and law enforcement perspectives on privacy and access differ.
*   Computer security and forensic computing are complementary but distinct.

## Lecture 2: Cyber Forensics in Practice

### Overview
*   Focus on forensic computing in law enforcement and national security.
*   Topics: CFSAP model, ACPO Guide, UK legislations, national security, link analysis.

### Scenarios in Computer Crime
*   **Early Cases:** Forensic examinations to recover evidence (computer as repository/facilitator).
*   **Advent of Networking:** Computers became targets themselves (e.g., hacking).

### CFSAP Model (Computer Forensics – Secure, Analyse, Present)
*   Combines four key elements:
    1.  **Identification:** Recognizing potential evidence.
    2.  **Preservation:** Protecting evidence from alteration or destruction.
    3.  **Analysis:** Examining and interpreting the evidence.
    4.  **Presentation:** Reporting the findings in a clear and understandable manner.
*   Provides a high-level view of procedures.
*   **Three distinct steps (as per diagram):**
    1.  **Secure:** Identify sources of digital evidence, Preserve digital evidence.
    2.  **Analyse:** Forensic analysis of digital evidence (Extract, Process, Interpret).
    3.  **Present:** Presentation of digital evidence (expert opinion and testimony).
    *   *Feedback loop from Analysis to Preserve if new evidence is found or re-preservation is needed.*

### In Practice: Reconstructing the Digital Environment
*   **FBI Handbook of Forensic Services - Types of Computer Examinations/Recovery Processes:**
    *   Content, Comparison, Transaction, Extraction, Deleted data files, Format conversion, Keyword searching, Passwords, Limited source code, Storage media.

### Principles of Evidence
Computer evidence must meet the same legal requirements as any other form of evidence. Applicable in legal and non-legal (commercial/corporate) investigations.
1.  **Admissible:** Evidence must be usable in court, conforming to legal rules.
2.  **Authentic:** Evidence must be proven to be what it purports to be; genuine and unaltered.
3.  **Complete:** Evidence should tell the whole story, not just a part that favors one side.
4.  **Reliable:** Evidence must be dependable and consistent; the methods used to obtain it must be sound.
5.  **Believable:** Evidence must be understandable and convincing to the trier of fact (judge or jury).

### Forensic Principles and Methodologies: ACPO Guide
*   **Association of Chief Police Officers (ACPO) "Good Practices Guide for Computer Based Evidence":** Predominant model in the UK.
*   Accepted current standard of practice for digital evidence.
*   Non-compliance doesn't automatically mean evidence is rejected.
*   Adapted by the International Organisation for Computer Evidence (IOCE).
*   Examiners must be trained for examination and court testimony.
*   **ACPO Guide Contents:**
    *   Principles
    *   Attending crime scenes
    *   Investigating personnel
    *   Evidence recovery
    *   Control of paedophile images
    *   External consulting witnesses
    *   Disclosure
    *   Handling mobile phones and PDAs
    *   Contact with victims

### ACPO Guide – Principles
1.  **Principle 1:** No action taken by law enforcement agencies or their agents should change data on a computer or storage media which might subsequently be relied on in court.
2.  **Principle 2:** In exceptional circumstances, where a person finds it necessary to access original data, that person must be competent to do so and be able to give evidence explaining the relevance and implications of their actions.
3.  **Principle 3:** An audit trail or other record of all processes applied to computer-based evidence should be created and preserved. An independent third party should be able to examine those processes and achieve the same results.
4.  **Principle 4:** The person in charge of the investigation (the case officer) has overall responsibility for ensuring that the law and these principles are adhered to.

### ACPO Guide – Investigating Personnel
*   **Pre-search:** Gather information about type, location, connection of computer systems.
*   **Briefing:** All personnel must be adequately briefed.
*   **Search preparation:** Plan the search.
*   **Toolkit:** Essential tools for evidence collection.
*   **Records to be kept:** Sketch map, persons present, computer details (make, model, serial), display details, etc.
*   **Interviews:** Conduct interviews as needed.
*   **Specialists:** Consider inviting trained personnel or independent specialists.

### ACPO Guide – Paedophile Images
*   Evidence subject to classification (minimum: Confidential).
*   Possession of paedophile material is an offense.
*   Enquiry will contain personal information, possibly victim identities.
*   Images seized and technical report should be on encrypted, password-controlled disk.
*   Printouts only in exceptional circumstances, maintained with security level.

### Government Security Classifications
*   **GPMS (Government Protected Marking Scheme - older):** Top Secret, Secret, Confidential, Restricted, Protect, NPM (Not Protectively Marked).
*   **GSC (Government Security Classifications - current):** Top Secret, Secret, Official.
    *   **OFFICIAL-SENSITIVE:** Descriptor within OFFICIAL. Requires safeguarding against unwarranted disclosure, more rigorous handling. Applied to reinforce 'need to know'. Damaging consequences if lost/stolen/published. Use by exception.

### Classification Scales for Illicit Images
*   **COPINE Scale:** Originally for therapeutic purposes, distinguishes child erotica from child pornography. Developed by University of Cork & London Met Police. Ten-level typology based on website/newsgroup images.
*   **Sexual Offences Definitive Guideline Categories:**
    *   **Category A:** Penile penetration, activity with animal, or sadism.
    *   **Category B:** Non-penile penetration sexual activity.
    *   **Category C:** Other indecent images not in A or B.
*   **SAP Scale (Simplified Scale):**
    1.  Nudity or erotic posing, no sexual activity.
    2.  Sexual activity between children, or solo masturbation by a child.
    3.  Non-penile penetration sexual activity between adult(s) and child(ren).
    4.  Penile penetration sexual activity between child(ren) and adult(s).
    5.  Sadism or bestiality.
*   **Europol Trace an Object:** Example of using public help to identify locations from images in child abuse cases.

### UK Legislations
*   **Computer Misuse Act 1990:**
    *   S1: Unauthorised access to computer material.
    *   S2: Unauthorised access with intent to commit or facilitate commission of further offences.
    *   S3: Unauthorised acts with intent to impair, or with recklessness as to impairing, operation of computer, etc. (e.g., modification of material).
    *   S3ZA: Unauthorised acts causing, or creating risk of, serious damage.
    *   S3A: Making, supplying or obtaining articles for use in S1, S3 or S3ZA offences.
*   **Police and Criminal Evidence Act 1984 (PACE):**
    *   General power of seizure.
    *   Power for requiring information held on a computer to be handed over.
*   **Criminal Justice and Police Act 2001:**
    *   Describes power to seize items if believed to contain lawfully seizable items.
*   **Electronic Communications Act 2000:**
    *   Electronic Signatures Regulations 2002.
    *   Electronic Commerce Regulations 2002.
    *   Three parts: Regulation of Cryptography Service Providers, Facilitation of electronic commerce/data storage, Telecommunications licences.

### Link Analysis
*   Important in law enforcement, major focus in national security.
*   "Extracting and reassembling fragments of seemingly unrelated needles located in many different haystacks."
*   Challenging due to complex patterns.
*   **Problematic in criminal investigations due to:**
    *   Multitude of devices.
    *   Need to specify devices/files in warrants.
    *   Admissible court evidence relies on concrete data (difficult to maintain assertions from link analysis alone).
    *   Cheap processing power (e.g., one-time use phones).
    *   Criminals using "not using technology" as a countermeasure.
*   Less problematic for intelligence-led/commercial internal investigations.
*   **Applications:**
    *   Indicate where to focus an investigation.
    *   Infer stateful knowledge about "players" (not statistical).
    *   Enhance with network diagrams (communications analysis/network security techniques applied to softer side).

### Forensic Challenges and Obstacles (Reiteration)
*   Evidence readily altered/deleted.
*   Evidence invisibly/undetectably altered.
*   Evidence can appear copied while undergoing alteration.
*   In transit, can share transport pipeline with other data.
*   Stored in different format than when printed/displayed.
*   Difficult for layman to understand.

## Lecture 3: Storage Media

### Aims
*   Basics of hard drives and storage media.
*   Nature of digital evidence, generic computer model, hard drive architecture, partitions, filesystem, deleted data analysis.

### Nature of Digital Evidence
*   Distinguishes hypothesis from groundless assertion.
*   Reliability and integrity are key for admissibility.
*   **Challenges:**
    *   Too many potential suspects.
    *   Identifying the crime.
    *   Too much potential evidence.
    *   Easily contaminated; contaminating some may contaminate all.
*   Correct "search and seizure" procedures are vital.
*   Investigations increasingly cross geopolitical borders (Link Analysis).

### Generic Computer Model / Components of Computer Architecture
*   **Hardware Layer:** Physical components.
*   **Operating System (OS):** Manages hardware and software resources (e.g., Windows, macOS, Linux).
*   **Middleware:** Software that provides services to applications beyond those available from the OS (e.g., database management systems, cryptographic services).
*   **Applications:** Software used by end-users (e.g., email clients, browsers, office suites).
*   **Core Components:**
    *   Input unit and associated peripherals (keyboard, mouse).
    *   Output unit and associated peripherals (monitor, printer).
    *   Storage unit/memory (HDD, SSD, RAM).
    *   Central Processing Unit (CPU).
    *   Operating System (OS).
*   **State Information during execution is distributed across:**
    *   **CPU:** Executing operations, registers show current operation.
    *   **Dynamic Storage (RAM):** Fragments of OS, running apps, temporary data.
    *   **Backup/Permanent Store (HDD, SSD, Tapes, CDs):** Persistent data, files retained between sessions.
    *   **Network:** Components record network data (data sent, connections, router info).

### Drive File Structure
*   Layered like a Matryoshka doll:
    *   **Hard Drive -> Partition -> File System -> File Record -> Field**

### Magnetic Hard Drive Architecture
*   **Platters:** Made of ceramic/aluminum, store data magnetically. Multiple platters stacked.
    *   Need to keep cool to prevent expansion/contraction.
    *   High capacity (e.g., 2.2TB per platter).
*   **Read/Write Heads:** Move over platters via an actuator arm to read/write data.
*   **Tracks:** Concentric circles on platters where data is stored.
*   **Sectors:** Smallest physical storage unit on a platter (typically 512 bytes or 4KB). Bytes addressed by position within sector.
*   **Cylinder:** Set of tracks at the same head position on all platters. Important for data access speed and defragmentation.
*   **Data Encoding:** Magnetic field lines represent binary data (0s and 1s) by changes in magnetic orientation (e.g., R = reverse, N = no reverse).

### Solid State Drives (SSD) Architecture
*   **Components:**
    *   **Controller:** Manages data storage and retrieval.
    *   **SATA Interface:** Connection to the motherboard.
    *   **NAND Flash Memory:** Chips where data is stored.
    *   **SSD PCB (Printed Circuit Board):** Connects all components.
*   **NAND Flash Memory:**
    *   Uses NAND logic gates ("not and").
    *   Cells arranged in pages, pages in blocks.
    *   Data stored by trapping electrons in floating gates of transistors.
    *   Reading involves checking conductivity of cells.

### Conceptual Storage & Partitions
*   **Partition:** A logical division of a hard drive.
*   Hard drive can be configured into one or more partitions.
*   OS references partitions separately.
*   Allows a single hard drive to appear as multiple individual drives.
*   **Uses:** Installing multiple OSs (e.g., Windows and Ubuntu).
*   **Partition Table:** Stores information about partitions (location, size, type). Typically in the MBR or GPT.
*   **Boot Partition:** Partition that takes control when the computer is switched on; contains OS boot files.
*   **Partitioning Tools:**
    *   GParted (Linux)
    *   Disk Management (Windows)
    *   Partition-Magic (Symantec - older)
    *   Partinfo (free)
    *   `fdisk` (command-line)
*   **Analysis:** Prior to analyzing, get configuration info. Tools like Partinfo can display partition info without allowing changes.

### Filesystem (FS) Data
*   A set of data objects referenced and manipulated externally.
*   OS stores files in a filesystem, allowing access by name, date, location, etc.
*   Contains index(es) or table(s) with unique identifiers for each object (file) and location information.
*   Enables access to objects when requested.
*   Vary in sophistication.

### Filesystem Types
*   **Windows File Allocation Table (FAT):**
    *   Originally for floppy disks, used by MS-DOS.
    *   Flat table listing files and their locations.
    *   Versions: FAT12, FAT16, FAT32.
*   **UNIX Filesystems (e.g., ext2, ext3, ext4, UFS):**
    *   Uses two main forms of tables:
        *   **inode table:** Contains metadata about files (permissions, owner, size, pointers to data blocks). Each file has an inode.
        *   **Filename table (directory):** Maps filenames to inode numbers.
*   **Windows NT File System (NTFS):**
    *   Similar to UNIX file systems in concept (uses Master File Table - MFT, analogous to inode table).
    *   More robust, supports larger files/partitions, security features, journaling.
*   **Modern Drive Allocation Types:**
    *   FAT (FAT32)
    *   NTFS
    *   exFAT (Extended File Allocation Table): For flash drives, larger file/partition sizes than FAT32.
    *   HFS+ (Hierarchical File System Plus): For macOS.
    *   EXT (Extended File System - ext2, ext3, ext4): For Linux.

### Detailed Filesystem Properties
*   **NTFS:**
    *   Partitions up to 16EB. Files as large as partition.
    *   Occasionally fragments. Read/writable by Windows/Linux; read-only by macOS (default, NTFS-3G for write).
    *   Recommended for modern Windows systems.
*   **FAT (FAT32):**
    *   Partitions up to 2TB (Windows formats up to 32GB as FAT32). Files up to 4GB.
    *   Over-fragments, file corruption issues.
    *   Used for small capacity, portable devices. Not recommended for modern hard disks unless old OS.
*   **exFAT:**
    *   Partitions up to 512TiB (recommended max). Files up to 16EiB.
    *   Not compatible with Linux/Unix by default until Linux 5.4 (released in 2019). Defragment often. Cannot pre-allocate disk space.
    *   Good for large flash drives, media devices.
*   **HFS+ (Mac OS Extended):**
    *   Max volume 8EB. Files as large as partition.
    *   Windows users can read but not write by default. Linux drivers available.
*   **ext4 (Linux):**
    *   Volumes up to 1EiB. 16TB max file size.
    *   Red Hat recommends XFS for volumes >100TB.
    *   Backwards compatible with ext2/ext3. Can pre-allocate disk space.
    *   Not readable by Windows/macOS by default.

### Filesystem Terminology
*   **Mounting:** Attaching an additional filesystem to the currently accessible filesystem of a computer.
*   **Filesystem (Directory Tree):** A hierarchy of directories used to organize files on storage media.
*   **File Format:** A specially coded template written on media, defining how data is structured and read.
*   **Mount Point:** A locally available link (e.g., drive letter in Windows, directory in Unix/Linux) through which an external device's filesystem is accessed after mounting.

### Data Sizes in Filesystems
*   **Blocks (UNIX):** Specifically sized units of data. In many Unix systems, 1000 blocks ≈ 1MB.
*   **Clusters (Windows):** Groups of sectors. Default max cluster size for NTFS (NT 4.0+) is 4KB.

### Slack Space
*   Excess capacity in the last block or cluster of a file; wasted space.
*   **Types:**
    *   **File Slack:** Space between the logical end of the file (EOF) and the physical end of the last cluster allocated to the file.
    *   **RAM Slack:** Part of file slack from the logical EOF to the end of the sector. May contain data from RAM.
    *   **Drive Slack (Unallocated Space within Cluster):** If the last sector in a cluster is not fully used by the file, the remaining space in that sector, plus any subsequent unused sectors in that cluster, constitute drive slack (often this term is used interchangeably with file slack or refers to the entirety of the unused portion of the last cluster).
*   OS usually has unallocated space containing some data.
*   Every file not an even multiple of block/cluster size has associated slack space.
*   Average slack space per file is about one-half the block/cluster size.
*   Larger block/cluster size = more potential slack space.
*   **Forensic Significance:** Slack space can contain remnants of previously deleted files or other data.
    *   OS does not allow direct access to slack space.
    *   Forensic imaging (bit-for-bit copy) is required to analyze slack space.

### Analyzing Partitions
*   Identify location, type, size, and number of partitions.
*   Ensure total space of partitions adds up to drive size (note: vendor 1KB=1000 bytes, OS 1KB=1024 bytes).
*   **Unallocated Space:** Can contain anything previously written to the hard drive.
*   **Virtual Memory (Swap Space):** A file that grows and shrinks as needed, can contain all types of sensitive data.

### Erasing a Hard Drive
*   **Magnetic Drives:**
    *   "Wiping" may leave feint images (magnetic residue).
    *   Electron microscopes can potentially recover overwritten tracks.
    *   Overwrite patterns can sometimes be reversed; truly random data makes recovery very difficult.
*   **SSDs:**
    *   **TRIM/UNMAP Command:** OS informs SSD which blocks are no longer in use and can be erased internally by the drive's garbage collection.
    *   **Wear Leveling:** SSDs write to different blocks to distribute wear, leaving old data in now-unmapped blocks. This data might be recoverable until garbage collection erases it.
    *   **ATA Secure Erase (SE):** Command to wipe entire drive contents at hardware level. If implemented correctly, makes data unrecoverable.
    *   **SSD Recovery:**
        *   "If it's running, don't turn it off. If it's off, don't turn it on." (Volatile data in controller/DRAM cache can be lost).
        *   **De-chipping:** Removing flash chips for direct analysis. Expensive, difficult, damaging.

## Lecture 4: Current Forensic Practice, Evidence Handling

### Operational Model of Forensic Computing
1.  **Collection:** Search, recognition, collection, documentation of evidence.
    *   Can involve real-time and stored information.
    *   **Small Scale Collection:** Imaging on-site or in lab.
        *   **Physical Imaging:** Bit-by-bit, sector-by-sector, or bit-stream image (exact copy of entire drive/partition).
        *   **Logical Imaging:** File-by-file imaging (copies only active files).
    *   **'Go Bag' Toolkit:**
        *   Hardware: Laptop, write-blockers, various cables, storage devices.
        *   Software: Imaging tools, fdisk, write-blocking software, analysis tools.
        *   Accessories: Notebook, pens, evidence bags, labels, camera, evidence log.
2.  **Examination:** Applying tools and techniques to analyze the collected data.
3.  **Analysis:** Interpreting the results of the examination to draw conclusions.
4.  **Reporting:** Documenting the findings in a clear, concise, and objective manner.
    *   Path: Media -> Data -> Information -> Evidence.

### Integrity of Investigation Aspects
*   **Collection:** Proper methods to gather evidence.
*   **Chain of Custody (ACPO Principle 4):** Documenting the chronological possession and handling of evidence from seizure to court. Critical for authenticity.
*   **Authentication:** Verifying that the evidence is genuine and unaltered.
    *   **File Imaging and Authentication:**
        *   Identify files needed.
        *   Duplicate (analysis on duplicate).
        *   Authenticate original and copies using checksums (e.g., MD5, SHA-1, SHA-256) or one-way hash functions.
*   **Recovery:** Retrieving deleted or hidden data.
*   **Verify:** Using hash functions (message digests) or checksums to prove data integrity.

### Write Blocking
*   **Central Requirement:** Original evidence must NOT be modified.
*   Investigator follows procedures to prevent any program from modifying disk contents.
*   **Strategies (Layered Defense):**
    1.  **Hardware Jumper:** Set disk to read-only if possible (older IDE drives).
    2.  **Trusted OS/Software:** Use a forensic boot disk/OS known not to write to connected drives unless explicitly instructed.
    3.  **Hard Disk Write Block Tool (Hardware or Software):** Intercepts write commands to the protected disk.
        *   **NIST Specification:** Shall not allow protected disk to be changed; shall not prevent obtaining info; shall not prevent changes to unprotected disks.
        *   **Forensic Disk Controller:** Hardware write-blocker example.

### Analysing the Evidence
*   **Logical Analysis (File-by-File Analysis):**
    *   Analyzes disk files at the application level.
    *   More convenient/efficient than purely physical analysis for understanding file content.
    *   Investigates file contents using the application that produced it or an application-specific tool.
    *   **Advantages:**
        *   Overcomes shortcomings of physical-only analysis (e.g., finding strings split across sectors).
        *   Provides high-level/semantic view of file contents.
*   **Time-lining:**
    *   Associating timestamps with each event or data item. Crucial for investigation.
    *   Correlate file last access/written times with other information.
    *   Build a time graph of activities; times must be consistent with non-computer crime events.
    *   Example: Access network (log) -> Pay for service (bill) -> Download image (file created) -> View image (last access) -> Change image (last write) -> Forward image (email log).

### ACPO Guide Recommendations for Search and Seizure
1.  **Preparation:** Review court order scope, plan for materials to be seized.
2.  **At the Site:**
    *   Take notes (cabling, etc.), photograph everything (especially screen if on).
    *   Document all actions.
3.  **Shut Down:**
    *   **If Off:** Accepted wisdom is to leave it off.
    *   **If On:**
        *   Record display. Note time.
        *   Circumstances may allow looking at running processes (live forensics).
        *   MS shutdown: disconnect power cord. UNIX: safe power down.
4.  **Seizure:**
    *   Appropriate labelling and packaging.
    *   Document all actions.
5.  **Imaging (Lab or Site):**
    *   Boot to known, trusted OS.
    *   Ensure write-blocking is in place.
    *   Image and authenticate disks/files.
    *   Document all actions.
6.  **Physical Analysis:** Sector-by-sector analysis of disk image for hidden/accidental residues, suspicious structures. Document.
7.  **Logical Analysis:** Boot to OS supporting seized disk filesystem, file-by-file analysis for keywords, metadata (timestamps). Document.

### Email Headers
*   Provide information about email origin and route.
*   **Full Headers are Important for Investigators:**
    *   Originating ISP (X-Originating-IP).
    *   Route taken by email (Received: lines).
*   **Key Information in Headers:**
    *   Return path
    *   Recipient's email address
    *   Type of sending email service
    *   IP address of sending server(s)
    *   Name of email server(s)
    *   Unique message number (Message-ID)
    *   Date and time email was sent/received at various hops
    *   Attachment file information (MIME details)
*   **IP Lookup Tools:** `infosniper.net`, `whatismyipaddress.com`, `mxtoolbox.com` (DNS lookup).

## Lecture 5: Data Hiding: Steganography, Steganalysis, Cryptanalysis

### Steganography
*   **Definition:** Greek for "covered writing." The art and science of hiding a message within another message or object (carrier file) so that the hidden message is not apparent.
*   **History:** Used for ~2500 years in military, diplomatic, personal, IP applications.
*   **Purpose:** Conceal the existence of communication.
*   **Modern Digital Steganography:**
    *   Data is often encrypted first, then inserted/hidden using an algorithm that may add/modify carrier file contents.
    *   Techniques: Appending data, dispersing throughout the file, LSB modification.
    *   Patterns should appear normal.
*   **Tools:** DarkCryptTC, OpenPuff, StegoShare, StegFS.
*   **Carrier Files:** BMP, JPEG, GIF, WAV, MP3, TXT, HTML, EXE, DLL, NTFS streams.
    *   Carrier is typically large, hidden message is smaller.
*   **Kerckhoffs’ Principle Analogy:** Security should rely on the secrecy of the stegokey, not the algorithm. If cover medium is exposed, comparison reveals changes.
*   **Transform Domain Techniques:** Use algorithms/coefficients from image processing to hide info in significant areas, more robust than LSB. May require original image for extraction.

### Steganalysis
*   **Definition:** The art and science of detecting hidden messages (steganography).
    *   Focuses on detection, not necessarily extraction (though identification of tool can lead to extraction).
*   **Importance for Investigation:**
    *   Identify tools used, potentially extract original message.
    *   Examine deleted image files, program registry leftovers.
*   **Common Hiding Techniques to Detect:**
    *   **Appended to a file:** Data added at the end.
    *   **Hidden in unused header portion:** Near beginning of file.
    *   **Dispersed via algorithm:** Spread throughout the file.
        *   **LSB (Least Significant Bit) Modification:** Altering the LSB of pixels in images or samples in audio. (e.g., changing binary `11111111` (255) to `11111110` (254) makes little visual/audible difference).
        *   **Other:** Masking, transform domain.
*   **Methods of Detection:**
    *   **Visual Detection:** (Images - JPEG, BMP, GIF) Look for unusual patterns, distortions, pixelation.
    *   **Audible Detection:** (Audio - WAV, MPEG) Listen for noise or anomalies.
    *   **Statistical Detection:**
        *   Changes in LSB patterns.
        *   **Histogram Analysis:** Compare color/pixel value distribution of suspect file with known clean files or expected distributions. Stego can alter histograms.
    *   **Structural Detection:**
        *   View file properties/contents: size difference, date/time modification, content modifications.
        *   **Checksum/Hash Comparison:** If original is available, compare hashes.
    *   **Signature Analysis:** Some stego tools leave identifiable patterns or signatures in the carrier file (e.g., Hiderman's "CDN" marker).
*   **Steganalysis Tools:**
    *   **WinHex:** Hex editor for manual inspection, comparison, string searches.
    *   **StegSpy:** Signature identification program (detects tools like JPHide, Hiderman).
*   **Goal:** Accuracy, consistency, minimize false-positives.

### Steganalysis meets Cryptanalysis
*   **Cryptanalysis:** The study of ciphertext, ciphers, and cryptosystems with the aim of finding weaknesses and extracting plaintext without knowing the key.
*   **Relationship:**
    *   Steganography hides the message's existence; Cryptography encrypts the message's content.
    *   Many stego tools also encrypt the hidden message.
*   **Process:**
    1.  **Identify steganography program used** (via steganalysis - signatures, patterns).
    2.  **Identify and crack the algorithm** (if custom or weak).
    3.  **Reveal or crack the password, seed, or secret key** used for steganography/encryption.
        *   **Password Guessing/Dictionary Attacks:** Tools like Stegbreak.
        *   **Brute Force:** Try all possible keys/passwords.
        *   **Reverse Engineering:** Analyze the stego program itself.
*   **Common Encryption in Stego:** LSB modification, password-masked contents, algorithms based on secret keys, passwords, or random seeds hidden elsewhere.

### Anti-Forensics
*   Techniques used to frustrate forensic investigations.
*   **Best Practices for Using Steganography (from an anti-forensics perspective):**
    *   Use a strong, unique password (different from OS password).
    *   Securely delete the original message after embedding.
    *   Remove the steganography program or run it from a live CD/USB.
    *   Use **Alternate Data Streams (ADS)**.
*   **Alternate Data Streams (ADS):**
    *   A feature of NTFS (New Technology File System).
    *   Allows multiple "streams" of data to be associated with a single file, where the primary stream is the normal file content.
    *   ADS are hidden from Windows Explorer and standard `dir` commands.
    *   Can hide files, directories, malware, steganography.
    *   Example: Store a 5MB .zip file in the ADS of a 1K text file; Explorer still shows 1K.
    *   Malware uses ADS to hide components after infection (ADS data is often lost during browser/FTP downloads, so not ideal for initial distribution).
    *   **Tools for Detecting ADS:** LNS (List NTFS Streams), LADS (List Alternate Data Streams), NTFS ADS Check.
*   **Anti-Forensics Investigation Steps (if steganized file found):**
    *   Look for steganography programs on the system.
    *   Leverage other OS/application passwords found.
    *   Look for physical hints (notes, diaries with passwords).
    *   Refer to guides like "Electronic Crime Scene Investigation – A Guide for First Responders, U.S. Dept of Justice".

## Lecture 6: Reporting Results of Cyber Forensics Investigations

### Importance of Reports
*   Communicate investigation results, including expert opinion.
*   Courts often require expert witnesses to submit written reports.
*   Reports must specify fees and list other cases testified in.
*   **Deposition Banks:** Store previous testimonies of expert witnesses (can be used to check for consistency or impeachment).

### Limiting a Report to Specifics
*   Start with the job mission or goal (e.g., find info on X, recover Y documents, recover Z file types).
*   Identify audience and purpose before writing.

### Logical Flow of a Report
1.  This is what I was asked to do (Scope/Objective).
2.  This is why I am qualified to do it (Examiner's qualifications).
3.  This is what I did (Methodology).
4.  This is what I found (Findings).
5.  These are my opinions/conclusions.

### Types of Reports
*   **Examination Plan:** Outlines questions attorney might ask, helps guide testimony, clarifies technical terms.
*   **Verbal Report:**
    *   Less structured.
    *   Attorneys may prefer as they are often not discoverable (until formalized).
    *   **Preliminary Report:** Addresses areas of investigation yet to be completed (tests, interrogatories, document production, depositions).
*   **Written Report:**
    *   **Affidavit:** Sworn statement made under oath.
    *   **Declaration:** Similar to affidavit but not necessarily sworn before an official.
    *   Limit what you write, pay attention to details, include thorough documentation.
    *   Subject to discovery by opposing attorney; considered high-risk.
    *   **Spoliation:** Destroying a preliminary report could be considered destroying/concealing evidence.

### Guidelines for Writing Reports
*   **Hypothetical Questions:** Based on factual evidence; less favored today but can guide/support opinion. Can be abused if overly complex.
*   **Opinions:** Must be based on expert knowledge and experience.
*   **Four Conditions for Expert Testimony (Opinion/Conclusion):**
    1.  Opinion depends on special knowledge/skills.
    2.  Expert must qualify as a true expert.
    3.  Expert must testify to a certain degree of certainty.
    4.  Expert must describe facts on which opinions are based or testify to a hypothetical question.

### Report Structure
*   Abstract
*   Table of Contents
*   Body of Report
*   Conclusion
*   References
*   Glossary
*   Acknowledgements
*   Appendixes

### Writing Reports Clearly
*   **Consider:** Communicative quality, ideas/organization, grammar/vocabulary, punctuation/spelling.
*   Lay out ideas logically, build arguments piece by piece.
*   Group related ideas/sentences into paragraphs, then sections.
*   Avoid jargon, slang, colloquial terms; define technical terms for the audience.
*   Use natural language, avoid repetition/vague language.
*   Be precise and specific. Use active voice.
*   Avoid presenting too many details and personal observations (stick to facts and relevant findings).

### Designing Layout and Presentation
*   **Numbering:**
    *   **Decimal Numbering:** (1.0, 1.1, 1.1.1) Divides material, easy to scan.
    *   **Legal-Sequential Numbering:** (I, A, 1, a) Used in pleadings.
*   **Supporting Material:** Figures, tables, data, equations to tell the story.
*   **Consistent Formatting.**
*   **Explain Examination/Data Collection Methods:** How the problem was studied.
*   **Include Calculations:** E.g., specify hashing algorithms used.
*   **Provide for Uncertainty and Error Analysis:** Protects credibility.
*   **Explain Results and Conclusions:** Use subheadings, save broad generalizations for conclusion.
*   **References:** Cite sources (e.g., author-year).
*   **Appendixes:** Raw data, figures not in body, anticipated exhibits.

### Example Report Format Sections
*   **Executive Summary:** Background, requirement for investigation, short description, details, pointers.
*   **Objectives:** Tasks planned, undertaken, method, status.
*   **Computer Evidence Analyzed:** Evidence tag numbers, description, media serial numbers, interpretations.
*   **Relevant Findings:** Summary of evidence of probative value.
*   **Supporting Details:** In-depth analysis, table of vital files, string search results, emails/URLs reviewed, charts, illustrations.
*   **Investigative Leads:** Action items for further discovery (critical for law enforcement).
*   **Additional Subsections (Client-dependent):**
    *   **Attacker Methodology:** For intrusion cases, how attacks were done, log analysis.
    *   **User Applications:** Relevant installed applications.
    *   **Internet Activity:** Browsing history, downloads, unallocated space, secure delete programs.
    *   **Recommendations:** For client to be more prepared for future incidents.

### Sources of Information for Reports
*   Personal observations (of the examiner during the process).
*   Applications (logs, data generated by them).
*   Network/host devices (firewall logs, router logs, system logs).
*   Forensic tools (output, reports generated by tools).

### Audience for Reports
*   Executives, Information Technology personnel, Legal teams, Marketing, Regulators, Law enforcement. (Tailor language and detail accordingly).

### Key Info to Include in a Forensics Report
*   Examiner bio/background/CV.
*   Tools utilized (hardware and software, versions).
*   Evidence items (description, chain of custody).
*   Forensic analysis performed (step-by-step methodology).
*   Tool output (relevant excerpts, logs, reports from tools).

### Generating Report Findings with Forensic Software Tools
*   Tools like FTK, EnCase, AXIOM, Autopsy can generate reports.
*   **Formats:** Plaintext, Word Processor (e.g., RTF, DOCX), HTML.
*   **Using FTK/EnCase/AXIOM:** Create case, add evidence, analyze (image files, encrypted files, keywords), create bookmarks, generate report from bookmarks.
*   **Using Autopsy:** Open case, Tools -> Generate Report, select HTML, export results.

### Types of Witness
*   **Technical Witness:** Testifies only on facts experienced or observed directly. Offers no opinions.
*   **Expert Witness:** A third party whose specialized knowledge, skills, experience, training, or education allows them to offer opinions or draw conclusions to assist the trier of fact. Must be qualified by the court.

## Lecture 7: Advanced Digital Forensics Practice

### Timelining
*   Visual representation of events in chronological order.
*   Correlates disparate pieces of evidence.
*   Categorizes evidence by date to visualize investigation results.
*   Can be built over days, weeks, or months.

### Forensic Data Carving
*   Identifying and recovering files or fragments of files based on their structure and content, often from unallocated space or slack space, without relying on filesystem metadata.
*   Helpful for finding hidden or deleted files.
*   Relies on:
    *   **File Headers (Signatures/Magic Numbers):** Standard byte sequences at the beginning of files identifying their type (e.g., `FF D8 FF E0` for JPEG).
    *   **File Footers:** Some file types have specific ending signatures.
    *   File structure and internal patterns.
*   Search for header, continue until footer or next header, or based on file size if known.

### Addressing Data-Hiding Techniques
*   **File Manipulation:**
    *   Changing file names and extensions (e.g., .txt to .dll).
    *   Using hidden file attributes (OS-level).
*   **Disk Manipulation:**
    *   **Hidden Partitions:** Deleting references in partition table or using tools like PartitionMagic.
    *   **Marking Bad Clusters:** Placing data in clusters and marking them as "bad" so the OS avoids them (common in FAT).
*   **Encryption:**
    *   **Bit-shifting:** Altering byte values by shifting bit patterns to make files appear as binary/executable code.
    *   **Steganography:** Hiding data within other files (covered in Lecture 5).

### Slack Space (Reiteration from Forensic Perspective)
*   Leftover storage on a hard disk when a file doesn't use all allocated space.
*   **File Slack:** Between logical EOF and physical end of the last allocated cluster.
    *   **RAM Slack:** Portion of file slack up to the end of the sector, may contain RAM data.
    *   **Drive Slack (or Cluster Slack):** Remaining unused sectors in the last allocated cluster.
*   Can contain valuable fragments of deleted files or other data.

### Examining Encrypted Files
*   Goal: Prevent unauthorized access. Uses password or passphrase.
*   Recovery is difficult without password.
*   **Methods for Access:**
    *   **Key Escrow:** A system where keys are held by a trusted third party.
    *   **Cracking Password:**
        *   Dictionary attack.
        *   Brute-force attack.
        *   Password guessing based on suspect's profile.
        *   Requires expertise and powerful computers.
    *   **Persuade suspect to reveal password** (legal means, warrants).
*   **Tools:** PRTK (Password Recovery Toolkit), Advanced Password Recovery Software Toolkit, L0phtCrack/@stake LC5 (older, for Windows passwords).

### Graphics File Forensics
*   **Recognizing a Graphics File:**
    *   Digital photos, line art, 3D images, scanned replicas.
    *   **Bitmap Images:** Collection of dots (pixels), e.g., BMP, JPEG, GIF, PNG.
    *   **Vector Graphics:** Based on mathematical instructions (lines, curves), e.g., SVG, AI. Scalable without loss of quality.
    *   **Metafile Graphics:** Combination of bitmap and vector, e.g., WMF, EMF.
*   **Understanding Graphics File Formats:**
    *   **Standard Bitmap:** GIF, JPEG, TIFF, BMP.
    *   **Standard Vector:** HPGL (Hewlett Packard Graphics Language), DXF (AutoCAD).
    *   **Nonstandard:** Targa (.tga), Raster Transfer Language (.rtl), Adobe Photoshop (.psd), Adobe Illustrator (.ai), Freehand (.fh9), Scalable Vector Graphics (.svg), Paintbrush (.pcx).
*   **Data Compression:**
    *   Some formats compress (GIF, JPEG, PNG), others don't (raw BMP).
    *   **Lossless Compression:** Reduces file size without removing data (e.g., Huffman, Lempel-Ziv-Welch). Used by GIF, PNG, TIFF (optionally). Utilities: WinZip, PKZip.
    *   **Lossy Compression:** Permanently discards bits of information to achieve higher compression (e.g., JPEG). Uses techniques like Vector Quantization (VQ).
*   **Locating and Recovering Graphics Files:**
    *   **OS Tools:** Time-consuming, results hard to verify.
    *   **Forensic Tools:**
        *   Identify **image headers** (magic numbers).
        *   Compare with good header samples.
        *   Reconstruct fragmented image files by identifying data patterns and modified/missing headers.
*   **Identifying Graphics File Fragments (Carving/Salvaging):**
    *   Recovering all file fragments from unallocated space, slack space.
    *   Tools help identify fragments and put them together.
*   **Repairing Damaged Headers:**
    *   Use good header samples for comparison.
    *   Each image file has a unique file header (e.g., JPEG: `FF D8 FF E0 00 10`, often with "JFIF" string).
*   **Reconstructing File Fragments:**
    1.  Locate and export all clusters of the fragmented file.
    2.  Determine starting and ending cluster numbers for each fragment group.
    3.  Copy fragments in proper sequence to a recovery file.
    4.  Rebuild corrupted file's header to make it viewable.
*   **Analyzing Graphics File Headers:**
    *   Necessary for unrecognized files.
    *   Use hex editors (e.g., Hex Workshop) to record hex values of headers and compare with known good samples.
*   **Tools for Viewing Images:** ThumbsPlus, ACDSee, QuickView, IrfanView; GUI forensic tools (ProDiscover, EnCase, FTK, X-Ways Forensics, iLook) often have built-in viewers.
*   **Steganography in Graphics Files:** Hiding information inside image files. Hidden data is not displayed by associated programs. Requires careful analysis of data structure.
*   **Steganalysis Tools:** Detect variations in image (e.g., statistical anomalies, palette changes), compare to known versions, compare hash values.

### Program Execution Artifact Investigations
*   Identify when programs/applications were executed, how often, and by whom.
*   Determine information about deleted and uninstalled programs.
*   Provide proof of data existing in a location no longer available (e.g., from prefetch files, registry).
*   Determine the last time a program was launched.
*   **Sources:** Windows Registry (UserAssist, MUICache), Prefetch files, ShimCache (Amcache.hve), Jump Lists, LNK files.

## Lecture 8: File Systems Investigation

### Understanding File Systems
*   Gives OS a "road map" to data on a disk.
*   Type of FS determines how data is stored.
*   Usually directly related to an OS.
*   Familiarity with platform is crucial for acquisition/inspection.

### Understanding the Boot Sequence
1.  **CMOS (Complementary Metal Oxide Semiconductor):** Stores system configuration, date/time information. Retains data when power is off (battery-backed).
2.  **BIOS (Basic Input/Output System):** Firmware containing programs for hardware-level input/output.
    *   Performs **POST (Power-On Self Test)**.
3.  **Bootstrap Process:**
    *   Code in ROM (part of BIOS) tells the computer how to proceed.
    *   Displays key(s) to open CMOS setup screen.
    *   **Forensic Implication:** CMOS boot order may need to be modified to boot from a forensic CD/USB.

### Startup in Windows NT and Later (e.g., XP)
1.  Power-On Self Test (POST).
2.  Initial Startup (BIOS loads MBR, MBR loads boot sector of active partition).
3.  Boot Loader (e.g., NTLDR for XP) loads.
4.  Hardware Detection and Configuration (NTDetect.com for XP).
5.  Kernel Loading (Ntoskrnl.exe for XP).
6.  User Logon.
*   **Startup Files for Windows XP:** NTLDR, Boot.ini (boot options), BootSect.dos (for dual-booting DOS), NTDetect.com, NTBootdd.sys (for SCSI drives), Ntoskrnl.exe, Hal.dll (Hardware Abstraction Layer), Pagefile.sys, Device drivers.
*   **Contamination Concerns (XP):** Starting an XP NTFS system accesses/updates last access times of several files, potentially destroying evidence of last use.

### Microsoft File Structures
*   **FAT (File Allocation Table):** FAT12, FAT16, FAT32.
*   **NTFS (New Technology File System).**
*   **Clusters:** Storage allocation units (groups of sectors, at least 512 bytes). Logical addresses.
*   **Sectors:** Smallest physical storage unit. Physical addresses.

### Disk Partitions
*   **Logical Drive:** A partition formatted with a file system.
*   **Hidden Partitions/Voids (Partition Gaps):** Unused space between partitions, can hide data.
*   Disk editors (Norton Disk Edit, WinHex, Hex Workshop) can view/modify partition tables.

### Master Boot Record (MBR)
*   First sector (Sector 0) of a partitioned storage device.
*   Stores information about partitions (location, size, type) in the partition table.
*   Contains boot code to load the OS from the active partition.
*   Software (e.g., PartitionMagic, bootkits) can replace/modify MBR.
*   Forensic tools should be used to examine MBR; use multiple tools for verification.

### Examining FAT Disks
*   Originally for floppy disks.
*   Stores: Filenames, directory names, date/time stamps, starting cluster number, attributes.
*   **FAT Table:** A map of clusters, indicating which are used, free, bad, or part of a file chain. Two copies for redundancy.
*   **Root Directory:** Fixed size and location in FAT12/16; can be anywhere in FAT32.
*   **Drive Slack:** Unused space in a cluster.
    *   **RAM Slack:** Space from logical EOF to end of sector in the last cluster.
    *   **File Slack:** Space from logical EOF to end of the last allocated cluster.
*   Can contain logon IDs, passwords, remnants of old data.

### Examining NTFS Disks
*   Introduced with Windows NT.
*   Improvements over FAT: Larger file/partition sizes, security (ACLs), compression, encryption (EFS), journaling (logs transactions to aid recovery).
*   **Partition Boot Sector (VBR):** Starts at sector 0 of the NTFS partition.
*   **Master File Table (MFT):**
    *   A relational database; first file on the disk.
    *   Contains information (metadata) about all files and folders on the disk in MFT records (typically 1KB each).
    *   The first MFT record describes the MFT itself.
*   Reduces slack space compared to FAT for small files (data can be stored directly in MFT if small enough - resident data).
*   Uses **Unicode** for filenames (UTF-8, UTF-16, UTF-32).
*   **NTFS File Attributes:**
    *   All files/folders have attributes.
    *   **Resident Attributes:** Stored directly within the MFT record (e.g., filename, timestamps, small data).
    *   **Nonresident Attributes:** Data too large for MFT record is stored in external clusters; MFT record contains pointers to these clusters.
    *   Uses **Logical Cluster Numbers (LCNs)** and **Virtual Cluster Numbers (VCNs)** to map file data.

### FAT32 vs NTFS Comparison

| Feature               | FAT32                 | NTFS                                         |
| :-------------------- | :-------------------- | :------------------------------------------- |
| Basic Structure       | Simple structure      | Complex structure (MFT, attributes)          |
| Max Chars in Filename | 83 (LFN up to 255)    | 255                                разрушен. |
| Max File Size         | 4GB                   | 16TB (theoretically 16EB)                    |
| Encryption            | Not provided          | Provided (EFS)                               |
| Security              | Network type (share)  | Local and network (ACLs)                     |
| Performance           | Good (simpler)        | Better than FAT32 (for large volumes)        |
| Compatibility with OS | Windows 95/98/XP etc. | Windows NT/2000/XP/Vista/7/8/10 etc.         |
| Accessing Speed       | Less Relatively       | More (efficient for large volumes)           |

### Windows Registry
*   Hierarchical database storing hardware/software configuration, network connections, user preferences, setup info.
*   Valuable evidence source for investigators.
*   View with **Regedit** (Windows 9x) or **Regedt32** (Windows 2000/XP and later, now just `regedit.exe`).
*   **Registry Terminology:**
    *   **Registry:** The entire database.
    *   **Registry Editor:** Tool to view/edit.
    *   **HKEY (Handle to Key):** Root keys (e.g., HKEY_LOCAL_MACHINE, HKEY_CURRENT_USER).
    *   **Key:** Folder-like container.
    *   **Subkey:** A key within another key.
    *   **Branch:** A key and its subkeys.
    *   **Value:** Name/data pair within a key. (Name, Type, Data).
    *   **Default Value:** A value for each key that has no name.
    *   **Hives:** Files on disk containing portions of the registry (e.g., SAM, SYSTEM, SOFTWARE, SECURITY, NTUSER.DAT).

### Macintosh File Structure and Boot Process
*   **Mac OS X (now macOS):**
    *   Based on **Darwin core** (hybrid of XNU kernel using Mach microkernel and BSD components).
    *   BSD UNIX application layer.
*   **File Systems:**
    *   **HFS (Hierarchical File System):** Older, files stored in nested directories (folders).
    *   **HFS+ (Extended Format File System / Mac OS Extended):** Introduced with Mac OS 8.1. Supports smaller file sizes on larger volumes, more efficient disk use, journaling.
    *   **APFS (Apple File System):** Newer, replaced HFS+ as default on modern Macs and iOS. Optimized for SSDs, strong encryption.
*   **File Manager Utility:** Handles reading, writing, storing data.
*   **Finder:** Manages files, user desktops.
*   **Older Mac OSs (Classic Mac OS):** Files consist of two parts (forks):
    *   **Data Fork:** Actual file content.
    *   **Resource Fork:** Metadata, application information, icons, menus.
*   **Macintosh OS 9 Volumes:**
    *   **Volume:** Any storage medium for files.
    *   **Allocation Blocks:** Groups of logical blocks (logical blocks <= 512 bytes).
    *   **Clumps:** Groups of contiguous allocation blocks to reduce fragmentation.
    *   **EOF Descriptors:**
        *   **Logical EOF:** Actual size of the file content.
        *   **Physical EOF:** Total size of blocks allocated to the file.
*   **Macintosh Boot Tasks (OS 9 example):**
    1.  Power on.
    2.  Hardware self-test and **Open Firmware** (processor/system-independent firmware) run.
    3.  Macintosh OS starts.
    4.  Startup disk located.
    5.  System files opened.
    6.  System extensions loaded.
    7.  Finder starts.
*   **Older Mac OS Volume Structures:**
    *   **Boot Blocks:** First two logical blocks.
    *   **MDB (Master Directory Block) / VIB (Volume Information Block):** Stores volume info.
    *   **VCB (Volume Control Block):** Stores MDB info when OS mounts.
    *   **Extents Overflow File:** Stores file info not in MDB/VCB.
    *   **Catalog File:** Listing of all files/directories, maintains relationships (B*-tree).
    *   **Volume Bitmap:** Tracks used/unused blocks.
    *   **B*-tree File System:** Used by File Manager for catalog and extents overflow. Data in leaf nodes.

### UNIX and Linux Disk Structures and Boot Processes
*   **Linux File Systems:**
    *   **Ext2fs (Second Extended File System).**
    *   **Ext3fs (Third Extended File System):** Journaling version of Ext2fs.
    *   **Ext4fs (Fourth Extended File System):** Further improvements, larger file/volume sizes, extents.
*   **Inodes (Index Nodes):**
    *   Data structure containing metadata about each file/directory (permissions, owner, size, timestamps, pointers to data blocks).
    *   Does NOT contain filename or actual data.
    *   **Pointers:** To other inodes (for directories) or data blocks.
    *   **Link Count:** Number of hard links to the inode. Deleted when count is 0 and no process has it open.
*   **UNIX/Linux System Components:**
    *   **Boot Block:** First block of a bootable partition, contains bootstrap code. Only one on the main hard disk for the system.
    *   **Superblock:** Contains critical info about the filesystem (disk geometry, available space, location of first inode, FS state).
    *   **Inode Blocks:** Area where inodes are stored.
    *   **Data Blocks:** Where actual file data and directory contents are stored.
    *   **Bad Block Inode:** Keeps track of bad sectors. Utilities: `badblocks`, `mke2fs`, `e2fsck`.
    *   **`ls` command:** Displays file/directory info (often from inodes).
    *   **Continuation Inode:** Inode structure includes: mode/file type, link count, UID, GID, size, access times, pointers.
*   **Inode Pointers (Typical Ext Structure):**
    *   First inode has 13 pointers (example):
        *   Pointers 1-10: Direct pointers to data blocks.
        *   Pointer 11: Indirect pointer (points to a block of direct pointers).
        *   Pointer 12: Double-indirect pointer (points to a block of indirect pointers).
        *   Pointer 13: Triple-indirect pointer (points to a block of double-indirect pointers).
*   **UNIX/Linux Boot Processes:**
    1.  Instruction code in firmware (BIOS/UEFI) loaded to RAM.
    2.  Hardware check.
    3.  Boot program (e.g., GRUB, LILO) loaded from MBR or boot partition.
    4.  Boot program loads the Kernel.
    5.  Kernel identifies devices.
    6.  Boots system (often to single-user mode initially).
    7.  Runs startup scripts (e.g., init scripts, systemd units).
    8.  Changes to multiuser mode.
    9.  Identifies root directory, swap, dump files.
    10. Sets hostname, time zone.
    11. Runs consistency checks on file system, mounts partitions.
    12. Starts services, sets up NIC.
    13. Establishes user/system accounting, quotas.
*   **Linux Loaders:**
    *   **LILO (LInux LOader):** Older boot manager, uses `Lilo.conf`.
    *   **GRUB (GRand Unified Bootloader):** More powerful, resides on MBR or partition boot sector, command line or menu-driven.
*   **UNIX/Linux Drives and Partition Schemes:**
    *   Labeled as path starting at root (`/`) directory.
    *   Primary master disk: `/dev/hda` (older PATA); Partitions: `/dev/hda1`, `/dev/hda2`.
    *   Primary slave/secondary master/slave: `/dev/hdb`.
    *   SCSI controllers: `/dev/sda` (first disk), `/dev/sdb` (second disk); Partitions: `/dev/sda1`.
    *   Linux treats SATA, USB, and FireWire devices similarly to SCSI devices (e.g., `/dev/sda`, `/dev/sdb`).

## Lecture 9: E-mail Investigations

### Role of E-mail in Investigations
*   Increase in e-mail scams, phishing, spoofing.
*   Investigators need to examine/interpret unique e-mail content.
*   **Phishing E-mails:** Often in HTML format to create deceptive links.
*   **Nigerian Scam (419 Scam):** Noteworthy e-mail scam.
*   **Spoofing E-mail:** Can be used to commit fraud by falsifying sender information.

### Roles of Client and Server in E-mail
*   **Environments:** Internet or controlled LAN/MAN/WAN.
*   **Client/Server Architecture:**
    *   **Client:** User's machine with email software (e.g., Outlook, Thunderbird).
    *   **Server:** Handles sending, receiving, storing emails (e.g., Exchange, Postfix).
    *   Server OS/email software differs from client side.
*   **Protected Accounts:** Require usernames and passwords.
*   **Name Conventions:**
    *   Corporate: `john.smith@somecompany.com`
    *   Public: `whatever@hotmail.com`
    *   Part after `@` is the domain name.
*   Tracing corporate e-mails is often easier due to standard naming and centralized administration.

### Investigating E-mail Crimes and Violations
*   **Goals:**
    1.  Find who is behind the crime/violation.
    2.  Collect the evidence.
    3.  Present findings.
    4.  Build a case.
*   Laws vary by jurisdiction (city, state, country).
*   **Examples of Crimes:** Spam, narcotics trafficking, extortion, sexual harassment, child abductions, pornography.

### Examining E-mail Messages
*   Access victim's computer to recover evidence (with proper authorization).
*   **Using Victim's E-mail Client or PST/OST files:**
    *   Find and copy evidence.
    *   Access protected/encrypted material (if possible).
    *   Print e-mails.
*   **Guiding Victim on Phone:** Instruct victim to open/copy e-mail including full headers.
*   **Deleted E-mails:** May require specialized recovery tools.
*   **Copying E-mails:**
    *   Before starting, copy and print the e-mail(s) in question.
    *   Forward as attachment to preserve original headers.
    *   Drag-and-drop or save to storage medium.

### Viewing and Examining E-mail Headers
*   **Finding Headers:**
    *   **GUI Clients:** Outlook (Message Options), Outlook Express (Properties -> Message Source), Novell Evolution (View -> All Message Headers).
    *   **Command-line Clients:** Pine, ELM (enable full headers).
    *   **Web-based Clients:** AOL (Action -> View Message Source), Gmail ("Show original"), etc.
*   Copy and paste headers into a text document for analysis.
*   **Information in Headers:**
    *   **Return Path:** Address for bounce messages.
    *   **Recipient's E-mail Address (To, Cc, Bcc - Bcc often not in received header).**
    *   **Type of Sending E-mail Service.**
    *   **IP Address of Sending Server(s):** Crucial for tracing. `Received:` lines show hops.
    *   **Name of E-mail Server(s).**
    *   **Unique Message Number (Message-ID).**
    *   **Date and Time E-mail was Sent/Received at each hop.**
    *   **Attachment Files Information (MIME details).**
    *   **X-Originating-IP:** Often reveals the sender's actual IP address if sent via some webmail services or clients.

### Examining Additional E-mail Files
*   Messages saved on client or server.
*   **Microsoft Outlook:** Uses `.pst` (Personal Storage Table) and `.ost` (Offline Storage Table) files.
*   **Electronic Address Book:** Most email programs have one (contacts).
*   **Web-based E-mail:**
    *   Messages displayed/saved as web pages in browser's cache.
    *   Many providers offer IM services (logs may exist).

### Tracing an E-mail Message
1.  Contact administrator of the sending server (identified from headers).
2.  **Find Domain Name's Point of Contact (POC):**
    *   `www.arin.net` (American Registry for Internet Numbers - for North America)
    *   `www.ripe.net` (Réseaux IP Européens - for Europe, Middle East, Central Asia)
    *   `www.apnic.net` (Asia Pacific Network Information Centre)
    *   `www.lacnic.net` (Latin American and Caribbean Internet Addresses Registry)
    *   `www.afrinic.net` (African Network Information Centre)
    *   `www.internic.com` (General domain info, Whois lookups).
    *   Other lookup sites: `www.freeality.com`, `www.google.com` (for general searches).
3.  Find suspect's contact information.
4.  Verify findings by checking network e-mail logs against e-mail addresses and IPs.

### Using Network E-mail Logs
*   **Router Logs:** Record all incoming/outgoing traffic, rules for allowing/disallowing, can help resolve path of email.
*   **Firewall Logs:** Filter e-mail traffic, verify if email passed through.
*   Use text editors or specialized log analysis tools.

### Understanding E-mail Servers
*   Computer with software using e-mail protocols (SMTP, POP3, IMAP).
*   Maintains logs for examination.
*   **E-mail Storage:**
    *   **Database:** (e.g., Microsoft Exchange uses EDB files).
    *   **Flat File:** (e.g., mbox format used by many Unix systems).
*   **Logs:**
    *   **Default or Manual Configuration.**
    *   **Continuous (appends) or Circular (overwrites oldest).**
    *   **Log Information:** E-mail content (sometimes), sending IP, receiving/reading date/time, system-specific info.
*   Contact suspect's network email admin ASAP.
*   Servers can sometimes recover deleted e-mails (similar to hard drive deletion, depends on server policies and backup).

### Examining Specific Server Logs
*   **UNIX E-mail Server Logs (e.g., Sendmail):**
    *   `/etc/sendmail.cf`: Configuration.
    *   `/etc/syslog.conf`: Specifies what Sendmail logs.
    *   `/var/log/maillog` (or `/var/log/mail.log`): SMTP, POP3 communications, IP addresses, timestamps.
    *   Check `man` pages for specific mail server software (Postfix, Qmail, Exim).
*   **Microsoft Exchange Server Logs:**
    *   Uses a database based on **ESE (Extensible Storage Engine)**.
    *   **Information Store Files:**
        *   `*.edb` (Exchange Database): MAPI information (mailboxes, public folders).
        *   `*.stm` (Streaming Media File - pre-Exchange 2007): Non-MAPI information (MIME content). Exchange 2007+ integrates this into EDB.
    *   **Transaction Logs (`E<nn>.log`):** Keep track of changes to e-mail databases before they are committed.
    *   **Checkpoints (`E<nn>.chk`):** Keep track of committed transaction logs.
    *   **Temporary Files.**
    *   **E-mail Communication Logs (`res#.log` - older versions).**
    *   **Tracking.log (Message Tracking Logs):** Tracks messages as they pass through Exchange.
    *   **Troubleshooting/Diagnostic Logs:** Windows Event Viewer (Application, System logs).

### Specialized E-mail Forensics Tools
*   AccessData’s Forensic Toolkit (FTK)
*   ProDiscover Basic
*   FINALeMAIL
*   Sawmill-GroupWise
*   DBXtract (for Outlook Express .dbx files)
*   Fookes Aid4Mail and MailBag Assistant
*   Paraben E-Mail Examiner
*   Ontrack Easy Recovery EmailRepair
*   R-Tools R-Mail
*   **Advantages:** Can find email database files, personal email files, offline storage files, log files without needing deep knowledge of server/client workings.
*   **FTK for E-mail Recovery:**
    *   Can index data on disk image/drive.
    *   Filters and finds files specific to email clients/servers.
    *   Integrates **dtSearch** to build b-tree index of text data for fast searching.

### Using a Hexadecimal Editor to Carve E-mail Messages
*   Fewer tools for non-Microsoft email systems.
*   **mbox format:** Stores emails in flat plaintext files, emails concatenated. Common in Unix.
*   **MIME (Multipurpose Internet Mail Extensions) format:** Standard for email content type, encoding, attachments. Used within various email file formats.
*   Example: Carving emails from Evolution (which may use mbox). Look for "From " line at start of messages in mbox.

## Lecture 10: Network Forensics and Cyber-Incident Investigation

### Internet Fundamentals
*   **Internet:** A global collection of interconnected networks.
*   **ISP (Internet Service Provider):** Provides access to the Internet.
*   **DNS (Domain Name Service):** Translates human-readable domain names (e.g., www.google.com) to IP addresses and vice-versa.
*   **Common Software:** Web browsers, e-mail clients.
*   **Protocols:**
    *   **TCP/IP Suite:** Default Internet protocol.
        *   **TCP (Transmission Control Protocol):** Connection-oriented, reliable, ordered delivery.
        *   **UDP (User Datagram Protocol):** Connectionless, unreliable, faster, used for DNS, VoIP, streaming.
        *   **FTP (File Transfer Protocol):** For transferring files.
        *   **HTTP/HTTPS (HyperText Transfer Protocol/Secure):** For web browsing.
        *   **SMTP (Simple Mail Transfer Protocol):** For sending email.
        *   **POP3/IMAP (Post Office Protocol 3 / Internet Message Access Protocol):** For retrieving email.
*   **OSI Model (7 Layers):** Application, Presentation, Session, Transport, Network, Data Link, Physical.
*   **TCP/IP Model (4/5 Layers):** Application, Transport, Internet (Network), Network Access (Data Link & Physical).
*   **IP Addressing (IPv4):**
    *   32-bit long, divided into four 8-bit groups (octets).
    *   Dotted quad notation (e.g., 205.55.29.170).
    *   **Classes:** A, B, C (for unicast), D (multicast), E (experimental). Defined by first octet range and default subnet mask.
    *   **Private IP Ranges:** (e.g., 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16). Not routable on public internet.
    *   **NAT (Network Address Translation):** Translates private IPs to a public IP for internet access.

### Key Network Devices (Sources of Evidence)
*   **Switches:** Operate at Layer 2 (Data Link), forward frames based on MAC addresses. Logs may show MAC addresses, port activity.
*   **Routers:** Operate at Layer 3 (Network), forward packets based on IP addresses. Logs show routing information, traffic flows, ACL activity.
*   **Firewalls:** Control incoming/outgoing network traffic based on rules.
    *   **Next-Generation Firewalls (NGFW):** Combine firewall with IDS/IPS, application control.
    *   **Evidence:** Connection logs (source/destination IP, port, protocol, allowed/denied), remote access (VPN) logs.
*   **Network Intrusion Detection/Prevention Systems (NIDS/NIPS):** Monitor network traffic for malicious activity or policy violations. Generate alerts and logs.
*   **Web Proxy Servers:** Mediate HTTP requests. Logs show websites visited, user agents, timestamps.
*   **Domain Controllers/Authentication Servers (e.g., Active Directory):** Manage user accounts, authentication. Logs show logon/logoff events, account changes.
*   **DHCP (Dynamic Host Configuration Protocol) Server:** Assigns IP addresses to devices. Logs show IP address assignments to MAC addresses over time.
*   **Application Servers:** Host applications. Application-specific logs.

### Network Forensics Overview
*   Systematic tracking of incoming and outgoing network traffic to ascertain how an attack was carried out or an event occurred.
*   Intruders often leave trails in network traffic and logs.
*   Determine cause of abnormal traffic (internal bug vs. attackers).

### Performing Live Acquisitions
*   Useful for active network intrusions/attacks.
*   Necessary before taking a system offline, as attacks might leave footprints only in running processes or RAM.
*   Doesn't always follow typical dead-box forensics procedures (due to volatility).
*   **Order of Volatility (OOV):** How long a piece of information lasts on a system. Collect most volatile first.
    1.  **Cache (CPU registers, L1/L2/L3 cache)**
    2.  **RAM (Routing tables, ARP cache, process tables, kernel stats, memory)**
    3.  **Paging File / Swap Space**
    4.  **HDD/SSD (Temporary file systems, system files, user files)**
    5.  **Logs stored on remote systems**
    6.  **Archive Media (Backups)**
*   **Steps for Live Acquisition:**
    1.  Create/download a bootable forensic CD/USB (with trusted tools).
    2.  Keep a detailed log of all actions.
    3.  Use a sterile network drive or dedicated forensic storage to send/save collected information.
    4.  Copy physical memory (RAM dump).
    5.  Next steps vary by incident (e.g., list running processes, network connections, open files).
    6.  Get forensic hash values of all files recovered.
*   **Windows RAM Capture Tools:** Mantech Memory DD, Win32dd, FTK Imager, DumpIt, Belkasoft Live RAM Capturer.

### Standard Procedures for Network Forensics
*   Use a standard installation image for systems on a network for comparison.
*   After an attack, close any way in (isolate compromised systems).
*   Attempt to retrieve all volatile data.
*   Acquire forensic images of all compromised drives.
*   Compare files on the forensic image to the original installation image to find changes.
*   Restore drives (in an isolated environment) to understand the attack.
*   Work on an isolated system to prevent malware spread.

### Reviewing Network Logs
*   Record ingoing/outgoing traffic from network servers, routers, firewalls.
*   **Tcpdump:** Command-line packet analyzer. Can generate top 10 lists, identify patterns.
*   If attacks involve other companies, do not reveal their information without proper authorization.

### Using Network Tools
*   **Sysinternals Suite (Microsoft):**
    *   **RegMon (older, now Process Monitor):** Shows Registry activity.
    *   **Process Explorer:** Detailed view of running processes.
    *   **Handle:** Shows open files and processes using them.
    *   **FileMon (older, now Process Monitor):** Shows file system activity.
*   **PsTools Suite (Sysinternals):**
    *   PsExec (run processes remotely), PsGetSid (display SID), PsKill (kill process), PsList (list process details), PsLoggedOn (show logged-on users), PsPasswd (change passwords), PsService (control services), PsShutdown (shutdown/restart PCs), PsSuspend (suspend processes).

### Using Packet Sniffers
*   Devices or software that monitor and capture network traffic.
*   Most work at Layer 2 (Data Link) or Layer 3 (Network).
*   **PCAP (Packet Capture) format:** Standard file format for captured packets.
*   TCP flags in headers can identify packet types (SYN, ACK, FIN, RST).
*   **Tools:**
    *   **Tcpdump:** Command-line.
    *   **Wireshark (formerly Ethereal):** GUI-based, powerful capture and analysis.
    *   **Snort:** NIDS, can also be used for packet logging.
    *   Tcpslice, Tcpreplay, Tcpdstat, Ngrep, Etherape, Netdude, Argus.
*   **Wireshark Features:**
    *   Capture and analysis.
    *   Filtering (display filters, capture filters).
    *   Finding attacker IP addresses.
    *   Filtering for specific protocols/requests (e.g., HTTP POST).
    *   "Find Packet" tool (by display filter, hex value, string; search in list, details, bytes).
*   **NetworkMiner:** Passive network sniffer/packet capture tool, can extract files, credentials, identify hosts from PCAP files.

### Security Operations Center (SOC)
*   **Team:** Dedicated to securing an enterprise.
*   **Components:** People (analysts, architects, etc.), Technologies/Tools, Frameworks/Methodologies.
*   **Objective:** Detect, investigate, triage, respond to real-time and historical threats.
*   **Key Steps:** Gather relevant evidence -> Enrich with contextual intelligence -> Pivot, filter, iterate -> Integrate lessons learned.
*   **Challenges:** Advanced Threat Actors, Lack of Visibility, Time-intensive Analysis, Alert Fatigue.
*   **Key Evidence Sources for SOC:** Network traffic, Firewall logs, Access logs, IDS/IPS alerts, DNS logs, Proxy logs, Web server logs, Threat Intelligence feeds.

## Exam Specifics & Preparation

### Exam Format and Structure

*   **Total Weight:** The exam is worth 70% of the total module grade.
*   **Date:** Friday, 16th (refer to official timetable for the specific month and year).
*   **Sections:** The exam has **two sections**, each worth 50% of the *exam mark*.
    *   **Section A (50% of exam mark):**
        *   Consists of **three questions**.
        *   You must **answer ALL three** questions.
        *   *Lecturer's emphasis: "Be careful to read this very well."*
    *   **Section B (50% of exam mark):**
        *   Consists of **four questions**.
        *   You must **answer any TWO out of the four** questions listed.
        *   *Lecturer's advice:*
            *   Read ALL four questions in this section first.
            *   Choose the two questions you are most comfortable with.
            *   **Crucially: Only answer TWO questions.** If you answer more than two (e.g., three), only the *first two* answers written will be marked, regardless of the quality of any subsequent answers. The examiners will not pick and choose the best ones.
            *   The lecturer assures that there will be "plenty of choice" and you should find at least two topics you have covered and are familiar with.

### Key Topics & Potential Question Types (Based on Examples in Revision)

*   **The CFSAP Model (Computer Forensics - Secure, Analyse, Present):**
    *   Be prepared to outline its key elements.
    *   Understand how it relates to specific stages, e.g., "Stage One: Secure."
    *   Be able to discuss different potential sources of computer information (Hardware: Hard Drive, RAM, CPU; Software stores: Database, online storage; Mobile devices).
    *   Describe a suitable process for securing each of these sources (e.g., write-blocking, isolation, Faraday cages, handling volatile vs. non-volatile data).
    *   Consider the implications of the system being ON vs. OFF.
*   **Volatile Data:**
    *   Define volatile data.
    *   Give examples of elements of volatile data in an operating system (e.g., Windows: RAM, running processes, network connections, swap space, console messages, system memory).
    *   Understand its importance and why it's lost if power is lost or a system fault occurs.
*   **Anti-forensics (Encryption and Steganography):**
    *   Understand methods to prevent forensic investigation.
    *   Be able to provide a detailed comparison and discussion of the similarities and differences between encryption and steganography as counter-forensic methods.
        *   Steganography: "covered or hidden writing" (conceals existence of message).
        *   Cryptography: "secret writing" (makes message unreadable without a key).
        *   Main structure of message in steganography is not changed vs. cryptography imposes a change on the secret message.
        *   Steganography provides confidentiality and authentication; Cryptography provides confidentiality, integrity, authentication, and non-repudiation.
*   **Corporate Investigator vs. Law Enforcement:**
    *   Understand the differences in their roles, procedures, and legal standing.
    *   Be able to answer: "Is a corporate investigator considered an agent of law enforcement? Why?"
        *   Generally no, unless working *closely with* law enforcement on a *particular case*.
        *   Corporate investigators often don't follow the same strict procedures (e.g., chain of custody) unless the case is likely to go to court for criminal prosecution. Their scope might be internal policy violations.
*   **ACPO Guidelines:**
    *   Be able to outline the four key principles of ACPO guidelines.
    *   Provide an example to demonstrate how each principle can be implemented.
        *   **Principle 1:** No action should change data. (Example: Use of write-blockers, imaging).
        *   **Principle 2:** If original data must be accessed, the person must be competent and able to explain actions. (Example: Documenting live acquisition steps when a system cannot be shut down).
        *   **Principle 3:** Audit trail of all processes. (Example: Detailed contemporaneous notes, logs from forensic tools, video/photo documentation of the scene and process).
        *   **Principle 4:** Case officer has overall responsibility. (Example: Ensuring all team members adhere to principles and legal requirements).
*   **UK Legislation - Computer Misuse Act 1990 (CMA):**
    *   Understand the key sections and the offenses they cover:
        *   **S1: Unauthorised access to computer material.** (e.g., guessing a password to access files not entitled to).
        *   **S2: Unauthorised access with intent to commit other offence.** (e.g., hacking into a system to then commit fraud).
        *   **S3: Unauthorised acts with intent to impair operation of computer.** (e.g., deploying a virus, DDoS).
        *   **S3A: Making, supplying or obtaining articles for use in S1 or S3 offences.** (e.g., creating/distributing malware or hacking tools).
*   **Other Potential Topics (from the "Other possible topics" slide):**
    *   **Storage devices forensics:** Magnetic media, HDD, CD/DVD, SSD.
    *   **Forensic acquisition and verification:** Techniques and algorithms.
    *   **Chain of Custody:** (Likely linked with ACPO).
    *   **File recovery (deleted files).**
    *   **Data-Hiding techniques:** (Likely linked with steganography/encryption).
    *   **Regular procedure in Computer Forensic Analysis.**
    *   **Professional conduct in Computer Forensics.**
    *   **Essential guidelines in processing a computer crime incident/scene.**

### How to Prepare for the Exam (Lecturer's Advice)

1.  **This Exam Revision Recording:**
    *   The lecturer explicitly states to "go back, read it very well."
    *   This recording itself is a key resource. *You will only have the recording, not the slides for this specific revision session.*
2.  **10 Weeks of Lecture Slides:**
    *   These are listed as a primary preparation resource on the "To prepare the EXAM" slide.
3.  **Weekly Lecture Recordings (Panopto):**
    *   All topics covered in the 10 weeks of lectures are examinable.
    *   The lecturer believes these recordings cover at least 90% of the necessary content for the module.
4.  **2 Books (from Reading Lists):**
    *   While available, the lecturer suggested they might not be essential to read thoroughly "two weeks before the exam" if time is short, implying the lectures and revision material are more targeted. However, they are listed as a preparation resource.

**Final Tip from Lecturer:** Focus on understanding the concepts and being able to explain them with examples and justifications, rather than just memorizing definitions. For questions asking "Why?" or "Demonstrate with an example," ensure you provide that depth.