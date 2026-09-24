# Domain 24: Security Automation, SOAR and Cybersecurity Data Analytics

## 1. Domain Overview

Security Automation, Security Orchestration, Automation and Response (SOAR), and Cybersecurity Data Analytics focus on using technology, workflows, data, and automation to improve the speed, consistency, scale, and effectiveness of cybersecurity operations.

This domain connects security telemetry, detection engineering, analytics, orchestration, automated response, threat intelligence, incident response, and security operations into an integrated capability.

It bridges the gap between:

Security Data → Detection → Analysis → Decision → Orchestration → Response → Validation → Continuous Improvement

---

## 2. Purpose

The purpose of this domain is to understand how organizations collect, normalize, analyze, correlate, automate, and operationalize cybersecurity data.

Key objectives include:

- Reduce repetitive manual security operations
- Improve detection and investigation efficiency
- Correlate security events across environments
- Automate appropriate response actions
- Improve incident response consistency
- Support security analysts with actionable context
- Reduce alert fatigue
- Improve mean time to detect and respond
- Enable scalable security operations
- Establish measurable and repeatable security workflows

---

## 3. Security Automation

Security automation uses software and machine-driven workflows to perform security activities with limited manual intervention.

Examples include:

- Automated alert enrichment
- IOC lookups
- Threat intelligence enrichment
- User and asset context retrieval
- Automated ticket creation
- Endpoint isolation
- Account suspension
- Firewall rule changes
- Malware quarantine
- Vulnerability ticket generation
- Compliance evidence collection
- Security configuration checks

Automation should be designed with appropriate authorization, validation, logging, rollback, and human oversight.

---

## 4. Security Orchestration

Security orchestration coordinates multiple security technologies, processes, and data sources.

Examples include integrating:

- SIEM
- SOAR
- EDR/XDR
- Firewalls
- IAM
- Vulnerability management platforms
- Threat intelligence platforms
- Ticketing systems
- Cloud security platforms
- Email security
- Network security tools
- Asset management systems

The objective is to create coordinated security workflows rather than isolated security-tool operations.

---

## 5. SOAR

Security Orchestration, Automation and Response (SOAR) platforms help security teams manage repeatable security workflows.

Typical SOAR capabilities include:

- Playbook execution
- Case management
- Alert enrichment
- Threat intelligence integration
- Workflow orchestration
- Automated response
- Investigation support
- Evidence collection
- Incident tracking
- Reporting

SOAR does not replace security analysts. It can reduce repetitive work and help analysts focus on higher-value investigation and decision-making.

---

## 6. Security Playbooks

A security playbook defines how a security event should be investigated and handled.

A playbook can contain:

1. Trigger
2. Context collection
3. Validation
4. Enrichment
5. Investigation
6. Decision point
7. Response action
8. Approval requirement
9. Evidence collection
10. Recovery
11. Documentation
12. Lessons learned

Examples:

- Phishing investigation playbook
- Malware detection playbook
- Suspicious login playbook
- Privileged account compromise playbook
- Ransomware response playbook
- Data exfiltration investigation playbook
- Vulnerability escalation playbook

---

## 7. Human-in-the-Loop Automation

Not every security decision should be fully automated.

Automation models include:

### Manual

Human performs the complete workflow.

### Assisted

System gathers information and recommends actions.

### Approval-Based

System prepares the action but requires human authorization.

### Semi-Automated

Some actions are automated while critical decisions remain human-controlled.

### Fully Automated

Pre-approved low-risk actions are executed automatically.

The appropriate model depends on risk, confidence, reversibility, business impact, and organizational requirements.

---

## 8. Security Telemetry

Security automation depends on reliable telemetry.

Common telemetry sources include:

- Network traffic
- DNS
- Authentication logs
- Identity events
- Endpoint telemetry
- Cloud activity
- Application logs
- Firewall events
- Email security events
- Vulnerability data
- Threat intelligence
- SaaS activity
- OT and ICS telemetry
- IoT telemetry

Telemetry quality directly affects detection and automation quality.

---

## 9. Security Data Pipeline

A typical cybersecurity data pipeline can include:

Data Sources
→ Collection
→ Ingestion
→ Parsing
→ Normalization
→ Enrichment
→ Storage
→ Correlation
→ Detection
→ Analytics
→ Investigation
→ Response

Important engineering considerations include:

- Data quality
- Timestamp consistency
- Schema normalization
- Deduplication
- Retention
- Scalability
- Availability
- Privacy
- Access control
- Data integrity
- Cost management

---

## 10. Security Information and Event Management

SIEM platforms aggregate and analyze security-relevant events from multiple sources.

Core capabilities commonly include:

- Log collection
- Event normalization
- Correlation
- Search
- Detection rules
- Alerting
- Dashboards
- Investigation
- Threat intelligence integration
- Incident support
- Compliance reporting

SIEM and SOAR often work together:

SIEM → Detects and contextualizes  
SOAR → Orchestrates and automates response

---

## 11. Detection Engineering

Detection engineering focuses on designing, testing, maintaining, and improving security detections.

Important concepts include:

- Detection logic
- Detection rules
- Behavioral analytics
- Indicator-based detection
- Anomaly detection
- Correlation rules
- Detection coverage
- False positives
- False negatives
- Detection testing
- Detection lifecycle management

A mature detection should be:

- Relevant
- Explainable
- Testable
- Maintainable
- Measurable
- Operationally useful

---

## 12. Security Analytics

Cybersecurity data analytics applies analytical techniques to security data to identify meaningful patterns and relationships.

Common approaches include:

- Descriptive analytics
- Diagnostic analytics
- Statistical analysis
- Behavioral analytics
- Anomaly detection
- Correlation analysis
- Time-series analysis
- Risk-based analytics
- Graph analysis
- Machine learning-assisted analytics

Analytics should support security decisions rather than generate unexplained outputs.

---

## 13. User and Entity Behavior Analytics

UEBA analyzes behavioral patterns associated with users and entities such as:

- Devices
- Servers
- Applications
- Service accounts
- Cloud resources
- Network assets

Examples of behavioral signals:

- Unusual login location
- Unusual login time
- Abnormal data access
- Privilege escalation
- Unusual administrative activity
- Unexpected service behavior
- Abnormal network communication

UEBA should account for legitimate operational variation to reduce unnecessary alerts.

---

## 14. Security Data Correlation

Correlation combines events from different sources to identify relationships that may not be visible from individual events.

Example:

Authentication Event
+
Endpoint Event
+
Privilege Change
+
Network Connection
+
Cloud Activity

→ Higher-confidence investigation context

Correlation can improve detection quality when telemetry is reliable and properly normalized.

---

## 15. Alert Management

Security operations can generate large volumes of alerts.

Alert management focuses on:

- Deduplication
- Prioritization
- Enrichment
- Correlation
- Suppression
- Routing
- Escalation
- Case creation
- Closure
- Feedback

The objective is not simply to reduce alert volume.

The objective is to increase the proportion of alerts that are actionable and appropriately prioritized.

---

## 16. Alert Triage Automation

Automated triage can collect:

- Asset information
- User information
- Identity context
- Historical activity
- Threat intelligence
- Vulnerability information
- Endpoint status
- Network context
- Previous incidents

This allows analysts to begin investigations with relevant context already assembled.

---

## 17. Threat Intelligence Automation

Threat intelligence can be integrated into security workflows.

Automated enrichment can query:

- IP reputation
- Domain reputation
- URL intelligence
- File hashes
- Malware intelligence
- Vulnerability intelligence
- Adversary information
- Campaign information

Threat intelligence should be evaluated for:

- Source reliability
- Confidence
- Relevance
- Timeliness
- Context
- Potential false positives

---

## 18. Incident Response Automation

Automation can support multiple incident response activities.

Examples:

### Identification

- Collect related events
- Enrich indicators
- Identify affected assets

### Containment

- Isolate endpoint
- Disable account
- Block indicator
- Restrict network communication

### Eradication

- Remove malicious artifacts
- Reset credentials
- Revoke sessions
- Apply remediation

### Recovery

- Restore services
- Validate systems
- Monitor for recurrence

### Lessons Learned

- Update detections
- Improve playbooks
- Update controls
- Document findings

High-impact response actions should include appropriate safeguards and authorization.

---

## 19. Case Management

Security cases provide structured tracking for investigations.

A case may contain:

- Incident summary
- Alerts
- Evidence
- Indicators
- Timeline
- Analyst notes
- Related assets
- Related users
- Actions performed
- Decisions
- Approvals
- Resolution
- Lessons learned

Case management creates an auditable investigation record.

---

