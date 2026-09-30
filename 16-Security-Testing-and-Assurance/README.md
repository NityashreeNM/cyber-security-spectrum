# Cyber Security Spectrum by Nityashree

# Security Testing and Assurance

*Building strong cybersecurity foundations for secure digital and cyber-physical systems.*

---

## 1. Overview

Security Testing and Assurance are essential capabilities for validating whether cybersecurity requirements, controls, architectures, applications, products, systems, and processes are designed and operating as intended.

Security testing provides evidence about security weaknesses and control effectiveness.

Security assurance provides confidence that security requirements are:

- Defined
- Implemented
- Verified
- Maintained
- Monitored
- Governed
- Continuously improved

Security Testing and Assurance apply across:

- Enterprise IT
- Applications
- APIs
- Cloud
- Networks
- IoT
- Embedded systems
- Products
- OT and ICS
- Cyber-physical systems
- Infrastructure
- Identity systems
- Security controls
- Third-party environments

A mature security assurance capability connects security requirements with architecture, implementation, verification, risk management, and operational evidence.

---

## 2. Objectives

The objectives of Security Testing and Assurance include:

- Identify security weaknesses.
- Validate security requirements.
- Verify security controls.
- Assess attack resistance.
- Validate secure design assumptions.
- Identify vulnerabilities before exploitation.
- Measure security control effectiveness.
- Support risk-based remediation.
- Provide evidence for assurance activities.
- Support regulatory and contractual requirements.
- Improve secure development practices.
- Strengthen product and system security.
- Improve organizational resilience.

---

## 3. Security Testing Principles

Security testing should be:

- Risk-based
- Evidence-driven
- Repeatable
- Documented
- Authorized
- Controlled
- Traceable
- Relevant to the environment
- Proportionate to risk
- Integrated with the development lifecycle

Security verification should begin during:

- Requirements
- Architecture
- Design
- Development
- Integration
- Deployment
- Operations
- Maintenance
- Decommissioning

Security testing should not be treated only as a final-stage activity.

---

## 4. Security Assurance Lifecycle

A typical security assurance lifecycle includes:

1. Define security requirements
2. Identify assets and risks
3. Establish security controls
4. Define verification objectives
5. Select testing methods
6. Execute testing
7. Analyze results
8. Document evidence
9. Remediate findings
10. Retest
11. Accept residual risk where appropriate
12. Continuously monitor

---

## 5. Security Requirements

Security testing should be traceable to explicit security requirements.

Security requirements may address:

### Confidentiality

Protection against unauthorized information disclosure.

### Integrity

Protection against unauthorized modification.

### Availability

Protection against disruption or loss of service.

### Authentication

Verification of identity.

### Authorization

Enforcement of permitted actions.

### Accountability

Ability to associate actions with responsible identities.

### Non-Repudiation

Ability to provide evidence regarding the origin or integrity of an action where required.

### Privacy

Protection and appropriate handling of personal information.

### Safety

Protection against cybersecurity events that could create unacceptable physical or operational consequences.

Safety considerations are particularly important for:

- OT
- ICS
- Medical devices
- Automotive systems
- Industrial equipment
- Critical infrastructure
- Cyber-physical systems

---

## 6. Security Testing Categories

Security testing may include:

- Vulnerability assessment
- Penetration testing
- Application security testing
- API security testing
- Network security testing
- Cloud security testing
- Configuration assessment
- Security architecture review
- Secure code review
- Software composition analysis
- Static application security testing
- Dynamic application security testing
- Interactive application security testing
- Mobile application security testing
- Container security testing
- Infrastructure-as-code security testing
- Firmware security testing
- Embedded device testing
- IoT security testing
- OT security assessment
- Wireless security testing
- Identity and access testing
- Security control testing
- Red teaming
- Purple teaming
- Adversary simulation

---

## 7. Vulnerability Assessment

Vulnerability assessment identifies known or suspected weaknesses in systems and applications.

Activities may include:

- Asset discovery
- Vulnerability scanning
- Version identification
- Configuration analysis
- Patch assessment
- Vulnerability validation
- Risk classification
- Remediation tracking
- Retesting

Vulnerability assessment generally provides broad coverage, while penetration testing provides deeper assessment of selected attack paths.

---

