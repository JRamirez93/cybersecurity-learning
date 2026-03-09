# Lab 01 – Business Continuity Plan (BCP) and Disaster Recovery Plan (DRP)

## Description

In this lab, I explored **Business Continuity Planning (BCP)** and **Disaster Recovery Planning (DRP)** using a hypothetical infrastructure scenario.  
The objective was to **identify risks, plan mitigation strategies, and understand recovery procedures** for critical business services.

---

## Lab Walkthrough

### Step 1 – Analyze Infrastructure

TechSolutions infrastructure includes:

- Primary data center with main servers and backup equipment  
- Secondary data centers distributed geographically for redundancy  
- Central office with internal servers and network devices  

Document resources and potential points of failure.

![Infrastructure Overview](screenshots/lab1/Step1.png)

### Step 2 – Identify Threats and Risks

1. List possible threats (e.g., power outages, hardware failures, cyberattacks).  
2. Determine the impact on services, customers, and revenue.  
3. Use tables to capture the analysis.

| Threat | Impact | Likelihood | Notes |
|--------|--------|-----------|-------|
| Power outage | High | Medium | Affects main servers |
| Server failure | Medium | Medium | Backup available |
| Cyberattack | High | Low | Security measures in place |

### Step 3 – Plan BCP & DRP

1. Fill out **BCP and DRP tables** with stages and descriptions.

| Stage | BCP – Description |
|-------|-----------------|
| 1     | Identify critical business functions |
| 2     | Determine maximum tolerable downtime |
| 3     | Assign roles and responsibilities |
| 4     | Implement continuity procedures |
| 5     | Test and maintain plan |

| Stage | DRP – Description |
|-------|-----------------|
| 1     | Identify critical systems and data |
| 2     | Determine recovery time objectives (RTO) |
| 3     | Define backup and recovery procedures |
| 4     | Test restoration process |
| 5     | Update DRP regularly |

### Step 4 – Document Findings

Record **impact analysis**, recovery steps, and mitigation strategies in a notes file or spreadsheet.

![BCP Table](screenshots/lab1/Step2.png)

---

## Actions Performed

1. Analyzed infrastructure and identified critical assets.  
2. Completed threat and risk assessment tables.  
3. Developed BCP and DRP tables with mitigation strategies.  
4. Prepared documentation for continuity and recovery procedures.

---

## Tools Used

- Microsoft Excel / Google Sheets (for tables)  
- Windows / Linux environments for infrastructure references  

---

## Key Takeaways

- BCP ensures critical business functions continue during disruptions.  
- DRP provides procedures to restore systems after a disaster.  
- Regular testing and updates are essential for both BCP and DRP.

---

## Status

- Completed