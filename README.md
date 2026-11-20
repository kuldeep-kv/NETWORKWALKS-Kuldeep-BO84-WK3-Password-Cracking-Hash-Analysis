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
