# Windows 10 User Account Security Project

This project documents the implementation of security measures for local user accounts on a Windows 10 system.

The objective is to improve account security through user management, password policies, and verification of password strength.

---

# Stage 1 – User Account Security

## Description

In this stage I implemented basic security controls for user accounts in Windows 10.

The goal was to create user accounts with secure passwords and configure password policy settings.

---

## Actions Performed

### 1. User Creation

Created local user accounts using Windows account management.

Example users created:

| Username   | Role          |
| ---------- | ------------- |
| test_user1 | standard user |
| test_admin | administrator |

Each account was configured with a strong password.

---

### 2. Password Policy Configuration

Modified local password policies using Windows Local Security Policy tools.

Key settings configured:

* Minimum password length
* Password complexity requirement
* Password expiration policy

---

### 3. Password Security Verification

Verified the security configuration of user accounts by reviewing:

* Password policy settings
* Account configuration
* Authentication requirements

---

## Tools Used

* Windows 10
* Local Security Policy
* Windows User Account Management

---

## Status

Stage 1 Completed

