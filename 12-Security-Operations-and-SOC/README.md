Cyber Security Spectrum by Nityashree

12. Security Operations and Security Operations Center

Overview

Security Operations is the continuous practice of monitoring, detecting, analyzing, responding to, and recovering from cybersecurity threats.

A Security Operations Center, commonly known as a SOC, is a team or function responsible for monitoring an organization's security environment and responding to suspicious or malicious activity.

Security Operations connects several cybersecurity capabilities, including:

- Security monitoring
- Threat detection
- Log management
- Incident response
- Threat intelligence
- Vulnerability management
- Digital forensics
- Threat hunting
- Security automation
- Risk management

Security Operations is essential for protecting:

- Enterprise IT environments
- Cloud infrastructure
- Applications
- Networks
- Endpoints
- IoT devices
- OT and ICS environments
- Cyber-Physical Systems

---

1. Security Operations Fundamentals

Security Operations focuses on identifying and managing security events throughout their lifecycle.

Main Objectives

- Detect threats early
- Reduce attacker dwell time
- Investigate suspicious activity
- Contain security incidents
- Support recovery
- Improve security visibility
- Protect critical assets
- Maintain security records
- Improve security controls continuously

Security Operations Activities

- Monitoring security logs
- Investigating alerts
- Correlating security events
- Identifying attack patterns
- Performing threat hunting
- Managing incidents
- Tracking vulnerabilities
- Coordinating with IT and OT teams
- Reporting security metrics

---

2. Security Operations Center

A SOC may be:

- Internal
- Managed by a third-party provider
- Hybrid
- Cloud-based
- Enterprise-wide
- Specialized for OT or critical infrastructure

Typical SOC Functions

1. Monitoring
2. Detection
3. Triage
4. Investigation
5. Incident response
6. Threat hunting
7. Reporting
8. Continuous improvement

SOC Team Roles

SOC Analyst — Tier 1

Responsibilities:

- Monitor alerts
- Perform initial triage
- Identify false positives
- Escalate suspicious events
- Document investigations

SOC Analyst — Tier 2

Responsibilities:

- Perform detailed investigations
- Correlate multiple events
- Analyze endpoint and network evidence
- Investigate suspicious accounts
- Support incident containment

SOC Analyst — Tier 3

Responsibilities:

- Conduct advanced investigations
- Perform threat hunting
- Analyze complex attacks
- Develop detection logic
- Support malware and forensic analysis

Incident Responder

Responsibilities:

- Coordinate incident response
- Contain affected systems
- Support eradication and recovery
- Maintain incident documentation
- Coordinate with stakeholders

Threat Hunter

Responsibilities:

- Search for hidden threats
- Investigate attacker behavior
- Develop hypotheses
- Analyze threat intelligence
- Identify previously undetected activity

SOC Engineer

Responsibilities:

- Maintain SIEM
- Configure security tools
- Develop detection rules
- Integrate log sources
- Improve automation and monitoring

---

3. Security Event and Security Incident

Security Event

A security event is an observable activity related to the security of a system.

Examples:

- Successful login
- Failed login
- Password change
- Firewall connection
- File modification
- Process execution

Security Alert

A security alert is a notification generated when an event or group of events matches a suspicious condition.

Security Incident

A security incident is an event or series of events that threatens the confidentiality, integrity, or availability of systems or data.

Examples:

- Confirmed malware infection
- Account takeover
- Data exfiltration
- Ransomware activity
- Unauthorized administrator access
- Malicious modification of a PLC program

---

4. SOC Monitoring Sources

A SOC requires visibility across multiple systems.

Common Log Sources

- Firewalls
- Routers and switches
- Servers
- Endpoints
- Active Directory
- Identity providers
- Cloud platforms
- Applications
- Databases
- VPN systems
- Email security systems
- Web proxies
- DNS servers
- EDR platforms
- OT network monitoring tools

OT and ICS Monitoring Sources

