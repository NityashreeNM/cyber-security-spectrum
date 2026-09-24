# Cyber Security Spectrum by Nityashree

# Domain 23: Critical Infrastructure and Cyber-Physical Systems Security

## 1. Domain Overview

Critical Infrastructure and Cyber-Physical Systems (CPS) Security focuses on protecting systems where digital technologies interact with physical processes, essential services, industrial environments, and societal infrastructure.

Modern critical infrastructure increasingly depends on interconnected:

- Information Technology (IT)
- Operational Technology (OT)
- Industrial Control Systems (ICS)
- Internet of Things (IoT)
- Industrial IoT (IIoT)
- Edge computing
- Cloud platforms
- Telecommunications
- Embedded systems
- Safety systems
- Physical processes

A simplified cyber-physical environment can be represented as:

Digital Systems → Control Systems → Physical Process → Human / Environmental Impact

A cybersecurity incident in such an environment may therefore affect more than data or computers. It may affect:

- Safety
- Availability
- Production
- Energy
- Water
- Transportation
- Healthcare
- Communications
- Manufacturing
- Public services
- The physical environment

This domain brings together cybersecurity, engineering, safety, resilience, risk management, and physical-world consequences.

---

# 2. Purpose of This Domain

The purpose of this domain is to develop a structured understanding of:

- Critical infrastructure security
- Cyber-physical systems security
- IT/OT convergence
- OT security architecture
- ICS security
- Industrial networks
- Safety and security relationships
- CPS threat modeling
- Critical infrastructure risk management
- Resilience engineering
- Sector-specific security
- Engineering-system security
- Physical process security
- Cyber-physical incident response
- Recovery and continuity
- Critical infrastructure governance

The objective is to understand how cybersecurity must adapt when digital systems influence real-world processes.

---

# 3. Critical Infrastructure

Critical infrastructure refers broadly to systems, assets, networks, and services whose disruption or compromise can have significant consequences for society, the economy, public safety, or national security.

Examples may include:

- Energy
- Electricity
- Oil and gas
- Water and wastewater
- Transportation
- Telecommunications
- Healthcare
- Financial services
- Manufacturing
- Government services
- Food and agriculture
- Data infrastructure

Definitions and designated sectors vary by jurisdiction.

---

# 4. Cyber-Physical Systems

A Cyber-Physical System combines computational, communication, sensing, control, and physical components.

A simplified CPS model is:

Sensors → Network → Compute → Decision → Control → Actuator → Physical Process

Examples include:

- Smart grids
- Industrial plants
- Autonomous vehicles
- Medical systems
- Smart buildings
- Robotics
- Water treatment
- Manufacturing systems
- Transportation systems
- Agricultural automation

---

# 5. CPS Security Objectives

Traditional information security emphasizes:

- Confidentiality
- Integrity
- Availability

CPS security often requires additional emphasis on:

- Safety
- Reliability
- Resilience
- Predictability
- Physical integrity
- Process integrity
- Human safety

The relative priority of these objectives depends on the system and its operational context.

---

# 6. IT, OT and CPS Relationship

A modern organization may contain:

IT → Enterprise Applications → Business Data

OT → Industrial Control → Physical Process

CPS → Integrated Digital + Physical Environment

The boundaries between these environments increasingly overlap.

Examples include:

- Enterprise systems communicating with production systems
- Cloud platforms receiving industrial telemetry
- Remote maintenance of industrial equipment
- AI systems supporting industrial decisions
- IoT devices connected to operational environments

This convergence increases both capability and attack surface.

---

# 7. Critical Infrastructure Attack Surface

Attack surfaces may include:

- Control systems
- PLCs
- RTUs
- HMIs
- SCADA systems
- Engineering workstations
- Industrial servers
- Sensors
- Actuators
- IoT devices
- Network equipment
- Remote access gateways
- Cloud services
- Enterprise interfaces
- Vendor connections
- Wireless systems
- Supply-chain components

Security architecture should consider the complete system rather than individual components in isolation.

---

# 8. CPS Threat Landscape

Representative threats include:

- Malware
- Ransomware
- Credential compromise
- Remote-access abuse
- Supply-chain compromise
- Vulnerable industrial devices
- Network intrusion
- Command manipulation
- Sensor manipulation
- Firmware compromise
- Denial of service
- Data manipulation
- Engineering workstation compromise
- Insider threats
- Physical tampering

The consequences depend heavily on the physical process being controlled.

---

# 9. Cyber-Physical Threat Modeling

CPS threat modeling should connect cyber events to physical consequences.

A useful model is:

Threat Actor → Cyber Attack → System Impact → Process Impact → Physical Consequence

Questions include:

- Which assets can be compromised?
- Which control functions depend on those assets?
- What physical process can be affected?
- What safety functions exist?
- What is the worst credible consequence?
- How can the system fail safely?
- What manual fallback exists?

---

# 10. Safety and Security

Safety and cybersecurity are related but distinct disciplines.

Safety generally focuses on preventing harm from hazards, failures, and unsafe conditions.

Cybersecurity focuses on protecting systems and information against unauthorized or malicious activity.

In CPS environments, the two disciplines may interact.

Example:

Cybersecurity Event → Incorrect Control Command → Unsafe Physical State

Security architecture should therefore identify where cybersecurity incidents could affect safety.

---

# 11. Safety Instrumented Systems

Safety Instrumented Systems (SIS) are designed to reduce risks associated with hazardous industrial processes.

Security considerations include:

- Unauthorized configuration
- Engineering access
- Network connectivity
- Firmware integrity
- Maintenance access
- Change management
- Vendor access

Security controls should not compromise the intended safety function.

Safety engineering and functional-safety requirements must remain part of the overall system design.

---

# 12. Critical Infrastructure Architecture

A simplified architecture may contain:

Enterprise IT
↓
Industrial DMZ
↓
OT Supervisory Layer
↓
Control Layer
↓
Field Devices
↓
Physical Process

Security controls may include:

- Segmentation
- Firewalls
- Controlled data flows
- Jump servers
- Privileged access management
- Monitoring
- Application allow-listing
- Secure remote access

The exact architecture depends on the sector and operational environment.

---

# 13. Purdue Model

The Purdue Enterprise Reference Architecture is commonly used as a conceptual model for industrial environments.

A simplified representation is:

Level 5 — Enterprise Network

Level 4 — Site Business Planning

Level 3 — Site Operations

Level 2 — Supervisory Control

Level 1 — Basic Control

Level 0 — Physical Process

The model can help structure discussions about:

- Network segmentation
- Data flows
- Security zones
- Trust boundaries
- Access paths

Modern architectures may not map perfectly to the traditional Purdue model, particularly with cloud, edge, IIoT, and converged architectures.

---

# 14. Zones and Conduits

IEC 62443 uses concepts including:

- Zones
- Conduits
- Security levels

A zone groups assets with similar security requirements.

A conduit controls communication between zones.

This approach can support:

- Segmentation
- Controlled communication
- Risk-based security requirements
- Defense in depth

---

# 15. Critical Infrastructure Segmentation

Segmentation can reduce:

- Lateral movement
- Malware propagation
- Unauthorized access
- Exposure of critical control systems

Potential zones include:

- Enterprise
- Industrial DMZ
- Operations
- Control
- Safety
- Engineering
- Remote access
- Vendor access

Segmentation should reflect actual data flows and operational requirements.

---

# 16. Industrial Communication Protocols

Industrial environments may use protocols such as:

- Modbus
- DNP3
- OPC UA
- EtherNet/IP
- PROFINET
- IEC 61850
- BACnet
- MQTT
- HART

Security capabilities vary between protocols and implementations.

Security architecture may therefore require compensating controls such as:

- Segmentation
- Authentication
- Encryption
- Monitoring
- Protocol-aware detection
- Strict access control

---

# 17. Industrial Asset Management

A critical infrastructure security program requires visibility into assets.

An asset inventory may include:

| Asset | Function | Location | Owner | Criticality | Connectivity | Security Status |
|---|---|---|---|---|---|---|
| PLC | Process Control | Plant A | OT | Critical | Industrial LAN | Monitored |
| HMI | Operator Interface | Plant A | OT | High | Control Network | Patched |
| RTU | Remote Monitoring | Field Site | Engineering | High | Cellular | Reviewed |
| Sensor | Process Measurement | Field | Operations | Medium | Wireless | Managed |

Asset inventories should include both technical and operational context.

---

# 18. Asset Criticality

Criticality may consider:

- Safety impact
- Production impact
- Availability requirements
- Environmental impact
- Financial impact
- Regulatory impact
- Recovery complexity
- Dependency relationships

Not every asset requires identical security controls.

Security investment should reflect risk and consequence.

---

# 19. Vulnerability Management in CPS

CPS vulnerability management is different from conventional IT patching because systems may have:

- Long operational lifetimes
- Limited maintenance windows
- Vendor certification requirements
- Safety constraints
- Legacy operating systems
- High availability requirements

A practical process is:

Identify → Validate → Assess Impact → Prioritize → Mitigate → Patch/Test → Verify → Monitor

Compensating controls may sometimes be required when immediate patching is not practical.

---

# 20. Secure Configuration Management

Security configuration should cover:

- PLCs
- HMIs
- Engineering workstations
- Servers
- Network devices
- Firewalls
- Remote-access systems
- Industrial applications

Controls may include:

- Baseline configurations
- Change control
- Configuration backups
- Access restrictions
- Secure administration
- Periodic validation

---

# 21. Engineering Workstation Security

Engineering workstations can have elevated privileges and access to critical control systems.

Security controls may include:

- Strong authentication
- Application allow-listing
- Endpoint protection where operationally suitable
- USB control
- Network segmentation
- Privileged access management
- Configuration control
- Secure backups
- Monitoring

Engineering workstations should be treated as high-value assets.

---

# 22. Remote Access Security

Remote access is a major CPS security consideration.

A controlled architecture may use:

Remote User → MFA → Secure Gateway → Jump Host → Authorized OT Zone

Controls may include:

- MFA
- Least privilege
- Time-bound access
- Privileged access management
- Session monitoring
- Approval workflows
- Network segmentation
- Vendor accountability

Direct unrestricted access to critical control environments should be avoided.

---

# 23. Vendor and Third-Party Access

Critical infrastructure often depends on:

- OEMs
- System integrators
- Maintenance providers
- Managed service providers
- Equipment vendors

Security controls should include:

- Identity verification
- MFA
- Least privilege
- Access approval
- Session monitoring
- Contractual requirements
- Access expiration
- Incident notification

Third-party security should integrate with the organization's C-SCRM program.

---

# 24. IoT and IIoT in Critical Infrastructure

IoT and IIoT can expand visibility and automation.

Examples include:

- Smart sensors
- Remote monitoring
- Predictive maintenance
- Smart meters
- Environmental sensors
- Connected equipment

Security considerations include:

- Device identity
- Firmware
- Secure updates
- Communication security
- Cloud connectivity
- Device lifecycle
- Supply chain
- Data protection

---

# 25. Edge Computing Security

Edge systems may process data close to physical processes.

Security considerations include:

- Physical protection
- Device identity
- Secure boot
- Software integrity
- Container security
- Local access control
- Network segmentation
- Secure updates
- Monitoring

Edge systems may become important security boundaries between field environments and centralized cloud platforms.

---

# 26. Cloud and CPS

Cloud services may support:

- Industrial analytics
- Digital twins
- Remote monitoring
- Predictive maintenance
- Fleet management
- AI workloads

Security architecture should address:

- Data flows
- Identity
- API security
- Encryption
- Cloud IAM
- Network connectivity
- Vendor dependencies
- Availability
- Recovery

Cloud connectivity should not automatically imply unrestricted access to control environments.

---

# 27. Digital Twins and CPS Security

Digital twins may represent:

- Manufacturing systems
- Industrial processes
- Buildings
- Infrastructure
- Energy systems

Security concerns include:

- Data integrity
- Model integrity
- Access control
- Synchronization
- API security
- Cloud security
- IoT security

