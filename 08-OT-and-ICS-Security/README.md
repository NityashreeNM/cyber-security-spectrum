OT and ICS Security

Overview

Operational Technology (OT) and Industrial Control Systems (ICS) security focuses on protecting systems that monitor and control physical processes in industries such as manufacturing, energy, water treatment, healthcare, transportation, and critical infrastructure.

Unlike traditional IT security, OT security must prioritize:

- Safety of people and processes
- Availability and reliability
- Real-time operations
- Equipment protection
- Process integrity
- Secure remote access
- Business continuity

1. OT and ICS Fundamentals

What is OT?

Operational Technology includes hardware and software used to monitor, control, and operate physical equipment and industrial processes.

Examples:

- Industrial machines
- Sensors and actuators
- PLCs
- SCADA systems
- Distributed Control Systems
- Safety Instrumented Systems
- Industrial networks
- Building automation systems

What is ICS?

Industrial Control Systems are systems used to control and monitor industrial processes.

Common ICS environments include:

- Manufacturing plants
- Power generation and distribution
- Oil and gas facilities
- Water treatment plants
- Chemical industries
- Transportation systems
- Healthcare facilities

2. Main ICS Components

Sensors

Collect physical data such as:

- Temperature
- Pressure
- Flow
- Level
- Vibration
- Humidity

Actuators

Perform physical actions such as:

- Opening or closing valves
- Starting or stopping motors
- Controlling pumps
- Adjusting temperature
- Moving industrial equipment

PLC — Programmable Logic Controller

A PLC is an industrial computer that executes control logic and interacts with sensors and actuators.

RTU — Remote Terminal Unit

An RTU collects field data and communicates with a central control system, especially in geographically distributed environments.

HMI — Human Machine Interface

An HMI allows operators to monitor processes and interact with industrial equipment.

SCADA — Supervisory Control and Data Acquisition

SCADA systems provide:

- Supervisory monitoring
- Data collection
- Alarm management
- Remote control
- Historical data visualization

DCS — Distributed Control System

A DCS is commonly used in continuous industrial processes such as:

- Chemical plants
- Refineries
- Power plants
- Pharmaceutical manufacturing

SIS — Safety Instrumented System

A Safety Instrumented System is designed to bring a process to a safe state when dangerous conditions occur.

3. OT vs IT Security


OT vs IT Security

Area	--- IT Security ---	 OT Security
1.Main priority --- 	Confidentiality ----	Safety and availability
2.System changes	---Frequent---	Carefully controlled
3.Downtime---	Usually manageable	---May be dangerous or expensive
4 Patch management---	Regular patching---	Risk-based patching
5.System lifespan	---Often shorter---	Often 10–30 years
6.Environment---	Enterprise systems	---Physical processes
7.Security testing---	More testing---Must avoid process disruption
8.Incident impact	---Data loss or service outage---	Safety, equipment, and production impact


4. Industrial Network Architecture

Common Network Layers

1. Enterprise IT Network
2. Industrial DMZ
3. Supervisory Network
4. Control Network
5. Cell/Area Zone
6. Field Network
7. Sensors and Actuators

Purdue Enterprise Reference Architecture

The Purdue Model helps separate enterprise IT systems from industrial control systems.

Typical levels include:

- Level 0: Physical process
- Level 1: Sensors and actuators
- Level 2: Basic control systems
- Level 3: Site operations and control
- Level 3.5: Industrial DMZ
- Level 4: Enterprise IT systems
- Level 5: Enterprise network

5. Industrial Communication Protocols

Important industrial protocols include:

- Modbus TCP
- Modbus RTU
- DNP3
- OPC UA
- OPC Classic
- EtherNet/IP
- PROFINET
- PROFIBUS
- IEC 60870-5-104
- IEC 61850
- MQTT
- BACnet
- CAN bus

Security Questions for Protocols

For every protocol, understand:

- Is authentication supported?
- Is encryption supported?
- Is message integrity protected?
- Can commands be replayed?
- Can unauthorized users write values?
- Is the protocol legacy or modern?
- What compensating controls are required?

6. OT Threat Landscape

Common OT security threats include:

- Unauthorized remote access
- Ransomware affecting production
- Malware entering through IT networks
- Compromised engineering workstations
- Manipulation of PLC logic
- Unauthorized changes to HMI screens
- Weak passwords
- Exposed industrial services
- Insecure vendor access
- USB-based malware
- Network misconfiguration
- Denial-of-service attacks
- Loss of visibility into industrial assets
- Manipulation of sensor values
- Unsafe process commands

7. OT Threat Modeling

Threat modeling helps identify how attackers could affect industrial systems and physical processes.

Useful Approaches

- STRIDE
- STRIDE-OT
- MITRE ATT&CK for ICS
- Attack trees
- Data Flow Diagrams
- Cyber Kill Chain
- Zones and Conduits analysis
- Safety and security risk assessment

Threat Modeling Questions

- What are the critical assets?
- What physical process does each asset control?
- Who can access the system?
- What happens if the system is unavailable?
- What happens if the process data is manipulated?
- Can an attacker change PLC logic?
- Can remote access bypass security controls?
- What is the safety impact?
- What is the recovery process?

8. IEC 62443 Concepts

IEC 62443 is a major cybersecurity standards family for industrial automation and control systems.

Important concepts include:

- Asset owners
- Product suppliers
- System integrators
- Security lifecycle
- Zones and conduits
- Security levels
- Defense in depth
- Secure development
- Risk-based security requirements

Zones

A zone is a group of assets with similar security requirements.

Conduits

A conduit is a controlled communication path between zones.

Defense in Depth

Security should be implemented using multiple layers such as:

- Network segmentation
- Firewalls
- Access control
- Monitoring
- Secure configuration
- Application allowlisting
- Backup and recovery
- Physical security
- Incident response

9. OT Security Architecture

A secure OT architecture may include:

- IT/OT network segmentation
- Industrial DMZ
- Firewalls between zones
- Jump servers
- Privileged access management
- Multi-factor authentication for remote access
- Secure vendor access
- Network monitoring
- Asset inventory
- Passive network discovery
- Centralized logging
- Secure backup systems
- Application allowlisting
- Endpoint protection where supported
- Strict USB controls
- Time synchronization
- Redundant systems
- Manual fallback procedures

10. OT Asset Inventory

Maintain an inventory of:

- PLCs
- RTUs
- HMIs
- SCADA servers
- Engineering workstations
- Historians
- Network switches
- Firewalls
- Sensors
- Actuators
- Safety systems
- Remote access devices
- Firmware versions
- Operating systems
- Communication protocols
- Asset owners
- Criticality
- Network location

11. OT Vulnerability Management

OT vulnerability management must consider operational risk.

Recommended Process

1. Identify assets
2. Classify asset criticality
3. Identify vulnerabilities
4. Check vendor advisories
5. Assess exploitability
6. Understand process impact
7. Select mitigation
8. Test changes
9. Schedule maintenance
10. Verify the result
11. Document residual risk

Possible Mitigations

- Network segmentation
- Firewall rules
- Disable unused services
- Strong authentication
- Application allowlisting
- Compensating controls
- Vendor-approved patches
- Monitoring and alerting
- Restricted physical access

12. OT Incident Response

An OT incident response plan should include:

Preparation

- Asset inventory
- Contact lists
- Backup validation
- Recovery procedures
- Communication plans
- Vendor escalation process
- Manual operation procedures

Detection and Analysis

- Identify abnormal commands
- Investigate unusual remote access
- Review network traffic
- Check PLC logic changes
- Review HMI and engineering workstation activity
- Identify affected processes

Containment

- Isolate affected network segments
- Disable compromised remote access
- Block malicious communication
- Preserve evidence
- Avoid unsafe shutdowns

Recovery

- Restore trusted configurations
- Validate PLC logic
- Recover systems safely
- Test process functionality
- Monitor for recurrence
- Document lessons learned

13. OT Product Security

Product security for industrial products should include:

- Secure product architecture
- Threat modeling
- Secure coding
- Security requirements
- Vulnerability management
- Secure update mechanisms
- Identity and access management
- Secure boot where applicable
- Firmware signing
- Logging and monitoring
- Security documentation
- SBOM management
- Coordinated vulnerability disclosure
- Security lifecycle management

14. OT Security Labs

Practice labs can include:

- Building a small virtual OT network
- Creating an IT/OT segmentation diagram
- Simulating a PLC and HMI environment
- Exploring Modbus communication
- Capturing industrial traffic using Wireshark
- Identifying insecure commands
- Creating firewall rules
- Designing an Industrial DMZ
- Mapping assets using a spreadsheet
- Creating a Purdue Model architecture
- Performing STRIDE-OT threat modeling
- Mapping threats to MITRE ATT&CK for ICS
- Designing an IEC 62443 zones-and-conduits model
- Creating an OT incident response playbook
- Developing a secure remote access architecture

15. Practical Projects

Project 1: Secure Manufacturing Network

Design a secure network for a manufacturing plant with:

- PLCs
- HMIs
- SCADA server
- Engineering workstation
- Historian
- Industrial firewall
- Industrial DMZ
- Enterprise network

Project 2: Modbus Security Assessment

Study:

- Modbus request and response
- Read and write operations
- Lack of native authentication
- Network exposure risks
- Compensating controls

Project 3: OT Threat Model

Create a threat model for a water treatment plant.

Include:

- Critical assets
- Data flows
- Threat actors
- Attack paths
- Safety impact
- Security controls
- Recovery actions

Project 4: Product Security Architecture

Create a security architecture for an IoT-to-OT gateway.

Include:

- Device identity
- Secure communication
- Certificate management
- Secure boot
- Firmware updates
- Access control
- Logging
- Cloud connectivity
- Industrial network segmentation

16. Learning Goals

By completing this section, you should be able to:

- Explain OT and ICS architecture
- Identify major ICS components
- Understand industrial protocols
- Compare IT and OT security
- Design basic OT network segmentation
- Use the Purdue Model
- Apply STRIDE-OT concepts
- Use MITRE ATT&CK for ICS
- Understand IEC 62443 concepts
- Perform basic OT asset classification
- Design secure remote access
- Develop an OT incident response plan
- Explain OT product security requirements
- Create a CPS security architecture

17. References

- IEC 62443
- NIST Cybersecurity Framework
- NIST SP 800-82
- MITRE ATT&CK for ICS
- CISA ICS Security Guidance
- Purdue Enterprise Reference Architecture
- ISA industrial cybersecurity guidance

---

Focus: Safety-first security architecture for cyber-physical systems, industrial automation, and critical infrastructure.