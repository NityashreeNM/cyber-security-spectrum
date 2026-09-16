Identity and Access Management — IAM

1. Overview

Identity and Access Management focuses on ensuring that the right person, device, application, or service gets the right access to the right resource at the right time.

IAM is a core cybersecurity domain used in:

- Enterprise IT
- Cloud security
- IoT security
- OT and ICS security
- Product security
- Zero Trust Architecture
- Security Operations

---

2. IAM Fundamentals

Key Concepts

- Identity
- Authentication
- Authorization
- Accountability
- Access control
- Privileged access
- Identity lifecycle
- Least privilege
- Separation of duties
- Zero Trust

Authentication Factors

1. Something you know
   
   - Password
   - PIN

2. Something you have
   
   - Smart card
   - Hardware token
   - Mobile authenticator

3. Something you are
   
   - Fingerprint
   - Face recognition

Authentication Methods

- Password-based authentication
- Multi-factor authentication
- Certificate-based authentication
- Biometric authentication
- Single Sign-On
- Federation
- Adaptive authentication

---

3. Authorization Models

Role-Based Access Control — RBAC

Access is assigned based on a user's role.

Examples:

- Administrator
- Security Analyst
- Developer
- Operator
- Auditor

Attribute-Based Access Control — ABAC

Access is granted based on attributes such as:

- User identity
- Device security status
- Location
- Time
- Resource sensitivity
- Business context

Mandatory Access Control — MAC

Access is controlled through centrally defined security labels and policies.

Discretionary Access Control — DAC

Resource owners can decide who gets access.

---

4. IAM Lifecycle

Joiner

When a new employee or user joins:

- Create identity
- Assign role
- Provide required access
- Enforce MFA
- Register approved devices

Mover

When a user changes role:

- Review existing permissions
- Remove unnecessary access
- Assign new role-based access
- Update privileged permissions

Leaver

When a user leaves:

- Disable account
- Revoke sessions
- Revoke tokens and certificates
- Remove group memberships
- Recover company devices
- Review service and application access

---

5. Privileged Access Management — PAM

Privileged accounts have elevated permissions and require stronger controls.

PAM Controls

- Separate administrator accounts
- Just-in-time access
- Just-enough access
- Privileged session monitoring
- Password vaulting
- Approval workflows
- Session recording
- Emergency access controls
- Regular privilege reviews

Examples of privileged identities:

- Domain Administrator
- Cloud Administrator
- Root user
- Database Administrator
- OT Engineering Workstation Administrator

---

6. IAM in Cloud Security

Important cloud IAM concepts:

- Users
- Groups
- Roles
- Policies
- Service accounts
- Managed identities
- Temporary credentials
- Federation
- Conditional access
- Workload identity

Cloud IAM Security Practices

- Avoid permanent access keys
- Use temporary credentials
- Enable MFA
- Apply least privilege
- Review unused permissions
- Separate production and development access
- Monitor privileged activities
- Protect service accounts
- Use centralized identity governance

---

7. IAM in IoT and Product Security

IoT devices may contain different identities:

- Device identity
- User identity
- Application identity
- Gateway identity
- Cloud service identity
- Manufacturer identity

IoT IAM Controls

- Unique identity per device
- Mutual TLS
- Device certificates
- Secure key storage
- Certificate rotation
- Device onboarding
- Device decommissioning
- Secure credential provisioning
- Device authorization
- API authentication

Avoid:

- Shared default passwords
- Hardcoded credentials
- Reused certificates
- Permanent device secrets
- Unauthenticated APIs

---

8. IAM in OT and ICS Security

OT environments require special consideration because availability and safety are critical.

OT IAM Controls

- Individual operator accounts
- Controlled engineering workstation access
- Strong authentication for remote access
- Jump servers
- Privileged access management
- Vendor access approval
- Time-bound remote access
- Session recording
- Access review
- Break-glass procedures
- Offline recovery accounts

OT-Specific Considerations

- Some legacy systems may not support modern authentication
- Safety systems require carefully controlled access
- Authentication changes must be tested before deployment
- Remote access should be disabled when not required
- Shared accounts should be minimized and monitored
- Emergency access must be documented and reviewed

