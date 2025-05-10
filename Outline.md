# Revision Outline

## General Exam Information (from Week 11 Revision Slides)

*   **Structure:** 2 Sections, each worth 50%.
    *   **Section A:** Answer ALL of the Three questions listed.
    *   **Section B:** Answer any TWO out of FOUR questions listed.
*   **Key Advice for Section B:** Read all four questions first, then choose the two you are most comfortable with. If you answer more than two, only the first two will be marked.
*   **Preparation Materials:** 10 weeks of lecture slides, 2 Recommended Books (from reading lists), Lecture Recordings (Panopto).

---

## Lecture 1: Forensic Computing

1.  **Introduction to Forensic Computing:**
    *   Definition: Application of investigation/analysis to gather/preserve evidence for presentation; building clear, evidence-based reports.
    *   Module scope: What it does (academic/practical experience, tools, analysis process understanding, legal aspects) and what it does NOT do (qualify as examiner, provide one "science"/methodology).
2.  **Core Concepts:**
    *   IT in commission and investigation of crimes.
    *   Internet as an arena for new crime types and tracking.
    *   Two main themes: Computer Forensics & Intrusion Forensics.
    *   Forensic Computing Process: Preservation, Identification, Extraction, Documentation, Interpretation.
    *   "Art" vs. Science: Importance of clear methodologies and flexibility.
3.  **Applications of Forensic Computing:**
    *   Legal (criminal prosecution) vs. Non-legal (root cause analysis, internal investigations, intelligence).
4.  **Impact of the Internet:**
    *   Global interconnectedness, rapid data discovery/sharing.
    *   Case Study: Clifford Stoll and the LBNL hack (illustrates early network forensics).
5.  **Human Behaviour & Cyber Crime:**
    *   Rising online activity and challenges in determining user actions.
    *   Global internet user distribution.
    *   Common Cyber Concerns: Paedophile activity, fraud (phishing, scams), cyber warfare, hate crimes, use of digital equipment for crime (encrypted comms), network traffic monitoring, hacking.
    *   Cybercrime Classification: Computer as a target, repository, or tool.
    *   Examples of Crimes: Table of various cyber-enabled crimes.
    *   Multiplicity of Crime: No "typical" computer crime; diverse scenarios.
6.  **Cybercriminal Landscape:**
    *   Potential points for criminal activity (diagram).
    *   What cybercriminals are after (personal data, financial info - infographics).
    *   The Dark Web Marketplace: Prices for stolen data/services.
    *   Cybercrime as a Service (CaaS): DDoS attacks, etc.
    *   Recent cybercrimes and data breaches (UK MoD, TFL).
7.  **Legal & Ethical Considerations:**
    *   Search and seizure.
    *   Privacy paradox (protecting privacy vs. solving crimes).
    *   User vs. Law enforcement perspectives.
    *   Global access issues (banking, travel, email).
    *   Challenges:
        *   Legal: Lack of boundaries, jurisdiction, differences in laws/legal systems, accessing digital evidence, authority, human rights, ethics.
        *   Operational: Technical/legal cooperation, harmonization of laws, cooperative investigation.
8.  **Protection from Cybercrime:**
    *   Diagram: Prevention (infrastructure, human factor, best practices) vs. Deterrents (penalties, laws, investigation, forensics).
9.  **Computer Security (CompSec) vs. Forensics:**
    *   CompSec: Preserve system as per policies.
    *   Forensics: Explain how policy was violated.
    *   CIA Triad: Confidentiality, Integrity, Availability (enforced by countermeasures).
    *   Overlap and opposing aims, minimal logging in security, security countermeasures potentially hindering forensics.
10. **Conclusion of Lecture 1:**
    *   Forensic computing searches for electronic evidence.
    *   Computer as target, repository, or tool.
    *   Different user/law enforcement perspectives.
    *   CompSec and forensics are complementary but distinct.

---

## Lecture 2: Cyber Forensics in Practice (Law Enforcement & National Security)