## 20. Security Workflow Automation

Security workflows can connect multiple systems.

Example:

SIEM Alert
→ SOAR Playbook
→ Threat Intelligence Lookup
→ Asset Lookup
→ Identity Lookup
→ Risk Evaluation
→ Analyst Approval
→ Response Action
→ Ticket Update
→ Evidence Storage

This creates repeatable operational processes.

---

## 21. Security Automation Architecture

A generalized architecture can contain:

### Data Layer

- Logs
- Events
- Telemetry
- Threat intelligence
- Asset data

### Analytics Layer

- Correlation
- Detection
- Behavioral analytics
- Risk analytics

### Orchestration Layer

- SOAR
- Workflow engine
- API integrations
- Playbooks

### Response Layer

- EDR
- IAM
- Firewall
- Cloud controls
- Email security
- Network controls

### Governance Layer

- Authorization
- Audit
- Change management
- Metrics
- Risk management

---

## 22. APIs for Security Automation

APIs are fundamental to security orchestration.

Common API operations include:

- Retrieve alerts
- Query assets
- Search users
- Retrieve threat intelligence
- Create tickets
- Update incidents
- Isolate endpoints
- Block indicators
- Disable accounts
- Collect evidence

Important API security considerations include:

- Authentication
- Authorization
- Secrets management
- Rate limiting
- Input validation
- Logging
- Error handling
- Certificate validation
- Least privilege

---

## 23. Webhooks and Event-Driven Security

Webhooks allow systems to trigger workflows based on events.

Example:

New Critical Alert
→ Webhook
→ Automation Workflow
→ Enrichment
→ Risk Evaluation
→ Response

Event-driven architecture can reduce manual polling and improve response speed.

---

## 24. Security Automation with Cloud Platforms

Cloud environments provide extensive automation opportunities.

Examples include:

- Automated identity response
- Cloud configuration remediation
- Security group validation
- Storage access monitoring
- Secret detection
- Container security workflows
- Infrastructure security checks
- Cloud incident response

Automation should respect cloud-native identity, permissions, APIs, and shared-responsibility boundaries.

---

## 25. Security Automation for DevSecOps

Automation can integrate security into software delivery.

Examples:

- SAST execution
- SCA scanning
- Secret detection
- Container scanning
- IaC scanning
- Dependency monitoring
- Security policy checks
- Automated ticket creation
- Deployment gates

Security automation should support development velocity without weakening necessary security controls.

---

## 26. Security Automation for Vulnerability Management

Automation can connect:

Asset Inventory
→ Vulnerability Scanner
→ Risk Context
→ Prioritization
→ Ticket
→ Remediation
→ Validation
→ Closure

Risk-aware automation can incorporate:

- Asset criticality
- Vulnerability severity
- Exploit availability
- Exposure
- Business context
- Compensating controls

---

## 27. SOAR and Identity Security

Identity-based automation may include:

- Suspicious login investigation
- Impossible-travel analysis
- Privilege escalation detection
- Account lockout workflows
- Session revocation
- MFA enforcement workflows
- Credential reset workflows
- Access review triggers

Automated identity actions require careful authorization because incorrect actions can disrupt legitimate users and critical operations.

---

## 28. SOAR and Endpoint Security

Endpoint automation may include:

- Endpoint isolation
- Process termination
- File quarantine
- Artifact collection
- Malware investigation
- Host information retrieval
- Endpoint remediation

Response actions should be risk-based and tested before production deployment.

---

## 29. SOAR and Network Security

Network automation can include:

- Blocking malicious IP addresses
- Domain blocking
- URL blocking
- Firewall rule workflows 
- Network isolation
- DNS response actions
- Proxy policy updates

Network automation requires change control and safeguards against accidentally disrupting legitimate traffic.

---

## 30. Automation Safety and Guardrails

Security automation can introduce operational risk.

Important safeguards include:

- Least privilege
- Approval gates
- Action allowlists
- Rate limits
- Rollback procedures
- Dry-run modes
- Testing environments
- Logging
- Audit trails
- Exception handling
- Failure handling
- Monitoring

Automation should be designed to fail safely.

---

## 31. Automation Testing

Before deployment, automation should be tested for:

- Functional correctness
- Security
- Reliability
- Performance
- Error handling
- False positives
- False negatives
- Rollback behavior
- Permission boundaries
- Integration failures

Testing approaches can include:

- Unit testing
- Integration testing
- Simulation
- Tabletop exercises
- Adversary emulation
- Production-safe validation

---

## 32. Security Automation Lifecycle

A mature automation lifecycle includes:

1. Identify repetitive task
2. Define objective
3. Assess risk
4. Design workflow
5. Define inputs
6. Define decisions
7. Define actions
8. Define authorization
9. Test
10. Deploy
11. Monitor
12. Measure
13. Improve
14. Retire when no longer required

---

## 33. Security Data Quality

Poor data quality can undermine automation.

Important dimensions include:

- Accuracy
- Completeness
- Timeliness
- Consistency
- Uniqueness
- Integrity
- Context
- Availability

Security teams should treat telemetry and security data as operational assets.

---

## 34. Data Normalization

Security platforms receive data from different systems and vendors.

Normalization creates consistent representations for:

- Users
- Devices
- IP addresses
- Domains
- Applications
- Events
- Timestamps
- Security outcomes

Common approaches include structured schemas and common event models.

---

## 35. Security Data Storage

Security data may be stored across:

- SIEM platforms
- Data lakes
- Security data warehouses
- Object storage
- Time-series databases
- Search platforms
- Case management systems

Key considerations include:

- Retention
- Search performance
- Cost
- Integrity
- Access control
- Regulatory requirements
- Data residency where applicable

---

## 36. Security Metrics and Analytics

Useful operational metrics can include:

- Mean time to detect
- Mean time to acknowledge
- Mean time to respond
- Mean time to contain
- Alert volume
- Alert fidelity
- Automation rate
- Analyst workload
- Playbook success rate
- Detection coverage
- Incident recurrence
- Response accuracy

Metrics should be interpreted in context rather than treated as isolated performance scores.

---

## 37. Automation Maturity

A security automation maturity journey can progress from:

### Level 1 — Manual

Human-driven security workflows.

### Level 2 — Assisted

Automation provides context and recommendations.

### Level 3 — Orchestrated

Multiple systems are integrated into workflows.

### Level 4 — Automated

Approved actions execute automatically.

### Level 5 — Adaptive

Automation continuously improves through feedback, analytics, and controlled optimization.

Organizations may operate at different maturity levels across different security capabilities.

---

## 38. AI-Assisted Security Operations

AI and machine learning can support:

- Alert summarization
- Investigation assistance
- Natural-language querying
- Anomaly detection
- Threat intelligence analysis
- Detection development
- Case summarization
- Knowledge retrieval
- Security workflow assistance

AI-assisted security operations require controls for:

- Data confidentiality
- Accuracy
- Explainability
- Human oversight
- Prompt and input security
- Model security
- Auditability
- Access control

---

## 39. AI-Augmented SOC

An AI-augmented SOC may combine:

Security Telemetry
+
Detection Engineering
+
Analytics
+
AI Assistance
+
SOAR
+
Human Analysts

The objective is to improve analyst effectiveness while retaining appropriate human control over consequential security decisions.

---

## 40. Security Automation and Threat Hunting

Automation can accelerate threat hunting by:

- Searching historical telemetry
- Querying indicators
- Correlating events
- Enriching suspicious activity
- Identifying related entities
- Repeating hunt queries
- Creating detection candidates

Automation should support hypothesis-driven hunting rather than replace analytical reasoning.

---

## 41. Security Automation and MITRE ATT&CK

MITRE ATT&CK can provide a common language for:

- Detection mapping
- Threat hunting
- Coverage analysis
- Incident investigation
- Adversary behavior analysis
- Detection engineering

Automation can enrich alerts with relevant ATT&CK techniques and tactics where appropriate.

---

## 42. SOAR for OT and CPS Environments

Automation in OT and CPS environments requires additional caution.

Important considerations include:

- Safety
- Availability
- Deterministic operations
- Process impact
- Asset criticality
- Legacy systems
- Change control
- Vendor requirements
- Segmentation
- Human authorization

Security automation actions that are acceptable in IT environments may not be appropriate for operational environments.

---

## 43. Security Automation and Critical Infrastructure

Critical infrastructure automation should account for:

- Operational continuity
- Safety
- Physical consequences
- Regulatory requirements
- Asset criticality
- Recovery requirements
- Engineering processes
- Manual fallback procedures

Automation should be designed around the operational risk of the environment.

---

## 44. Security Automation Governance