---

9. Zero Trust and IAM

Zero Trust assumes that no user, device, application, or network should be trusted automatically.

Zero Trust IAM Principles

- Verify explicitly
- Use least-privilege access
- Continuously evaluate risk
- Authenticate users and devices
- Validate device posture
- Segment sensitive resources
- Monitor access continuously
- Revoke access when risk changes

Example

A user may be allowed to access a production system only when:

- The user identity is verified
- MFA is completed
- The device is compliant
- The user has the required role
- The request is within an approved time window
- The session is monitored

---

10. IAM Threats

Common IAM-related threats include:

- Credential theft
- Password spraying
- Brute-force attacks
- Phishing
- Session hijacking
- Token theft
- Privilege escalation
- Account takeover
- Excessive permissions
- Orphaned accounts
- Insider misuse
- Shared credentials
- Compromised service accounts
- Misconfigured cloud policies
- Unprotected API keys

---

11. IAM Security Controls

Preventive Controls

- MFA
- Strong password policy
- Least privilege
- Role-based access
- Privileged access management
- Network restrictions
- Secure credential storage

Detective Controls

- Login monitoring
- Failed authentication alerts
- Privilege escalation alerts
- Impossible-travel detection
- Abnormal access detection
- Privileged session monitoring

Corrective Controls

- Account lockout
- Token revocation
- Password reset
- Session termination
- Access removal
- Incident response
- Credential rotation

---

12. IAM Architecture Components

A typical IAM architecture may include:

- Identity Provider — IdP
- Directory Service
- Authentication Service
- Authorization Service
- Single Sign-On
- Multi-Factor Authentication
- Privileged Access Management
- Identity Governance
- Access Review
- Security Information and Event Management
- Endpoint Security
- Policy Enforcement Point

---

13. Practical Labs

Beginner Labs

- Create Linux users
- Create Linux groups
- Configure file permissions
- Configure sudo access
- Review login logs
- Disable unused accounts
- Configure SSH key authentication

Intermediate Labs

- Configure a local identity directory
- Implement RBAC
- Create an access matrix
- Configure MFA in a test environment
- Analyze authentication logs
- Build a basic access review process
- Detect repeated failed logins

Advanced Labs

- Design cloud IAM policies
- Build a Zero Trust access flow
- Design privileged remote access for OT
- Create an IoT device identity lifecycle
- Model an IAM threat scenario
- Design identity monitoring and incident response
- Create a product security IAM architecture

---

14. IAM Project Ideas

Project 1: Enterprise Access Matrix

Create an access matrix for:

- HR
- Finance
- IT
- Security
- Engineering
- Management

Document:

- Role
- Resource
- Access type
- Approval authority
- Review frequency

Project 2: Secure Remote Access Architecture

Design secure remote access for an OT environment using:

- MFA
- VPN or zero trust access
- Jump server
- PAM
- Session monitoring
- Time-bound access
- Approval workflow

Project 3: IoT Device Identity Lifecycle

Design the lifecycle of an IoT device:

1. Manufacturing
2. Provisioning
3. Onboarding
4. Authentication
5. Certificate rotation
6. Maintenance
7. Decommissioning

Project 4: IAM Threat Model

Use STRIDE to analyse:

- Credential theft
- Token theft
- Privilege escalation
- Identity spoofing
- Unauthorized access
- Account takeover

---

15. Career Relevance

IAM knowledge is important for roles such as:

- Cybersecurity Architect
- Product Security Architect
- Cloud Security Architect
- IAM Engineer
- Zero Trust Architect
- IoT Security Architect
- OT Security Architect
- Security Consultant
- Security Operations Engineer

---

16. Learning Outcome

After completing this domain, you should be able to:

- Explain authentication and authorization
- Design RBAC and ABAC models
- Understand privileged access management
- Build an identity lifecycle process
- Secure cloud identities
- Secure IoT device identities
- Design IAM for OT environments
- Apply Zero Trust principles
- Identify IAM-related threats
- Create IAM architecture and access-control documentation