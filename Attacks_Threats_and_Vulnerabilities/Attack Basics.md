<!-- omit in toc -->
# Attack Basics

<!-- omit in toc -->
## Topics

- [Malware](#malware)
- [Viruses](#viruses)
  - [Virus Classifications](#virus-classifications)
  - [Virus Characteristics](#virus-characteristics)
- [Worms](#worms)
- [Trojans](#trojans)
- [Rootkits](#rootkits)
- [Logic Bombs](#logic-bombs)
- [Bots](#bots)
- [Crypto-Malware](#crypto-malware)
- [Potentially Unwanted Programs (PUPs)](#potentially-unwanted-programs-pups)
- [Spyware](#spyware)
- [Adware](#adware)
- [Cryptomining Software](#cryptomining-software)
- [Physical Attacks](#physical-attacks)
- [Adversarial Artificial Intelligence (AI)](#adversarial-artificial-intelligence-ai)
- [Password Attacks](#password-attacks)
- [Birthday Attacks](#birthday-attacks)
- [Downgrade Attacks](#downgrade-attacks)

## Malware

- Software designed to harm a user's computer or data.
- Target is not only information stored locally but also other resources and other computers.
- Typically takes advantage of system vulnerabilities, this makes it more dangerous and allows it to spread more effectively
- Symptoms of infection:
  - **Memory** - after execution, it can reside in memory as a rogue process.
  - **Registries** - often targeted by malware. Malware can take advantage of registry entries to make sure that executables are run each time the computer starts up.
  - **Macros** - give malware the ability to automatically create instructions when documents launch. Usually in Office applications.

## Viruses

A **virus** is a program or piece of code that runs on a computer, often without the user being aware of it or the user's permission
- Designed to attach themselves to other code and replicate.
- They often make copies of themselves and spread through networks when an infected file executes or launches

### Virus Classifications

- **Resident virus**
  - Lives in memory
  - Loaded each time the system is started and can infect other areas
  - Need to be called up from some kind of storage

- **Nonresident Virus**
  - Need to first be executed
  - Looks for targets locally and across the network and then infects and exits
  - Does not remain active

- **Boot sector virus**
  - These are stored in the first sector of the hard drive so that as soon as the computer boots, the virus loads into memory
  - Virus is loaded before the OS starts
  - Where more common back in the day of floppy disks

- **Macro virus**
  - This one is inserted into a Microsoft Office document and emailed to unsuspecting users
  - Uses macros and executes when the document opens

### Virus Characteristics

- **Program and file infecting virus**
  - Most common type of virus
  - Virus infects executable program files and is active in memory
  - Binary pattern is essentially like a fingerprint

- **Polymorphic Virus**
  - This virus can change form or signature each time it gets executed to avoid detection
  - Each time it infects a new file or system, it changes its code
  - Detecting these is harder

- **Armored Virus**
  - These make it hard to analyze functions, creates a layer of "armor" around the virus
  - They try to prevent disassembly and debugging, making it harder for researchers to analyze code and come up with better countermeasures

- **Stealth Virus**
  - This virus lives in memory
  - Use techniques to avoid detection, things like removing itself from an infected file or masking the file size
  - They can remove itself and copy itself to a different location

**Multipartite Virus**
  - Infects executable files and also attacks the master boot record of the system
  - If the boot sector and the infected files are not cleaned, the files can easily be infected again

## Worms

- Similar in function and behavior to viruses but they are self-replicating and do not need a host file
- Worms take advantage of security holes in applications or operating systems, then they find other systems running the same software and automatically copies itself to the new host.
- Main difference between viruses and worms is that worms do not need to be attached to files and programs and can reproduce on their own
- Common methods of replication
  - Email
  - Network
  - Internet

## Trojans

- Programs pretending to be useful applications
- They do not replicate themselves like viruses do but are just as destructive
- They can do things without the user's knowledge (collecting and sending data)
- They are classified by their payload or function. The most common are:
  - Backdoor - open an entry into the system
    - Also known as ***Remote Access Trojan (RAT)***
    - Allow a remote attacker to get control of the system
  - Downloader - download other malicious software to the system
  - Infostealer - steal information from the infected machine
  - Keylogger - capture and send keystrokes typed on the infected machine

## Rootkits

- A piece of software that can be installed and hidden on a computer to compromise the system and get escalated privileges
- Let's the attacker gain root or privileged access to the computer
- Can be included as part of
  - Software packages
  - Unpatched vulnerability
  - Downloaded and installed by users
- Antivirus cannot always detect rootkits because they run in the background

## Logic Bombs

- A virus or Trojan horse designed to take malicious actions when a specific event happens or after a specific period of time

## Bots

- An automated computer program that needs no user interaction
- Bots are systems that fall under the control of outside sources
- Often used to spread spam or viruses
- ***Botnet*** is a large number of computers that forward transmissions to other computers on the internet
  - Also called a ***zombie army***
  - Often used to do Distributed Denial of Service (DDoS) attacks

## Crypto-Malware

- Designed to find potentially valuable data on a system and uses cryptography to encrypt the data to prevent access
- You need the decryption key to access the data
- Often associated with ***Ransomware***
  - Form of malware that encrypts data and ask for ransom money
  - Decryption key is given only after the ransom is paid

## Potentially Unwanted Programs (PUPs)

- A program that is unwanted even though the user consented to download it
- Example -
  - Spyware
  - Adware
  - Dialers

## Spyware

- Often included with commercial software downloaded from the Internet
- shows behaviors like advertising, personal information collection, changing computer configuration without permission
- Hints that spyware might be present:
  - System slow down when browsing the Internet
  - Windows desktop is slow coming up
  - Clicking on a link does nothing or takes you somewhere else
  - Browser home page changes and you can't reset it
  - Websites are automatically added to your favorite lists

## Adware

- Form of spyware that gives advertisers an online way to make a sale
- Sometimes install tracking software on the system

## Cryptomining Software

- Software that uses compute resources to mine cryptocurrencies
- These make heavy use of the CPU
- Malware has been used to deliver malicious cryptomining software to user the resources of others (this is called ***cryptojacking***)

## Physical Attacks

- Use things like USB drives loaded with malware to infect machines
- Can also use malicious cables and plugs, mobile device charging cables and wall or power adapters
- ***Skimming***
  - Attack type that involve copying data from a credit or debit card by using a specialized terminal
  - Often done in compromised ATMs

## Adversarial Artificial Intelligence (AI)

- Uses things like Machine learning to solve problems and challenges
- Attackers can corrupt the data fed to these algorithms and have negative impacts

## Password Attacks

- Common methods of attacking passwords
  - **Dictionary Attack**
    - Use every word in the dictionary to gain access
    - Can be automated by software tools
    - Work best on simple passwords
  - **Brute-force attack**
    - Relies on cryptanalysis or hashing algorithms to do key searches
    - Can crack short password more quickly than dictionary attacks
    - Take a lot of time and computing power when cracking complex passwords because tries all possible combinations of letters, numbers and symbols
  - **Spraying**
    - Tries to avoid account lockout by spreading the use of a single password attempt across multiple accounts
    - A slow approach but targets more accounts at once
  - **Rainbow table**
    - Think of this as a table of precomputed hash values for every possible combination of characters
    - This attack can be done offline
    - The attacker only needs to search the rainbow table for the required password hash
    - Salting (adding random data to the hash) can protect against this attack

- Passwords should **never** be stored unencrypted in plaintext
- Passwords are stored as hashes
  - A hash is a one-way function, this means you can't turn a hashed value into a password
  - If you hash a password, you can compare the output to a previously hashed password

## Birthday Attacks

- A cryptographic method of attack against a secure hash
- Finds collisions within hash functions
- A more efficient method of brute-forcing one-way hashing

## Downgrade Attacks

- Often a result of security configurations not being updated
- An attacker can force the use of an older and less secure version of a protocol
- This downgrade of protocol versions make cryptographic attacks easier
