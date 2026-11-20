# 🔐 Week 3 Milestone: Password Cracking & Hash Analysis (Networkwalks)

This repository documents my Week 3 practical assignments for the **Cybersecurity Internship at Networkwalks**, covering password vulnerability assessment, cryptographic hashing, and dictionary-based credential recovery across both CLI and browser-based auditing tools.

## 🔗 LinkedIn Milestone Post
- **📝 Post:** [Week 3 Milestone | Cybersecurity Internship at NETWORKWALKS: Password Cracking & Hash Analysis](https://lnkd.in/p/dwRN6eB8)
- **🏢 Program / Mentorship:** Networkwalks (Waqas Karim, CCIE)

## 🎯 Modules Covered
- **🔹 W3-PM1: Auditing with John the Ripper (JTR)** — Exploring JTR capabilities in a controlled lab environment, examining password hash structure, and running wordlist-driven dictionary recovery attacks.
- **🔹 W3-PM2: Browser-Based Auditing with Networkwalks Tools** — Using the **Networkwalks Hash Calculator** and **Password Cracker** to practice hash generation, PDF hash extraction, and dictionary-based recovery to observe how password length and complexity affect cracking resistance.

## 🛠️ Lab Workflow & Notes

### 1️⃣ W3-PM1 — John the Ripper (CLI Workflow)
1. **📥 Hash Preparation & Extraction:** Inspect target hash formats or extract crackable hashes from supported files/inputs in the lab environment.
2. **⚡ Dictionary Attack Execution:** Run John the Ripper with a wordlist against extracted hashes to evaluate weak credential exposure.
3. **✅ Result Analysis:** Review cracked outputs and assess how wordlists and rule sets speed up recovery of predictable passwords.

### 2️⃣ W3-PM2 — Networkwalks Browser Tools
1. **🔍 Hash Calculation & PDF Hash Extraction:** Use the Networkwalks Hash Calculator to generate hashes and extract crackable hash strings from protected PDFs[cite: 1].
2. **⚔️ Dictionary Recovery Testing:** Submit extracted hashes into the Networkwalks Dictionary Attack Lab to test wordlist matching and observe how password length and complexity impact attack effort[cite: 2].

## 💡 Key Security Takeaways
- **🔄 Hashing vs. Encryption:** One-way cryptographic hashing is distinct from reversible encryption, and hash formats reveal structural clues that attackers target.
- **📖 Dictionary Attack Mechanics:** Weak, common, or predictable passwords fall quickly to wordlist-based attacks regardless of tool interface[cite: 2].
- **🛡️ Credential Hardening:** Strong password policies (sufficient length and complexity) combined with salted hashing are essential for defending stored credentials and protected files.

## 📂 Repository Structure
```text
networkwalks-w3-password-cracking-hash-analysis/
├── README.md
└── screenshots/        # Optional: add your lab & verification screenshots here