Organizations should establish governance for:

- Automation ownership
- Approval authority
- Change management
- Access control
- Playbook lifecycle
- Testing
- Audit
- Monitoring
- Exception handling
- Incident accountability

Every significant automated action should have a clearly defined owner and purpose.

---

## 45. Security Automation Risk Management

Automation risk can arise from:

- Incorrect detection
- Bad data
- Integration failure
- Excessive permissions
- Logic errors
- Automation loops
- Misclassification
- Unauthorized actions
- Vendor/API changes
- Unexpected operational impact

Risk assessment should precede high-impact automation.

---

## 46. Security Automation Architecture Patterns

Common patterns include:

### Alert Enrichment

Alert
→ Context
→ Intelligence
→ Analyst

### Automated Triage

Alert
→ Enrichment
→ Classification
→ Prioritization

### Response Automation

Detection
→ Validation
→ Approval
→ Response

### Continuous Security

Telemetry
→ Detection
→ Analytics
→ Automation
→ Feedback
→ Improved Detection

---

## 47. Practical Labs

Suggested labs include:

### Lab 1 — Log Analysis

- Generate security logs
- Collect logs
- Normalize events
- Search for suspicious activity

### Lab 2 — SIEM Detection

- Create a detection rule
- Generate test events
- Trigger an alert
- Investigate the alert

### Lab 3 — SOAR Playbook

- Create a basic workflow
- Enrich an IP address
- Query threat intelligence
- Create an investigation case

### Lab 4 — Automated Phishing Triage

- Process a simulated phishing alert
- Extract indicators
- Enrich indicators
- Classify the event
- Generate a response workflow

### Lab 5 — Endpoint Response

- Generate a simulated endpoint alert
- Collect context
- Execute a controlled response action
- Record the outcome

### Lab 6 — Vulnerability Automation

- Import vulnerability findings
- Map affected assets
- Prioritize findings
- Generate remediation tickets

### Lab 7 — Security Metrics

- Build an operational dashboard
- Track alert volume
- Track response time
- Track automation success

---

## 48. Professional Projects

Potential projects include:

- SOC automation framework
- Phishing response automation
- Threat intelligence enrichment pipeline
- Security alert triage system
- Vulnerability remediation workflow
- Automated IAM incident response
- Cloud security automation platform
- Security telemetry pipeline
- Detection engineering framework
- SOAR playbook library
- Security operations metrics dashboard
- AI-assisted SOC investigation workflow

---

## 49. Professional Workflow

A professional security automation workflow can follow:

1. Understand the security problem
2. Identify data sources
3. Define detection or trigger
4. Define decision logic
5. Identify integrations
6. Define permissions
7. Design workflow
8. Define human approval points
9. Build
10. Test
11. Validate
12. Deploy
13. Monitor
14. Measure
15. Improve
16. Document

---

## 50. Global Enterprise Context

Security automation is relevant across:

- Financial services
- Healthcare
- Manufacturing
- Energy
- Telecommunications
- Government
- Technology
- Retail
- Transportation
- Critical infrastructure
- Cloud-native enterprises

Enterprise implementations commonly integrate multiple security, identity, infrastructure, application, and business systems.

---

## 51. Standards and Reference Landscape

Relevant reference frameworks and standards include:

- NIST Cybersecurity Framework 2.0
- NIST SP 800-61 — Computer Security Incident Handling Guide
- NIST SP 800-82 — Guide to Operational Technology Security
- NIST SP 800-207 — Zero Trust Architecture
- NIST AI Risk Management Framework
- MITRE ATT&CK
- MITRE ATT&CK for ICS
- ISO/IEC 27001
- ISO/IEC 27002
- IEC 62443, where applicable
- Relevant CISA guidance
- Relevant sector-specific security requirements

Applicability depends on organizational environment, geography, sector, contractual obligations, and regulatory requirements.

---

## 52. Career Relevance

This domain supports roles such as:

- Security Automation Engineer
- SOAR Engineer
- Security Operations Engineer
- Detection Engineer
- Security Data Analyst
- SOC Engineer
- Threat Detection Engineer
- Security Platform Engineer
- Incident Response Engineer
- Security Architect
- Security Engineering Lead
- Security Operations Architect

It is particularly valuable for professionals working across SOC, detection engineering, security engineering, incident response, cloud security, and security architecture.

---

## 53. Learning Outcomes