A compromised digital representation could influence operational decisions if trusted without appropriate validation.

---

# 28. Critical Infrastructure Threat Intelligence

Threat intelligence can support identification of:

- Relevant threat actors
- Vulnerabilities
- Exploitation trends
- Sector-specific campaigns
- Malware
- Indicators of compromise
- Tactics and techniques

Relevant intelligence should be translated into actionable defensive measures.

---

# 29. MITRE ATT&CK for ICS

MITRE ATT&CK for ICS provides a knowledge base describing adversary behaviors relevant to industrial control environments.

It can support:

- Threat modeling
- Detection engineering
- Threat hunting
- Purple teaming
- Incident response
- Security architecture

It should complement, rather than replace, asset-specific risk assessment.

---

# 30. Critical Infrastructure Monitoring

Monitoring may include:

- Authentication
- Network traffic
- Industrial protocols
- Engineering workstation activity
- Configuration changes
- PLC changes
- Remote access
- Vendor activity
- Security alerts
- Process anomalies

Monitoring should balance security visibility with operational and safety requirements.

---

# 31. OT Security Operations

An OT security monitoring capability may integrate:

OT Telemetry → Network Monitoring → Detection → SOC/OT SOC → Investigation → Response

Security operations should understand:

- Industrial protocols
- Normal process behavior
- Asset criticality
- Operational constraints
- Safety implications

IT-centric detection alone may not provide sufficient context for OT incidents.

---

# 32. CPS Incident Response

A CPS incident-response process should consider:

1. Detect
2. Validate
3. Assess physical impact
4. Contain safely
5. Preserve evidence
6. Coordinate with operations
7. Recover
8. Validate safe operation
9. Monitor
10. Improve

Containment decisions must account for the possibility that abruptly shutting down systems can itself create operational or safety consequences.

---

# 33. Cyber-Physical Incident Scenarios

## Scenario 1: Unauthorized PLC Modification

An attacker gains access to an engineering workstation and modifies PLC logic.

Potential consequences:

- Process disruption
- Equipment damage
- Safety risk
- Production loss

## Scenario 2: Ransomware in an Industrial Environment

Ransomware affects enterprise systems connected to production.

Potential consequences:

- Loss of visibility
- Production interruption
- Manual operations
- Recovery challenges

## Scenario 3: Compromised Remote Vendor Access

A supplier account is compromised.

Potential consequences:

- Unauthorized OT access
- Configuration changes
- Data exposure
- Operational disruption

## Scenario 4: Sensor Manipulation

An attacker manipulates sensor data.

Potential consequences:

- Incorrect operator decisions
- Incorrect automation
- Process instability

---

# 34. Resilience Engineering

Critical infrastructure security must include resilience.

Resilience capabilities may include:

- Redundancy
- Backup systems
- Alternative communication
- Manual operating procedures
- Recovery plans
- Spare equipment
- Geographic diversity
- Emergency procedures
- Tested restoration

The objective is not only to prevent attacks but also to maintain or restore essential functions.

---

# 35. Business Continuity and Disaster Recovery

Critical infrastructure continuity planning should consider:

- Cyber incidents
- Equipment failure
- Power failure
- Network failure
- Natural disasters
- Supplier disruption
- Personnel availability

Plans should define:

- Critical functions
- Recovery priorities
- Recovery time objectives
- Recovery point objectives
- Dependencies
- Alternative processes
- Roles and responsibilities

ISO 22301 provides a recognized framework for business continuity management systems.

---

# 36. Physical Security

Cyber-physical environments require both cybersecurity and physical protection.

Physical security may include:

- Restricted facility access
- Secure control rooms
- Equipment protection
- Cabinet locks
- Surveillance
- Environmental controls
- Tamper detection
- Secure media handling

Physical compromise can bypass many logical security controls.

---

# 37. Human Factors

Critical infrastructure security depends on:

- Operators
- Engineers
- Administrators
- Maintenance teams
- Vendors
- Security teams

Human-centered security should address:

- Training
- Privileged access
- Procedures
- Emergency operations
- Social engineering
- Fatigue and workload
- Clear escalation paths

Security controls should be designed around how systems are actually operated.

---

# 38. Critical Infrastructure Supply Chain

Critical infrastructure may depend on:

- PLC manufacturers
- Network equipment vendors
- Cloud providers
- Software suppliers
- System integrators
- Hardware manufacturers
- Maintenance contractors

Supply-chain security should address:

- Vendor assurance
- Secure development
- Firmware integrity
- Software provenance
- SBOM where applicable
- Vulnerability management
- Remote access
- Incident notification
- Secure updates

---

# 39. Security by Design for CPS

Security should be considered during:

- Requirements
- Architecture
- Procurement
- Engineering
- Development
- Deployment
- Operation
- Maintenance
- Decommissioning

Security-by-design principles include:

- Least privilege
- Secure defaults
- Segmentation
- Defense in depth
- Strong identity
- Secure updates
- Monitoring
- Resilience
- Safe failure

---

# 40. Secure-by-Design Architecture

A CPS security architecture should consider:

Physical Process
↓
Field Devices
↓
Control Systems
↓
Supervisory Systems
↓
Industrial DMZ
↓
Enterprise / Cloud

Security controls should be mapped to:

- Assets
- Trust boundaries
- Data flows
- Control flows
- Safety requirements
- Recovery requirements

---

# 41. Zero Trust for Critical Infrastructure

Zero Trust principles can be adapted to CPS environments.

Key principles include:

- Verify explicitly
- Apply least privilege
- Continuously evaluate access
- Segment critical resources
- Monitor activity
- Assume compromise

However, Zero Trust implementation in OT must account for:

- Legacy protocols
- Safety requirements
- Availability
- Device limitations
- Deterministic communication
- Maintenance constraints

---

# 42. Critical Infrastructure Governance

Governance should establish:

- Asset ownership
- Risk ownership
- Security requirements
- Safety responsibilities
- Supplier requirements
- Incident escalation
- Recovery priorities
- Regulatory responsibilities
- Security exceptions

Security governance should connect executive leadership, engineering, operations, IT, OT, safety, and cybersecurity.

---

# 43. Risk Management

Critical infrastructure risk assessment should consider:

Risk = Threat × Vulnerability × Exposure × Consequence

The actual methodology should follow the organization's approved risk framework.

Risk assessment should include:

- Cyber impact
- Operational impact
- Safety impact
- Environmental impact
- Financial impact
- Regulatory impact
- Recovery complexity

---

# 44. Sector-Specific Security

Different sectors have different security priorities.

### Energy

Focus areas may include:

- Grid security
- Generation
- Transmission
- Distribution
- Substations

### Water

Focus areas may include:

- Treatment
- Distribution
- Pumping
- Chemical processes

### Healthcare

Focus areas may include:

- Medical devices
- Clinical systems
- Patient safety
- Availability

### Transportation

Focus areas may include:

- Signaling
- Traffic management
- Fleet systems
- Autonomous systems

### Manufacturing

Focus areas may include:

- Production systems
- Robotics
- PLCs
- Industrial networks

Security architecture should be adapted to the physical process and sector.

---

# 45. Regulatory and Standards Landscape

Important references include:

- NIST Cybersecurity Framework 2.0
- NIST SP 800-82 — Guide to Operational Technology Security
- NIST SP 800-53
- NIST SP 800-207 — Zero Trust Architecture
- IEC 62443 series
- ISO/IEC 27001
- ISO/IEC 27002
- ISO 22301
- MITRE ATT&CK for ICS
- CISA Cross-Sector Cybersecurity Performance Goals
- Sector-specific CISA guidance
- NERC CIP, where applicable to the North American bulk electric system
- EU NIS2 requirements, where applicable
- EU CER requirements, where applicable
- Applicable national critical-infrastructure requirements
- Applicable sector-specific regulatory requirements

Regulatory applicability depends on jurisdiction, sector, organization, and system classification.

---

# 46. NIST SP 800-82

NIST SP 800-82 provides guidance for securing Operational Technology environments.

