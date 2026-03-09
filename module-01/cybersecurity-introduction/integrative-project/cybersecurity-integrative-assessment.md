# Windows 10 User Account Security Project

This project documents the implementation of security measures for local user accounts on a Windows 10 system.

The objective is to improve account security through user management, password policies, and verification of password strength.

---

# Stage 1 – User Account Security

## Description

In this stage I implemented basic security controls for user accounts in Windows 10.

The goal was to create user accounts with secure passwords, configure password policy settings, and review credential management practices.

---

# Actions Performed

## 1. User Creation

Local user accounts were created and managed using the Windows **Computer Management** console.

Tool used:

Win + R → compmgmt.msc

Navigation path:

Computer Management  
System Tools  
Local Users and Groups  
Users  

Example users created:

| Username | Role |
|--------|------|
| test_user1 | Standard User |
| test_admin | Administrator |

Each account was configured with a strong password following basic security best practices.

---

## 2. Password Policy Configuration

Local password policies were configured using **Local Security Policy**.

Tool used:

Win + R → secpol.msc

Configured settings included:

- Minimum password length
- Password complexity requirement
- Password expiration policy
- Account lockout configuration

These policies enforce stronger authentication standards for local accounts and reduce the risk of weak passwords.

---

## 3. Password Security Verification

After configuring the policies, the system configuration was verified by reviewing:

- Password policy settings
- User account configuration
- Authentication requirements

This step ensures that the defined security policies are correctly applied.

---

# Credential Management

Proper credential management is an important aspect of system security.

To avoid insecure practices such as password reuse or storing credentials in plain text, password managers can be used.

Two common tools are:

## LastPass

LastPass is a cloud-based password manager that securely stores encrypted credentials and integrates with web browsers.

Features include:

- Secure password storage
- Automatic password generation
- Browser autofill
- Synchronization across devices

LastPass typically operates through browser extensions for:

- Google Chrome
- Mozilla Firefox
- Microsoft Edge

---

## KeePass

KeePass is a local open-source password manager.

Unlike cloud-based solutions, KeePass stores passwords in an encrypted local database file (.kdbx).

Key features:

- Local encrypted password database
- No cloud dependency
- Open-source security model
- Strong encryption algorithms

KeePass can integrate with browsers through extensions such as **KeePassXC-Browser**.

---

# Tools Used

- Windows 10
- Computer Management (compmgmt.msc)
- Local Security Policy (secpol.msc)
- Windows User Account Management
- Password Managers (LastPass / KeePass)

---

# Status

Stage 1 Completed

---

# Stage 2 – Risk Management

## Scenario

TechSecure Solutions is a company specialized in providing cybersecurity services to enterprise clients. The company offers services such as security audits, security policy consulting, firewall implementation, and intrusion detection systems.

To support its operations, the organization manages multiple information assets including hardware, software, data, and personnel. Protecting these assets is critical to maintain business continuity and ensure information confidentiality, integrity, and availability.

---

# Information Assets Identification

The following assets were identified within the organization.

## Hardware

- Servers
- Desktop computers
- Laptops
- Network devices (routers, switches, firewalls)
- Mobile devices

## Software

- Operating systems
- Productivity tools (Office Suite)
- Security tools (antivirus, firewall)
- Proprietary applications

## Data

- Confidential client information
- Employee data
- Internal documentation
- Financial data

## People

- Company employees
- Clients
- Business partners

---

# Cybersecurity Risk Assessment

The following table identifies potential threats associated with each asset and evaluates the probability and impact of those threats.

| Asset | Potential Threat | Probability (1-5) | Impact (1-5) | Qualitative Risk | Quantitative Risk |
|------|------------------|------------------|-------------|-----------------|------------------|
| Servers | Distributed Denial of Service (DDoS) attack | 4 | 5 | High | 20 |
| Desktop Computers | Malware infection | 3 | 4 | Moderate | 12 |
| Laptops | Theft or loss | 2 | 4 | Low | 8 |
| Network Devices | Traffic interception | 3 | 4 | Moderate | 12 |
| Mobile Devices | Unauthorized access | 3 | 4 | Moderate | 12 |
| Operating Systems | Security vulnerabilities | 4 | 5 | High | 20 |
| Productivity Tools | Phishing attacks | 3 | 3 | Moderate | 9 |
| Security Tools | Misconfiguration or failed updates | 2 | 5 | Moderate | 10 |
| Proprietary Applications | Data leakage | 3 | 5 | High | 15 |
| Confidential Client Information | Unauthorized access | 4 | 5 | High | 20 |
| Employee Data | Phishing attacks | 3 | 4 | Moderate | 12 |
| Internal Documentation | Unauthorized access | 3 | 3 | Moderate | 9 |
| Financial Data | Malware infection | 4 | 5 | High | 20 |

---

# Risk Calculation Method

The quantitative risk value was calculated using the following formula:

Risk = Probability × Impact

Where:

- Probability is rated from **1 (Very Low)** to **5 (Very High)**
- Impact is rated from **1 (Low)** to **5 (Critical)**

This approach allows prioritization of security risks based on their potential effect on the organization.

---

# Conclusions

The analysis identified several cybersecurity risks affecting the information assets of TechSecure Solutions.

The most critical risks are associated with:

- Operating system vulnerabilities
- Confidential client information
- Financial data
- Server infrastructure

These risks present high impact levels and therefore require mitigation strategies such as:

- Strong access control policies
- Endpoint protection and monitoring
- Security awareness training
- Regular system updates and patch management
- Security audits and monitoring mechanisms

Implementing these measures helps reduce both the probability and impact of potential cyber threats.

---

# Stage Status

Stage 2 Completed
