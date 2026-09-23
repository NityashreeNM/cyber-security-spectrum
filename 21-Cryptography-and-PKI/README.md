# Cyber Security Spectrum by Nityashree

# Domain 21: Cryptography and Public Key Infrastructure (PKI)

## 1. Domain Overview

Cryptography is a foundational cybersecurity discipline used to protect information, communications, identities, transactions, software, devices, and digital infrastructure.

Public Key Infrastructure (PKI) provides the trust infrastructure required to manage public-key cryptography at organizational scale.

Together, cryptography and PKI support security services such as:

- Confidentiality
- Integrity
- Authentication
- Authorization support
- Digital signatures
- Key establishment
- Non-repudiation
- Secure communication
- Identity assurance
- Data protection

Cryptography is therefore not simply an encryption technique.

It is a foundational security capability used throughout modern digital and cyber-physical environments.

---

# 2. Purpose of This Domain

The purpose of this domain is to develop a structured understanding of:

- Cryptographic fundamentals
- Symmetric cryptography
- Asymmetric cryptography
- Hash functions
- Message authentication
- Digital signatures
- Key establishment
- Cryptographic key management
- PKI
- Digital certificates
- Certificate Authorities
- Trust models
- TLS
- Secure email
- Code signing
- Device identity
- Hardware security
- Cryptographic modules
- Cryptographic agility
- Post-quantum cryptography

The objective is to understand both the mathematical foundations and the practical enterprise implementation of cryptography.

---

# 3. Security Services Provided by Cryptography

Cryptography can support:

### Confidentiality

Protect information from unauthorized disclosure.

### Integrity

Detect unauthorized modification.

### Authentication

Establish confidence in the identity of an entity or the origin of information.

### Digital Signature

Provide cryptographic evidence that data was signed using a particular private key and has not been modified after signing.

### Key Establishment

Enable communicating parties to establish cryptographic keys securely.

### Non-Repudiation

Digital signature systems can provide evidence that supports attribution of a signature, subject to the applicable technical, operational, and legal framework.

---

# 4. Cryptographic Fundamentals

A simplified cryptographic model is:

Plaintext → Cryptographic Operation → Ciphertext

and:

Ciphertext → Cryptographic Operation → Plaintext

Security depends on:

- Algorithm
- Key
- Key length
- Implementation
- Randomness
- Key management
- Operational controls

A strong algorithm cannot compensate for poor key management or insecure implementation.

---

# 5. Kerckhoffs's Principle

A cryptographic system should remain secure even when the algorithm is publicly known.

The security should depend primarily on the secrecy and protection of cryptographic keys rather than secrecy of the algorithm.

This principle is central to modern cryptographic engineering.

---

# 6. Symmetric Cryptography

Symmetric cryptography uses related or shared secret key material for cryptographic operations.

Common use cases include:

- Bulk data encryption
- Disk encryption
- Database encryption
- Network encryption
- File encryption
- Backup protection

Important concepts include:

- Block ciphers
- Stream ciphers
- Modes of operation
- Initialization vectors
- Nonces
- Authentication tags
- Key rotation

Examples of widely used symmetric algorithms include:

- AES
- ChaCha20

---

# 7. Authenticated Encryption

Authenticated Encryption provides confidentiality together with integrity and authenticity protection.

A commonly used construction is:

Plaintext + Key + Nonce → Ciphertext + Authentication Tag

Examples include:

- AES-GCM
- ChaCha20-Poly1305

Authenticated encryption is widely used in modern secure protocols and applications.

---

# 8. Asymmetric Cryptography

Asymmetric cryptography uses a public key and a corresponding private key.

Public key:

- May be distributed
- Used for verification or certain key-establishment operations

Private key:

- Must be protected
- Used for signing or corresponding private-key operations

Applications include:

- Digital signatures
- Key establishment
- Certificates
- Authentication
- Secure communication

---

# 9. Public Key Cryptography

Public-key cryptography enables security relationships without requiring the communicating parties to share a secret key beforehand.

Major mathematical families historically include:

- Integer factorization
- Discrete logarithms
- Elliptic curves

Modern cryptographic systems also include post-quantum approaches based on different mathematical assumptions.

