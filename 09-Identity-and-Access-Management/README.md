# Cyber Security Spectrum by Nityashree

## 09. Identity and Access Management

Overview

Identity and Access Management (IAM) is the process of managing digital identities and controlling who or what can access systems, applications, devices, networks, and data.

IAM helps organizations ensure that:

- The right user gets the right access
- Access is provided for the right purpose
- Access is available at the right time
- Unauthorized access is prevented
- User activities are traceable
- Access is reviewed and removed when no longer required

IAM is a core security capability for enterprise IT, cloud, IoT, OT, and Cyber-Physical Systems.

1. Core IAM Concepts

Identity

An identity represents a user, device, application, service, or system.

Examples:

- Employee identity
- Administrator identity
- Service account
- IoT device identity
- Machine identity
- Application identity
- Vendor identity

Authentication

Authentication verifies who or what an entity is.

Common authentication methods:

- Username and password
- Multi-factor authentication
- Smart cards
- Digital certificates
- Biometrics
- Security keys
- One-time passwords
- Device-based authentication

Authorization

Authorization determines what an authenticated identity is allowed to do.

Examples:

- Read a file
- Modify a database
- Access a cloud service
- Configure a PLC
- Restart a server
- Change a security policy

Accounting and Auditing

Accounting records what an identity did.

Audit information may include:

- Login time
- Logout time
- Source IP address
- Accessed resource
- Performed action
- Privilege changes
- Failed login attempts
- Administrative activity

2. AAA Security Model

IAM commonly follows the AAA model.

Authentication

Who are you?

Authorization

What are you allowed to do?

Accounting

What did you do?

3. IAM Lifecycle

Identity management should cover the complete identity lifecycle.

Joiner

When a new employee, device, or application is created:

- Create identity
- Verify identity
- Assign role
- Provide required access
- Enable security controls

Mover

When responsibilities change:

- Review current access
- Remove unnecessary permissions
- Assign new permissions
- Update roles
- Record the change

Leaver

When a user or device leaves the environment:

- Disable identity
- Revoke sessions
- Remove access
- Rotate shared credentials
- Recover devices and tokens
- Preserve audit records

4. Principle of Least Privilege

The principle of least privilege means that an identity should receive only the minimum access required to perform its task.

Examples:

- A developer should not automatically receive production access
- A user should not have administrator privileges by default
- An IoT device should communicate only with required services
- An OT engineer should access only authorized industrial systems
- A service account should have limited permissions

5. Need-to-Know and Separation of Duties

Need-to-Know

Users should access only the information required for their responsibilities.

Separation of Duties

Critical activities should be divided between different people or roles to reduce fraud, misuse, and unauthorized changes.

Example:

- One person requests access
- Another person approves access
- The system administrator provisions access
- An auditor reviews the activity

6. Access Control Models

Role-Based Access Control — RBAC

Access is assigned according to a user's role.

Examples:

- HR user
- Network administrator
- Security analyst
- Cloud administrator
- OT engineer

Attribute-Based Access Control — ABAC

Access decisions are based on attributes such as:

- User identity
- Department
- Device security status
- Location
- Time
- Resource sensitivity
- Risk level

Mandatory Access Control — MAC

Access is controlled through centrally defined security labels and policies.

Discretionary Access Control — DAC

Resource owners can decide who receives access.

Rule-Based Access Control

Access is granted or denied based on predefined rules.

7. Multi-Factor Authentication

Multi-factor authentication uses two or more different authentication factors.

Knowledge Factor

Something you know:

- Password
- PIN
- Security answer

Possession Factor

Something you have:

- Mobile device
- Hardware token
- Smart card
- Security key

Inherence Factor

Something you are:

- Fingerprint
- Facial recognition
- Iris recognition

A strong IAM architecture should use MFA for:

- Administrator accounts
- Remote access
- Cloud consoles
- VPN access
- Privileged operations
- Vendor access
- Critical OT systems, where technically and operationally feasible

8. Privileged Access Management

Privileged Access Management (PAM) controls accounts with elevated permissions.

Privileged accounts include:

- Domain administrators
- Root users
- Cloud administrators
- Database administrators
- Network administrators
- OT engineering accounts
- Application administrators

PAM Controls

- Just-in-time access
- Just-enough access
- Password vaulting
- Session recording
- Approval workflows
- Credential rotation
- Privileged activity monitoring
- Emergency access procedures
- Administrative account separation

9. Identity Federation and Single Sign-On

Single Sign-On — SSO

