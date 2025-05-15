# "Computer Forensics - PRACTICE" Exam Paper

## Section A

### Q1

1. It captures addresses and ports of both parties, which can identify sources and services. This can be used together to verify other sources.
2. If the data is unencrypted, the content of communication can be extracted and used as direct evidence of crime.
3. Network logs will have timestamp, which can be used to reconstruct the events.
4. It can be done in real-time, even before arresting the criminal and seize their devices. This can help understanding the events in progress.
5. If LE follows standard procedures, the data is raw and unaltered, suitable for presentation in court.

### Q2

1. SHA-1 takes a series of data and output a hash, this process is one way, one cannot infer the data from the hash. This can ensure the hash will not leak original data.
2. By calculating the hash of the original forensic image of the storage media, and compare it with possible copies, it can be guaranteed the copy is genuine and unaltered.
3. Some known illicit materials or programs can have known SHA-1 hashes. This can quickly identify them.
4. SHA-1 itself is moderately resistant to collision. Can prevent false positive. But SHA-256 and SHA-512 are superior here.

### Q3

#### Q3.1

Chain of custody means the record of actions taken on the digital evidences, including who handled the evidence, when, how, why and what has been done to the evidence.

It ensures the evidence is properly handled, not altered from the moment is was seized until it is presented in court. It makes forensic experts take responsibility for the integrity of data. 

#### Q3.2

1. They need to prove they are competent by showing their experiences and CV.

2. They should have a comprehensive record of what they've done to the evidence, and show the record in court.
3. They should show that they follow standards, like ACPO guides. They can include steps promoted by ACPO guides in their report shown in court.

#### Q3.3

Order of Volatility means the order of collecting evidence should be based on the volatility of the data. The volatility is determined by how fast the data can be lost if not collected.

OOV means the most volatile data should be collected first. CPU registers and cache is the most volatile, followed by RAM and in-ram cache like ARP tables. They can be lost over time or when the computer is shutdown. So a memory dump should be created as soon as possible. Data stored on disk and network topology are less volatile. So the disk image can be copied later.

1. CPU registers and cache: lost extremely quickly
2. RAM: can lost over time or when power off
3. Swapfile and paging files: can change over time when the computer is on
4. HDD/SSD: non-volatile
5. Logs on remote system: non-volatile
6. Archive media such as dvds: non-volatile

### Q4

#### Q4.1

Live acquisition means collecting evidence from a device that is powered on, with data left in RAM.

Post mortem acquisition means collecting evidence from a device that is powered off. Data in RAM has been lost.

#### Q4.2

**Live acquisition:**

**Advantages:**

1. can collect more data because of the ability to access RAM. Can collect process lists and dump the memory.
2. direct insights into the system's active state.
3. can bypass disk encryptions.
4. can still collect all the data that post-mortem acquisition can collect.

**Disadvantages:**

1. need more effort to maintain forensic soundness, as running forensic software on the device may change its state.
2. the device may have specific software running to interference with forensic software.
3. require more skills and extra software

**Post mortem acquisition**

**Advantages:**

1. easier to maintain forensics soundness. If the write blocker is used, it would be difficult to alter the system's state.
2. more available software and more established process.

**Disadvantages:**

1. cannot bypass full disk encryption
2. cannot collect RAM data, hard to get insights into the system's active states.

#### Q4.3

When the disk is fully encrypted, and the encryption key is unknown, and the encryption itself does not have exploitable vulnerability.

# "Computer Forensics" (Actual Past Paper) Exam Paper

## Section A

### Q1

forensic methodology is a set of structured and systematic procedures or principles to follow during forensic investigations. It ensures the investigation process is reliable and legally defensible. Examples include CFSAP model and procedures listed in ACPO guidelines.

1. It is essential for the investigation to be admissible in court.
2. It ensures the results are reliable, not tampered with.
3. It offers steps to follow, making the investigation process more streamlined.
4. It can be used to train forensic experts consistently.

- Different goals: legal investigation wants to find evidence supporting the existence of breaches of laws. Internal investigations seek evidences violating company policy, like security incidents, IP theft.
- Different requirements: legal investigation needs to be admissible on court, so the process should follow strict rules. internal investigation is more flexible here, but still should follow relevant laws.
- Different scope: legal investigation only tries to collect evidence based on the warrants. internal investigation has more flexibility especially on company-owned devices.
- Different outcome: legal investigation needs to report on court, which may influence the outcome of a legal case. Internal investigation may need to report to HR or management department, may lead to firing misconducting employee or even legal cases.

