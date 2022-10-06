# Threat Actors, Vectors, and Intelligence Sources

## Topics

  - [Threat Actors](#threat-actors)
  - [Vectors](#vectors)
  - [Threat Intelligence and Research Sources](#threat-intelligence-and-research-sources)


## Threat Actors

- **Threat Actor** - an individual, a group, or entity that contributes to an incident. Simply a person or entity that executes a given threat.

- **Threat Actor Attributes**
  - ***Relationship*** - can be internal or external to the organization, they might even come from a partner
  - ***Motive*** - can be either accidental or driven by financial gain or ideological differences
  - ***Intent*** - Threat could be malicious, looking to destroy data or steal valuable information
  - ***Capability*** - Things like technical ability, financial means, access, political and social support, and persistence

- **Threat Actor Types**
  - ***Common Threat Actors***
    - **Script kiddies**
      - Not a lot of knowledge or skills but they simply run exploits that others have developed
      - Cannot write complex code or know how to program
      - Use readily available exploits and information
      - Often associated with website defacement attacks, DoS, Trojans and remote access tools
    - **Insiders**
      - Often employees that are either not aware of security policies or just ignore them
      - Deliberate malicious insider threats are also possible
      - Insider threat is one of the most difficult things to protect against
    - **Hacktivists**
      - Use digital tools for malicious intent, based on political, social or ideological reasons
    - **Criminal syndicates**
    - **Competitors**
      - Anti-competitive practices and industrial espionage
      - Usually are looking to grab information to gain an advantage or steal trade secrets and intellectual property
    - **Nation-state actors**
      - The most sophisticated threat actor
      - Advanced Persistent Threats (APTs) are associated with this threat actor
      - They are often "low and slow"
      - The goal is to infiltrate networks and remain inside undetected to exfiltrate information over a long period of time
  - ***Hackers***
    - Fundamentally, a hacker is someone who uses their knowledge of and skills to break, tamper or gain unauthorized access to systems and/or networks
    - ***Types***
      - **Black Hat (unauthorized)** - hackers involved with criminal activities or malicious intent
      - **White Hat (authorized)** - or Ethical Hackers, hired as penetration testers with permission to attack or test system security
      - **Gray Hat (semi-authorized)** - Falls somewhere in the middle of black and white hat.

## Vectors

- **Attack Vectors** - is the path they take to execute attacks
- **Common Attack Vectors**
  - Direct Access
  - Wireless
  - Removable media
  - Cloud
  - Email
  - Improper Usage
  - Equipment damage, loss, or theft
  - Supply Chain

## Threat Intelligence and Research Sources

- Organizations rely on threat intelligence data for both preventive and response measures
- **Sharing Centers**
  - Promote threat information across different industry sectors
  - Facilitate collaboration between private and public groups
  - National Council of ISACs (Information Sharing and Analysis Centers) have more than 20 member ISACs in multiple industries
  
- **Open-source Intelligence (OSINT)**
  - Name given to information that is available for collection from publicly available information sources
  - Attackers can also leverage OSINT to advance their attacks (identify and explore their targets)
  - Threat intelligence platforms can collect data from different OSINT sources and the aggregate and correlate the data
  - Main drawback of OSINT: information overload
  - **Common OSINT sources**
    - **Vulnerability Databases**
      - Provide data for publicly known vulnerabilities
        - [MITRE](https://cve.mitre.org/)
        - [CVE Details](https://cvedetails.com/)
        - [VulnDB](https://vulndb.cyberriskanalytics.com/)
    - **Adversary Tactics, Techniques and Procedures (TTPs)**
      - [MITRE ATT&CK](https://attack.mitre.org/) gives us attack methods and activities associated with specific threat actors
    - **Dark Web**
      - Can't be accessed like regular websites, requires use of special software (TOR)
      - Where attackers live and operations of questionable legality happen
    - **Indicators of Compromise (IOC)**
      - Serve as evidence or components that point to security breaches or events
      - Things like malware signatures, IP addresses, domain names, and file hash values
    - **Automated Indicator Sharing (AIS)**
      - Initiative that enables the exchange of cybersecurity threat indicators. 
      - Uses two important standards
        - **Structured Threat Information eXpression (STIX)** - A standardized and structured language that represents threat information in a flexible, automatable, and easy to use way
        - **Trusted Automated eXchange of Indicator Information (TAXII)** - specification for machine-to-machine communication the let's organizations share security information
    - **Threat Maps**
      - Give us a real-time look at cyber-attacks happening around the globe
      - Example: [Kaspersky Map](https://cybermap.kaspersky.com/)
    - **File/code repositories**
      - Online code repositories like GitHub that are publicly available
      - These provide opportunities to obtain open-source code and also specific threat research and information gathering
    - **Other Sources**
      - Television
      - Newspapers and magazines
      - Professional publications
      - Academic publications
      - Photos
      - Geospatial information
      - Vendor websites
      - Conferences
      - Requests for comments (RFCs)
      - Social media