---

# 10. Hash Functions

A cryptographic hash function maps input data to a fixed-size output.

Properties generally expected from a secure cryptographic hash include:

- Preimage resistance
- Second-preimage resistance
- Collision resistance

Common modern hash functions include:

- SHA-256
- SHA-384
- SHA-512
- SHA-3 family

Hash functions are used for:

- Integrity verification
- Digital signatures
- Password-related constructions
- Key derivation
- Message authentication constructions
- Software integrity
- Blockchain and distributed systems

A hash function is not encryption because a cryptographic hash is designed as a one-way transformation rather than reversible encryption.

---

# 11. Message Authentication Codes

A Message Authentication Code (MAC) provides integrity and authentication using shared secret key material.

Conceptually:

Message + Shared Secret → MAC

The recipient uses the shared secret to verify the MAC.

Examples include:

- HMAC
- CMAC

MACs are useful when communicating parties already share secret key material.

---

# 12. Key Derivation Functions

A Key Derivation Function (KDF) derives cryptographic keys from existing secret material.

KDFs are used to:

- Derive session keys
- Derive multiple keys from one secret
- Strengthen password-based key derivation
- Separate cryptographic purposes

Examples include:

- HKDF
- PBKDF2
- scrypt
- Argon2

Password-based key derivation requires special consideration because passwords are generally low-entropy human secrets.

---

# 13. Randomness and Entropy

Cryptographic security depends heavily on high-quality randomness.

Random values may be required for:

- Keys
- Nonces
- Initialization vectors
- Session identifiers
- Challenges
- Tokens

Weak randomness can compromise otherwise strong cryptographic systems.

Important concepts include:

- Entropy
- Cryptographically secure random number generation
- DRBG
- Seed material
- Randomness testing

---

# 14. Cryptographic Nonces and Initialization Vectors

Nonces and initialization vectors are values used by many cryptographic constructions.

Their security requirements depend on the algorithm and mode.

Important principles include:

- Correct generation
- Correct length
- Uniqueness where required
- Appropriate randomness where required
- No accidental reuse

Incorrect nonce reuse can cause severe security failures in certain cryptographic constructions.

---

# 15. Digital Signatures

Digital signatures provide cryptographic mechanisms for:

- Integrity
- Authentication of the signer
- Evidence associated with a signed message

A simplified model is:

Message + Private Key → Digital Signature

Verification:

Message + Signature + Public Key → Valid / Invalid

Applications include:

- Software signing
- Document signing
- Certificate signing
- Secure email
- Firmware signing
- Package signing
- Code integrity

---

# 16. Key Establishment

Key establishment enables parties to obtain shared cryptographic key material over potentially untrusted networks.

Common concepts include:

- Key agreement
- Key transport
- Diffie-Hellman
- Elliptic Curve Diffie-Hellman
- Key Encapsulation Mechanisms

Modern protocols typically combine key establishment with authentication and symmetric encryption.

---

# 17. Perfect Forward Secrecy

Perfect Forward Secrecy (PFS) limits the impact of later compromise of long-term private keys on previously established session keys.

Modern secure communication protocols can use ephemeral key-exchange mechanisms to provide this property.

PFS is particularly important for protecting historical communications.

---

# 18. Cryptographic Key Management

Key management is one of the most important operational aspects of cryptography.

The key lifecycle may include:

Generate → Distribute → Activate → Use → Rotate → Suspend → Revoke → Archive/Destroy

Key management must address:

- Generation
- Storage
- Distribution
- Access control
- Rotation
- Backup
- Recovery
- Revocation
- Compromise
- Destruction

NIST SP 800-57 provides key-management guidance covering cryptographic keying material and related management practices.

---

# 19. Cryptographic Key Hierarchies

Organizations may use hierarchical key structures.

Example:

Root Key
→ Key Encryption Key
→ Data Encryption Key
→ Encrypted Data

Benefits can include:

- Separation of duties
- Controlled key rotation
- Reduced exposure
- Scalable key management
- Different protection levels

Key hierarchy design should reflect the security architecture and operational requirements.

---

# 20. Key Rotation

Cryptographic keys should be rotated according to:

- Algorithm
- Key type
- Risk
- Exposure
- Usage
- Regulatory requirements
- Organizational policy
- Cryptographic lifecycle

Key rotation should be designed so that dependent systems can transition safely.

---

# 21. Key Compromise

If a cryptographic key is compromised, an organization may need to:

1. Detect compromise
2. Determine affected systems
3. Revoke affected credentials or certificates
4. Generate replacement keys
5. Reconfigure dependent systems
6. Investigate historical exposure
7. Rotate related credentials
8. Monitor for continued misuse
9. Document the incident

Key compromise procedures should be included in incident-response planning.

---

# 22. Cryptographic Key Storage

Sensitive key material may be protected using:

- Hardware Security Modules
- Trusted Platform Modules
- Secure enclaves
- Operating-system key stores
- Cloud Key Management Services
- Secrets-management platforms

Private keys and other sensitive cryptographic material should receive protection appropriate to their value and threat environment.

---

# 23. Hardware Security Modules

An HSM is a specialized security device designed to protect and perform operations involving cryptographic keys.

Typical capabilities include:

- Key generation
- Key storage
- Cryptographic operations
- Digital signing
- Key wrapping
- Secure key import/export
- Access control
- Audit support
- Tamper-related protections

HSMs are widely used in:

- Banking
- Payment systems
- Certificate Authorities
- Cloud services
- Enterprise PKI
- Code signing
- High-value transaction systems

---

# 24. Cryptographic Modules

A cryptographic module is the hardware, software, firmware, or combination that implements cryptographic functions and protects associated sensitive security parameters.

NIST FIPS 140-3 defines security requirements for cryptographic modules and references ISO/IEC 19790 and ISO/IEC 24759.

FIPS 140-3 validation is particularly relevant where validated cryptographic modules are required by applicable environments or procurement requirements.

---

# 25. Public Key Infrastructure

PKI is the collection of technologies, processes, policies, roles, and trust relationships used to manage public-key certificates and associated identities.

A simplified PKI ecosystem is:

Root CA → Intermediate CA → End-Entity Certificate

Supporting components may include:

- Certificate Authorities
- Registration Authorities
- Certificate repositories
- Certificate policies
- Certificate practice statements
- Revocation infrastructure
- OCSP
- CRLs
- Trust stores
- Key-management systems

---

# 26. Certificate Authority

A Certificate Authority (CA) issues and manages digital certificates.

A CA may:

- Validate certificate requests
- Issue certificates
- Renew certificates
- Revoke certificates
- Publish certificate status
- Protect CA private keys

CA compromise can have significant consequences because trusted certificates may be used to impersonate systems or identities.

---

# 27. Root CA

The Root CA is a trust anchor within a PKI hierarchy.

Root CA private keys require strong protection because compromise can undermine trust across the certificate hierarchy.

Security controls may include:

- Offline operation
- HSM protection
- Strict access control
- Multi-person control
- Ceremonies
- Secure backup
- Auditing
- Controlled activation

---

# 28. Intermediate CA

Intermediate CAs provide operational separation between the root trust anchor and end-entity certificates.

Benefits can include:

- Reduced root-key exposure
- Separation of functions
- Different certificate policies
- Easier operational management
- Limited blast radius

---

# 29. Digital Certificates

A digital certificate binds identity-related information to a public key.

Common certificate information includes:

- Subject
- Issuer
- Public key
- Validity period
- Serial number
- Key usage
- Extended key usage
- Subject Alternative Name
- Signature
- Certificate policies

X.509 is widely used for digital certificates and PKI systems.

---

# 30. Certificate Lifecycle

Certificate lifecycle management includes:

Request → Validate → Issue → Deploy → Monitor → Renew → Revoke/Expire → Replace

Organizations should maintain visibility into:

- Certificate ownership
- Expiration dates
- Key usage
- Issuing CA
- Deployment locations
- Renewal status
- Revocation status

Certificate expiration can cause large-scale service outages when not properly managed.

---

# 31. Certificate Revocation

Certificates may need to be revoked when:

- Private keys are compromised
- Certificates are incorrectly issued
- Identity information becomes invalid
- A system is retired
- Security policy requires revocation

Common revocation mechanisms include:

- Certificate Revocation Lists
- Online Certificate Status Protocol

Revocation design should consider availability and operational requirements.

---

# 32. Trust Models

Common trust models include:

### Hierarchical Trust

Root CA → Intermediate CA → End Entity

### Web of Trust

Trust relationships are established through peer or community-based signing relationships.

### Bridge or Federated Trust

Multiple PKI domains establish controlled trust relationships.

### Trust Stores

Operating systems, browsers, applications, and devices maintain collections of trusted certificates or trust anchors.

---

# 33. TLS and Secure Communications

Transport Layer Security (TLS) provides security for network communications.

TLS can provide:

- Confidentiality
- Integrity
- Server authentication
- Optional client authentication

A simplified TLS architecture is:

Client → TLS Handshake → Certificate Validation → Key Establishment → Encrypted Session

TLS security depends on:

- Protocol version
- Cipher suites
- Certificate validation
- Key exchange
- Randomness
- Endpoint configuration
- Private-key protection

TLS 1.3 is the modern TLS protocol version standardized by the IETF.

---

# 34. Mutual TLS

Mutual TLS (mTLS) authenticates both sides of a connection using certificates.

Traditional TLS:

Client → Server Authentication

mTLS:

Client ↔ Server Authentication

Common use cases include:

- Service-to-service communication
- APIs
- Microservices
- Zero Trust architectures
- Device authentication
- Enterprise applications

---

# 35. Certificate Pinning

Certificate or public-key pinning historically allowed applications to restrict which certificates or public keys they trusted for a particular service.

However, pinning introduces operational risks such as:

- Certificate rotation failures
- Key replacement problems
- Recovery complexity

Modern application architectures should carefully evaluate whether pinning is appropriate and how trust changes will be managed.

---

# 36. Code Signing

Code signing uses digital signatures to establish software integrity and publisher authenticity.

Applications include:

- Executables
- Mobile applications
- Firmware
- Drivers
- Packages
- Scripts
- Software updates

A secure code-signing architecture should protect:

- Signing keys
- Build systems
- Signing services
- Release pipelines
- Certificate lifecycle

Code-signing keys should receive protection appropriate to their criticality.

---

# 37. Firmware Signing

Firmware signing helps devices verify that firmware originates from an authorized source and has not been modified.

A simplified process is:

Firmware → Hash → Digital Signature → Device Verification → Installation

Firmware signing can support:

- Secure boot
- Secure updates
- Device integrity
- Supply-chain security

This is particularly important for IoT and OT environments.

---

# 38. Secure Boot

Secure boot establishes a chain of trust beginning with a hardware- or firmware-rooted trust anchor.

Example:

Hardware Root of Trust → Bootloader → Firmware → Operating System

Each stage verifies the integrity or authenticity of the next stage.

Secure boot helps prevent unauthorized software from executing during system startup.

---

# 39. Cryptography in Identity and Access Management

Cryptography supports:

- Authentication
- Password protection
- MFA
- Smart cards
- Hardware security keys
- Certificates
- Kerberos
- Token protection
- Session security

Cryptographic mechanisms should be integrated with identity architecture rather than treated as isolated components.

---

# 40. Cryptography in Cloud Security

Cloud environments commonly use:

- Key Management Services
- Hardware Security Modules
- Encryption at rest
- Encryption in transit
- Certificate services
- Secrets management
- Customer-managed keys
- Envelope encryption

Cloud cryptographic architecture should address:

- Key ownership
- Key location
- Key access
- Separation of duties
- Rotation
- Backup
- Recovery
- Provider dependency

---

# 41. Cryptography in IoT Security

IoT systems may use cryptography for:

- Device identity
- Secure onboarding
- Secure communication
- Firmware verification
- Secure updates
- Data protection
- Device authentication

A common architecture is:

Device Identity → Secure Channel → Cloud/Platform Authentication

Cryptographic design must account for constrained devices, hardware capabilities, lifecycle, and manufacturing processes.

---

# 42. Cryptography in OT and ICS Security

OT environments may use cryptography for:

- Secure remote access
- Device authentication
- Secure protocols
- Firmware integrity
- Software signing
- Engineering workstation protection
- Data protection