1.  **Evolution of Computer Crime Cases:**
    *   Early: Recovering evidence.
    *   Later (networking): Computers as targets.
    *   Scenarios: Computers as facilitators/repositories vs. computers as targets.
2.  **CFSAP Model (Computer Forensics – Secure, Analyse, Present):**
    *   Key elements: Identification, Preservation, Analysis, Presentation.
    *   High-level view of procedures, 3 distinct steps with processes (diagram).
3.  **Forensic Practice & Evidence Principles:**
    *   Techniques for reconstructing digital environment.
    *   FBI Handbook of Forensic Services: Types of examinations (Content, Comparison, Transaction, Extraction, Deleted data, etc.).
    *   Principles of Evidence: Admissible, Authentic, Complete, Reliable, Believable (applicable in legal and non-legal contexts).
4.  **ACPO (Association of Chief Police Officers) Guide:**
    *   "Good Practices Guide for Computer Based Evidence" - predominant UK model.
    *   Accepted standard for digital evidence.
    *   Adapted by IOCE (International Organisation for Computer Evidence).
    *   Examiner training is crucial.
    *   Topics covered: Principles, crime scenes, personnel, recovery, paedophile images, witnesses, disclosure, mobile/PDAs, victim contact.
    *   **ACPO Principles (4 Key Principles):**
        1.  No action should change data relied upon in court.
        2.  Exceptional access to original data requires competence and ability to explain actions.
        3.  Audit trail of all processes must be created/preserved for independent verification.
        4.  Case officer has overall responsibility for adherence to law and principles.
    *   **ACPO - Investigating Personnel:** Pre-search, briefing, search prep, toolkit, record keeping (scene sketch, persons, computer details), interviews, specialists.
    *   **ACPO - Paedophile Images:** Classification (minimum Confidential), possession as an offence, handling of personal/victim info, use of encrypted disks for exhibits, printouts only in exceptional circumstances.
        *   Government Protected Marking Scheme (GPMS) vs. Government Security Classifications (GSC) - OFFICIAL-SENSITIVE.
        *   Classification Scales: COPINE scale (therapeutic origin, 10-level typology for child abuse images).
        *   Sexual Offences Definitive Guideline (Categories A, B, C).
        *   SAP Scale (5 levels).
        *   Europol "Trace an Object" initiative.
5.  **UK Legislations:**
    *   Computer Misuse Act 1990 (unauthorised access, modification).
    *   Police and Criminal Evidence Act 1984 (power of seizure).
    *   Criminal Justice and Police Act 2001 (power to seize items believed to contain evidence).
    *   Electronic Communications Act 2000 (e-signatures, e-commerce, crypto service providers).
6.  **Forensics in the Real World & National Security:**
    *   Process model table: Identification -> Preservation -> Collection -> Examination -> Analysis -> Presentation -> Decision.
    *   **Link Analysis:** Crucial for LE/national security, "needles in haystacks," challenging with complex patterns, problematic with multiple devices/warrants but useful for intelligence-led investigations. Infers stateful knowledge.
7.  **Challenges & Overwhelm:**
    *   Need for skilled technical workforce.
    *   Police forces struggling with cybercrime volume.
    *   Forensic Challenges/Obstacles (data alteration, invisibility, copying, shared transit, format differences, layman understanding).
8.  **Cyber Investigations (Examples covered in module):**
    *   Banking heists, WannaCry, TalkTalk, Facebook.

---

## Lecture 3: Storage Media

1.  **Nature of Digital Evidence & Challenges:**
    *   Computer forensics vs. traditional (physical sciences).
    *   Challenges: Too many suspects/evidence, easy contamination, search & seizure complexities, link analysis, geopolitical borders.
2.  **Computer Architecture (Generic Model):**
    *   Components: Input, Output, Storage/Memory, CPU, OS.
    *   Layers: Hardware, OS, Middleware, Applications.
    *   State Information Distribution: CPU, Dynamic Storage (RAM), Backup/Permanent Store, Network.
