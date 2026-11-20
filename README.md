# 🔐 PDF Password Auditing & Recovery Using John the Ripper

### Hands-on Cybersecurity | Ethical Hacking | Kali Linu


## 📌 Project Overview

This project demonstrates a practical approach to auditing password-protected PDF documents using **John the Ripper** in a Kali Linux environment.

The objective was to understand how PDF password hashes can be extracted and tested against a wordlist using dictionary-based password auditing techniques.

Through this hands-on exercise, I explored password hash extraction, wordlist preparation, password recovery, and result verification.

## 🎯 Project Objectives

- Understand PDF password protection and hash extraction.
- Learn how PDF2John works.
- Install and configure John the Ripper.
- Perform dictionary-based password auditing.
- Work with the RockYou wordlist.
- Verify password recovery results.
- Understand the importance of strong password security.

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Kali Linux | Penetration testing environment |
| John the Ripper | Password auditing and recovery |
| PDF2John | PDF password hash extraction |
| RockYou | Password wordlist |
| Linux Terminal | Command execution |

## ⚙️ Practical Implementation

### 1. Environment Setup

Installed and verified John the Ripper on Kali Linux.

```bash
john --list=build-info
```

### 2. PDF Hash Extraction

Used PDF2John to extract password hashes from the authorized lab PDF documents.

```bash
perl /usr/share/john/pdf2john.pl "sample.pdf" > pdf_hash.txt
```

### 3. Wordlist Preparation

Used the RockYou wordlist available in Kali Linux.

```bash
ls -lh /usr/share/wordlists/rockyou.txt
```

### 4. Dictionary-Based Password Auditing

Executed John the Ripper against the extracted PDF hashes.

```bash
john --wordlist=/usr/share/wordlists/rockyou.txt pdf_hash.txt
```

### 5. Result Verification

Verified recovered passwords using:

```bash
john --show --format=PDF pdf_hash.txt
```

## 🔄 Project Workflow

```text
       PDF Document
             |
             v
     PDF2John Extraction
             |
             v
       PDF Hash File
             |
             v
       RockYou Wordlist
             |
             v
      John the Ripper
             |
             v
      Password Testing
             |
             v
      Result Verification
```

## 📸 Practical Screenshots

Screenshots below document the actual practical implementation

### 1. Password Recovery – Practical 1
![image alt](https://github.com/kavyag41168-bot/PDF-Password-Auditing-John-The-Ripper/blob/9f007e2b5d0eb6be5354b02e24c5da5f12bc19f8/password%20unlock%201.jpeg)

### 2. Password Recovery – Practical 2
![image alt](https://github.com/kavyag41168-bot/PDF-Password-Auditing-John-The-Ripper/blob/ba39cdf219c18bf822658b049196d34404b71fdd/password%20unlock%202.jpeg)

### 3. Password Recovery – Practical 3
![image alt](https://github.com/kavyag41168-bot/PDF-Password-Auditing-John-The-Ripper/blob/13eb2938898bfc5633b7caf77e1020ef406706dd/password%20unlock%203.jpeg)

### 4. Password Recovery – Practical 4
![image alt](https://github.com/kavyag41168-bot/PDF-Password-Auditing-John-The-Ripper/blob/cd5ea3db9df7b59c4e609ae27b5f313230ec651c/password%20unlock%204.jpeg)


## 📊 Practical Results

The following results were confirmed during the lab:

| Activity | Result |
|---|---|
| PDF hash extraction | Successfully performed |
| PDF password format detection | Confirmed |
| RockYou wordlist integration | Successful |
| Dictionary attack | Successfully performed |
| Password recovery | 2 confirmed recoveries |
| Result verification | Performed for recovered results |

Two additional PDF hashes were extracted; their password recovery results were not confirmed in the recorded practical.

## 📚 Key Learning Outcomes

- Gained hands-on experience with Kali Linux.
- Understood PDF password hash extraction.
- Learned to use John the Ripper for password auditing.
- Practiced dictionary-based password attacks.
- Understood the role of wordlists in password security testing.
- Learned to verify password recovery results.

## 🔐 Security Awareness

This practical highlights why weak and commonly used passwords can create security risks.

Using strong, unique passwords and avoiding predictable password patterns can improve document security.

## ⚖️ Disclaimer

This project was performed for educational purposes in an authorized lab environment.

All password auditing activities should only be performed on documents you own or have explicit permission to test.

---

### 👩‍💻 Project Category
**Cybersecurity | Ethical Hacking | Password Security | Practical Learning**