OT cryptographic design must consider:

- Availability
- Latency
- Legacy systems
- Safety
- Protocol limitations
- Maintenance windows
- Long equipment lifecycles

Security controls should not be introduced without considering operational and safety requirements.

---

# 43. Cryptography in Privacy Engineering

Cryptographic techniques can support privacy through:

- Encryption
- Pseudonymization
- Tokenization
- Secure key management
- Confidential computing
- Secure multiparty computation
- Homomorphic encryption
- Privacy-preserving protocols

The appropriate technique depends on the use case, threat model, performance requirements, and data lifecycle.

---

# 44. Cryptographic Failures

Common cryptographic failures include:

- Weak algorithms
- Deprecated protocols
- Short keys
- Hard-coded keys
- Key reuse
- Poor randomness
- Nonce reuse
- Improper certificate validation
- Insecure key storage
- Missing certificate renewal
- Weak password hashing
- Incorrect cryptographic implementation
- Failure to rotate keys
- Inadequate revocation
- Unsupported cryptographic dependencies

Many cryptographic failures result from implementation and lifecycle weaknesses rather than from breaking the underlying mathematics.

---

# 45. Cryptographic Agility

Cryptographic agility is the capability to change cryptographic algorithms, parameters, keys, and protocols without requiring uncontrolled redesign of the entire environment.

Organizations should consider:

- Algorithm inventories
- Protocol dependencies
- Certificate dependencies
- Key-management systems
- Hardware support
- Software support
- Migration processes
- Testing
- Backward compatibility

Cryptographic agility is increasingly important because cryptographic standards and threat assumptions evolve.

---

# 46. Cryptographic Inventory

Organizations should know where cryptography is used.

An inventory may include:

| Asset | Protocol/Algorithm | Key Type | Certificate | Owner | Criticality | Migration Status |
|---|---|---|---|---|---|---|
| Web Application | TLS | EC/RSA | Yes | Application Team | High | Current |
| Database | AES | Symmetric | No | Data Team | Critical | Current |
| Firmware | Digital Signature | Public Key | Yes | Product Security | High | Review |
| VPN | TLS/IPsec | Mixed | Yes | Network Team | High | Current |

A cryptographic inventory is a foundational requirement for effective crypto-agility and post-quantum migration.

---

# 47. Post-Quantum Cryptography

Quantum computing creates a future threat to some widely used public-key cryptographic systems.

Post-Quantum Cryptography (PQC) develops cryptographic algorithms designed to resist attacks from sufficiently capable quantum computers.

NIST finalized three principal PQC standards in 2024:

- FIPS 203 — ML-KEM
- FIPS 204 — ML-DSA
- FIPS 205 — SLH-DSA

These standards cover key establishment and digital signatures.

NIST's current guidance encourages organizations to begin migration planning and implementation toward quantum-resistant cryptography.

---

# 48. Quantum-Related Cryptographic Risk

Important concepts include:

### Harvest Now, Decrypt Later

An adversary may collect encrypted information today with the intention of decrypting it in the future if suitable quantum capabilities become available.

This is especially relevant to information with long confidentiality lifetimes.

### Cryptographically Relevant Quantum Computing

A sufficiently capable quantum computer could threaten some existing public-key cryptographic mechanisms.

Organizations should therefore evaluate the lifespan and sensitivity of protected information.

---

# 49. Post-Quantum Migration

A practical migration lifecycle is:

Discover → Inventory → Classify → Prioritize → Test → Pilot → Migrate → Validate → Monitor

Organizations should identify:

- Vulnerable algorithms
- Long-lived certificates
- Public-key dependencies
- Embedded cryptography
- Vendor dependencies
- Legacy systems
- Protocol dependencies
- Long-lived sensitive data

Migration should include interoperability and operational testing.

---

# 50. PKI and Post-Quantum Cryptography

Post-quantum migration affects PKI because organizations may need to update:

- Certificate formats
- Certificate Authorities
- Signature algorithms
- Key establishment
- HSM capabilities
- Trust stores
- TLS implementations
- Device certificates
- Code-signing infrastructure

PKI migration should therefore be treated as an enterprise architecture activity.

---