3.  **Hard Drive Architecture:**
    *   **Drive File Structure:** Hard Drive -> Partition -> File System -> File Record -> Field.
    *   **Magnetic Hard Drives:**
        *   Platters (ceramic/aluminum), Read/Write heads, Actuator (arm), Tracks, Sectors (smallest unit), Cylinders.
        *   Defragmentation importance.
        *   Magnetic field lines & binary encoding.
    *   **Solid State Drives (SSDs):**
        *   Components: Controller, SATA Interface, NAND Flash Memory, SSD PCB.
        *   NAND logic gates ("not and").
        *   Logic and storage arrangement.
4.  **Partitions & Drive Arrangement:**
    *   Conceptual storage: Drive configured into one or more partitions.
    *   Partitions referenced separately by OS, allow multiple logical drives on one physical drive.
    *   Uses: Multiple OS installations.
    *   Partition Table: Holds partition information.
    *   Boot Partition: Takes control on startup.
    *   Tools: GParted, Windows Disk Management, PartitionMagic, Partinfo.
    *   Analysis: Configuration, size, number, total space, unallocated space.
5.  **File Systems (FS):**
    *   Set of data objects, OS stores files with attributes (name, date, location).
    *   Indexes/tables for object location.
    *   **Types:**
        *   FAT (File Allocation Table): FAT12, FAT16, FAT32 (properties, limitations).
        *   NTFS (New Technology File System): (properties, capabilities, compatibility).
        *   exFAT (Extended File Allocation Table): (properties, for flash drives, compatibility).
        *   HFS+ (Hierarchical File System Plus - Mac): (properties, compatibility).
        *   EXT (Extended File System - Linux): ext2, ext3, ext4 (properties, compatibility).
    *   **Terminology:** Mounting (attaching FS), Filesystem (hierarchy/tree).
    *   File Formats: Structured templates, define data start/end, writability.
6.  **Data Storage Concepts:**
    *   **Data Sizes:** Blocks (UNIX), Clusters (Windows).
    *   **Slack Space:** Excess capacity in last block/cluster.
        *   Unallocated space, RAM slack, file slack.
        *   Forensic analysis of unallocated space (diagram).
        *   Data not deliberately hidden, OS doesn't allow direct access, requires imaging.
7.  **Data Erasure & Recovery on Storage Media:**
    *   Magnetic Drives: Feint images, magnetic residue, overwrite patterns.
    *   SSDs: TRIM/UNMAP commands, wear leveling, ATA Secure Erase.
    *   SSD Recovery: "If it's running, don't turn it off...", de-chipping (risks).

---

## Lecture 4: Current Forensic Practice, Evidence Handling

1.  **Obstacles & Complexity (Recap):**
    *   Obstacles to forensic process (alteration, invisibility, etc.).
    *   Increasing complexity: multiple sources (HDD, logs, mobile, smart devices).
2.  **Extracting Evidence:**
    *   Court requirements: Non-invasive imaging, specific warrants.
    *   Focus on embedded devices/smart technology.
3.  **Operational Model of Forensic Computing (Recap):**
    *   Media -> Data -> Information -> Evidence.
    *   Process: Collection -> Examination -> Analysis -> Reporting.
4.  **Integrity of Investigation Aspects:**
    *   Collection, Chain of Evidence, Authentication, Recovery, Verification.
5.  **Evidence Collection:**
    *   Briefing personnel.
    *   Search, recognition, collection, documentation.
    *   Real-time vs. Stored information.
    *   Toolkit ("Go Bag"): Hardware (laptop, cables, storage), Software (imaging, write-blocking), Accessories (notebook, bags, camera, logs).
    *   Small Scale Collection: Imaging on-site/lab, physical (bit-by-bit) vs. logical (file-by-file) imaging.
6.  **Documentation & Records:**
    *   Contemporaneous notes: Scene sketch, persons present, computer details, on-screen display, user remarks, actions & times.
7.  **Chain of Custody (Principle 4 of ACPO):**
    *   Critical for authenticity and admissibility.
    *   Continuity of possession from discovery to court.
8.  **File Imaging and Authentication:**
    *   Identify files needed.
    *   Duplicate for analysis.
    *   Authenticate original and copies (checksums, one-way hash functions like MD5, SHA).