## 8. Penetration Testing

Penetration testing is an authorized security assessment in which testers attempt to identify and, where permitted, demonstrate exploitable weaknesses.

Typical phases include:

1. Authorization and scope
2. Reconnaissance
3. Enumeration
4. Vulnerability identification
5. Controlled exploitation
6. Privilege assessment
7. Lateral movement where authorized
8. Impact validation
9. Evidence collection
10. Reporting
11. Remediation
12. Retesting

Penetration testing must always operate within an explicitly approved scope.

---

## 9. Penetration Testing Approaches

### Black Box

The tester begins with limited information about the target.

This can simulate an external attacker perspective.

### Gray Box

The tester receives limited internal information or access.

This can represent a partially informed attacker or authenticated user.

### White Box

The tester receives extensive information about the target.

This may include:

- Architecture
- Source code
- Credentials
- Documentation
- Configuration
- System design

The selected approach should align with the testing objective.

---

## 10. Security Testing Scope

A professional testing scope should define:

- Target systems
- Applications
- IP ranges
- Domains
- APIs
- Cloud environments
- Devices
- Test accounts
- Testing windows
- Permitted techniques
- Prohibited techniques
- Data handling requirements
- Communication procedures
- Emergency contacts
- Stop conditions
- Reporting requirements
- Rules of engagement

---

## 11. Rules of Engagement

Rules of Engagement establish how testing will be performed.

They may define:

- Authorized targets
- Authorized testing periods
- Source IP addresses
- Permitted techniques
- Prohibited techniques
- Social engineering authorization
- Denial-of-service restrictions
- Data extraction restrictions
- Evidence handling
- Communication channels
- Incident escalation
- Testing termination criteria

Rules of Engagement reduce operational risk and establish accountability.

---

## 12. Vulnerability Classification

Security findings should be classified using appropriate risk methodologies.

Relevant factors may include:

- Exploitability
- Impact
- Exposure
- Asset criticality
- Authentication requirements
- Privilege requirements
- Attack complexity
- User interaction
- Business impact
- Safety impact
- Availability requirements
- Compensating controls

CVSS can be used as one input for vulnerability severity assessment.

Risk decisions should not rely solely on a numerical vulnerability score.

---

## 13. CVE and CVSS

### CVE

Common Vulnerabilities and Exposures provides standardized identifiers for publicly known vulnerabilities.

Example:

CVE-YYYY-NNNNN

### CVSS

Common Vulnerability Scoring System provides a standardized methodology for communicating vulnerability severity.

CVSS should be interpreted together with:

- Asset exposure
- Business criticality
- Exploitation status
- Threat intelligence
- Environmental factors
- Compensating controls
- Operational constraints

---

## 14. Security Testing Standards and Frameworks

Security testing may reference internationally recognized standards and frameworks, including:

- ISO/IEC 27001
- ISO/IEC 27002
- ISO/IEC 27005
- ISO/IEC 27034
- ISO/IEC 15408 Common Criteria
- NIST Cybersecurity Framework
- NIST SP 800-53
- NIST SP 800-115
- OWASP Testing Guide
- OWASP ASVS
- OWASP MASVS
- OWASP API Security guidance
- PCI DSS
- CIS Controls
- MITRE ATT&CK
- MITRE ATT&CK for ICS
- IEC 62443
- ISO/SAE 21434
- UNECE R155/R156 where applicable

The applicable standard should be selected according to the technology, industry, regulatory environment, and assurance objective.

---

## 15. NIST SP 800-115

NIST SP 800-115 provides technical guidance for information security testing and assessment.

It supports activities such as:

- Planning
- Discovery
- Attack and penetration testing
- Security assessment
- Analysis
- Reporting
- Remediation

It can provide a structured foundation for enterprise security testing programs.

---

## 16. OWASP Security Testing

OWASP provides widely used resources for application and web security testing.

Security testing may examine:

- Authentication
- Authorization
- Session management
- Input validation
- Injection
- Access control
- Cryptography
- Security configuration
- Error handling
- Logging
- API security
- Business logic
- File handling
- Server-side functionality

---

## 17. OWASP ASVS

The OWASP Application Security Verification Standard provides requirements that can be used to define and verify application security controls.

It can support:

- Security requirements
- Secure architecture
- Authentication
- Session management
- Access control
- Validation
- Cryptography
- Error handling
- Data protection
- Communications
- Malicious input handling

ASVS can help establish measurable application security verification requirements.

---

## 18. Secure Code Review

Secure code review identifies security weaknesses through manual and automated analysis.

Review areas may include:

- Authentication
- Authorization
- Input validation
- Output encoding
- Cryptography
- Secrets management
- Error handling
- Logging
- File operations
- Database access
- API security
- Memory safety
- Dependency usage
- Race conditions
- Business logic
- Secure configuration

Code review can be:

- Manual
- Automated
- Peer-based
- Tool-assisted
- Architecture-driven

---

## 19. Static Application Security Testing

SAST analyzes source code, bytecode, or other application representations to identify potential security weaknesses.

Potential findings include:

- Injection vulnerabilities
- Unsafe APIs
- Hardcoded secrets
- Weak cryptographic implementations
- Insecure data handling
- Authentication weaknesses
- Authorization problems

SAST is particularly valuable when integrated into CI/CD pipelines.

---

## 20. Dynamic Application Security Testing

DAST evaluates running applications from an external perspective.

It may identify:

- Web vulnerabilities
- Authentication issues
- Session weaknesses
- Configuration problems
- Injection vulnerabilities
- API weaknesses
- Runtime behavior issues

DAST complements SAST because the two approaches observe applications from different perspectives.

---

## 21. Software Composition Analysis

Modern applications frequently depend on:

- Open-source libraries
- Frameworks
- Packages
- Container images
- External components

Software Composition Analysis can help identify:

- Known vulnerabilities
- Outdated dependencies
- License risks
- Dependency relationships
- Vulnerable transitive dependencies

Dependency management should include:

- Inventory
- Version control
- Vulnerability monitoring
- Update processes
- Exception management

---

## 22. Software Supply Chain Assurance

Software supply-chain assurance should address:

- Third-party components
- Open-source dependencies
- Build systems
- CI/CD pipelines
- Package repositories
- Signing
- Artifact integrity
- Developer access
- Build provenance
- Release controls
- Dependency risks

Relevant practices may include:

- Software Bill of Materials
- Artifact signing
- Provenance verification
- Secure build environments
- Dependency pinning
- Vulnerability monitoring

---

## 23. Software Bill of Materials

A Software Bill of Materials provides an inventory of software components contained within a software product.

SBOMs can support:

- Vulnerability management
- Supply-chain visibility
- Component inventory
- Incident response
- Regulatory requirements
- Customer assurance
- Dependency management

Common SBOM formats include:

- SPDX
- CycloneDX

---

## 24. API Security Testing

API testing should examine:

- Authentication
- Authorization
- Object-level authorization
- Rate limiting
- Input validation
- Output handling
- Token management
- API versioning
- Error handling
- Sensitive data exposure
- Business logic
- Excessive resource consumption

API testing should consider both technical vulnerabilities and business logic abuse.

---

## 25. Cloud Security Testing

Cloud security testing may assess:

- Identity and access management
- Storage permissions
- Network security
- Security groups
- Encryption
- Key management
- Logging
- Monitoring
- Serverless functions
- Containers
- Kubernetes
- Cloud APIs
- Secrets management
- Configuration
- Multi-account architecture

Testing should respect cloud provider policies and organizational authorization boundaries.

---

## 26. Container and Kubernetes Security Testing

Container security testing may examine:

- Image vulnerabilities
- Image provenance
- Container privileges
- Secrets
- Runtime configuration
- Network policies
- Registry security
- Host interaction
- Escape risks
- Admission controls

Kubernetes testing may include:

- RBAC
- API server configuration
- Service accounts
- Network policies
- Secrets
- Pod security
- Cluster configuration
- Control-plane security
- Workload isolation

---

## 27. IoT Security Testing

IoT security testing should consider the complete ecosystem:

- Device
- Firmware
- Hardware
- Mobile application
- Cloud backend
- APIs
- Network
- Identity
- Update mechanism
- Manufacturing process

Testing areas may include:

### Hardware

- Debug interfaces
- JTAG
- UART
- Secure boot
- Hardware security mechanisms
- Physical access controls

### Firmware

