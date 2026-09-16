Cyber Security Spectrum by Nityashree

10. Security Architecture and Zero Trust

Overview

Security Architecture is the structured design of security controls, technologies, processes, and policies that protect an organization's systems, applications, networks, data, devices, and cyber-physical environments.

A security architecture connects business requirements with technical security controls.

It helps organizations achieve:

- Confidentiality
- Integrity
- Availability
- Safety
- Resilience
- Regulatory compliance
- Secure business operations
- Protection against cyber threats

Zero Trust Architecture is a modern security approach based on the principle:

«Never trust automatically. Always verify.»

Zero Trust does not assume that a user, device, application, or network is trusted simply because it is inside an organization’s network.

---

1. Fundamentals of Security Architecture

Security architecture defines how security is implemented across an organization.

It includes:

- Security policies
- Security principles
- Security requirements
- Security controls
- Network architecture
- Identity architecture
- Application security
- Data security
- Cloud security
- Monitoring and detection
- Incident response
- Business continuity
- Recovery planning

Main Objectives

- Reduce security risks
- Protect critical assets
- Prevent unauthorized access
- Detect malicious activity
- Limit the impact of incidents
- Support secure business growth
- Enable secure digital transformation

---

2. Security Architecture Principles

Defense in Depth

Use multiple security layers instead of depending on one security control.

Examples:

- Identity security
- Network segmentation
- Firewalls
- Endpoint security
- Encryption
- Monitoring
- Backup
- Physical security

Least Privilege

Provide only the access required to perform a specific task.

Secure by Design

Security should be considered during the design phase rather than added after implementation.

Fail Securely

When a system fails, it should move to a secure state whenever possible.

Separation of Duties

Critical activities should be divided between different roles.

Assume Breach

Design systems with the assumption that an attacker may already have access to part of the environment.

Minimize Attack Surface

Reduce unnecessary:

- Services
- Ports
- Applications
- Privileges
- Network paths
- External interfaces
- Administrative access

---

3. Security Architecture Layers

Enterprise Security Architecture

Protects the overall organization.

Includes:

- Business security requirements
- Enterprise security policies
- Risk management
- Governance
- Compliance
- Security operations

Network Security Architecture

Protects communication and network infrastructure.

Includes:

- Firewalls
- Network segmentation
- VPN
- IDS/IPS
- Secure routing
- Network access control
- Industrial DMZ

Application Security Architecture

Protects applications and software services.

Includes:

- Secure design
- Authentication
- Authorization
- Input validation
- Secure APIs
- Secrets management
- Secure software development

Data Security Architecture

Protects data throughout its lifecycle.

Includes:

- Data classification
- Encryption
- Key management
- Data loss prevention
- Backup
- Access control
- Data retention

Identity Security Architecture

Controls identities and access.

Includes:

- IAM
- MFA
- SSO
- RBAC
- PAM
- Identity federation
- Conditional access

Cloud Security Architecture

Protects cloud infrastructure and services.

Includes:

- Cloud IAM
- Network security
- Workload protection
- Container security
- Cloud monitoring
- Secure configuration
- Cloud data protection

OT and CPS Security Architecture

Protects industrial and physical processes.

Includes:

- Safety considerations
- Industrial segmentation
- Secure remote access
- PLC and HMI protection
- Asset visibility
- Protocol security
- Availability and resilience

---

4. Security Architecture Frameworks

Common frameworks and approaches include:

- NIST Cybersecurity Framework
- NIST Zero Trust Architecture
- NIST Risk Management Framework
- SABSA
- TOGAF Security Architecture
- CIS Controls
- ISO/IEC 27001
- ISO/IEC 27002
- IEC 62443
- MITRE ATT&CK
- Cloud security architecture frameworks

These frameworks help organizations structure security requirements, controls, governance, and risk management.

---

5. Security Architecture Design Process

Step 1: Understand Business Requirements

Identify:

- Business objectives
- Critical processes
- Regulatory requirements
- Availability requirements
- Safety requirements
- Recovery requirements

Step 2: Identify Critical Assets

Identify:

- Applications
- Servers
- Databases
- Devices
- Networks
- Cloud resources
- Industrial systems
- Sensitive data

Step 3: Perform Risk Assessment

Evaluate:

- Threats
- Vulnerabilities
- Attack paths
- Business impact
- Safety impact
- Existing controls
- Residual risk