9.  **Verification:**
    *   Secure one-way hash functions (message digests) for data integrity.
    *   Checksums for transmission/storage integrity.
10. **Write Blocking:**
    *   Central requirement: Original evidence must NOT be modified.
    *   Strategies: Hardware jumpers, trusted OS/software, write block tools (hardware/software).
    *   NIST Write Block Tool Specification.
    *   Forensic disk controller examples.
11. **Analyzing Evidence:**
    *   **Logical Analysis (File-by-File):** At application level, convenient, semantic view.
    *   **Time-lining:** Associating timestamps, crucial for correlating events, building activity graphs.
12. **ACPO Guide - Search and Seizure Recommendations:**
    *   Preparation: Review court order, plan.
    *   At Site: Notes, photos, document actions.
    *   Shut Down: If off, leave off. If on, record display, time, processes (MS vs. UNIX shutdown).
    *   Seizure: Labelling, packaging, documentation.
    *   Imaging: Boot to trusted OS, write blocking, image & authenticate, document.
    *   Physical Analysis: Sector-by-sector for hidden/accidental residues.
    *   Logical Analysis: Boot to supported OS, file-by-file for keywords, metadata.
13. **Email Header Analysis:**
    *   Importance for tracing origin (X-Originating-IP).
    *   Using IP lookup tools.

---

## Lecture 5: Data Hiding: Steganography, Steganalysis, Cryptanalysis

1.  **Steganography:**
    *   Definition: "Covered/secret writing," hiding a message within an ordinary object.
    *   History & Uses: Military, diplomatic, corporate espionage, terrorist communication, anti-forensics.
    *   Modern Digital Steganography: Data encrypted then inserted/hidden using algorithms (append, disperse).
    *   Tools: DarkCryptTC, OpenPuff, StegoShare, StegFS (and their supported file types).
    *   Concept: Carrier File + Hidden Message -> Stego File.
    *   Traditional Methods: Hidden text, LSB modification, noise insertion, document layout.
    *   Kerckhoffs' Principle: Security relies on the key; cover medium must be secret.
    *   Transform Domain Techniques: Robust to compression/cropping, may require original image.
    *   Carrier Files: BMP, JPEG, GIF, WAV, MP3 etc. (large carrier, small hidden).
2.  **Steganalysis:**
    *   Definition: Detection of hidden content (not necessarily extraction).
    *   Purpose: Identify tools used, potentially extract message, find deleted stego images, registry leftovers.
    *   Common Hiding Techniques: Appended to file, unused header, dispersed via algorithm (LSB, etc.).
    *   LSB (Least Significant Bit) Manipulation: How it works with pixel color data.
    *   Methods of Detection:
        *   Visual (image distortion), Audible (audio artifacts).
        *   Statistical (pixel/LSB patterns, histogram analysis).
        *   Structural (file property changes: size, date/time, checksum).
        *   Signature-based (patterns specific to stego tools).
    *   Analysis Tools: Hex editors (WinHex), specialized tools (StegSpy for signature ID).
    *   Hiderman Example: Appends data with a "CDN" signature.
3.  **Steganalysis meets Cryptanalysis:**
    *   Goal: Reveal the actual hidden message.
    *   Process: Identify stego program -> Identify algorithm -> Crack/reveal password, seed, or key.
    *   Cryptanalysis Steps: ID program -> ID signature location -> ID password location -> ID hidden message location -> ID encryption algorithm.
    *   Password Attacks: Dictionary attacks, brute-force, password guessing programs (Stegbreak).
    *   Strong Password Practices.
    *   Brute Force for Algorithms: Reverse engineering, common encryption techniques (LSB, masked content, key/password/seed-based algorithms).