- Firmware extraction
- Static analysis
- Dynamic analysis
- Update mechanisms
- Cryptographic implementation
- Secrets
- Hardcoded credentials

### Network

- Protocol security
- Encryption
- Authentication
- Device discovery
- Unexpected communication

### Cloud and APIs

- Authentication
- Authorization
- API security
- Device identity
- Data protection
- Tenant isolation

---

## 28. OT and ICS Security Testing

OT and ICS security testing requires additional caution because testing can affect:

- Safety
- Availability
- Process integrity
- Production
- Equipment
- Physical operations

Testing should consider:

- PLCs
- RTUs
- HMIs
- SCADA
- Historians
- Engineering workstations
- Industrial networks
- Industrial protocols
- Remote access
- Safety systems

Testing should preferably use:

- Laboratory environments
- Digital twins
- Test systems
- Simulators
- Offline environments

Production testing should be formally authorized and carefully controlled.

---

## 29. IEC 62443 Context

IEC 62443 provides a framework for cybersecurity of industrial automation and control systems.

Relevant concepts include:

- Asset owners
- Automation solution providers
- Product suppliers
- Security levels
- Zones
- Conduits
- Secure development
- System security
- Component security
- Security lifecycle

Security testing for industrial environments should align with relevant IEC 62443 requirements and the system lifecycle.

---

## 30. Product Security Assurance

Product security testing should cover the product lifecycle:

- Requirements
- Architecture
- Design
- Development
- Verification
- Release
- Deployment
- Maintenance
- Vulnerability management
- End-of-life

Testing may include:

- Threat modeling validation
- Secure code review
- Vulnerability scanning
- Penetration testing
- Firmware analysis
- API testing
- Authentication testing
- Cryptography assessment
- Update mechanism testing
- Supply-chain assessment
- Security regression testing

---

## 31. Security Regression Testing

Security regression testing verifies that previously fixed vulnerabilities do not reappear.

Regression testing should be integrated into:

- CI/CD
- Release management
- Patch management
- Product maintenance
- Application testing
- Firmware testing

Examples:

- Re-test authentication controls.
- Re-test authorization boundaries.
- Re-test previously vulnerable APIs.
- Re-test security patches.
- Re-test input validation.
- Re-test access-control logic.

---

## 32. Red Teaming

Red teaming is an authorized adversary simulation designed to evaluate organizational detection, response, and resilience.

It may assess:

- People
- Processes
- Technology
- Physical controls where authorized
- Detection capabilities
- Incident response
- Security operations
- Attack paths

Red team exercises should have clearly defined:

- Objectives
- Scope
- Rules of engagement
- Safety constraints
- Communication procedures
- Success criteria
- Reporting requirements

---

## 33. Purple Teaming

Purple teaming brings offensive and defensive security teams together to improve security controls.

Activities may include:

1. Select an attack technique.
2. Simulate the technique safely.
3. Observe security telemetry.
4. Evaluate detection.
5. Identify gaps.
6. Improve detection.
7. Re-test.
8. Document lessons learned.

Purple teaming promotes continuous improvement between:

- Red teams
- Blue teams
- SOC
- Threat intelligence
- Detection engineering
- Incident response

---

## 34. Security Control Testing

Security control testing validates whether controls operate as intended.

Controls may include:

- MFA
- Firewalls
- EDR
- Network segmentation
- Encryption
- Backup
- Logging
- Monitoring
- Access reviews
- Vulnerability management
- Secure configuration
- Data loss prevention
- Privileged access management

Testing should establish:

- Control objective
- Test procedure
- Evidence
- Result
- Exception
- Risk
- Remediation
- Retest status

---

## 35. Security Assurance Evidence

Security assurance requires evidence that can demonstrate control implementation and effectiveness.

Examples include:

- Test reports
- Scan results
- Configuration evidence
- Code review records
- Audit logs
- Architecture diagrams
- Security requirements
- Test cases
- Test results
- Remediation records
- Retest results
- Risk acceptance records
- Approval records

Evidence should be:

- Relevant
- Accurate
- Traceable
- Protected
- Reproducible where appropriate
- Maintained according to organizational requirements

---

## 36. Finding Management

A security finding should generally include:

