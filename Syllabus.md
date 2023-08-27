```markdown
# BlueSec Syllabus

## Module 1: Security Operations(SecOps) Fundamentals

### Environment Setup (2023.08.20)

1. Prepare your analysis environment based on the following two operating systems. You can use the free licenses from AWS or GCP, or a virtual emulator on your host PC:

   - For Linux (Ubuntu 20.04 LTS), install the following two platforms:
     + Sift-Workstation + Remnux: https://www.sans.org/blog/how-to-install-sift-workstation-and-remnux-on-the-same-forensics-system/

   - For Windows 10 (21H2, 19044 or above), install the following two platforms:
     + flare-vm: https://github.com/mandiant/flare-vm
     + commando-vm: https://github.com/mandiant/commando-vm

2. Install the following extensions on the Chrome browser of your main PC:

   - workona: https://workona.com
   - WebChatGPT: https://tools.zmo.ai/webchatgpt
   - Sputnik OSINT: https://github.com/mitchmoser/sputnik

3. Miscellaneous: Sign up for GitHub and join the DoubleS1405 Organizations. You can freely use your personal Git or DS Git Repo, but a collection of integrated tools will be managed and created at https://github.com/DoubleS1405/OpenSOC.



### Suricata Investigation and Implementation (2023.09.03)

- Research and provide a brief overview of Suricata, referencing the official documentation (https://docs.suricata.io).

### Comparative Analysis of IDS

- Conduct a comparative analysis of Snort, Suricata, and Bro IDS. Highlight the differences, including strengths, weaknesses, ideal use cases, and key feature comparisons. Provide personal opinions and conclusions.

### Suricata Installation and Configuration File Investigation

- Install Suricata on Ubuntu 20.04 LTS, study the configuration file, and provide a detailed report on the functionality and role of each setting. Include brief installation instructions and commentary on each configuration item.

### Suricata Detection Rule Investigation

- Learn how to write Suricata detection rules, research commonly used rules, and identify how these rules overlap and differ from Snort rules.

### Detection Rule Testing Practice

- Write Suricata detection rules for the following three scenarios, test each rule, and report the results:

  1. A rule to detect a specific Hex pattern within a TCP stream.
  2. A rule to detect DNS queries with a specific Command and Control (CnC) server.
  3. A rule to detect a specific attack pattern sent via HTTP GET or POST requests.


### Malware Analysis: Static vs. Dynamic Approaches and Sandboxing

### Using Honeypots and Decoys for Defense

### Understanding Cloud Computing and CASB

### Threat Intelligence: Mitigating and Defending

### Using Machine and Deep Learning for Security

### Ticketing Systems for Incident Response

### The Importance of Asset Inventory in Security

### SOC components - people

- Organizational Chart and SOC Roles
- Creating Effective Cybersecurity Training Plans
- Challenges and Solutions for SOC Jobs
- Avoiding Burnout: Tips for SOC Analysts

### SOC components - processes

- Effective Policies: Business Protection Through Documentation
- Efficient SOC Procedures: The How-To
- Security Standards: Compliance is Mandatory
- Security Guidelines and Benchmarks: Best Practices
- Perform Windows Security Assessments with CIS-CAT Lite

## Module 2: Incident Response

### Incident Response (IR) - Overview

- Understanding Key Concepts for Incident Response
- Continuous Incident Response: Before, During, After
- Remote Incident Response: Challenges and Benefits
- Structured Approach to Incident Response Phases

### Preparation

- Effective Incident Prevention Strategies and Controls
- Effective Incident Communication Planning in IR
- IR Architecture: Defense and Zero Trust
- IR Policy, Plan, and Procedure
- Efficient Incident Resolution with Management Platforms

### Detection & Analysis

- Detection Engineering: Building Effective Detectors
- Network Perimeter-level Detection
- Endpoint Perimeter Detection: Catching Threats In and Out
- Achieving System-Level Detection with EDR
- Application-Level Detection: Prioritize, Monitor, Parse

### Containment, Eradication, and Recovery

- Effective Incident Containment Strategies in IR
- Attack Remediation: Eliminating Vulnerabilities and Artifacts
- System Recovery: Restore, Validate, Monitor

### Post-Incident Activity

- Post-Incident Review: Lessons Learned Meeting
- IR Report: Guidelines for Effective Writing

## Module 3: Perimeter Defense - Email Security

### Email Spoofing

- Email Attack Prevention: Spoofing & DMARC
- Understanding SPF: Email Authentication Protocol
- DKIM: Email authentication with digital signatures
- Protecting Against Email Spoofing with DMARC

### Malicious Attachments

- Malicious Attachments: Risks and Responses
- Secure Email Attachments: Best Practices
- Activity - Cuckoo Sandbox Deployment

### Malicious URLs

- Malicious URLs: A Growing Threat
- Protecting Users from Malicious URLs
- Activity – Detect Lookalike Domains

### Extra Mile Controls

- User Education: Key to Email Security
- Measuring User Awareness with Phishing Simulators
- Activity - GoPhish Deployment
- Early Phishing Detection Using Honeypots Tokens


## Module 4: Perimeter Defense - Network Security

### Firewalls

- Understanding Firewall: Types and Functions
- Configuring Firewalls: Best Practices
- Activity - pfSense Firewall Deployment

### Intrusion Prevention Systems (IPS)

- Understanding IPS: Types and Functions
- Configuring IPS: Best Practices
- Activity - Snort IPS Deployment

### Virtual Private Networks (VPN)

- Understanding VPN: Benefits and Risks
- Configuring VPN: Best Practices
- Activity - OpenVPN Deployment

### Extra Mile Controls

- Network Segmentation: Benefits and Strategies
- Implementing Advanced Threat Protection
- Activity - Network Traffic Analysis with Wireshark

## Module 5: Endpoint Defense

### Antivirus and Antimalware Solutions

- Understanding Antivirus and Antimalware: Functions and Limitations
- Configuring Antivirus and Antimalware: Best Practices
- Activity - Malwarebytes Deployment

### Host-based Intrusion Prevention Systems (HIPS)

- Understanding HIPS: Functions and Benefits
- Configuring HIPS: Best Practices
- Activity - OSSEC HIPS Deployment

### Application Whitelisting

- Understanding Application Whitelisting: Benefits and Challenges
- Implementing Application Whitelisting: Best Practices
- Activity - AppLocker Deployment

### Extra Mile Controls

- Implementing Disk Encryption: Benefits and Strategies
- User Education: Importance and Strategies
- Activity - BitLocker Deployment

## Module 6: Identity and Access Management

### User Management

- Understanding User Roles and Privileges
- Implementing Role-Based Access Control (RBAC)
- Activity - User Management in Active Directory

### Authentication

- Understanding Authentication Mechanisms: Passwords, Tokens, Biometrics
- Implementing Multi-Factor Authentication (MFA)
- Activity - Setting Up MFA with Google Authenticator

### Authorization

- Understanding Authorization Mechanisms: ACLs, Capabilities, Policies
- Implementing Least Privilege Principle
- Activity - Configuring File Permissions in Linux

### Extra Mile Controls

- Implementing Single Sign-On (SSO)
- User Education: Password Management and Phishing Awareness
- Activity - Setting Up SSO with Okta

## Module 7: Security Operations and Monitoring

### Log Management

- Understanding the Importance of Log Management
- Implementing Centralized Log Management
- Activity - Setting Up a Log Management Solution with ELK Stack

### Network Monitoring

- Understanding Network Monitoring: IDS, IPS, SIEM
- Implementing Network Monitoring with Open Source Tools
- Activity - Network Monitoring with Security Onion

### Incident Response

- Understanding the Incident Response Lifecycle
- Implementing an Incident Response Plan
- Activity - Incident Response Simulation

### Extra Mile Controls

- Implementing Threat Hunting Practices
- Continuous Improvement of Security Operations
- Activity - Threat Hunting with YARA


## Module 8: Application Security

### Secure Coding Practices

- Understanding Common Security Vulnerabilities in Code
- Implementing Secure Coding Guidelines
- Activity - Code Review for Security Vulnerabilities

### Security Testing

- Understanding Different Types of Security Testing: SAST, DAST, IAST
- Implementing Security Testing in CI/CD Pipeline
- Activity - Setting Up Security Testing with OWASP ZAP

### Web Application Firewalls (WAF)

- Understanding the Role and Benefits of WAF
- Implementing WAF for Web Application Protection
- Activity - Setting Up WAF with ModSecurity

### Extra Mile Controls

- Implementing Runtime Application Self-Protection (RASP)
- User Education: Secure Usage of Applications
- Activity - Setting Up RASP with Contrast Security

## Module 9: Cloud Security

### Cloud Service Models

- Understanding Different Cloud Service Models: IaaS, PaaS, SaaS
- Implementing Security Best Practices for Each Service Model
- Activity - Security Configuration in AWS

### Cloud Security Architecture

- Understanding Shared Responsibility Model
- Implementing Security Architecture in Cloud
- Activity - Setting Up a Secure VPC in AWS

### Cloud Security Tools

- Understanding Cloud Native Security Tools
- Implementing Cloud Security Monitoring and Alerting
- Activity - Setting Up AWS GuardDuty and AWS Security Hub

### Extra Mile Controls

- Implementing Cloud Security Posture Management (CSPM)
- User Education: Secure Usage of Cloud Services
- Activity - Setting Up CSPM with Prisma Cloud

## Module 10: Data Security

### Data Classification

- Understanding Different Data Classification Levels
- Implementing Data Classification Policies
- Activity - Data Classification with Microsoft Azure Information Protection

### Data Protection

- Understanding Data Protection Mechanisms: Encryption, Masking, Tokenization
- Implementing Data Protection in Transit, at Rest, and in Use
- Activity - Setting Up Data Encryption with VeraCrypt

### Data Loss Prevention (DLP)

- Understanding the Role and Benefits of DLP
- Implementing DLP Policies for Data at Rest, in Use, and in Motion
- Activity - Setting Up DLP with Symantec DLP

### Extra Mile Controls

- Implementing Data Rights Management (DRM)
- User Education: Safe Data Handling Practices
- Activity - Setting Up DRM with Microsoft Azure Rights Management

## Module 11: Compliance and Audit

### Understanding Compliance Requirements

- Understanding Different Compliance Standards: GDPR, HIPAA, PCI-DSS
- Implementing Compliance Policies and Procedures
- Activity - Compliance Audit with Microsoft Compliance Manager

### Security Audit

- Understanding the Role and Benefits of Security Audits
- Implementing Regular Security Audits
- Activity - Security Audit with Nessus

### Risk Management

- Understanding Risk Management Frameworks: NIST, ISO 27001
- Implementing Risk Assessment and Mitigation Strategies
- Activity - Risk Assessment with FAIR Model

### Extra Mile Controls

- Implementing Continuous Compliance Monitoring
- User Education: Understanding Compliance Requirements
- Activity - Continuous Compliance Monitoring with Splunk

last modified date: 2023.08.27
```