4.  **Anti-Forensics & Forensics:**
    *   **Anti-Forensics (Perpetrator techniques):**
        *   Use strong, unique passwords for stego.
        *   Delete original message after hiding.
        *   Remove stego program or run from CD.
        *   Use Alternate Data Streams (ADS).
    *   **Alternate Data Streams (ADS - NTFS feature):**
        *   Allows hiding files/directories within other files' "forks" or "streams."
        *   Invisible to standard Windows Explorer/ `dir` command.
        *   Stream portion often lost in downloads (less for malware distribution, more for post-infection hiding).
        *   Can hide viruses, trojans, stego files; many scanners miss ADS.
    *   **Forensic Investigation of Anti-Forensics:**
        *   Look for stego programs.
        *   Leverage other recovered passwords.
        *   Look for written password hints.
        *   Use ADS detection tools (LNS, LADS, NTFS ADS Check).
    *   Future of Steganalysis: New signature detection, weak stego crackers, password grinders, advanced statistical analysis.

---

## Lecture 6: Reporting Results of Cyber Forensics Investigations

1.  **Importance of Reports:**
    *   Communicate investigation results, including expert opinion.
    *   Court requirements for expert witness reports (fees, case history).
    *   Deposition banks for previous testimonies.
2.  **Report Fundamentals:**
    *   Start with job mission/goal.
    *   Identify audience and purpose.
    *   **Logical Flow:** What asked -> Why qualified -> What did -> What found -> Opinions/Conclusions.
3.  **Types of Reports:**
    *   **Examination Plan:** Questions for testimony, attorney guidance.
    *   **Verbal Report:** Less structured, preliminary, addresses ongoing areas.
    *   **Written Report:** Affidavit/declaration, detailed, documented, supported.
4.  **Guidelines for Writing Reports:**
    *   Hypothetical questions (based on factual evidence, less favored).
    *   Opinions based on knowledge/experience.
    *   Expert witness testimony conditions (special knowledge, qualified expert, certainty, factual basis).
    *   Preliminary reports: Subject to discovery, spoliation risk.
5.  **Report Structure:**
    *   Abstract, Table of Contents, Body, Conclusion, References, Glossary, Acknowledgements, Appendixes.
6.  **Writing Clearly:**
    *   Communicative quality, organization, grammar, vocabulary, punctuation, spelling.
    *   Logical order, build arguments, group ideas.
    *   Avoid jargon, define technical terms, natural language, precision, active voice.
7.  **Layout and Presentation:**
    *   Numbering (decimal, legal-sequential).
    *   Supporting material (figures, tables).
    *   Consistent formatting.
    *   Explain examination/data collection methods.
    *   Include calculations (e.g., hashing algorithms).
    *   Address uncertainty and error analysis.
    *   Explain results and conclusions clearly.
    *   Provide references and appendixes.
    *   **Standard Report Sections (Example):**
        *   Executive Summary
        *   Objectives
        *   Computer Evidence Analyzed
        *   Relevant Findings
        *   Supporting Details (vital files, string searches, emails/URLs)
        *   Investigative Leads
        *   Additional Subsections (Attacker Methodology, User Applications, Internet Activity, Recommendations).
8.  **Sources of Information & Audience:**
    *   Sources: Personal observations, applications, network/host devices, forensic tools.
    *   Audience: Executives, IT, Legal, Marketing, Regulators, Law Enforcement.
9.  **Key Information to Include:**
    *   Examiner bio/background, tools utilized, evidence items, forensic analysis, tool output.
10. **Generating Reports with Software Tools:**
    *   FTK, EnCase, AXIOM, Autopsy.
    *   Common formats: Plaintext, Word Processor, HTML.
    *   Process: Create case, add evidence, analyze (images, encryption, keywords), create bookmarks, generate report from bookmarks.
11. **Types of Witnesses:**
    *   **Technical Witness:** Testifies on facts experienced, no opinions.
    *   **Expert Witness:** Third party whose testimony is accepted, must be qualified, can issue opinions/conclusions within their expertise.

---

## Lecture 7: Advanced Digital Forensics Practice

1.  **Basic Forensic Work Process (Recap):**
    *   Identification (trace evidence).
    *   Preservation (safeguard from modification/deletion).
    *   Collection (order of volatility, chain of custody).
    *   Examination (tools/techniques to discover/extract).
    *   Analysis (correlate with other data).
    *   Presentation (clear, concise, unbiased reporting, testimony).