SSO allows users to access multiple applications using one authenticated identity.

Benefits include:

- Better user experience
- Centralized authentication
- Reduced password reuse
- Easier access management
- Centralized logging

Identity Federation

Federation allows identities managed by one organization or identity provider to access services provided by another organization.

Common technologies include:

- SAML
- OAuth 2.0
- OpenID Connect
- WS-Federation

10. Important IAM Technologies

Common IAM components include:

- Identity Provider
- Directory Service
- Authentication Server
- Authorization Server
- Access Management System
- Privileged Access Management
- Identity Governance and Administration
- Multi-Factor Authentication
- Single Sign-On
- Certificate Authority
- Secrets Management System
- Policy Decision Point
- Policy Enforcement Point

11. Directory and Identity Services

Examples of directory and identity services:

- Active Directory
- LDAP
- Microsoft Entra ID
- OpenLDAP
- FreeIPA
- Cloud Identity Services
- Identity-as-a-Service platforms

Directory Security Topics

- User and group management
- Password policies
- Account lockout
- Group membership
- Privileged groups
- Service accounts
- Directory replication
- Authentication protocols
- Directory auditing

12. Service Accounts and Machine Identities

Service accounts are used by applications, services, scripts, and automated systems.

Security risks include:

- Hardcoded passwords
- Excessive permissions
- Never-expiring credentials
- Shared accounts
- Lack of monitoring
- Unmanaged secrets

Recommended Controls

- Use managed identities where possible
- Avoid shared accounts
- Rotate credentials
- Restrict permissions
- Store secrets securely
- Monitor usage
- Disable unused accounts
- Review service account access regularly

13. IAM in Cloud Security

Cloud IAM controls access to:

- Virtual machines
- Storage
- Databases
- Cloud networks
- Kubernetes clusters
- Serverless functions
- Security services
- Cloud management consoles

Cloud IAM Best Practices

- Enable MFA
- Avoid using root accounts
- Use roles instead of permanent credentials
- Apply least privilege
- Separate development and production access
- Use temporary credentials
- Monitor privilege escalation
- Review policies regularly
- Protect access keys
- Log administrative actions

14. IAM in IoT Security

IoT environments require identity management for both users and devices.

IoT Identity Requirements

- Unique device identity
- Device registration
- Certificate-based authentication
- Secure credential storage
- Device ownership tracking
- Device lifecycle management
- Secure provisioning
- Credential rotation
- Device revocation
- Mutual TLS where appropriate

IoT IAM Questions

- Is every device uniquely identifiable?
- Can a device impersonate another device?
- How are devices onboarded?
- How are compromised devices revoked?
- Are credentials embedded in firmware?
- Can devices communicate with unauthorized services?
- How are device identities retired?

15. IAM in OT and ICS Security

IAM is important for controlling access to:

- SCADA systems
- HMIs
- PLC engineering workstations
- DCS systems
- Historian servers
- Remote access gateways
- Industrial network devices
- Safety systems

OT IAM Considerations

- Use named accounts where possible
- Restrict shared accounts
- Control vendor access
- Use jump servers
- Apply role-based permissions
- Review engineering workstation access
- Protect privileged accounts
- Monitor configuration changes
- Avoid unsafe authentication changes
- Consider legacy system limitations
- Maintain emergency and manual access procedures

16. Zero Trust and IAM

Zero Trust assumes that access should not be trusted automatically based only on network location.

Important principles include:

- Verify explicitly
- Use least-privilege access
- Assume breach
- Continuously evaluate risk
- Validate user and device identity
- Enforce policy before access
- Monitor sessions and activities

Zero Trust IAM Controls

- Strong identity verification
- MFA
- Device posture checks
- Conditional access
- Micro-segmentation
- Just-in-time access
- Continuous monitoring
- Risk-based authorization
- Privileged access controls

17. IAM Threats

Common IAM-related threats include:

- Password attacks
- Credential stuffing
- Phishing
- MFA fatigue
- Session hijacking
- Token theft
- Privilege escalation
- Account takeover
- Excessive permissions
- Orphaned accounts
- Insider misuse
- Compromised service accounts
- Hardcoded credentials
- Weak API authentication
- Insecure device provisioning
- Unauthorized vendor access

18. IAM Security Controls

Recommended controls include:

- Strong password policies
- MFA
- Least privilege
- RBAC
- PAM
- SSO
- Access reviews
- Joiner-mover-leaver process
- Conditional access
- Secure secrets management
- Certificate management
- Session management
- Identity monitoring
- Privilege escalation detection
- Account disablement
- Audit logging
- Periodic compliance reviews