- SCADA systems
- HMIs
- PLC engineering workstations
- Industrial firewalls
- Remote access gateways
- Historians
- Industrial network sensors
- Engineering software
- Safety system logs, where supported

---

5. SIEM

SIEM stands for Security Information and Event Management.

A SIEM collects, normalizes, correlates, searches, and analyzes security data from different sources.

SIEM Functions

- Log collection
- Log normalization
- Event correlation
- Alert generation
- Search and investigation
- Dashboard creation
- Threat detection
- Compliance reporting
- Incident timeline creation

SIEM Workflow

1. Collect logs
2. Normalize events
3. Enrich data
4. Correlate events
5. Generate alerts
6. Investigate activity
7. Respond to incidents
8. Document findings

SIEM Examples

- Microsoft Sentinel
- Splunk
- IBM QRadar
- Elastic Security
- Wazuh
- Google Security Operations

---

6. EDR and XDR

EDR — Endpoint Detection and Response

EDR monitors endpoint activity and helps detect and investigate threats.

EDR may collect:

- Process activity
- File activity
- Network connections
- Registry changes
- User activity
- Persistence mechanisms
- Suspicious command execution

EDR Capabilities

- Threat detection
- Endpoint investigation
- Process termination
- Host isolation
- Threat remediation
- Forensic evidence collection

XDR — Extended Detection and Response

XDR combines security telemetry from multiple domains.

Possible sources include:

- Endpoints
- Email
- Identity
- Network
- Cloud
- Applications

XDR helps correlate activity across different security layers.

---

7. Security Monitoring

Security monitoring is the continuous observation of systems and activities to identify suspicious behavior.

Monitoring Categories

- Identity monitoring
- Network monitoring
- Endpoint monitoring
- Application monitoring
- Cloud monitoring
- Data monitoring
- Email monitoring
- OT monitoring

Important Monitoring Activities

- Detect unusual logins
- Identify privilege escalation
- Detect suspicious processes
- Monitor network connections
- Identify data transfer anomalies
- Monitor configuration changes
- Detect malware indicators
- Monitor administrative actions

---

8. Alert Triage

Alert triage is the process of reviewing and prioritizing security alerts.

Triage Process

1. Receive alert
2. Validate the alert
3. Identify affected asset
4. Identify affected identity
5. Check event timeline
6. Review related activity
7. Determine severity
8. Escalate or close
9. Document the decision

Triage Questions

- Is the alert genuine?
- Is the activity authorized?
- Which user or system is involved?
- Is the asset critical?
- Is the activity still occurring?
- Are other systems affected?
- Is there evidence of compromise?
- What immediate action is required?

---

9. Incident Severity

Organizations may classify incidents according to:

- Business impact
- Asset criticality
- Data sensitivity
- Number of affected systems
- Safety impact
- Operational disruption
- Attacker access level
- Recovery complexity

Example Severity Levels

Low

Limited impact and no evidence of significant compromise.

Medium

Suspicious activity affecting a limited number of systems or users.

High

Confirmed compromise of important systems or sensitive data.

Critical

Major disruption, widespread compromise, significant data exposure, or potential safety impact.

Severity definitions should be customized to the organization.

---

10. Incident Response Workflow

A common incident response lifecycle includes:

1. Preparation
2. Detection and analysis
3. Containment
4. Eradication
5. Recovery
6. Lessons learned

Preparation

- Define incident response procedures
- Maintain contact lists
- Prepare tools
- Establish escalation paths
- Maintain backups
- Conduct exercises
- Define communication plans

Detection and Analysis

- Review alerts
- Validate evidence
- Identify affected assets
- Establish a timeline
- Determine attack scope
- Identify indicators of compromise

Containment

- Isolate affected systems
- Disable compromised accounts
- Block malicious communication
- Revoke access tokens
- Restrict remote access

Eradication

- Remove malware
- Remove persistence
- Patch vulnerabilities
- Reset compromised credentials
- Eliminate unauthorized access

Recovery

