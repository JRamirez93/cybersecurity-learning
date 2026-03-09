# Lab 02 – Windows ACL Configuration

## Description

In this lab I configured and managed **Access Control Lists (ACLs) on Windows** to control access to files and folders.  
The goal was to apply access permissions based on user roles and understand inheritance.

---

## Lab Walkthrough

### Step 1 – Create Test Folder

1. On the desktop, create a folder called `Laboratorio_ACL`.  
2. Add several files and subfolders inside.

### Step 2 – Open Security Properties

1. Right-click the folder → Properties → Security tab.  
2. Click **Edit** to modify permissions.  
3. Add users or groups via **Add…**.  
4. Assign permissions such as Full Control, Read, Write, or Deny.  
5. Apply changes and validate inheritance in subfolders.

![ACL Configuration](screenshots/lab2/Step1.png)
![ACL Configuration](screenshots/lab2/Step2.png)

### Step 3 – Verify Permissions

1. Open each file/subfolder and check effective permissions.  
2. Use `icacls` in **Command Prompt** to confirm settings:

 - `icacls` "C:\Users<YourUser>\Desktop\Laboratorio_ACL"
 
![ACL Verification](screenshots/lab2/Step3.png)

---

## Actions Performed

1. Created test folder and files.  
2. Configured ACLs for multiple users and groups.  
3. Verified inheritance and effective permissions.  
4. Used `icacls` and GUI to confirm settings.

---

## Tools Used

- Windows Explorer (Security tab)  
- Command Prompt (`cmd.exe`)  
- `icacls` command-line tool  

---

## Key Takeaways

- ACLs allow fine-grained access control on Windows files/folders.  
- Understanding inheritance prevents accidental exposure of sensitive data.  
- Both GUI and CLI tools are useful for auditing and verification.

---

## Status

- Completed