# 51. Cryptographic Supply Chain

Cryptographic dependencies may exist in:

- Operating systems
- Libraries
- Applications
- Hardware
- HSMs
- Cloud services
- Network equipment
- IoT devices
- OT systems
- PKI products

Supply-chain security should consider:

- Algorithm implementation
- Vendor support
- Security validation
- Update mechanisms
- Vulnerability management
- Cryptographic agility
- Long-term support

---

# 52. Cryptographic Governance

Organizations should establish policies covering:

- Approved algorithms
- Key lengths
- Key lifetimes
- Certificate requirements
- Key storage
- HSM usage
- Cryptographic exceptions
- Deprecated algorithms
- Key compromise
- Certificate revocation
- Cryptographic migration
- Post-quantum readiness

Cryptographic policy should align with enterprise security architecture and applicable regulatory requirements.

---

# 53. Practical Labs

## Lab 1: Hashing

Implement and compare:

- SHA-256
- SHA-384
- SHA-512
- SHA-3

Measure:

- Output
- Input sensitivity
- Collision considerations
- Performance

Do not use hashing as a substitute for encryption.

## Lab 2: Symmetric Encryption

Create a controlled demonstration using:

- AES
- Authenticated encryption
- Secure key handling

Document:

- Plaintext
- Key
- Nonce/IV
- Ciphertext
- Authentication result

## Lab 3: Public-Key Cryptography

Generate a test key pair and demonstrate:

- Public key
- Private key
- Signing
- Verification

Use only controlled test keys.

## Lab 4: TLS Inspection

Analyze a TLS connection and identify:

- Protocol version
- Certificate
- Issuer
- Subject Alternative Name
- Validity
- Key exchange
- Cipher suite

## Lab 5: PKI Lab

Build a controlled test PKI containing:

- Root CA
- Intermediate CA
- End-entity certificate

Demonstrate:

- Certificate issuance
- Certificate validation
- Certificate renewal
- Certificate revocation

## Lab 6: Certificate Lifecycle

Create a certificate inventory and identify:

- Expiring certificates
- Owners
- Services
- Issuing CA
- Renewal process

## Lab 7: Code Signing

Create a controlled code-signing workflow:

Build → Hash → Sign → Verify → Release

Document key protection and verification steps.

## Lab 8: Cryptographic Inventory

Create a cryptographic inventory for a hypothetical enterprise.

Map:

Application → Protocol → Algorithm → Key → Certificate → Owner → Risk

## Lab 9: PQC Readiness

Create a migration assessment for a hypothetical enterprise.

Identify:

- RSA dependencies
- ECC dependencies
- TLS dependencies
- PKI dependencies
- Code-signing dependencies
- Long-lived sensitive data

---

# 54. Professional Projects

## Project 1: Enterprise PKI Architecture

Design:

- Root CA
- Intermediate CAs
- Certificate policies
- Certificate lifecycle
- Revocation
- HSM protection
- Monitoring
- Disaster recovery

## Project 2: Enterprise Cryptographic Management Program

Develop:

- Cryptographic policy
- Algorithm standards
- Key-management lifecycle
- Key inventory
- Certificate inventory
- Exception process
- Compromise-response process

## Project 3: Cryptographic Discovery Program

Create a framework for discovering cryptography across:

- Applications
- Networks
- Cloud
- IoT
- OT
- Endpoints
- Databases
- PKI
- Code signing

## Project 4: Post-Quantum Migration Strategy

Develop:

- Cryptographic inventory
- Dependency map
- Risk classification
- Migration priorities
- Vendor assessment
- Pilot strategy
- Validation plan

## Project 5: Secure IoT PKI

Design a device-identity architecture using:

- Device certificates
- Manufacturing identity
- Secure provisioning
- Certificate lifecycle
- Secure firmware updates
- Revocation
- Device retirement

---

# 55. Professional Workflow

A cybersecurity professional working in cryptography and PKI may follow:

1. Identify the business requirement
2. Identify the security service required
3. Select appropriate cryptographic mechanisms
4. Identify algorithms and protocols
5. Design key management
6. Establish trust relationships
7. Protect cryptographic keys
8. Implement certificates where required
9. Integrate cryptography into applications and infrastructure
10. Validate implementation
11. Monitor cryptographic assets
12. Manage key and certificate lifecycle
13. Respond to compromise
14. Track cryptographic vulnerabilities
15. Maintain cryptographic agility
16. Assess post-quantum dependencies
17. Migrate when required
18. Retire obsolete cryptography securely

---

# 56. Global Enterprise Context

Cryptography and PKI are foundational across:

- Banking
- Healthcare
- Government
- Telecommunications
- Cloud computing
- Manufacturing
- Automotive
- Aerospace
- Energy
- Utilities
- Retail
- Software
- IoT
- OT
- Critical infrastructure

Cryptographic architecture must account for:

- Business criticality
- Data sensitivity
- System lifetime
- Threat model
- Performance
- Interoperability
- Regulatory requirements
- Vendor dependencies
- Future cryptographic migration

---

# 57. Career Relevance

This domain connects to roles such as:

- Cryptography Engineer
- PKI Engineer
- Security Engineer
- Security Architect
- Security Infrastructure Engineer
- Identity Security Engineer
- Cloud Security Engineer
- Application Security Engineer
- Product Security Architect
- Hardware Security Engineer
- IoT Security Architect
- OT Security Architect
- Cybersecurity Researcher
- Post-Quantum Cryptography Specialist

Cryptography is also an important foundational capability for professionals working in security architecture, product security, identity, privacy, cloud, IoT, OT, and cyber-physical systems.

---

# 58. Learning Outcomes

After completing this domain, a learner should be able to:

- Explain fundamental cryptographic concepts
- Distinguish symmetric and asymmetric cryptography
- Explain hashing and MACs
- Understand digital signatures
- Understand key establishment
- Explain cryptographic key management
- Understand PKI architecture
- Explain Certificate Authorities
- Understand digital certificates
- Understand certificate lifecycle management
- Explain TLS and mTLS
- Understand code signing
- Understand secure boot and firmware signing
- Understand HSMs and cryptographic modules
- Identify common cryptographic failures
- Build a cryptographic inventory
- Understand cryptographic agility
- Explain post-quantum cryptography
- Understand PQC migration requirements
- Design basic enterprise PKI architecture

---

# 59. Domain Relationships

Cryptography and PKI connects directly with:

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
- Vulnerability Management
- Governance, Risk and Compliance
- Security Engineering and Resilience
- Privacy Engineering and Data Protection
- Cybersecurity Supply Chain Risk Management
- AI and Emerging Technology Security

Cryptography therefore functions as a foundational security capability supporting almost every major cybersecurity domain.

---

# 60. Standards and Frameworks

Important references include:

- NIST SP 800-57 — Recommendation for Key Management
- NIST FIPS 140-3 — Security Requirements for Cryptographic Modules
- NIST FIPS 186-5 — Digital Signature Standard
- NIST SP 800-56A — Key-Establishment Schemes Using Discrete Logarithm Cryptography
- NIST SP 800-56B — Key-Establishment Schemes Using Integer Factorization Cryptography
- NIST SP 800-208 — Stateful Hash-Based Signature Schemes
- NIST FIPS 203 — ML-KEM
- NIST FIPS 204 — ML-DSA
- NIST FIPS 205 — SLH-DSA
- ISO/IEC 19790 — Security Requirements for Cryptographic Modules
- ISO/IEC 24759 — Test Requirements for Cryptographic Modules
- ISO/IEC 11770 series — Key Management
- ISO/IEC 27001
- ISO/IEC 27002
- IETF TLS standards
- X.509 certificate and PKI standards
- Relevant industry-specific cryptographic requirements

Standards should be selected according to the organization's architecture, regulatory environment, risk profile, and applicable requirements.

---

# 61. Security Design Principles

Effective cryptographic architecture should follow:

- Use well-established cryptographic standards
- Do not design proprietary cryptographic algorithms without specialist justification
- Protect keys as high-value security assets
- Separate key management from application logic where appropriate
- Use authenticated encryption where appropriate
- Validate certificates correctly
- Avoid deprecated algorithms and protocols
- Maintain cryptographic inventories
- Plan for key compromise
- Plan for certificate expiration
- Maintain cryptographic agility
- Prepare for post-quantum migration

