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
4. SSD’s contorller is usually more advanced, some even supports built-in full disk encryption. This may make live aquision necessary.
5. Generally, they are both non-volatile storage and bit-for-bit image can be created from either of them. So most steps will remain the same.

## Section B