Step 4: Define Security Requirements

Examples:

- MFA must be enabled
- Sensitive data must be encrypted
- Critical systems must be segmented
- Administrative access must be monitored
- Remote access must be approved
- Security logs must be retained

Step 5: Design Security Controls

Select appropriate:

- Preventive controls
- Detective controls
- Corrective controls
- Compensating controls

Step 6: Validate the Architecture

Validation may include:

- Threat modeling
- Security testing
- Architecture review
- Configuration review
- Compliance assessment
- Attack-path analysis

Step 7: Monitor and Improve

Security architecture should be reviewed continuously as:

- Business requirements change
- New threats emerge
- Technology changes
- New vulnerabilities are discovered
- Systems are connected or retired

---

6. Zero Trust Architecture

Zero Trust is a security model that continuously verifies identities, devices, applications, and access requests.

Core Principles

- Verify explicitly
- Apply least-privilege access
- Assume breach
- Continuously monitor
- Enforce policy dynamically
- Protect resources rather than only network boundaries

Zero Trust Components

- Identity Provider
- Policy Engine
- Policy Administrator
- Policy Enforcement Point
- Device security assessment
- Security analytics
- Threat intelligence
- Continuous monitoring
- Access control system

---

7. Zero Trust Policy Decision Process

A Zero Trust access decision may consider:

- User identity
- Device identity
- Device security posture
- Application
- Requested resource
- Location
- Time
- Network context
- Risk level
- Previous activity
- Data sensitivity

Example

A user may be allowed to access a development application from a managed device with MFA.

The same user may be denied access when:

- The device is compromised
- MFA is disabled
- The request comes from an unusual location
- The user requests an administrative resource
- The session risk becomes high

---

8. Zero Trust for Cloud

Cloud Zero Trust controls include:

- Strong IAM
- MFA
- Conditional access
- Temporary credentials
- Workload identity
- Micro-segmentation
- Secure APIs
- Cloud logging
- Continuous posture assessment
- Privileged access management

Cloud Security Questions

- Who is accessing the resource?
- Is the device trusted?
- Is the workload authorized?
- Is the access required?
- Is the session being monitored?
- Can the permission be time-bound?
- Is the activity consistent with normal behavior?

---

9. Zero Trust for IoT

IoT devices should not automatically trust other devices or services.

Important controls include:

- Unique device identity
- Secure onboarding
- Certificate-based authentication
- Device authorization
- Mutual TLS
- Device posture monitoring
- Network segmentation
- Secure firmware
- Device revocation
- Continuous monitoring

IoT Example

An IoT sensor should communicate only with its authorized gateway or cloud endpoint.

It should not have unrestricted access to:

- Enterprise databases
- Administrative systems
- Other IoT devices
- Industrial controllers
- Unrelated cloud services

---

10. Zero Trust for OT and CPS

Zero Trust in OT and CPS environments must consider:

- Safety
- Availability
- Legacy systems
- Real-time communication
- Industrial protocols
- Maintenance windows
- Emergency operations
- Vendor access
- Physical process impact

OT Zero Trust Controls

- Strong identity verification
- Role-based access
- Secure remote access
- Jump servers
- Industrial DMZ
- Network segmentation
- Time-bound vendor access
- Privileged access management
- Passive monitoring
- Application allowlisting
- Approved engineering workstation access
- Continuous logging

Important Consideration

Zero Trust controls should be implemented carefully in OT environments.

Security changes must not interrupt critical processes or create unsafe operating conditions.

---

11. Security Zones and Segmentation

Network segmentation separates systems based on:

- Function
- Criticality
- Trust level
- Security requirements
- Communication requirements

Example Zones

- Enterprise IT Zone
- Industrial DMZ
- Supervisory Control Zone
- Control Zone
- Safety Zone
- Vendor Access Zone
- Management Zone
- Backup Zone

Benefits

- Limits lateral movement
- Reduces attack surface
- Controls communication
- Protects critical assets
- Improves monitoring
- Supports incident containment

---

12. Security Controls

Preventive Controls

- MFA
- Firewalls
- Encryption
- Access control
- Secure configuration
- Network segmentation
- Application allowlisting

Detective Controls

- SIEM
- IDS/IPS
- EDR
- Network monitoring
- Log analysis
- Threat detection
- User behavior monitoring

Corrective Controls

- Account disablement
- Malware removal
- System restoration
- Credential rotation
- Configuration recovery
- Incident response

