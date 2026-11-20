# 🔐 Week 3 Milestone: Password Cracking & Hash Analysis

![Cybersecurity](https://img.shields.io/badge/Focus-Password%20Cracking%20%26%20Hash%20Analysis-blue)
![Internship](https://img.shields.io/badge/Internship-Networkwalks-darkgreen)
![Platform](https://img.shields.io/badge/Environment-Kali%20Linux-blueviolet)

This repository documents my **Week 3** practical assignments for the **Cybersecurity Internship at Networkwalks**, focusing on password vulnerability assessment, cryptographic hashing mechanics, and dictionary-based recovery methodologies across CLI and browser-based tools.

---

## 🔗 LinkedIn Milestone & Program Details
* **📝 LinkedIn Post:** [Week 3 Milestone | Cybersecurity Internship at NETWORKWALKS: Password Cracking & Hash Analysis](https://lnkd.in/p/dwRN6eB8)
* **🏢 Organization:** Networkwalks
* **👨‍🏫 Mentorship:** Waqas Karim (CCIE)

---

## 🎯 Lab Objectives & Modules

| Module | Focus Area | Tools & Methodology |
| :--- | :--- | :--- |
| **🔹 W3-PM1** | **Auditing with John the Ripper (JTR)** | CLI hash extraction, hash structure analysis, and wordlist-driven dictionary attacks on Kali Linux. |
| **🔹 W3-PM2** | **Browser-Based Auditing with Networkwalks Tools** | Hash generation, PDF hash extraction, and dictionary recovery testing via web utilities. |

---

## 🛠️ Execution Workflow

### 1️⃣ W3-PM1: Password Auditing with John the Ripper (CLI)
1. **📥 Hash Extraction:**
   Convert password-protected files into crackable hash formats:
   ```bash
   pdf2john "My Locked PDF1.pdf" > pdf.hash


⚡ Dictionary Attack Execution:

1.Run John the Ripper against the extracted hash using a wordlist:

john --wordlist=/usr/share/wordlists/rockyou.txt pdf.hash

2.✅ Credential Verification:

Inspect the cracked password output and validate file access:

john --show pdf.hash

2️⃣ W3-PM2: Browser-Based Auditing with Networkwalks Tools
🔍 Hash Calculation & PDF Hash Extraction:

Utilized the Networkwalks Hash Calculator to generate cryptographic hashes and parse encrypted PDF files locally.

Extracted a 128-bit $pdf$ hash string (Revision R4, Version V4) compatible with pdf2john and hashcat.

⚔️ Dictionary Recovery Testing:

Submitted the extracted $pdf$ hash into the Networkwalks Dictionary Attack Lab.

Executed a wordlist scan to observe how password length and complexity impact cracking speed, recovering the credential (password1) at iteration 91.

🔓 Decryption & Flag Capture:

Unlocked the target document (My Locked PDF2.pdf) using the recovered password and verified lab completion via the captured flag:

nw{networkwalks_persistence_jtr_270521}

💡 Key Security Takeaways
🔄 Hashing vs. Encryption: One-way cryptographic hashing is fundamentally distinct from reversible encryption, and hash formats reveal structural metadata that auditing tools leverage.

📖 Dictionary Attack Mechanics: Common, short, or predictable passwords (password1) fail rapidly against optimized wordlists, even when wrapped in 128-bit encryption.

🛡️ Credential Hardening: Enforcing strong password policies (14+ characters with mixed character sets) alongside salted hashing is critical for protecting stored credentials and sensitive files.

📂 Repository Structure

networkwalks-w3-password-cracking-hash-analysis/
├── README.md
└── screenshots/
    ├── 01-hash-calculator.png
    ├── 02-password-cracked.png
    ├── 03-unlock-prompt.png
    └── 04-flag-captured.png


⚠️ Disclaimer
All password auditing and hash analysis exercises documented in this repository were conducted strictly within an authorized educational lab environment provided by Networkwalks.