It addresses areas including:

- OT characteristics
- OT threats
- OT vulnerabilities
- OT security architecture
- Network segmentation
- Security controls
- Incident response

It is particularly useful for understanding how conventional cybersecurity practices must be adapted to operational environments.

---

# 47. IEC 62443

IEC 62443 provides a comprehensive framework for industrial automation and control system security.

It addresses areas including:

- Asset owner requirements
- System security
- Component security
- Secure development
- Security lifecycle
- Zones and conduits
- Security levels

IEC 62443 is particularly relevant to industrial cybersecurity architecture and product security.

---

# 48. CISA Cybersecurity Performance Goals

CISA Cybersecurity Performance Goals provide prioritized cybersecurity practices intended to help organizations establish foundational protections.

For critical infrastructure environments, these can support areas such as:

- Asset inventory
- Identity
- MFA
- Vulnerability management
- Logging
- Incident response
- Network segmentation
- Resilience

They should be used alongside sector-specific requirements and risk assessments.

---

# 49. Critical Infrastructure Security Metrics

Possible metrics include:

- Percentage of critical assets inventoried
- Percentage of critical assets with defined owners
- Percentage of critical remote-access paths using MFA
- Percentage of critical zones with documented communication paths
- Percentage of critical vulnerabilities assessed
- Mean time to detect critical incidents
- Mean time to respond
- Recovery exercise completion rate
- Backup restoration success rate
- Supplier assessment coverage
- Percentage of critical systems with tested recovery procedures
- Number of unauthorized configuration changes
- Security monitoring coverage

Metrics should measure resilience and risk reduction rather than only compliance activity.

---

# 50. Practical Labs

## Lab 1: CPS Asset Inventory

Create an inventory containing:

- PLCs
- HMIs
- RTUs
- Sensors
- Engineering workstations
- Network devices
- Servers

Document:

- Function
- Criticality
- Connectivity
- Owner
- Security controls

## Lab 2: Purdue Architecture

Design a simplified industrial network using:

- Enterprise
- Industrial DMZ
- Operations
- Control
- Field

Identify:

- Trust boundaries
- Data flows
- Security controls

## Lab 3: CPS Threat Model

Threat-model:

Sensor → Network → Controller → Actuator → Physical Process

Identify:

- Threats
- Attack paths
- Safety consequences
- Controls
- Recovery mechanisms

## Lab 4: OT Remote Access

Design:

Vendor → MFA → Secure Gateway → Jump Server → OT Zone

Include:

- Least privilege
- Time-bound access
- Session monitoring
- Approval
- Logging

## Lab 5: Industrial Network Segmentation

Design segmented zones for:

- Enterprise
- Industrial DMZ
- Supervisory
- Control
- Safety

Document allowed communication paths.

## Lab 6: CPS Incident Response

Create an incident involving unauthorized PLC logic modification.

Develop:

- Detection
- Validation
- Containment
- Operational coordination
- Evidence preservation
- Recovery
- Safe-state validation

## Lab 7: Critical Infrastructure Risk Register

Create a risk register containing:

Asset → Threat → Vulnerability → Consequence → Control → Residual Risk → Owner

## Lab 8: Resilience Exercise

Design a tabletop exercise involving:

- Loss of network connectivity
- Loss of control visibility
- Cyberattack
- Supplier outage

Define:

- Essential functions
- Manual fallback
- Recovery priorities
- Communication plan

---

# 51. Professional Projects

## Project 1: Critical Infrastructure Security Architecture

Design an end-to-end architecture containing:

Enterprise → DMZ → OT → Control → Physical Process

Include:

- Segmentation
- IAM
- Remote access
- Monitoring
- Incident response
- Resilience

## Project 2: CPS Threat Modeling Framework

Develop a reusable methodology for:

- Asset identification
- Data-flow mapping
- Threat modeling
- Physical consequence analysis
- Control selection
- Risk treatment

## Project 3: Industrial Zero Trust Architecture

Design a Zero Trust model for an industrial environment.

Address:

- Identity
- Device trust
- Network segmentation
- Privileged access
- Continuous monitoring
- Operational constraints

## Project 4: Critical Infrastructure Incident Response

Create an incident-response playbook for:

- Ransomware
- PLC compromise
- Remote-access compromise
- Sensor manipulation

## Project 5: CPS Security Architecture for Smart Agriculture

Design:

Sensors → Gateway → Edge → Cloud → Analytics → Actuation

Address:

- Device identity
- Secure communication
- Firmware
- Cloud security
- Data integrity
- Remote access
- Physical consequences

---

# 52. Professional Workflow

A cybersecurity professional working in this domain may follow:

1. Understand the physical process
2. Identify critical services
3. Identify cyber-physical assets
4. Establish asset ownership
5. Map dependencies
6. Map data and control flows
7. Identify trust boundaries
8. Perform threat modeling
9. Assess cyber and physical consequences
10. Define security requirements
11. Design segmentation
12. Establish identity and access controls
13. Secure remote access
14. Manage vulnerabilities
15. Establish monitoring
16. Integrate threat intelligence
17. Prepare incident-response procedures
18. Test recovery and resilience
19. Assess suppliers
20. Continuously improve the security architecture

---

# 53. Global Enterprise Context

Critical Infrastructure and CPS Security is relevant across:

- Energy
- Utilities
- Water
- Healthcare
- Manufacturing
- Automotive
- Aerospace
- Transportation
- Telecommunications
- Agriculture
- Oil and gas
- Mining
- Smart cities
- Government
- Critical digital infrastructure

The security architecture varies according to:

- Physical process
- Safety requirements
- Availability requirements
- Technology lifecycle
- Threat landscape
- Regulatory environment
- Operational constraints
- Recovery requirements

---

# 54. Career Relevance

This domain connects to roles such as:

- Cyber-Physical Systems Security Architect
- OT Security Architect
- Industrial Cybersecurity Engineer
- Critical Infrastructure Security Engineer
- ICS Security Engineer
- OT Security Consultant
- Product Security Architect
- IoT Security Architect
- Security Architect
- Cybersecurity Risk Manager
- Security Operations Engineer
- Industrial Threat Hunter
- CPS Security Researcher
- Critical Infrastructure Security Consultant

It is particularly relevant to professionals who combine:

Cybersecurity + Networking + IoT + OT + Cloud + Embedded Systems + Engineering + Safety + Architecture

---

# 55. Learning Outcomes

After completing this domain, a learner should be able to:

- Explain critical infrastructure security
- Explain cyber-physical systems
- Distinguish IT, OT, ICS, IoT, and CPS concepts
- Identify CPS attack surfaces
- Understand cyber-physical threat modeling
- Connect cyber incidents to physical consequences
- Understand safety and security relationships
- Design basic OT/CPS security architecture
- Apply segmentation concepts
- Understand zones and conduits
- Understand industrial protocols
- Build critical asset inventories
- Assess CPS vulnerabilities
- Design secure remote access
- Understand vendor security
- Apply Zero Trust principles to OT environments
- Design CPS incident-response processes
- Design resilience and recovery strategies
- Understand critical infrastructure governance
- Map security requirements to recognized standards
- Design practical CPS security architectures

---

# 56. Domain Relationships

Critical Infrastructure and CPS Security connects directly with:

- Cybersecurity Fundamentals
- Networking
- Linux
- Cloud Security
- IoT Security
- OT and ICS Security
- Identity and Access Management
- Security Architecture and Zero Trust
- Application Security and Secure SDLC
- Security Operations and SOC
- Vulnerability Management and Penetration Testing
- Governance, Risk and Compliance
- Threat Intelligence and Threat Hunting
- Security Testing and Assurance
- Security Engineering and Resilience
- Privacy Engineering and Data Protection
- Cybersecurity Supply Chain Risk Management
- AI and Emerging Technology Security
- Cryptography and PKI
- Mobile, Wireless and Telecom Security

This domain brings multiple cybersecurity disciplines together around systems where cyber events can influence physical processes and essential services.

---

# 57. Key Takeaways

