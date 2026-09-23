# 🔐 Password Cracking — Cybersecurity & Ethical Hacking

## 📚 Week 3 — Project Modules 1 & 2

This repository contains my **Week 3 Cybersecurity & Ethical Hacking practical projects** completed as part of my cybersecurity learning journey.

The projects cover two password-security and password-recovery labs:

* 🔐 **Module 1 — Password Cracking with John the Ripper (JTR)**
* 🌐 **Module 2 — Password Cracking with Networkwalks Tools**

These practical labs helped me understand password hashes, password security, Linux command-line tools, and authorized password-recovery techniques.

> ⚠️ **Ethical Use:** All techniques demonstrated in this repository are intended for educational purposes and authorized cybersecurity labs only. Never use password-cracking techniques against systems, accounts, or files without explicit permission.

---

# 📌 Project Overview

| Module   | Project                                   | Environment | Main Tool                     |
| -------- | ----------------------------------------- | ----------- | ----------------------------- |
| Module 1 | Password Cracking with JTR                | Kali Linux  | John the Ripper               |
| Module 2 | Password Cracking with Networkwalks Tools | Web Browser | Networkwalks Password Cracker |

---

# 🔐 Module 1 — Password Cracking with John the Ripper

## 📖 Overview

**John the Ripper (JTR)** is a password-cracking tool commonly used in cybersecurity to test password strength and perform authorized password-recovery tasks.

For this module, I completed the practical work using **John the Ripper directly on Kali Linux** through the terminal.

The workflow involved preparing a password hash from an authorized protected PDF, loading the hash into John the Ripper, performing the password-recovery process, and verifying the result.

---

## 🛠️ Tools & Environment

* Kali Linux
* John the Ripper (JTR)
* Kali Linux Terminal
* Authorized encrypted PDF
* PDF password hash
* Password candidates / wordlist

---

## ⚙️ Module 1 Workflow

### Step 1 — Prepare the Hash

The password hash from the authorized protected PDF was stored in a text file.

Example filename:

```text
file3.txt
```

The file contained the password hash in a format supported by John the Ripper.

---

### Step 2 — Run John the Ripper

I executed the following command in the Kali Linux terminal:

```bash
john file3.txt
```

John the Ripper then loaded the hash and started the password-recovery process.

---

### Step 3 — Display the Recovered Password

After the cracking process, I used:

```bash
john --show file3.txt
```

This command displays the recovered password and provides information about successfully cracked hashes.

The practical result showed:

```text
1 password hash cracked, 0 left
```

---

### Step 4 — Verify the Password

The recovered password was used to verify access to the authorized protected PDF.

The actual recovered password is **not included in this repository** to avoid exposing credentials.

---

## ✅ Module 1 Result

**Status: Successfully Completed ✅**

The practical JTR lab was successfully completed on Kali Linux.

The result confirmed:

```text
1 password hash cracked, 0 left
```

This demonstrated the successful password-recovery process using John the Ripper.

---

# 🌐 Module 2 — Password Cracking with Networkwalks Tools

## 📖 Overview

The second module demonstrates password recovery using the **Networkwalks Hash Calculator** and **Networkwalks Password Cracker**.

Unlike Module 1, this module uses browser-based tools instead of running John the Ripper directly from the Linux terminal.

The workflow involves extracting a password hash from an authorized encrypted PDF and then using the Networkwalks Password Cracker to perform the password-recovery process.

---

## 🛠️ Tools Used

* Networkwalks Hash Calculator
* Networkwalks Password Cracker
* Web Browser
* Authorized encrypted PDF
* Kali Linux / Windows

---

## 🔗 Networkwalks Resources

### Networkwalks Hash Calculator

https://networkwalks.com/hash-calculator/

### Networkwalks Password Cracker

https://networkwalks.com/password-cracker/

### Networkwalks Project Lab

https://networkwalks.com/project-task-lab-password-cracking-with-networkwalks-tools/

---

# ⚙️ Module 2 Workflow

## Step 1 — Obtain the Authorized Encrypted PDF

An encrypted PDF provided for the cybersecurity lab was used for the practical exercise.

---

## Step 2 — Extract the PDF Hash

The encrypted PDF was uploaded to the **Networkwalks Hash Calculator**.

The tool generates a PDF password hash beginning with:

```text
$pdf$...
```

---

## Step 3 — Copy the Complete Hash

The complete generated hash was copied.

It is important to copy the entire hash without missing any characters.

---

## Step 4 — Open the Networkwalks Password Cracker

The generated hash was entered into the **Networkwalks Password Cracker**.

---

## Step 5 — Start Password Recovery

The password-recovery process was started using the extracted PDF hash.

The tool attempts password candidates until the matching password is identified.

---

## Step 6 — Verify the Recovered Password

After the process completed, the recovered password was obtained.

The password was then used to verify access to the authorized encrypted PDF.

---

## ✅ Module 2 Result

**Status: Successfully Completed ✅**

The Networkwalks password-recovery workflow was completed successfully as part of the authorized cybersecurity lab.

---

# 📊 Module 1 vs Module 2

| Feature | 🔐 Module 1
