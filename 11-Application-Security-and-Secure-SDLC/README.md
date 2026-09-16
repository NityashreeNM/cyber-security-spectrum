Cyber Security Spectrum by Nityashree

11. Application Security and Secure SDLC

Overview

Application Security focuses on protecting software applications from vulnerabilities, unauthorized access, data exposure, and malicious activities.

Secure Software Development Life Cycle (Secure SDLC) integrates security practices into every stage of software development.

Instead of identifying security issues only after deployment, Secure SDLC introduces security from the planning and design stages.

Application security is important for:

- Web applications
- Mobile applications
- APIs
- Cloud applications
- IoT platforms
- OT applications
- Embedded software
- Cyber-Physical Systems
- Enterprise applications
- Product security

This section covers application security fundamentals, secure coding, threat modeling, security testing, API security, DevSecOps, and secure software delivery.

---

1. Application Security Fundamentals

Application security protects:

- Application code
- User identities
- Business logic
- APIs
- Databases
- Sessions
- Sensitive information
- Application infrastructure
- Third-party components

Main Security Objectives

- Prevent unauthorized access
- Protect sensitive data
- Maintain application integrity
- Prevent data manipulation
- Reduce vulnerabilities
- Detect malicious activity
- Support secure application development
- Improve application resilience

---

2. Secure Software Development Life Cycle

A Secure SDLC integrates security into each software development phase.

Main Phases

1. Planning and requirements
2. Design
3. Development
4. Security testing
5. Deployment
6. Operations and maintenance
7. Retirement

Security Activities

SDLC Phase| Security Activities
Planning| Identify security objectives and compliance requirements
Requirements| Define security and privacy requirements
Design| Perform threat modeling and architecture review
Development| Apply secure coding practices
Testing| Perform SAST, DAST, and security testing
Deployment| Secure configurations and release approval
Operations| Monitoring, patching, and vulnerability management
Retirement| Secure data removal and access revocation

---

3. Security Requirements

Security requirements define what the application must do to remain secure.

Examples:

- Users must authenticate before accessing protected resources
- Sensitive data must be encrypted
- Administrative functions must require additional protection
- Passwords must not be stored in plain text
- User input must be validated
- Security events must be logged
- Sessions must expire after inactivity
- APIs must enforce authorization
- Secrets must not be stored in source code
- Security updates must be supported

Security requirements should be:

- Clear
- Testable
- Measurable
- Traceable
- Aligned with business needs

---

4. Secure Application Architecture

Secure application architecture considers security before implementation.

Important design areas include:

- Authentication
- Authorization
- Session management
- Input validation
- Data protection
- API security
- Error handling
- Logging
- Secrets management
- Dependency management
- Network communication
- Availability and resilience

Architecture Questions

- What are the application’s trust boundaries?
- Which components process sensitive data?
- Who can access administrative functions?
- How are APIs protected?
- Where are secrets stored?
- What happens if a component is compromised?
- Can an attacker move laterally?
- How is suspicious activity detected?

---

5. Threat Modeling

Threat modeling identifies possible threats and security weaknesses during design.

Common Approaches

- STRIDE
- Attack trees
- Data Flow Diagrams
- Trust boundary analysis
- Abuse cases
- MITRE ATT&CK
- Threat-based risk assessment

STRIDE Categories

Threat| Meaning
Spoofing| Pretending to be another identity
Tampering| Unauthorized modification of data
Repudiation| Denying an action without sufficient evidence
Information Disclosure| Exposing sensitive information
Denial of Service| Making a service unavailable
Elevation of Privilege| Gaining unauthorized permissions

Threat Modeling Process

1. Identify assets
2. Identify users and systems
3. Draw data flows
4. Identify trust boundaries
5. Identify threats
6. Assess risk
7. Define security controls
8. Validate mitigations
9. Review during changes

---

6. Secure Coding Principles

Secure coding reduces vulnerabilities during software development.

Important principles include:

- Validate all input
- Encode output correctly
- Avoid hardcoded secrets
- Use secure libraries
- Apply least privilege
- Handle errors securely
- Protect sensitive data
- Avoid unnecessary functionality
- Use secure defaults
- Keep dependencies updated
- Review code changes
- Avoid exposing internal details

Common Coding Risks

- SQL injection
- Command injection
- Cross-site scripting
- Path traversal
- Insecure deserialization
- Buffer overflow
- Integer overflow
- Race conditions
- Improper input validation
- Weak cryptography
- Hardcoded credentials

---

7. Authentication Security

Authentication verifies the identity of a user, device, or service.

Secure Authentication Controls

- Strong passwords
- Multi-factor authentication
- Account lockout or rate limiting
- Secure password storage
- Password reset protection
- Session timeout
- Secure cookies
- Protection against credential stuffing
- Login monitoring
- Risk-based authentication

