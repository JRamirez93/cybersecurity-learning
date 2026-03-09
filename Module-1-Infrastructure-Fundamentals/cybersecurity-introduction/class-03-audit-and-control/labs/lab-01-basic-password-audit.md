# Lab 01 – Windows Password Audit

## Description

In this lab I performed a basic **password audit in a Windows environment** to evaluate the strength of user passwords.  
Techniques included retrieving user account information and analyzing security-related fields.

---

## Lab Walkthrough

### Step 1 – Create Test Environment

1. On the Windows desktop, create a folder called `Laboratorio_ACL`.  
2. Inside this folder, create several test files and subfolders.

### Step 2 – Obtain User List

1. Open the **Command Prompt** (cmd.exe):  
   - Press Windows + R → type `cmd` → Enter.  
2. Run the following command to list users:

 -`net user`

3. Document all usernames listed.

![User List](screenshots/lab1/Step1.png)

---

### Step 3 – Analyze Passwords

For each user:

- Document key security attributes:  
  - Account enabled/disabled  
  - Password set / expires / change required  
  - Last password change  
  - Group memberships  
  - Remote Desktop access  
  - Login hours and allowed workstations  
  - Scripts, home directories, profiles  

- Optional: Use **Local Users and Groups** (`lusrmgr.msc`) for GUI verification.

![Password Audit](screenshots/lab1/Step2.png)

---

## Actions Performed

1. Created folder structure for lab.  
2. Retrieved user account list using `net user`.  
3. Analyzed account attributes and documented in spreadsheet.  
4. Verified account properties with `lusrmgr.msc`.  

---

## Tools Used

- Command Prompt (`cmd.exe`)  
- Local Users and Groups (`lusrmgr.msc`)  

---

## Key Takeaways

- Understanding user account attributes is crucial for auditing.  
- Windows provides CLI and GUI tools for password and account analysis.  
- Proper documentation supports security compliance.

---

## Status

- Completed