1. Finding identifier
2. Title
3. Description
4. Affected asset
5. Security impact
6. Evidence
7. Risk
8. Severity
9. Attack scenario
10. Recommended remediation
11. Owner
12. Target date
13. Status
14. Retest result
15. Risk acceptance where applicable

---

## 37. Remediation and Retesting

Security testing creates value when findings are appropriately addressed.

A typical process is:

Identify → Validate → Classify → Prioritize → Remediate → Retest → Close or Accept Risk → Monitor

Remediation should consider:

- Root cause
- Business impact
- Asset criticality
- Exploitability
- Threat activity
- Operational constraints
- Compensating controls

---

## 38. Risk Acceptance

Not every security finding can immediately be eliminated.

Where appropriate, an organization may formally accept residual risk.

Risk acceptance should include:

- Finding
- Business justification
- Risk assessment
- Compensating controls
- Risk owner
- Approval
- Expiration or review date
- Monitoring requirements

Risk acceptance should be an accountable business decision rather than an informal technical closure.

---

## 39. Security Testing in the SDLC

Security testing should be integrated throughout the Software Development Lifecycle.

### Requirements

- Define security requirements.
- Establish security acceptance criteria.

### Architecture

- Threat modeling
- Security architecture review
- Trust boundary analysis

### Development

- Secure coding
- SAST
- Dependency analysis
- Secret detection

### Integration

- DAST
- API testing
- Configuration testing

### Release

- Penetration testing
- Security regression testing
- Risk review

### Operations

- Vulnerability monitoring
- Continuous testing
- Incident-driven testing

---

## 40. Continuous Security Testing

Modern environments require continuous security validation.

Continuous security testing may include:

- Automated vulnerability scanning
- SAST
- DAST
- SCA
- Container scanning
- IaC scanning
- Configuration validation
- Cloud security assessment
- Continuous attack-surface monitoring
- Security regression testing
- Detection validation

Automation should be combined with human analysis for high-risk findings.

---

## 41. Security Testing Metrics

Useful metrics may include:

- Number of systems tested
- Test coverage
- Vulnerabilities identified
- Critical findings
- High-risk findings
- Mean time to remediate
- Retest success rate
- Recurring vulnerabilities
- Security regression rate
- Detection coverage
- Control effectiveness
- Percentage of applications with security testing
- Percentage of critical assets assessed
- Number of overdue findings

Metrics should measure meaningful security outcomes rather than only testing volume.

---

## 42. Security Assurance Maturity

A security assurance program can progressively develop from:

### Level 1 — Reactive

Testing occurs mainly after incidents or major issues.

### Level 2 — Defined

Security testing processes and responsibilities are established.

### Level 3 — Integrated

Testing is integrated into development, architecture, operations, and risk management.

### Level 4 — Automated

Security verification is increasingly automated through engineering pipelines.

### Level 5 — Continuous Assurance

Security controls are continuously validated using:

- Automation
- Threat intelligence
- Telemetry
- Adversary simulation
- Risk analytics
- Continuous monitoring

Maturity should be evaluated against organizational objectives and risk.

---

## 43. Practical Labs and Projects

### Project 1: Web Application Security Assessment

Use an intentionally vulnerable application to perform:

- Reconnaissance
- Enumeration
- Authentication testing
- Authorization testing
- Input validation testing
- Session testing
- Reporting

Document:

- Scope
- Findings
- Evidence
- Risk
- Remediation
- Retest

---

### Project 2: API Security Testing

Build or use a safe API laboratory and test:

- Authentication
- Authorization
- Object access
- Rate limiting
- Input validation
- Token handling
- Business logic

---

### Project 3: Secure Code Review

Select a deliberately vulnerable application and identify:

- Injection
- Authentication flaws
- Authorization weaknesses
- Hardcoded secrets
- Insecure cryptography
- Unsafe APIs

Map findings to appropriate security requirements.

---

### Project 4: CI/CD Security Pipeline

Create a laboratory pipeline containing:

- SAST
- SCA
- Secret scanning
- Container scanning
- IaC scanning
- Security gates

Document how security findings affect the release process.

---

### Project 5: IoT Security Assessment

Using a legally obtained or simulated IoT device:

- Identify attack surface.
- Analyze firmware.
- Examine communication protocols.
- Review authentication.
- Test update mechanisms.
- Analyze APIs.
- Document security findings.