19. IAM Monitoring and Detection

Monitor events such as:

- Repeated failed logins
- Login from unusual locations
- Login at unusual times
- New administrator creation
- Privilege changes
- Group membership changes
- MFA changes
- Password reset activity
- Service account misuse
- Unusual API access
- Suspicious token usage
- Dormant account activity
- Vendor access outside approved windows

20. IAM Incident Response

Detection

Identify suspicious identity activity through:

- IAM logs
- SIEM alerts
- Authentication monitoring
- Cloud activity logs
- Endpoint telemetry
- Network monitoring

Containment

- Disable compromised accounts
- Revoke active sessions
- Reset credentials
- Rotate secrets
- Remove unauthorized permissions
- Block suspicious devices
- Restrict remote access

Recovery

- Restore approved permissions
- Re-register compromised devices
- Validate identity policies
- Review access logs
- Investigate the root cause
- Improve preventive controls

21. Practical IAM Labs

Practice the following activities:

- Create users and groups in Linux
- Configure Linux file permissions
- Explore Active Directory concepts
- Configure RBAC in a cloud platform
- Create and test IAM policies
- Enable MFA
- Build a simple SSO flow
- Explore OAuth 2.0 and OpenID Connect
- Configure an LDAP directory
- Study Kerberos authentication
- Create a PAM access workflow
- Analyze authentication logs
- Detect brute-force login attempts
- Implement certificate-based device identity
- Design IAM for an IoT gateway
- Design secure vendor access for an OT network

22. Practical Projects

Project 1: Enterprise IAM Architecture

Design an IAM architecture containing:

- Identity provider
- Directory service
- MFA
- SSO
- RBAC
- PAM
- SIEM integration
- Access review process

Project 2: Cloud IAM Policy Review

Review cloud IAM policies and identify:

- Excessive permissions
- Wildcard permissions
- Unused roles
- Long-lived access keys
- Missing MFA
- Privilege escalation paths

Project 3: IoT Device Identity Architecture

Design a device identity lifecycle covering:

- Device manufacturing
- Secure provisioning
- Certificate issuance
- Device onboarding
- Authentication
- Authorization
- Credential rotation
- Device revocation
- Device retirement

Project 4: OT Remote Access Architecture

Design secure remote access for an industrial facility using:

- Vendor identity verification
- MFA
- Jump server
- Time-bound access
- Approval workflow
- Session monitoring
- Network segmentation
- Emergency access procedure

23. Learning Goals

By completing this section, you should be able to:

- Explain authentication and authorization
- Understand the AAA model
- Apply least privilege
- Design RBAC and ABAC models
- Explain MFA and SSO
- Understand identity federation
- Design privileged access controls
- Secure service accounts
- Manage machine and device identities
- Apply IAM to cloud environments
- Apply IAM to IoT and OT systems
- Understand Zero Trust IAM
- Identify IAM threats
- Design IAM monitoring and incident response
- Create an enterprise IAM architecture

24. References

- NIST Digital Identity Guidelines
- NIST Zero Trust Architecture
- NIST Cybersecurity Framework
- CIS Controls
- OWASP Authentication Cheat Sheet
- OWASP Authorization Cheat Sheet
- OAuth 2.0
- OpenID Connect
- SAML
- MITRE ATT&CK
- IEC 62443 identity and access control concepts

---

Focus: Secure identities, controlled access, least privilege, and Zero Trust across enterprise IT, cloud, IoT, OT, and cyber-physical systems.

## Learning Outcome

After completing this section, you should be able to:

- Explain identity, authentication, authorization, and accounting
- Understand the IAM lifecycle
- Apply the principle of least privilege
- Design RBAC and ABAC models
- Explain MFA, SSO, and identity federation
- Understand Privileged Access Management
- Secure service accounts and machine identities
- Apply IAM principles to cloud, IoT, OT, and CPS environments
- Understand IAM in Zero Trust Architecture
- Identify common IAM threats
- Design basic IAM security controls
- Create an IAM architecture for enterprise and product security

## Conclusion

Identity and Access Management is the foundation of secure access across modern digital and cyber-physical environments.

Strong IAM practices reduce unauthorized access, privilege misuse, credential compromise, and identity-related security risks.

**Cyber Security Spectrum by Nityashree**  
*Building strong cybersecurity foundations for secure digital and cyber-physical systems.*