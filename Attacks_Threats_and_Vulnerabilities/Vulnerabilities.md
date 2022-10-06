# Vulnerabilities

## Topics

  - [Cloud-Based vs On-Premises](#cloud-based-vs-on-premises)
  - [Zero-Day](#zero-day)
  - [Weak Configurations](#weak-configurations)
  - [Improper or Weak Patch Management](#improper-or-weak-patch-management)
  - [Third-Party Risks](#third-party-risks)
  - [Impacts](#impacts)

## Cloud-Based vs On-Premises

- When systems are moved to the cloud, the organization is no longer responsible for the physical aspects
- However, many of the same vulnerabilities that affect on-premises systems also affect cloud-based systems
- Cloud-based systems bring new vulnerabilities and exposures
  - Everything in the cloud is accessible from behind a single console so a small misconfiguration can have big impacts

## Zero-Day

- A **zero-day** is a threat that tries to exploit computer application vulnerabilities that are unknown to others - even the software developer
- Involves using software to exploit holes to carry out attacks
  - Attackers carry out these attacks or share information about them before the developer knows about the vulnerability
- Patches are usually not available for these

## Weak Configurations

- Improper or weak configurations can contribute to continued vulnerabilities
- Examples of weak configurations
  - Software that lets users do things with unnecessary privileges, violating the principle of least privilege
  - Systems that fail open instead of failing securely, letting an attacker to access resources
  - Security through obscurity, only protects against mostly insignificant threat actors
  - Unneeded complexity, makes system management more difficult
- System sprawl and lack of clear documentation can lead to loss of visibility and control, this can have negative impacts on an organization and lead to weak configurations
- Other examples of improper configurations:
  - Errors
  - Open permissions
  - Unsecured root accounts
  - Weak encryption
  - Unsecure protocols
  - Default settings
  - Open ports and services
  - Default or weak passwords

## Improper or Weak Patch Management

- Software exploitation takes advantage of a program's flaws and searches for problems, weaknesses, or security holes in code
- The best way to prevent this is to ensure proper patch management, this includes:
  - Evaluation, testing and deployment of latest patches and updates
  - Monitoring for new vulnerabilities
- **Types of Updates**
  - **Hotfix**
    - small and specific-purpose update that changes the behavior of installed apps
    - These are the most common type of update
  - **Service Pack**
    - A tested, cumulative set of all hotfixes, security updates, critical updates, and updates
  - **Update**
    - Addresses a non-critical, non-security-related bug and is usually a fix for a specific problem

## Third-Party Risks

- Organizations interact with third parties in one way or another, this creates third-party risk
- Examples of third party relations
  - Vendor management
  - Supply chain
  - Outsourced code development
  - Data storage
- Proper governance is key when dealing with areas that are often out of sight:
  - outsourced code development
  - supply chain
  - data storage

## Impacts

- Analysis should be based on ***impacts*** they are likely to face
- Things like breaches, loss of business process or information will result in some sort of impact that has to be measured to understand severity
- When measuring impact, organizations should take into account consequences across categories like:
  - Data loss
  - Data breaches and exfiltration
  - Identity Theft
  - Financial
  - Reputation
  - Availability loss
  - Life and safety