- Restore systems
- Validate security controls
- Monitor restored systems
- Confirm business functionality
- Obtain system owner approval

Lessons Learned

- Identify root cause
- Review response effectiveness
- Improve detection rules
- Update procedures
- Record corrective actions

---

11. Threat Intelligence

Threat Intelligence is the collection and analysis of information about threats, threat actors, tactics, techniques, procedures, and indicators.

Types of Threat Intelligence

Strategic

Focuses on business risks, trends, and long-term decisions.

Tactical

Focuses on attacker tactics, techniques, and procedures.

Operational

Focuses on current campaigns and attack activities.

Technical

Focuses on technical indicators such as:

- IP addresses
- Domains
- URLs
- File hashes
- Malware signatures
- Email indicators

Threat Intelligence Sources

- Government advisories
- Security vendors
- Information sharing groups
- Incident reports
- Internal investigations
- Threat research
- Industry communities

Threat intelligence should be validated before being used for detection or blocking.

---

12. Threat Hunting

Threat hunting is a proactive process of searching for malicious activity that may not have been detected by existing security tools.

Threat Hunting Process

1. Develop a hypothesis
2. Identify required data
3. Search for suspicious behavior
4. Investigate findings
5. Validate the threat
6. Create detection rules
7. Document results

Example Hypotheses

- An attacker may be using stolen credentials
- A compromised endpoint may be communicating with an unusual domain
- A service account may be used outside its normal schedule
- An engineering workstation may be executing unauthorized tools
- A device may be communicating with an unexpected external service

---

13. Detection Engineering

Detection engineering focuses on creating, testing, and improving security detections.

Detection Sources

- Authentication logs
- Process activity
- Network traffic
- DNS activity
- Cloud activity
- Endpoint telemetry
- Application logs
- Identity events
- OT network data

Detection Engineering Activities

- Identify threat behavior
- Define detection logic
- Create correlation rules
- Test detections
- Reduce false positives
- Measure detection quality
- Update rules as threats change

Detection Quality Factors

- Accuracy
- Coverage
- Timeliness
- Explainability
- Maintainability
- Operational usefulness

---

14. MITRE ATT&CK

MITRE ATT&CK is a knowledge base of adversary tactics and techniques.

It helps security teams:

- Understand attacker behavior
- Map alerts to techniques
- Develop detection rules
- Identify visibility gaps
- Support threat hunting
- Improve incident investigations

Common Enterprise Tactics

- Initial Access
- Execution
- Persistence
- Privilege Escalation
- Defense Evasion
- Credential Access
- Discovery
- Lateral Movement
- Collection
- Command and Control
- Exfiltration
- Impact

OT and ICS

MITRE ATT&CK for ICS focuses on adversary behavior in industrial control environments.

It can support:

- OT threat modeling
- Detection planning
- Incident investigation
- Security monitoring
- Industrial risk assessment

---

15. Security Automation and SOAR

SOAR stands for Security Orchestration, Automation, and Response.

SOAR platforms help security teams automate repetitive tasks and coordinate response activities.

Common SOAR Actions

- Enrich an IP address
- Check a file hash
- Disable a compromised account
- Isolate an endpoint
- Create an incident ticket
- Notify stakeholders
- Collect evidence
- Update threat intelligence records

Automation Considerations

Automation should be:

- Authorized
- Tested
- Auditable
- Reversible where possible
- Appropriate to the incident
- Safe for critical systems

In OT environments, automated actions must be carefully evaluated to avoid disrupting physical processes.

---

16. Security Operations for OT and ICS

OT SOC operations require additional awareness of:

- Safety
- Availability
- Industrial protocols
- Legacy systems
- Maintenance windows
- Process dependencies
- Vendor access
- Physical consequences

OT SOC Activities

- Monitor industrial network traffic
- Identify unauthorized commands
- Detect changes to PLC logic
- Monitor engineering workstation activity
- Review remote access
- Identify unusual HMI activity
- Detect unauthorized firmware changes
- Monitor industrial firewall events
- Coordinate with plant operators
- Avoid unsafe containment actions

