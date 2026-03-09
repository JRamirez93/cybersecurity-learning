# Cybersecurity Integrative Assessment

## Overview

This document records the execution of several cybersecurity exercises.
Each stage documents the steps performed, the results obtained, and structured tables used to organize the information gathered during the assessment.

The goal is to present the workflow followed during the analysis while documenting the data generated in each stage.

---

# Stage 1 — Windows User Account Configuration

## Result

Local users were created in a Windows environment and password policies were configured to enforce stronger authentication practices.

## Steps Performed

1. Opened the **Run dialog**:

```
Win + R
```

2. Opened **Computer Management**:

```
compmgmt.msc
```

3. Navigated to:

```
System Tools
→ Local Users and Groups
→ Users
```

4. Created new users using:

```
Right Click → New User
```

5. Assigned passwords to each user account.

6. Opened the **Local Security Policy** console:

```
Win + R
secpol.msc
```

7. Navigated to:

```
Account Policies
→ Password Policy
```

8. Configured the following settings:

* Minimum password length
* Password complexity requirement
* Password expiration policy

## Example Users Created

| Username       | Role          |
| -------------- | ------------- |
| test_user1     | Standard User |
| analyst_user   | Standard User |
| security_admin | Administrator |

## Tools Used

* Windows 10
* Computer Management (`compmgmt.msc`)
* Local Security Policy (`secpol.msc`)
* User Account Control (UAC)

---

# Stage 2 — Risk Identification and Assessment

## Result

Organizational assets were identified and potential threats were evaluated using a probability and impact scoring method.

## Steps Performed

1. Identified critical organizational assets including infrastructure, systems, and data.

2. Identified possible threats affecting those assets.

3. Assigned a **probability score** from **1 to 5** for each threat.

4. Assigned an **impact score** from **1 to 5** representing the severity if the threat occurs.

5. Calculated a **quantitative risk value**:

```
Risk Score = Probability × Impact
```

6. Classified the qualitative risk level based on the final score.

## Risk Assessment Table

| Asset                           | Potential Threat                            | Probability (1-5) | Impact (1-5) | Qualitative Risk | Quantitative Risk |
| ------------------------------- | ------------------------------------------- | ----------------- | ------------ | ---------------- | ----------------- |
| Servers                         | Distributed Denial of Service (DDoS) attack | 4                 | 5            | High             | 20                |
| Desktop Computers               | Malware infection                           | 3                 | 4            | Moderate         | 12                |
| Laptops                         | Theft or loss                               | 2                 | 4            | Low              | 8                 |
| Network Devices                 | Traffic interception                        | 3                 | 4            | Moderate         | 12                |
| Mobile Devices                  | Unauthorized access                         | 3                 | 4            | Moderate         | 12                |
| Operating Systems               | Security vulnerabilities                    | 4                 | 5            | High             | 20                |
| Productivity Tools              | Phishing attacks                            | 3                 | 3            | Moderate         | 9                 |
| Security Tools                  | Misconfiguration or failed updates          | 2                 | 5            | Moderate         | 10                |
| Proprietary Applications        | Data leakage                                | 3                 | 5            | High             | 15                |
| Confidential Client Information | Unauthorized access                         | 4                 | 5            | High             | 20                |
| Employee Data                   | Phishing attacks                            | 3                 | 4            | Moderate         | 12                |
| Internal Documentation          | Unauthorized access                         | 3                 | 3            | Moderate         | 9                 |
| Financial Data                  | Malware infection                           | 4                 | 5            | High             | 20                |

## Tools Used

* Risk matrix methodology
* Spreadsheet software for analysis

---

# Stage 3 — Security Controls and Access Management

## Result

Security controls were defined to mitigate risks related to unauthorized access and system monitoring.

## Steps Performed

1. Reviewed authentication and access control mechanisms.

2. Evaluated user privilege distribution.

3. Defined role-based permissions for system access.

4. Proposed centralized logging and monitoring mechanisms.

5. Recommended implementing periodic security audits.

## Security Control Overview

| Control Type            | Description                                             |
| ----------------------- | ------------------------------------------------------- |
| Authentication Controls | Strong password policies and user identity verification |
| Authorization Controls  | Role-Based Access Control (RBAC)                        |
| Monitoring Controls     | Centralized logging and event monitoring                |
| Audit Controls          | Periodic security audits and log analysis               |

## Tools Used

* Access control policies
* RBAC model
* System logging mechanisms

---

# Stage 4 — Social Engineering Simulation

## Result

A controlled simulation demonstrated how a phishing-based social engineering attack can capture user credentials.

## Steps Performed

1. Booted a penetration testing environment using **Kali Linux**.

2. Opened a terminal.

3. Executed the Social Engineering Toolkit:

```
setoolkit
```

4. Selected the following attack vector:

```
Social Engineering Attacks
→ Website Attack Vectors
→ Credential Harvester Attack Method
```

5. Configured a test phishing page in the lab environment.

6. Simulated a victim interaction with the phishing page.

7. Observed how credentials entered into the page were captured.

## Attack Simulation Summary

| Attack Type           | Target               | Result                        |
| --------------------- | -------------------- | ----------------------------- |
| Credential Harvesting | Simulated user login | Credentials captured          |
| Phishing Page         | Web login clone      | Successful credential capture |

## Tools Used

* Kali Linux
* Social Engineering Toolkit (SET)

---

# Stage 5 — External Reconnaissance

## Result

Publicly available information about an organization’s infrastructure was collected to identify potential weaknesses.

## Steps Performed

1. Performed external reconnaissance on a target domain.

2. Collected DNS and domain registration information.

3. Identified exposed services and infrastructure components.

4. Documented potential weaknesses and attack surfaces.

5. Proposed mitigation measures.

## Reconnaissance Findings

| Category         | Observation                          |
| ---------------- | ------------------------------------ |
| DNS Records      | Publicly accessible domain records   |
| Network Services | Exposed services detected            |
| Infrastructure   | Public-facing servers identified     |
| Security Posture | Potential outdated software versions |

## Tools Used

* DNS lookup tools
* OSINT techniques
* Network reconnaissance utilities

---

# Summary

The exercises documented in this assessment demonstrate the execution of several cybersecurity tasks including:

* user account security configuration
* risk assessment
* access control design
* social engineering simulation
* external reconnaissance

Each stage documents the workflow used to obtain results and organize findings using structured tables.