Password Storage

Passwords should be stored using secure password-hashing algorithms with appropriate salts.

Applications should never store passwords in plain text.

---

8. Authorization Security

Authorization determines what an authenticated identity can access.

Common Authorization Models

- Role-Based Access Control
- Attribute-Based Access Control
- Resource-Based Access Control
- Policy-Based Access Control

Authorization Risks

- Broken access control
- Insecure direct object references
- Excessive permissions
- Missing function-level authorization
- Privilege escalation
- Access control bypass
- Insecure default permissions

Authorization Questions

- Can a user access another user’s data?
- Can a normal user access administrative functions?
- Are permissions checked on the server?
- Are API resources protected?
- Are access decisions logged?

---

9. Web Application Security

Web applications commonly face risks such as:

- Injection
- Broken access control
- Authentication failures
- Security misconfiguration
- Cross-site scripting
- Cross-site request forgery
- Vulnerable components
- Insecure design
- Software integrity failures
- Logging and monitoring failures

Web Application Security Controls

- Secure authentication
- Server-side authorization
- Input validation
- Output encoding
- Secure headers
- HTTPS
- CSRF protection
- Secure session management
- Security logging
- Dependency scanning
- Rate limiting

---

10. API Security

Application Programming Interfaces allow systems and applications to communicate.

API security protects:

- API endpoints
- Authentication tokens
- Request parameters
- Response data
- Backend services
- API gateways
- Service-to-service communication

API Security Controls

- Strong authentication
- Authorization for every endpoint
- Input validation
- Rate limiting
- API gateway protection
- TLS encryption
- Token expiration
- Secure secret storage
- Request logging
- Schema validation
- API inventory

API Security Risks

- Broken object-level authorization
- Broken authentication
- Excessive data exposure
- Unrestricted resource consumption
- Improper asset management
- Injection
- Misconfigured APIs
- Exposed debug endpoints

---

11. Data Protection

Applications must protect data during:

- Collection
- Processing
- Storage
- Transmission
- Sharing
- Backup
- Deletion

Data Security Controls

- Data classification
- Encryption at rest
- Encryption in transit
- Key management
- Access control
- Data masking
- Tokenization
- Secure backup
- Data retention
- Secure deletion

---

12. Session Security

Sessions maintain a user’s authenticated state.

Session Security Controls

- Use secure session identifiers
- Regenerate session IDs after login
- Set session expiration
- Invalidate sessions after logout
- Protect cookies
- Use Secure and HttpOnly cookie attributes
- Apply appropriate SameSite settings
- Detect suspicious session activity
- Avoid exposing session tokens in URLs

Session Threats

- Session hijacking
- Session fixation
- Token theft
- Insecure logout
- Long-lived sessions
- Session prediction

---

13. Software Dependencies and Supply Chain Security

Applications often depend on third-party libraries, packages, frameworks, and services.

Supply Chain Risks

- Vulnerable dependencies
- Malicious packages
- Compromised build systems
- Dependency confusion
- Typosquatting
- Unsigned software
- Insecure build pipelines
- Exposed secrets
- Untrusted third-party code

Security Controls

- Maintain a dependency inventory
- Use approved repositories
- Scan dependencies
- Pin important versions
- Review package permissions
- Verify package integrity
- Generate SBOMs
- Monitor vendor advisories
- Secure the build pipeline

---

14. Application Security Testing

Security testing identifies weaknesses before and after deployment.

SAST — Static Application Security Testing

Analyzes source code or binaries without running the application.

DAST — Dynamic Application Security Testing

Tests a running application from an external perspective.

IAST — Interactive Application Security Testing

Combines application runtime information with testing activity.

SCA — Software Composition Analysis

Identifies vulnerabilities and licensing risks in third-party dependencies.

Fuzz Testing

Provides unexpected or malformed input to identify crashes and weaknesses.

Penetration Testing

Simulates authorized attacks to identify exploitable vulnerabilities.

Security Testing Activities

- Code review
- SAST
- DAST
- SCA
- API testing
- Authentication testing
- Authorization testing
- Configuration testing
- Penetration testing
- Fuzz testing

---

15. DevSecOps

DevSecOps integrates security into development and operations.

DevSecOps Principles

- Security automation
- Continuous testing
- Shared responsibility
- Secure coding
- Infrastructure security
- Continuous monitoring
- Early vulnerability detection
- Secure deployment

DevSecOps Pipeline

1. Source code commit
2. Secret scanning
3. SAST
4. Dependency scanning
5. Build
6. Container scanning
7. DAST
8. Security approval
9. Deployment
10. Runtime monitoring

Security should be integrated into the development workflow rather than treated as a final-stage activity.

---

16. Container and Kubernetes Security

Modern applications may run in containers and Kubernetes environments.

Container Security Areas