### Q2

Four key elements include: Identification, Preservation, Analysis, Presentation. “Secure” includes indentification and preservation.

Source 1: Hard Disk.

1. Record the scene, including the location of the device and its state
2. Ensure the device is turned off.
3. Remove the disk from the device.
4. Use a write blocker to connect to the disk.
5. Create a bit-to-bit copy of the disk.
6. Compute the hash of the copy, record the hash.
7. For each step above, record who, when and how.

Source 2: RAM

1. Record the scene, including the location of the device and its state
2. Ensure the device is on
3. Connect the device to an external drive or a network drive
4. Create a dump of RAM and store it on that drive
5. Compute hash for the dump
6. For each step above, record who, when and how.

### Q3

1. They use different interfaces. This means they may not be able to share the same write blocker. So we should use the correct write blocker for each one.
2. Due to the existence of TRIM command on SSDs, which does not immediately erase the data, it may be possible to recover data from SSDs. For HDD, it does not have similar command.
3. SSD is usually faster, which may save time when creating a bit-for-bit forensic image.
4. SSD’s controller is usually more advanced, some even supports built-in full disk encryption. This may make live acquision necessary.
5. Generally, they are both non-volatile storage and bit-for-bit image can be created from either of them. So most steps will remain the same.

### Q4

Full drive encryption means all the contents on the disk is encrypted. When a disk with FDE enabled captured powered off, without a decryption key or known exploit of the encryption algorithm, it is impossible for forensic experts to decrypt it, so a meaningful forensic image cannot be created from this disk. Steganography focus on hiding possible evidence in other seemingly unrelated data. It tries to prevent forensic experts to even realize the existence of certain evidence.

Similarities:

1. Both aim to prevent forensic experts from finding the evidence of crime.
2. Both rely on some degree of secrecy. FDE needs the decryption key to be secret. Steganography needs the method to hide information to be secret.

Differences:

1. FDE does not hide the existence of data, it just prevents investigators from accessing its contents. Steganography tries to hide the existence of data.
2. In live acquisition, FDE may be bypassed, but Steganography will still hind the existence of evidence.
3. The encryption usually does not increase the size of data, it just turns data into unreadable format. Steganography may embed data into a much larger carrier file.
4. Steganalysis may reveal the method used for steganography, but full drive encryption is more difficult to crack. 

## Section B

### Q1

1. The contents of storage device that may be presented on court should not be changed during forensics.
   - This means the evidence should be original and authentic. Any modification may invalidate the evidence.
   - Write blocker may be used.
2. Someone must prove they are competent enough to access the original data, and should explain the reason and the implication.
   - This means only forensic experts can access the original data. It can avoid unprofessional handling of evidence.
   - The investigator need to write down their experiences on the report presented on court, including reasons and impact behind their actions to the original data.
3. Any process applied on the digital evidence should be recorded, and should be possible for 3rd party to follow and replicate.
   - This means there will be audit records of everything done by the experts to the evidence. This ensures chain of custody.
   - The investigator should record when, how, who, what when they take any action to the evidence, including when secure and analysis.
4. The case officer is responsible for the above principles to be followed during investigation.
   - This means if any principle is violated, the case officer may face punishment. They need to monitor the whole process to prevent things from going wrong.
   - There will be a case officer assigned to each case, monitoring the whole investigation and ensure they follow the ACPO guide.

### Q2

S1: a company employee download a confidential document which they do not have the permission to access by using other's credentials. Forensic investigator may try to find the log in record. 

S2: a company employee download a confidential document onto their computer and try to sell it online. Forensic investigator may need to find the material on the suspect's computer or records of selling.

S3: a company employee intentionally delete all the records from company database without permission, causing chaos. Forensic investigator may try to find the connection record. 

S3A: a company employee selling the accounts and passwords in the company's database.

### Q3

1. The extensive logging may be able to collect more detailed evidence than post-mortem acquisition. As some user activity may not be originally recorded. 
2. The logs are directly linked to the user, making it easy to link the actions with the person.
3. The logs have timestamps, can be used to reconstruct timeline.
4. The logs are real-time, which means the suspect can not delete it or hide it.

But ethically:

1. May capture too much unrelated data, out of the scope of warrant.
2. May violate privacy rights.
3. May cause public backslash if widely used.