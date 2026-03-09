# Lab 02 – Passive Fingerprinting

## Description

In this lab, I performed **passive fingerprinting** to identify network assets and online services without directly interacting with target systems.  
The objective was to **collect information about devices and services for security assessment purposes**.

---

## Lab Walkthrough

### Step 1 – Identify Targets

1. Use passive search engines and scanners like **Shodan**, **ZoomEye**, or **Censys**.  
2. Identify at least:

- 5 different types of IP cameras  
- 3 websites running WordPress

### Step 2 – Perform Passive Scanning

1. Input search queries using advanced search operators (dorks) to find devices or services.  
2. Collect publicly available metadata such as:

- Device model and version  
- Operating system  
- Open ports  
- Hostname / IP

![Passive Fingerprinting](screenshots/lab2/Step1.png)

### Step 3 – Document Findings

| Device / Site | Type | IP / URL | OS / Service | Notes |
|---------------|------|----------|--------------|-------|
| IP Camera 1   | Camera | 192.168.1.10 | Firmware v1.2 | Publicly visible |
| WordPress Site 1 | Website | example.com | WP v6.1 | Plugin info collected |

### Step 4 – Analyze Security Implications

1. Assess potential risks associated with exposed services.  
2. Document observations and recommendations.

---

## Actions Performed

1. Collected information passively on network devices and web services.  
2. Identified exposed assets that may require security hardening.  
3. Used search engines and dorks to gather data without interacting with targets.

---

## Tools Used

- Shodan (search engine for internet-connected devices)  
- ZoomEye (search engine for cyber reconnaissance)  
- Censys (internet scanning platform)  
- Web browser (Chrome/Edge/Firefox)  

---

## Key Takeaways

- Passive fingerprinting allows reconnaissance without alerting the target.  
- Publicly available information can reveal security weaknesses.  
- Understanding passive scanning techniques helps in designing better defensive strategies.

---

## Status

- Completed