# Security Assessment Techniques

## Topics



## Vulnerability Scans

- Vulnerability scans help organizations to do the following:
  - Identify vulnerabilities
  - Uncover common misconfigurations
  - Understand where security controls are needed
  
- Vulnerability scanners fall into three categories:
  - **Network Scanners**
    - Probe hosts for open ports
    - Enumerate information about users and groups
    - Look for known vulnerabilities
  - **Application Scanners**
    - These require access to application source code or binaries but don't need to actually execute the application
    - Tests applications from the inside
    - Also known as static application security testing (SAST)
  - **Web application scanners**
    - Apply specifically to web applications and identifies vulnerabilities like:
      - Cross-site scripting
      - SQL injection
      - Path traversal
    - Executes application and tests from the outside in
    - Also called Dynamic Application Security Testing (DAST)
  - **Approaches after a vulnerability scan**
    - **Remediation** - patch the vulnerability
    - **Mitigation** - introduction of control to reduce the likelihood of the vulnerability being exploited or the impact if it is exploited
    - **Acceptance** - take no action if the risk is low, especially when compared with the cost of fixing it

- Scanners rely on vulnerability catalogs, two commonly standards used are:
    - [Common Vulnerability and Exposures (CVE)](https://cve.mitre.org/)
      - A standard for identifying vulnerabilities
      - Allows vulnerability databases to be linked together
      - Includes a description and unique identifier
      - Also include related references (reports and advisories)
    - [Common Vulnerability Scoring System (CVSS)](https://nvd.nist.gov/vuln-metrics/cvss)
      - A framework for communicating the characteristics and severity scores of vulnerabilities
      - CVSS score is from 0 to 10
      - 