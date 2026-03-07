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