After studying this domain, a learner should understand:

- Security automation principles
- SOAR architecture
- Security playbooks
- Security orchestration
- Security telemetry
- SIEM integration
- Detection engineering
- Security analytics
- Alert triage
- Threat intelligence enrichment
- Incident response automation
- Security APIs
- Event-driven security
- Automation governance
- Automation safety
- Security metrics
- AI-assisted security operations

---

## 54. Domain Relationships

This domain connects strongly with:

- Domain 04 — Security Tools and Ethical Hacking
- Domain 05 — Digital Forensics and Incident Response
- Domain 06 — Cloud Security
- Domain 08 — OT and ICS Security
- Domain 09 — Identity and Access Management
- Domain 10 — Security Architecture and Zero Trust
- Domain 11 — Application Security and Secure SDLC
- Domain 12 — Security Operations and SOC
- Domain 13 — Vulnerability Management and Penetration Testing
- Domain 15 — Threat Intelligence and Threat Hunting
- Domain 16 — Security Testing and Assurance
- Domain 17 — Security Engineering and Resilience
- Domain 19 — Cybersecurity Supply Chain Risk Management and Third-Party Security
- Domain 20 — AI and Emerging Technology Security
- Domain 23 — Critical Infrastructure and Cyber-Physical Systems Security

---

## 55. Key Takeaways

Security automation is more than automating individual security tasks.

A mature capability combines:

- Reliable telemetry
- Detection engineering
- Analytics
- Orchestration
- Automation
- Human decision-making
- Governance
- Measurement
- Continuous improvement

The objective is to create security operations that are scalable, repeatable, measurable, and appropriately controlled.

---

## 56. Professional Perspective

Modern cybersecurity environments generate more data and security events than human teams can efficiently process manually.

Security automation and SOAR provide mechanisms to connect people, processes, technologies, and data into coordinated security workflows.

The strongest implementations do not automate everything.

They automate appropriate activities, preserve human oversight for consequential decisions, and continuously measure whether automation improves security outcomes.

---

## 57. Domain Completion Checklist

- [ ] Understand security automation
- [ ] Understand security orchestration
- [ ] Understand SOAR
- [ ] Understand security playbooks
- [ ] Understand security telemetry
- [ ] Understand SIEM integration
- [ ] Understand detection engineering
- [ ] Understand security analytics
- [ ] Understand UEBA
- [ ] Understand alert triage
- [ ] Understand threat intelligence enrichment
- [ ] Understand incident response automation
- [ ] Understand security APIs
- [ ] Understand event-driven security
- [ ] Understand automation safety
- [ ] Understand automation governance
- [ ] Understand security metrics
- [ ] Build at least one automation workflow
- [ ] Build at least one SOAR-style playbook
- [ ] Build at least one security analytics project
- [ ] Understand enterprise automation architecture

---

## 58. Recommended Reference Landscape

Recommended areas for continued study:

- NIST Cybersecurity Framework
- NIST incident response guidance
- NIST Security and Privacy Controls
- NIST AI Risk Management Framework
- MITRE ATT&CK
- MITRE ATT&CK for ICS
- CISA cybersecurity guidance
- ISO/IEC 27001
- ISO/IEC 27002
- IEC 62443
- Security operations engineering practices
- Detection engineering practices
- SIEM and SOAR platform documentation
- Cloud provider security documentation
- Security API documentation

---

## 59. Conclusion

Security Automation, SOAR and Cybersecurity Data Analytics form an important layer of modern security operations.

They connect security data, detection, investigation, orchestration, response, and continuous improvement.

The progression is:

Security Data
→ Detection
→ Analytics
→ Context
→ Decision
→ Orchestration
→ Automation
→ Response
→ Measurement
→ Improvement

Understanding this domain enables cybersecurity professionals to move from manually executing individual security tasks toward designing scalable, measurable, and resilient security operations.

---

## 60. Cyber Security Spectrum by Nityashree

This domain represents the transition from individual security operations toward automated, data-driven, and orchestrated cybersecurity capabilities.

**Cyber Security Spectrum by Nityashree**

From Generic → Fundamentals → Domains → Specialisation → Niche

Security Automation, SOAR and Cybersecurity Data Analytics sits at the intersection of Security Operations, Security Engineering, Threat Detection, Incident Response, Cloud Security, AI-assisted Security, and Enterprise Security Architecture.