Critical infrastructure security is not simply IT security applied to industrial environments.

It requires understanding:

Cyber System → Control System → Physical Process → Human / Environmental Consequence

A mature CPS security program therefore combines:

- Cybersecurity
- Engineering
- Safety
- Architecture
- Risk management
- Resilience
- Operations
- Physical security
- Supply-chain security

The objective is to protect both digital systems and the essential physical functions they support.

---

# 58. Professional Perspective

Traditional cybersecurity often asks:

"How do we protect the information system?"

Critical Infrastructure and CPS Security expands the question:

"What happens in the physical world if the digital system is compromised, unavailable, manipulated, or incorrectly configured?"

This requires security professionals to understand both:

Digital Consequence

and

Physical Consequence

The strongest CPS security architecture therefore considers security, safety, availability, resilience, and operational reality together.

---

# 59. Domain Completion Checklist

- [ ] I understand critical infrastructure concepts.
- [ ] I understand cyber-physical systems.
- [ ] I understand IT/OT convergence.
- [ ] I understand CPS attack surfaces.
- [ ] I can perform CPS threat modeling.
- [ ] I can connect cyber threats to physical consequences.
- [ ] I understand safety and security relationships.
- [ ] I understand the Purdue model.
- [ ] I understand zones and conduits.
- [ ] I understand industrial network segmentation.
- [ ] I understand industrial communication protocols.
- [ ] I can build a critical asset inventory.
- [ ] I understand OT vulnerability management.
- [ ] I understand engineering workstation security.
- [ ] I can design secure remote vendor access.
- [ ] I understand CPS monitoring.
- [ ] I understand OT incident response.
- [ ] I understand resilience engineering.
- [ ] I understand business continuity and recovery.
- [ ] I understand critical infrastructure supply-chain risk.
- [ ] I can apply Zero Trust principles to CPS environments.
- [ ] I can map CPS security controls to recognized standards.
- [ ] I can design a practical critical infrastructure security architecture.

---

# 60. Recommended Reference Landscape

Primary references for further study include:

- NIST Cybersecurity Framework 2.0
- NIST SP 800-82 — Guide to Operational Technology Security
- NIST SP 800-53 — Security and Privacy Controls
- NIST SP 800-207 — Zero Trust Architecture
- IEC 62443 series — Industrial Automation and Control Systems Security
- ISO/IEC 27001
- ISO/IEC 27002
- ISO 22301 — Business Continuity Management Systems
- MITRE ATT&CK for ICS
- CISA Cybersecurity Performance Goals
- CISA Cross-Sector Cybersecurity Performance Goals
- NERC CIP, where applicable
- EU NIS2 requirements, where applicable
- EU CER requirements, where applicable
- Relevant national critical-infrastructure security requirements
- Relevant sector-specific standards and regulations

Always verify the current edition, jurisdiction, scope, and applicability of a standard or regulation before using it for formal compliance, audit, procurement, or regulatory purposes.

---

# 61. Conclusion

Critical Infrastructure and Cyber-Physical Systems Security represents a major convergence point within modern cybersecurity.

It connects:

Cybersecurity → IT → OT → IoT → CPS → Engineering → Safety → Physical Infrastructure → Essential Services

The discipline requires security professionals to think beyond traditional digital assets and understand how technology interacts with the physical world.

A mature approach follows the lifecycle:

Understand the Physical Process → Identify Critical Assets → Model Threats → Assess Consequences → Design Controls → Monitor → Respond → Recover → Improve

The ultimate objective is to maintain secure, safe, resilient, and trustworthy operation of systems that society and organizations depend upon.

---

# 62. Cyber Security Spectrum by Nityashree

## From Generic to Niche

A structured cybersecurity spectrum connecting:

Awareness → Fundamentals → Domains → Specialization → Architecture → Engineering → Advanced Security

Domain 23 brings the spectrum into the cyber-physical world, connecting cybersecurity with critical infrastructure, industrial environments, engineering systems, safety, resilience, and essential services.

**Cyber Security Spectrum by Nityashree**

**From Generic to Niche.**