<!-- omit in toc -->
# Enterprise Security Concepts

<!-- omit in toc -->
## Topics

- [Configuration Management](#configuration-management)
- [Data Confidentiality](#data-confidentiality)
  - [Data Loss Prevention](#data-loss-prevention)
  - [Cloud Access Security Brokers](#cloud-access-security-brokers)
  - [Encryption and Data Obfuscation](#encryption-and-data-obfuscation)
  - [Rights Management](#rights-management)
  - [Hardware Security Module (HSM)](#hardware-security-module-hsm)
  - [Encrypted Traffic Management](#encrypted-traffic-management)
- [Data Integrity](#data-integrity)
- [Data Availability](#data-availability)

## Configuration Management

- Process of identifying, controlling and auditing the deployment and changes made to an established baseline
- Benefits:
  - Improved efficiency and effectiveness
  - Strong security controls
  - Adherence to best practices
- Processes:
  - Provisioning new systems
  - Replicating environments
  - Disaster Recovery
  - Onboarding and employee training
  - Stability through change management
  - Ensuring hardened and secure systems
- ***Baseline Configuration***
  - Includes the configurations and settings that are set as the foundation for similar systems
  - Without an established baseline configuration you are more prone for errors, malfunctions, and security breaches to happen
- **Documentation**
  - All of the following should be properly documented
    - **Baseline configuration** - documented so that others are able to easily replicate the configuration
    - **Diagrams** - important for networks and complex systems. Things like network maps, cabling and wiring diagrams, application configuration and connections.
    - **Standard naming convention** - agreed-upon method of naming assets is important for everyday management and in emergency situations
    - **Internet Protocol (IP) Schema** - Keeps track of IP address assignments to systems as they are added to the network
- **OS Hardening**
  - Configuring log files and auditing
  - Change default admin accounts names and default passwords
  - Configure account lockout and password policies
  - File-level security and access control mechanisms

## Data Confidentiality

- Confidentiality is all about protecting data and making sure only those authorized to view it are allowed to do so
- Preventing theft or disclosure of data - both intentional or unintentional

### Data Loss Prevention

- Protects confidentiality or sensitive information with content analysis
- Content analysis techniques
  - Rule-based
  - Data-based
  - Exact file or data matching
  - Partial document matching
  - Statistical analysis
- A way of detecting and preventing confidential data from being exfiltrated physically or logically from an organization by accident or on purpose
- Designed to detect and prevent unauthorized use and transmission of confidential information based on three states of data:
  - In use
  - In motion/transit
  - At rest

### Cloud Access Security Brokers

- ***Cloud Access Security Broker (CASB)***
  - term that describes a cloud security layer focused on visibility, compliance, data security and threat protection
  - Designed to understand these situations and provide dynamic policies to control and respond to several circumstances
  - Work as part of the DLP program and serve as extension, applying DLP policies to the cloud

### Encryption and Data Obfuscation

- Sensitive data should be encrypted at all times whenever possible
- Three categories based on the state of data
  - **Data at rest** - stored or resting state on some type of persistent storage (hard drives). Symmetric encryption is used here.
  - **Data in Transit** - data moving across a network or from one system to another. Transport layer encryption like SSL/TLS is used here.
  - **Data in processing** - data being processed in memory or cache. Homomorphic and other emerging techniques are used in this case.
- **Other methods**
  - These accomplish confidentiality and privacy **without** having to use encryption
    - **Tokenization**
      - Assigns a random value with no mathematical value that can be reversed by linking the token back to the original data
      - Can preserve the format of data which makes it suitable for databases and card payment processing
    - **Data masking**
      - Desensitizes or removes sensitive or personal data but enables the data to remain usable
      - False data that looks real is changed for the real data
      - Commonly required for application development
      - Preserves the data format and referential integrity
    - **Redaction**
      - Obscuring the data by replacing all or part of the content for security or privacy purposes.
  
### Rights Management

- Protect data from unauthorized access through encryption
- **Digital Rights Management (DRM)** - used for protection of copyrighted materials (CDs and DVDs)
- **Information Rights Management (IRM)**
  - commonly applied to email, engineering documents and other business related files.
  - Allows you to control:
    - **Who** - who can and cannot access documents (by individual, group or based on email domains)
    - **What** - what documents can be accessed by allowing access to specific documents
    - **When** - when and for how long documents can be accessed
    - **Where** - control from where a document can be accessed. Based on location or other attributes
    - **How** - control how users are able to interact with the document

### Hardware Security Module (HSM)

- Used when data security through cryptographic functions is needed and the keys used to protect the data are of high value
- An HSM is a device used to protect and manage the keys needed as part of an encryption and decryption operation
- HSM devices have tamper-preventive secure cryptoprocessors
- Benefits:
  - Generate secure cryptographic keys
  - Provides secure key storage
  - Provides key management capabilities
  - Performs digital signing and encryption/decryption operations
  - Increased performance through cryptographic acceleration

### Encrypted Traffic Management

- SSL or TLS is now used by default
- This has a positive impact on data confidentiality but makes it difficult for organizations to monitor and ensure the sage use of their employees
- SSL/TLS decryption appliances and services are used for:
  - Monitoring of application performance
  - Cloud services monitoring
  - Malware detection
  - DLP
  - Forensic analysis
- After decryption, the data has to be sent to the right device for inspection
  - IDS/IPS
  - Firewalls
  - Secure web gateways
  - DLP solutions

## Data Integrity

- Provided through a method known as ***hashing*** or ***file integrity monitoring***
- ***Hashing*** is a cryptographic checksum
  - The algorithm is applied to a file and outputs a simple block of data
  - If the original document is modified, a different checksum is produced
- Applications:
  - Documents and email communication
  - Maintaining integrity of system files

## Data Availability

- Ensures adequate response and recovery for organizations in case of breaches and disasters
- Examples:
  - Regular backups of key information