OT Incident Response Principle

Security actions must be coordinated with OT engineers, plant operators, safety teams, and system owners before disrupting critical industrial systems.

---

17. SOC Metrics

Metrics help measure SOC performance.

Common Metrics

- Number of alerts
- Number of confirmed incidents
- Mean Time to Detect
- Mean Time to Respond
- Mean Time to Contain
- False-positive rate
- Escalation rate
- Detection coverage
- Incident recurrence
- Investigation backlog
- Log source availability

Metrics should be interpreted with context and should not encourage unsafe or incomplete investigations.

---

18. SOC Documentation

Important SOC documents include:

- Incident response plan
- Alert triage guide
- Escalation matrix
- Playbooks
- Detection rules
- Threat hunting reports
- Incident tickets
- Evidence records
- Asset inventory
- Contact list
- Communication plan
- Lessons-learned report
- Security monitoring dashboard

---

19. Practical Security Operations Labs

Practice the following activities:

- Analyze authentication logs
- Investigate failed login attempts
- Build a basic SIEM dashboard
- Create a simple detection rule
- Investigate suspicious network traffic
- Analyze endpoint process activity
- Perform basic threat hunting
- Map an alert to MITRE ATT&CK
- Create an incident response playbook
- Investigate a phishing scenario
- Analyze a suspicious IP address
- Build a basic SOAR workflow
- Create an incident timeline
- Develop an OT monitoring checklist
- Investigate simulated Modbus traffic in an authorized lab

---

20. Practical Projects

Project 1: Mini SOC Monitoring Environment

Build a learning environment containing:

- Log sources
- SIEM
- Endpoint telemetry
- Network monitoring
- Alert rules
- Investigation workflow
- Incident documentation

Project 2: Authentication Attack Investigation

Investigate a simulated account attack.

Include:

- Failed login analysis
- Source IP investigation
- User activity timeline
- Account containment
- Root cause
- Corrective actions

Project 3: Threat Hunting Exercise

Develop a threat hunting hypothesis and investigate:

- Unusual processes
- Suspicious network connections
- Abnormal account activity
- Persistence mechanisms
- Data transfer anomalies

Project 4: OT Security Monitoring

Design an OT monitoring approach for a manufacturing environment.

Include:

- Critical assets
- Industrial network visibility
- Monitoring points
- Alert conditions
- Escalation process
- Plant operator coordination
- Safe containment procedures

---

21. Learning Goals

After completing this section, you should be able to:

- Explain Security Operations and SOC functions
- Understand SOC roles and responsibilities
- Differentiate events, alerts, and incidents
- Understand SIEM, EDR, XDR, and SOAR
- Perform basic alert triage
- Understand incident response phases
- Analyze security logs
- Understand threat intelligence
- Perform basic threat hunting
- Map threats to MITRE ATT&CK
- Understand detection engineering
- Apply security monitoring to cloud, IoT, OT, and CPS
- Design basic SOC workflows
- Create incident response playbooks
- Develop security operations projects

---

22. References

- NIST Computer Security Incident Handling Guide
- NIST Cybersecurity Framework
- MITRE ATT&CK
- MITRE ATT&CK for ICS
- CISA Cybersecurity Guidance
- NIST Security and Privacy Controls
- FIRST Incident Response Guidance
- SANS Incident Response Resources
- OWASP Logging Guidance
- IEC 62443 security monitoring concepts

---

Conclusion

Security Operations provides continuous visibility and response capability across an organization’s digital and cyber-physical environments.

A mature SOC combines people, processes, technology, threat intelligence, monitoring, and incident response.

Effective Security Operations helps organizations detect threats early, reduce impact, improve resilience, and continuously strengthen their security architecture.

Cyber Security Spectrum by Nityashree
Building strong cybersecurity foundations for secure digital and cyber-physical systems.