Compensating Controls

Alternative controls used when the preferred control cannot be implemented.

Examples:

- Network isolation
- Additional monitoring
- Restricted physical access
- Application allowlisting
- Manual approval
- Vendor-controlled mitigation

---

13. Security Architecture Documentation

Important architecture documents include:

- High-Level Design
- Low-Level Design
- Network architecture diagram
- Data Flow Diagram
- Trust boundary diagram
- Asset inventory
- Threat model
- Risk register
- Security requirements
- Control matrix
- Access control matrix
- Incident response plan
- Disaster recovery plan
- Security test plan

---

14. Security Architecture Review

A security architecture review should examine:

- Asset protection
- Identity and access control
- Network communication
- Data protection
- Logging and monitoring
- Vulnerability management
- Incident response
- Recovery capability
- Compliance requirements
- Safety and availability impact

Review Questions

- Are critical assets identified?
- Are trust boundaries documented?
- Are unnecessary network paths removed?
- Is privileged access controlled?
- Are sensitive data flows protected?
- Are security logs available?
- Can the system recover from an incident?
- Are third-party connections controlled?
- Are security requirements testable?

---

15. Security Architecture Threats

Common architectural weaknesses include:

- Flat networks
- Excessive trust relationships
- Weak identity controls
- Unrestricted remote access
- Shared administrator accounts
- Unencrypted communication
- Missing logging
- Poor asset visibility
- Insecure APIs
- Hardcoded credentials
- Excessive permissions
- Unsupported legacy systems
- Inadequate backup
- Poor incident recovery design

---

16. Practical Security Architecture Labs

Practice the following:

- Create a basic enterprise security architecture
- Design a segmented network
- Create an Industrial DMZ
- Build a Zero Trust access flow
- Create a trust boundary diagram
- Develop a security control matrix
- Design a secure cloud architecture
- Design IAM for a product
- Create an IoT security architecture
- Create an OT remote access architecture
- Map threats to security controls
- Review a sample architecture for weaknesses
- Create a risk register
- Develop a security architecture review checklist

---

17. Practical Projects

Project 1: Enterprise Zero Trust Architecture

Design an architecture containing:

- Identity provider
- MFA
- Device posture assessment
- Policy engine
- Policy enforcement point
- Application access
- Monitoring
- SIEM integration

Project 2: Secure IoT-to-Cloud Architecture

Include:

- Device identity
- Secure provisioning
- Gateway
- Encrypted communication
- Cloud IAM
- Certificate management
- Device monitoring
- Secure firmware updates

Project 3: OT Security Architecture

Design a manufacturing network containing:

- Enterprise IT
- Industrial DMZ
- SCADA
- HMI
- PLC network
- Engineering workstation
- Vendor access
- Firewall
- Monitoring system

Project 4: Product Security Architecture

Design security for a cyber-physical product.

Include:

- Threat modeling
- Identity management
- Secure communication
- Access control
- Secure boot
- Firmware updates
- Logging
- Vulnerability management
- Incident response
- Recovery

---

18. Learning Goals

After completing this section, you should be able to:

- Explain security architecture fundamentals
- Apply defense-in-depth principles
- Understand security architecture layers
- Identify critical assets and trust boundaries
- Design security requirements
- Understand Zero Trust Architecture
- Apply least privilege and continuous verification
- Design secure cloud architectures
- Apply Zero Trust to IoT, OT, and CPS
- Design network segmentation
- Create security architecture diagrams
- Develop security control matrices
- Perform architecture reviews
- Identify architectural security weaknesses
- Design security for cyber-physical products

---

19. References

- NIST Cybersecurity Framework
- NIST Zero Trust Architecture
- NIST Risk Management Framework
- CIS Controls
- ISO/IEC 27001
- ISO/IEC 27002
- IEC 62443
- MITRE ATT&CK
- OWASP Application Security Guidance
- Cloud Security Alliance Guidance

---

Conclusion

Security Architecture provides the foundation for designing secure, resilient, and trustworthy digital systems.

Zero Trust strengthens this foundation by continuously verifying identities, devices, applications, and access requests.

Together, Security Architecture and Zero Trust support secure enterprise systems, cloud environments, IoT platforms, OT networks, and cyber-physical products.

Cyber Security Spectrum by Nityashree
Building strong cybersecurity foundations for secure digital and cyber-physical systems.