2.  **Timelining:**
    *   Visual correlation of evidence over time.
    *   Categorizes evidence by date, helps visualize investigation.
3.  **Forensic Data Carving:**
    *   Identifying/recovering files based on file format analysis (headers/footers).
    *   Finding hidden/deleted files in unallocated clusters, slack space.
4.  **Addressing Data-Hiding Techniques:**
    *   File Manipulation (names, extensions, hidden properties).
    *   Disk Manipulation (hidden partitions, marking bad clusters).
    *   Encryption & Obfuscation (bit-shifting, steganography).
5.  **Specific Hiding Locations & Techniques:**
    *   **Hidden Partitions:** Deleting references, using disk-partitioning utilities.
    *   **Marking Bad Clusters:** Placing data in free space then marking as bad (common in FAT).
    *   **Slack Space:** Leftover storage (RAM slack, file slack).
    *   **Bit-shifting:** Altering byte values to disguise files.
6.  **Steganography (Recap & Tools):**
    *   Hiding information in image/text files (S-Tools, DPEnvelope, etc.).
7.  **Examining Encrypted Files & Password Recovery:**
    *   Challenges: Difficult without password.
    *   Methods: Key escrow, password cracking (dictionary, brute-force, profile-based).
    *   Tools: PRTK, Advanced Password Recovery Software Toolkit, LC5.
8.  **Graphics File Forensics:**
    *   **Recognizing Graphics Files:** Bitmap, vector, metafile.
    *   **File Formats:** Standard (GIF, JPEG, TIFF, BMP, HPGL, DXF) and nonstandard (TGA, PSD, AI, SVG).
    *   **Data Compression:** Lossless (reduces size, no data loss, e.g., GIF, PNG via Huffman/Lempel-Ziv-Welch) vs. Lossy (discards data, e.g., JPEG via VQ).
    *   **Locating & Recovering:** OS tools vs. forensic tools (image headers, reconstruct fragments).
    *   **Identifying Fragments (Carving/Salvaging):** From slack/free space.
    *   **Repairing Damaged Headers:** Using good header samples (e.g., JPEG: FF D8 FF E0 00 10 JFIF).
    *   **Reconstructing File Fragments:** Locate clusters, export, determine sequence, copy, rebuild header.
    *   **Analyzing Headers:** Hex editors for unknown file types.
    *   **Viewing Tools:** ThumbsPlus, ACDSee, IrfanView; GUI forensic tools (ProDiscover, EnCase, FTK).
9.  **Steganography in Graphics Files & Steganalysis:**
    *   Hiding info in images (insertion, hidden data not displayed).
    *   Steganalysis Tools: Detect variations, compare to known good/bad, mathematical calculations, hash values.
10. **Program Execution Artifact Investigations:**
    *   Identify when/how often programs were executed, by whom.
    *   Information on deleted/uninstalled programs.
    *   Proof of data in no-longer-available locations, last launch times.

---

## Lecture 8: File Systems Investigation

1.  **Understanding File Systems:**
    *   OS "road map" to data, determines storage structure.
2.  **Boot Sequence:**
    *   CMOS (system config, date/time).
    *   BIOS (hardware-level I/O programs).
    *   Bootstrap Process (ROM instructions, CMOS setup).
    *   Modifying CMOS to boot from forensic media.
3.  **Windows Startup (NT and Later):**
    *   Steps: POST -> Initial Startup -> Boot Loader -> Hardware Detection -> Kernel Loading -> User Logon.
    *   Startup Files (XP): NTLDR, Boot.ini, BootSect.dos, NTDetect.com, etc.
    *   Contamination Concerns: Starting XP NTFS changes last access timestamps.
4.  **Microsoft File Structures:**
    *   FAT & NTFS.
    *   Sectors grouped into Clusters (storage allocation units).
    *   Clusters = Logical Addresses; Sectors = Physical Addresses.
