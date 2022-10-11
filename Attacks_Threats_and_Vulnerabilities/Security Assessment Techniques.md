# Security Assessment Techniques

## Topics

  - [Vulnerability Scans](#vulnerability-scans)
  - [Intrusive vs. Non-Intrusive](#intrusive-vs-non-intrusive)
  - [Credentialed vs. Non-Credentialed](#credentialed-vs-non-credentialed)
  - [Threat Assessment](#threat-assessment)
    - [SIEM](#security-information-and-event-management-siem)
  - 

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
      - CVSS score is from 0 to 10 that indicates the severity of a vulnerability

## Intrusive vs. Non-Intrusive

- Intrusive scans try to verify vulnerabilities by trying to exploit them
- Non-intrusive testing helps organizations minimize disruptions related to vulnerability assessment.


## Credentialed vs. Non-Credentialed

- ***Non-credentialed*** scans are less invasive and provide an outsider's perspective
- ***Credentialed*** scans can get more information, resulting in more complete vulnerability status with more certainty
  - These tend to reduce false positives and false negatives
- ***False Negatives*** - a lack of result when there should be one
- ***False positives*** - scanner detects a vulnerability when one does not exist.

## Threat Assessment

- Organizations now tend to assume they have already been breached.
- Security teams try to be proactive rather than reactive

### Security Information and Event Management (SIEM)

- A system that provides a way to accomplish security monitoring:
  - Identifying internal and external threats
  - Monitoring activity and resource usage
  - Conduction compliance reporting for internal and external audits
  - Supporting incident response

- SIEM tools collect and correlate data, providing alerts and information dashboards based on that data.
- Main purpose of SIEM tools is to store and turn large amounts of data into knowledge that can then be acted upon
- **SIEM Basic Functions**
  - Centrally manage security events
  - Correlate and normalize events for context and alerting
  - Reporting on data gathered from various applications

- **SIEM Components**
  - ***Log collectors*** - responsible for aggregating and ingesting the log data from various sources
  - ***Log aggregation*** - process by which SIEM systems combine similar events to reduce volume
  - ***Correlation Engine*** - automates threat detection and log analysis using these techniques: 
    - Pattern matching
    - Anomaly detection
    - Boolean logic
    - Combination of boolean logic and context-relevant data

## Threat Hunting

- A proactive approach to finding an attacker before alerts are triggered
- Not reactive or detective
- Threat Hunters' goal is to disrupt the attacker during any phase of the ***cyber kill chain***

- **Key Attributes**
  - **Hypothesis**
    - Starts with a hunch, based on clues
    - Can be driven by the following:
      - Behavior analytics
      - Situational Awareness
      - Intelligence bulletins
      - Intelligence feeds
      - Vulnerability scans
  - **People**
    - Centered around the security analyst, who has deep expertize and knowledge of the organization's environment
  - **Assumptive**
    - Does not take breach-preventive approach but assumes the organization has already been breached
  - **Iterative**
    - Threat hunters have to pivot frequently to continue lateral movement while trying to find more evidence
- **Data Sources**
  - **Internal threat data**
    - Alert and event data from SIEM system and other raw log sources
    - Knowledge about previous attacks (vulnerabilities exploited, IOCs, attacker details, packet captures)
    - Network traffic baseline
  - **External threat data**
    - Structured threat information (STIX)
    - Security advisories, bulletins and other OSINT tools

## Security Orchestration, Automation, and Response (SOAR)

- SOAR tools can aggregate intelligence from internal and external sources to provide analysis and other insights
- Combines data and provides for case management and automated workflows
- **Primary functions**
  - Threat and vulnerability management
  - Security incident response
  - Security operations automation
- SOAR integrates all the security tools available in an organization and then automates incident responses.