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

TechSecure Solutions is a company specialized in providing cybersecurity solutions for enterprise clients.  
The company offers a wide range of services including security audits, security policy consulting, firewall deployment, and intrusion detection systems.

With a highly trained team that constantly updates its knowledge about emerging cyber threats, TechSecure Solutions has built a strong reputation in the cybersecurity market.

The organization manages several critical assets that support its operations and must be properly protected.

---

# Information Assets Identification

The following information assets were identified within TechSecure Solutions.

### Hardware

- Database servers (2 units)
- Software development workstations (10 units)
- Employee laptops and mobile devices

### Software

- Security software used to protect systems and networks
- Development tools and software environments

### Data

- Internal documentation and procedure manuals
- Confidential client data stored in cloud services
- Internal emails and communications
- Contracts and commercial agreements

### People

- Software development team
- Security consultants
- System administrators
- Company employees

---

# Identified Cybersecurity Risks

Several risks were identified based on the assets listed above.

Each risk considers potential threats, probability of occurrence, and the possible impact on the organization.

Examples of potential threats include:

- Unauthorized access
- Data breaches
- Malware infections
- Phishing attacks
- Data loss or corruption
- Insider threats

---

# Risk Assessment Table

| Asset | Potential Threats | Probability (1–5) | Impact (1–5) | Qualitative Risk | Quantitative Risk |
|------|------------------|------------------|-------------|-----------------|------------------|
| Database Servers | Unauthorized access, ransomware attack | 3 | 5 | High | 15 |
| Development Workstations | Malware infection, compromised developer credentials | 4 | 4 | High | 16 |
| Internal Documentation | Unauthorized access or accidental data leakage | 2 | 3 | Medium | 6 |
| Client Data in Cloud | Data breach, misconfigured cloud permissions | 3 | 5 | High | 15 |
| Email and Internal Communications | Phishing attacks, email compromise | 4 | 3 | Medium | 12 |
| Security Software | Misconfiguration, vulnerability exploitation | 2 | 4 | Medium | 8 |
| Employee Devices | Device theft, malware infection | 3 | 3 | Medium | 9 |
| Contracts and Agreements | Unauthorized access or data exposure | 2 | 4 | Medium | 8 |

---

# Risk Evaluation Method

The quantitative risk value is calculated using the formula:

Risk = Probability × Impact

Where:

- **Probability** is rated from 1 (Very Low) to 5 (Very High)
- **Impact** is rated from 1 (Low) to 5 (Critical)

The qualitative risk level is interpreted based on the resulting score.

Example interpretation:

| Score | Risk Level |
|------|-------------|
| 1–5 | Low |
| 6–10 | Medium |
| 11–15 | High |
| 16–25 | Critical |

---

# Conclusion

The risk assessment identified several high-priority risks related to sensitive data, development systems, and communication channels.

Proper risk management requires implementing additional security measures such as:

- Access control policies
- Endpoint protection
- Security awareness training
- Regular security audits
- Monitoring and logging systems

These measures will help reduce the probability and impact of potential cybersecurity incidents.

---

# Stage Status

Stage 2 Completed