- Base image security
- Image scanning
- Minimal images
- Non-root execution
- Secrets management
- Container isolation
- Runtime monitoring
- Registry security

Kubernetes Security Areas

- RBAC
- Network policies
- Pod security
- API server protection
- Secrets management
- Admission control
- Cluster monitoring
- Workload identity
- Secure configuration

---

17. Application Logging and Monitoring

Applications should generate useful security logs.

Important events include:

- Login success and failure
- Password changes
- MFA changes
- Permission changes
- Administrative actions
- Sensitive data access
- API failures
- Suspicious requests
- Configuration changes
- Security exceptions

Logging Principles

- Do not log passwords
- Do not expose access tokens
- Protect log integrity
- Synchronize time
- Restrict log access
- Define retention requirements
- Send important logs to a SIEM

---

18. Application Security Incident Response

Preparation

- Maintain application inventory
- Define incident contacts
- Prepare response procedures
- Maintain secure backups
- Document dependencies
- Establish escalation paths

Detection

- Review application logs
- Analyze alerts
- Identify unusual access
- Detect data exposure
- Investigate suspicious API activity

Containment

- Disable compromised accounts
- Revoke tokens
- Block malicious requests
- Isolate affected services
- Apply temporary security controls

Recovery

- Remove malicious code
- Patch vulnerabilities
- Restore trusted versions
- Rotate secrets
- Validate application behavior
- Monitor for recurrence

Lessons Learned

- Identify root cause
- Review security controls
- Improve testing
- Update threat models
- Document corrective actions

---

19. Application Security for IoT, OT, and CPS

Application security is also important for software that interacts with physical devices and industrial systems.

Security considerations include:

- Secure device APIs
- Strong device identity
- Secure command authorization
- Input validation
- Firmware security
- Secure update mechanisms
- Protection of control commands
- Safety-aware error handling
- Secure cloud-to-device communication
- Protection of industrial gateways
- Logging of configuration changes

CPS Security Questions

- Can unauthorized users send control commands?
- Are device commands authenticated?
- Can data be modified in transit?
- Are firmware updates verified?
- Can a compromised application affect physical safety?
- Are dangerous operations protected by additional authorization?
- Is there a safe fallback mode?

---

20. Practical Application Security Labs

Practice the following:

- Create a simple secure login application
- Implement password hashing
- Add MFA to an application
- Build RBAC authorization
- Test broken access control
- Explore SQL injection in an authorized lab
- Identify cross-site scripting
- Secure an API
- Configure HTTPS
- Analyze application logs
- Perform dependency scanning
- Use SAST and DAST tools
- Scan container images
- Create a secure CI/CD pipeline
- Generate a software bill of materials
- Perform threat modeling for an IoT application

---

21. Practical Projects

Project 1: Secure Web Application

Design a web application with:

- User registration
- Secure login
- MFA
- RBAC
- Session management
- Input validation
- Audit logging
- Secure password reset

Project 2: API Security Assessment

Assess an API for:

- Authentication weaknesses
- Authorization flaws
- Excessive data exposure
- Rate limiting issues
- Input validation problems
- Token management risks

Project 3: DevSecOps Pipeline

Create a pipeline containing:

- Source control
- Secret scanning
- SAST
- SCA
- Container scanning
- DAST
- Security gates
- Deployment monitoring

Project 4: Secure IoT Application

Design an IoT application with:

- Device identity
- Secure APIs
- Encrypted communication
- Role-based access
- Secure commands
- Device monitoring
- Firmware update validation
- Incident response

---

22. Learning Goals

After completing this section, you should be able to:

- Explain application security fundamentals
- Understand Secure SDLC
- Define application security requirements
- Perform basic threat modeling
- Apply secure coding principles
- Understand authentication and authorization
- Identify common web and API vulnerabilities
- Protect application sessions and data
- Understand software supply chain security
- Explain SAST, DAST, IAST, and SCA
- Understand DevSecOps
- Apply security to containers and Kubernetes
- Design application security monitoring
- Apply application security to IoT, OT, and CPS
- Create secure application architecture projects

---

23. References

- OWASP Top 10
- OWASP API Security Top 10
- OWASP Application Security Verification Standard
- OWASP Secure Coding Practices
- NIST Secure Software Development Framework
- NIST Cybersecurity Framework
- SLSA Supply Chain Security Framework
- MITRE CWE
- MITRE ATT&CK
- CIS Controls
- ISO/IEC 27001

---

Conclusion

Application Security and Secure SDLC help organizations build software that is secure, reliable, maintainable, and resilient.

Security must be integrated into requirements, architecture, development, testing, deployment, and operations.

Strong application security practices are essential for enterprise applications, cloud platforms, IoT systems, OT environments, and cyber-physical products.

Cyber Security Spectrum by Nityashree
Building strong cybersecurity foundations for secure digital and cyber-physical systems.