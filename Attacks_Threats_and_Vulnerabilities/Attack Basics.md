# Attack Basics

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