5.  **Disk Partitions & MBR:**
    *   Logical drives, hidden partitions/voids (partition gaps).
    *   Disk editors for viewing/modifying partition tables.
    *   Master Boot Record (MBR): Stores partition info (location, size); can be replaced/interfered with.
6.  **FAT Disks:**
    *   Origin (floppy disks), structure (filenames, timestamps, starting cluster).
    *   FAT12, FAT16, FAT32.
    *   Drive Slack: Unused space in a cluster (RAM slack, File slack).
7.  **NTFS Disks:**
    *   Improvements over FAT: More info per file, journaling.
    *   Partition Boot Sector, Master File Table (MFT - metadata for all files).
    *   Reduced slack space, Unicode support (UTF-8/16/32).
    *   NTFS File Attributes: Resident (in MFT) vs. Nonresident (outside MFT, uses inodes), LCN/VCN.
    *   FAT32 vs. NTFS Comparison Table.
8.  **Windows Registry:**
    *   Database for hardware/software config, network connections, user preferences.
    *   Valuable evidence source.
    *   Tools: Regedit (9x), Regedt32 (2000/XP).
    *   Terminology: HKEY, Key, Subkey, Branch, Value, Default Value, Hives.
9.  **Macintosh File Structure & Boot Process:**
    *   Mac OS X (Darwin core, BSD UNIX layer).
    *   HFS (Hierarchical File System), HFS+ (Extended Format File System).
    *   File Manager, Finder.
    *   Older Mac OS: Data Fork & Resource Fork.
    *   Volumes, Allocation & Logical Blocks, Clumps, EOF Descriptors.
    *   Boot Tasks: Open Firmware, self-test, OS start, startup disk location, system files, extensions, Finder.
    *   Older Mac OS structures: Boot Blocks, MDB/VIB, VCB, Extents Overflow File, Catalog, Volume Bitmap, B*-Tree.
10. **UNIX/Linux Disk Structures & Boot Processes:**
    *   File Systems: Ext2fs, Ext3fs (journaling).
    *   Inodes: Info about files/directories, pointers, link count.
    *   **UNIX/Linux Components:**
        *   Boot Block (bootstrap code).
        *   Superblock (disk geometry, space, 1st inode).
        *   Inode Blocks (data after superblock).
        *   Data Blocks (directories/files).
    *   Bad Block Inode, `ls` command, Continuation Inode.
    *   Inode Pointers (direct, indirect, double-indirect, triple-indirect).
    *   Boot Process: Firmware -> RAM -> Hardware Check -> Boot Program -> Kernel Load -> Device ID.
    *   Kernel Tasks: Single/multiuser mode, startup scripts, root/swap/dump ID, hostname, consistency checks, services.
    *   Loaders: LILO (Linux Loader), GRUB (Grand Unified Boot Loader).
    *   Drive/Partition Schemes: /dev/hda, /dev/sda, etc.

---

## Lecture 9: E-mail Investigations

1.  **Role of E-mail in Investigations:**
    *   E-mail scams (phishing, spoofing), HTML format vulnerabilities.
    *   Nigerian Scam (419), fraud.
2.  **Client/Server Roles in E-mail:**
    *   Environments: Internet, LAN/MAN/WAN.
    *   Client/Server architecture, protected accounts.
    *   Naming conventions (corporate vs. public).
3.  **Investigating E-mail Crimes/Violations:**
    *   Goals: Identify perpetrator, collect evidence, present findings, build case.
    *   Common e-mail related crimes.
4.  **Examining E-mail Messages:**
    *   Accessing victim's computer/client/PST files.
    *   Copying/printing messages, including headers.
    *   Handling deleted e-mails.
5.  **Viewing & Examining E-mail Headers:**
    *   Finding headers in various clients (GUI, command-line, web-based).
    *   Information in headers: Return path, recipient, sending service, IP addresses, server names, unique message numbers, timestamps, attachments.
6.  **Additional E-mail Files:**
    *   Client-side storage (.pst, .ost for Outlook).
    *   Electronic address books.
    *   Web-based e-mail (browser cache, IM services).