Strong cryptography requires strong engineering and lifecycle management.

---

# 62. Key Takeaways

Cryptography is more than encryption.

It provides the security foundations for:

- Confidentiality
- Integrity
- Authentication
- Digital signatures
- Secure communication
- Identity
- Trust
- Software integrity
- Device identity
- Data protection

PKI operationalizes public-key trust at organizational scale.

Key management determines whether cryptographic protection remains secure throughout its lifecycle.

Post-quantum migration adds another strategic requirement: organizations need visibility into their cryptographic dependencies and the ability to change cryptographic mechanisms when required.

---

# 63. Professional Perspective

Traditional cybersecurity often asks:

"How do we protect this system?"

Cryptographic engineering adds another fundamental question:

"How do we establish, protect, verify, and maintain trust between systems, identities, data, and devices?"

That trust may depend on:

Keys → Certificates → Algorithms → Protocols → Identity → Hardware → Software → Governance

A mature security architecture therefore treats cryptography as a strategic infrastructure capability rather than an implementation detail.

---

# 64. Domain Completion Checklist

- [ ] I understand cryptographic security services.
- [ ] I understand symmetric cryptography.
- [ ] I understand asymmetric cryptography.
- [ ] I understand cryptographic hashing.
- [ ] I understand MACs.
- [ ] I understand KDFs.
- [ ] I understand randomness and entropy.
- [ ] I understand digital signatures.
- [ ] I understand key establishment.
- [ ] I understand cryptographic key management.
- [ ] I understand HSMs.
- [ ] I understand cryptographic modules.
- [ ] I understand PKI architecture.
- [ ] I understand Certificate Authorities.
- [ ] I understand X.509 certificates.
- [ ] I understand certificate lifecycle management.
- [ ] I understand TLS and mTLS.
- [ ] I understand code signing.
- [ ] I understand secure boot.
- [ ] I understand firmware signing.
- [ ] I understand cryptographic failures.
- [ ] I understand cryptographic agility.
- [ ] I can build a cryptographic inventory.
- [ ] I understand post-quantum cryptography.
- [ ] I understand PQC migration.
- [ ] I can map cryptographic controls to recognized standards.
- [ ] I can design a basic enterprise PKI architecture.

---

# 65. Recommended Reference Landscape

Primary references for further study include:

- NIST Cryptographic Standards and Guidelines
- NIST SP 800-57
- NIST FIPS 140-3
- NIST FIPS 186-5
- NIST FIPS 203
- NIST FIPS 204
- NIST FIPS 205
- NIST SP 800-208
- ISO/IEC 11770 series
- ISO/IEC 19790
- ISO/IEC 24759
- IETF TLS specifications
- X.509 and PKI standards
- Relevant cloud-provider cryptographic architecture guidance
- Relevant industry-specific cryptographic requirements

Standards evolve. Always verify the current publication, revision, errata, and applicability before using a standard for production architecture, formal compliance, audit, procurement, or regulatory purposes.

---

# 66. Conclusion

Cryptography and Public Key Infrastructure form one of the foundational layers of modern cybersecurity.

The discipline connects:

Cryptography → Keys → Identity → Certificates → Trust → Secure Communication → Software Integrity → Device Security → Data Protection

A mature enterprise capability therefore requires more than selecting an encryption algorithm.

It requires:

- Sound cryptographic design
- Strong key management
- Secure PKI
- Protected cryptographic modules
- Correct implementation
- Lifecycle management
- Continuous monitoring
- Cryptographic agility
- Post-quantum readiness

The long-term objective is to establish and maintain trustworthy digital interactions across applications, users, devices, services, cloud platforms, industrial systems, and cyber-physical environments.

---

# 67. Cyber Security Spectrum by Nityashree

## From Generic to Niche

A structured cybersecurity spectrum connecting:

Awareness → Fundamentals → Domains → Specialization → Architecture → Engineering → Advanced Security

Domain 21 establishes the cryptographic trust layer underlying many of the cybersecurity capabilities explored across the spectrum.

**Cyber Security Spectrum by Nityashree**

**From Generic to Niche.**