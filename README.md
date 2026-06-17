# 🛡️ DecodeLabs Cybersecurity Internship

**Industrial Training Kit — Batch 2026**  
**Domain:** Cyber Security  
**Intern:** Joykan  
**Powered by:** [DecodeLabs](https://www.decodelabs.tech)

---

## 📋 Overview

This repository contains all completed projects from the DecodeLabs Cybersecurity Internship program. Each project builds foundational cybersecurity skills through hands-on implementation — from password security to encryption to threat identification.

---

## 📁 Projects

### Project 1: Password Strength Checker
**📂 Folder:** [`Task-1-Joy Kandie/`](./Task-1-Joy%20Kandie/)  
**🎯 Goal:** Evaluate password strength using security best practices.

**Key Features:**
- Checks length, uppercase, lowercase, digits, and special characters
- Scores passwords on a 0–7 scale (WEAK / MEDIUM / STRONG)
- Detects commonly leaked passwords using constant-time comparison (`hmac.compare_digest`)
- Provides actionable feedback to improve weak passwords

**Skills:** Input validation, security scoring, defensive programming

**How to Run:**
```bash
py "Task-1-Joy Kandie/password_checker.py"
```

---

### Project 2: Basic Encryption & Decryption
**📂 Folder:** [`Task-2-Joy Kandie/`](./Task-2-Joy%20Kandie/)  
**🎯 Goal:** Implement classical ciphers to understand encryption fundamentals.

**Key Features:**
- **Caesar Cipher** — Mono-alphabetic shift cipher with formula: `E(x) = (x + n) % 26`
- **Vigenère Cipher** — Polyalphabetic cipher using a keyword for variable shifts
- Handles edge cases: preserves case, spaces, punctuation, and digits
- Includes both **CLI** and **Tkinter GUI** versions

**Skills:** Encryption algorithms, modular arithmetic, GUI development

**How to Run:**
```bash
# CLI version
py "Task-2-Joy Kandie/caesar_cipher.py"

# GUI version
py "Task-2-Joy Kandie/cipher_gui.py"
```

---

### Project 3: Phishing Awareness Analysis
**📂 Folder:** [`Task-3-Joy Kandie/`](./Task-3-Joy%20Kandie/)  
**🎯 Goal:** Analyze emails/messages to identify phishing attempts and explain why they are unsafe.

**Key Features:**
- Scans messages across **5 threat categories**:

  | Category | What It Detects |
  |---|---|
  | Suspicious URLs | IP-address links, URL shorteners, spoofed domains, non-HTTPS |
  | Urgency / Pressure | "Act now", "account suspended", artificial deadlines |
  | Credential Harvesting | Password requests, SSN, credit card, wire transfers |
  | Spoofed Sender | Lookalike domains (paypa1.com), free-email impersonation |
  | Technical Red Flags | Generic greetings, .exe attachments, phishing language |

- **Weighted confidence scoring** (0–100%) with verdict: 🔴 PHISHING / 🟡 SUSPICIOUS / 🟢 LIKELY SAFE
- **5 built-in sample emails** for demonstration (4 phishing + 1 legitimate control)
- Each red flag includes a **human-readable explanation** of why it's dangerous
- **Actionable recommendations** based on verdict
- Both **CLI** and **Tkinter GUI** versions with color-coded output

**Skills:** Threat analysis, pattern recognition, security awareness, analytical thinking

**How to Run:**
```bash
# CLI version
py "Task-3-Joy Kandie/phishing_analyzer.py"

# GUI version
py "Task-3-Joy Kandie/phishing_gui.py"
```

**Sample Analysis Output:**
```
  VERDICT:    🔴 PHISHING
  CONFIDENCE: 100%
  FLAGS FOUND: 13

  [1] [Suspicious URL]
      Indicator:   URL shortener detected: http://bit.ly/3xR9kLm
      Explanation: The link uses 'bit.ly' to hide the true destination.

  [2] [Credential Harvesting]
      Indicator:   Phrase: "confirm your password"
      Explanation: No legitimate service asks for your password via email.
  ...
```

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **GUI Framework:** Tkinter
- **External Dependencies:** None (stdlib only)

---

## 🚀 Quick Start

```bash
# Clone the repo
git clone https://github.com/Joykan/DecodeLabs-Internship.git
cd DecodeLabs-Internship

# Run any project
py "Task-1-Joy Kandie/password_checker.py"
py "Task-2-Joy Kandie/cipher_gui.py"
py "Task-3-Joy Kandie/phishing_gui.py"
```

---

## 📞 Contact

**DecodeLabs**  
📞 +91 89330 06408  
✉️ decodelabs.tech@gmail.com  
🌎 [www.decodelabs.tech](https://www.decodelabs.tech)  
📍 Greater Lucknow, India