7.  **Tracing E-mail Messages:**
    *   Contacting server administrators.
    *   Finding domain POC (ARIN, InterNIC).
    *   Verifying with network e-mail logs.
8.  **Network E-mail Logs:**
    *   Router logs (incoming/outgoing traffic).
    *   Firewall logs (filtered traffic).
9.  **Understanding E-mail Servers:**
    *   Software using e-mail protocols, log maintenance.
    *   Storage: Database, flat file.
    *   Log types: Default/manual, continuous/circular.
    *   Log information: Content, IPs, timestamps, system-specific info.
    *   Server-side recovery of deleted e-mails.
    *   **UNIX Logs:** sendmail.cf, syslog.conf, maillog.
    *   **Microsoft Exchange Logs:** Information Store files (.edb, .stm), transaction logs, checkpoints, temporary files, tracking.log, diagnostic logs (Event Viewer).
10. **Specialized E-mail Forensics Tools:**
    *   Examples: FTK, ProDiscover, FINALeMAIL, DBXtract, Paraben E-Mail Examiner.
    *   Capabilities: Find database files, personal files, offline storage, log files.
    *   Using FTK to recover e-mail (indexing, dtSearch).
11. **Carving E-mail Messages:**
    *   Using hexadecimal editors for non-standard/unsupported formats.
    *   Mbox format (flat plaintext).
    *   MIME format.
12. **E-mail Forensics Case Study (Spoofing Example):**
    *   Analyzing headers to detect spoofed fields by comparing `From:` with `Received:` fields.

---

## Lecture 10: Network Forensics and Cyber-Incident Investigation

1.  **Internet & Networking Fundamentals:**
    *   Internet as a collection of networks, ISP, DNS.
    *   OSI and TCP/IP models.
    *   IP Addressing (IPv4, classes, NAT).
2.  **Key Network Devices as Evidence Sources:**
    *   Switches, Routers, Firewalls (connection logs, remote access logs), NIDS/NIPS, Web proxies, Domain controllers, DHCP servers, Application servers.
3.  **Network Forensics Overview:**
    *   Systematic tracking of incoming/outgoing traffic.
    *   Identifying attack methods, intruder trails, cause of abnormal traffic.
4.  **Live Acquisitions:**
    *   Importance for active intrusions (footprints in RAM/processes).
    *   **Order of Volatility (OOV):** How long data persists (Cache > RAM > Paging File > HDD > Remote Logs > Archive Media). Prioritize collection accordingly.
    *   Steps: Bootable forensic CD, log actions, copy RAM, forensic hash.
    *   Windows RAM capture tools (Mantech Memory DD, FTK Imager).
5.  **Standard Procedures for Network Forensics:**
    *   Use standard installation images for comparison.
    *   Isolate compromised systems.
    *   Retrieve volatile data, acquire drives.
    *   Compare forensic image to original installation.
6.  **Reviewing Network Logs:**
    *   From network servers, routers, firewalls, web servers.
    *   Tools like `tcpdump` for traffic examination.
7.  **Network Forensics Tools:**
    *   **Sysinternals Suite:** RegMon, Process Explorer, Handle, Filemon.
    *   **PsTools Suite:** PsExec, PsGetSid, PsKill, etc.
    *   **Packet Sniffers:** Monitor network traffic (e.g., Wireshark, Snort, Tethereal/tshark).
        *   PCAP format.
        *   Analyzing TCP flags.
        *   Wireshark: Capture/analysis, finding attacker IPs, filtering (e.g., HTTP POST), finding specific packets.
        *   NetworkMiner: Alternative analysis tool.
8.  **Security Operations Center (SOC):**
    *   Team, technologies, frameworks for enterprise security.
    *   Objective: Detect, investigate, triage, respond to threats.
    *   Key steps: Gather evidence, enrich with intelligence, pivot/filter, integrate lessons.
    *   Challenges: Advanced Threat Actors, lack of visibility, time-intensive analysis, alert fatigue.
    *   Evidence sources for SOC: Network traffic, firewall logs, access logs, DNS, proxy, web, IDS, threat intelligence.