---

### Project 6: OT Security Testing Laboratory

Build a safe simulated OT environment containing:

- PLC simulator
- HMI simulator
- Engineering workstation
- Industrial protocol traffic
- Network monitoring

Perform non-disruptive:

- Configuration review
- Network analysis
- Access-control testing
- Protocol analysis
- Detection validation

Do not perform destructive testing against production systems.

---

### Project 7: Purple Team Exercise

Select a controlled ATT&CK technique and:

1. Define the scenario.
2. Simulate the technique safely.
3. Capture telemetry.
4. Validate detection.
5. Identify gaps.
6. Improve detection.
7. Re-test.
8. Document lessons learned.

---

## 44. Security Test Report Structure

A professional security test report should contain:

1. Executive Summary
2. Assessment Objective
3. Scope
4. Methodology
5. Rules of Engagement
6. Assets Tested
7. Limitations
8. Findings Summary
9. Detailed Findings
10. Evidence
11. Risk Assessment
12. Business Impact
13. Recommended Remediation
14. Retest Results
15. Residual Risk
16. Conclusion
17. Appendices

The report should distinguish verified facts from assumptions and testing limitations.

---

## 45. Professional Security Testing Ethics

Security testing must be:

- Authorized
- Legal
- Controlled
- Responsible
- Confidential
- Evidence-based

Security professionals should:

- Obtain appropriate authorization.
- Respect scope boundaries.
- Protect sensitive information.
- Avoid unnecessary disruption.
- Preserve evidence appropriately.
- Report vulnerabilities responsibly.
- Follow organizational policies.
- Respect applicable laws and contractual obligations.

Unauthorized testing is not equivalent to professional security testing.

---

## 46. Global Enterprise Context

Security Testing and Assurance support organizations operating across:

- Multiple regions
- Multiple cloud platforms
- Distributed development teams
- Global supply chains
- Critical infrastructure
- Connected products
- Industrial environments
- Regulated industries

An enterprise security assurance program should connect:

- Security requirements
- Threat modeling
- Secure architecture
- Secure development
- Security testing
- Vulnerability management
- Risk management
- Incident response
- Compliance
- Product security
- Operational security

---

## 47. Security Testing Career Relevance

Security Testing and Assurance provide foundations for roles such as:

- Security Analyst
- Vulnerability Analyst
- Penetration Tester
- Application Security Engineer
- Product Security Engineer
- Security Architect
- Cloud Security Engineer
- IoT Security Engineer
- OT Security Engineer
- Security Assurance Engineer
- Red Team Operator
- Purple Team Engineer
- Security Consultant
- Security Testing Lead
- Product Security Architect

---

## 48. Learning Outcomes

After completing this domain, the learner should be able to:

- Explain security testing principles.
- Understand vulnerability assessment.
- Understand penetration testing methodologies.
- Define testing scope and rules of engagement.
- Understand CVE and CVSS.
- Apply security testing standards and frameworks.
- Understand OWASP testing practices.
- Perform basic application security testing.
- Understand SAST, DAST, and SCA.
- Understand software supply-chain assurance.
- Understand SBOM concepts.
- Perform basic API security assessment.
- Understand cloud security testing.
- Understand container and Kubernetes security testing.
- Understand IoT security assessment.
- Understand OT and ICS testing considerations.
- Understand product security verification.
- Understand red teaming and purple teaming.
- Build security testing evidence.
- Manage security findings and remediation.
- Conduct security retesting.
- Connect testing results with enterprise risk.

---

## 49. Conclusion

Security Testing and Assurance transform cybersecurity requirements into measurable evidence.

A mature security assurance capability does not depend on a single penetration test or vulnerability scan.

It establishes continuous confidence through:

- Secure requirements
- Threat modeling
- Architecture review
- Secure development
- Automated security testing
- Manual security assessment
- Vulnerability management
- Adversary simulation
- Control validation
- Remediation
- Retesting
- Continuous monitoring

For enterprise IT, cloud, applications, IoT, products, OT, ICS, and cyber-physical systems, security assurance provides evidence needed to understand whether security controls are functioning as intended and where additional risk reduction is required.

**Cyber Security Spectrum by Nityashree**

*Building strong cybersecurity foundations for secure digital and cyber-physical systems.*