# 🛡️ CyLab Security Academy — Learning Journey & CTF Writeups

Welcome to my personal cybersecurity archive! 

This repository documents my hands-on learning journey through the **CyLab Security Academy** (powered by Carnegie Mellon University's picoCTF platform). It serves as my practical notebook, containing detailed writeups, technical breakdowns, and solver scripts for every challenge I completed across the curriculum.

---

## ❓ What is CyLab Security Academy?

The **CyLab Security Academy** is an intensive, practical training program designed to teach core cybersecurity concepts through Capture The Flag (CTF) challenges. Rather than just memorizing theory, the curriculum focuses on hands-on problem-solving in:

- **Linux Fundamentals & Command-Line Operations**
- **Data Encoding, Ciphers & Cryptography**
- **Python Scripting, Automation & Hash Analysis**
- **Reverse Engineering & Code Analysis**

---

## 🎯 Purpose of This Repository

I created this repository to:
1. **Document My Growth:** Keep a structured record of how I approached, debugged, and solved security challenges step-by-step.
2. **Build Reusable Tools:** Save custom Python solver scripts, keygens, and terminal commands for future reference.
3. **Demonstrate Methodology:** Show my thought process, static analysis skills, and ability to reverse engineer unknown code.

---

## 📂 Repository Structure & What I Learned

The repository follows the exact module progression of the academy. Each folder contains my Markdown writeups alongside raw challenge files and solver code.

```text
cylab-security-academy-writeups/
│
├── 📜 README.md                         # Repository overview & learning notes
│
├── 📁 01-CTF-Onboarding/                # Platform mechanics & environment setup
│   └── README.md                        # Linux shell configuration & basic tools
│
├── 📁 02-Section-1-Sanity/              # Warmup verification challenges
│   └── Writeups/                        # Understanding CTF flag formats and validation
│
├── 📁 03-Section-2-CyberChef/           # Data Manipulation & Cryptography
│   └── Writeups/                        # Base64 encoding/decoding, XOR operations, 
│                                        # ROT13, and multi-stage CyberChef pipelines
│
├── 📁 04-Section-3-General-Skills/       # Command-Line Mastery
│   └── Writeups/                        # Deep-directory searches (`grep -r`), 
│                                        # text filtering (`cut`/`awk`), file permissions
│
├── 📁 05-Section-4-Python/              # Scripting, Automation & Hashing
│   ├── keygenme-py/                     # Dynamic keygen reverse engineering
│   └── Writeups/                        # `hashlib`, character slicing, and dictionary attacks
│
└── 📁 06-Section-5-Binary-and-RE/       # Reverse Engineering & Code Analysis
    ├── Arcane-Calculator/               # Python source analysis & Fernet decryption
    └── Writeups/                        # Control flow analysis, interactive debugging (`pdb`)

## 💡 Technical Skills Demonstrated

### 🔬 Reverse Engineering & Code Analysis
> **Static Analysis:** Reading and tracing Python and Java source code to map out program logic, input constraints, and validation rules without running untrusted code.
> **Control Flow Mapping:** Reconstructing how programs validate keys and inputs character-by-character (e.g., tracing function checks in `check_key()`).
> **Cryptographic Slicing:** Understanding how applications generate or verify keys using character slicing and index mapping over hash outputs (SHA-256).

### 🐍 Python Scripting & Security Automation
> **Standard Library Mechanics:** Utilizing `hashlib`, `base64`, and `cryptography` (Fernet) modules to automate key generation, payload decryption, and hash verification.
> **Command-Line One-Liners:** Executing Python inline scripts (`python3 -c`) to quickly inspect variables, evaluate hashes, or solve challenges directly inside the terminal.
> **Interactive Debugging:** Using Python REPL sessions (`python3 -i`) and `pdb` to inspect dynamic variable states in memory at runtime.

### 💻 Linux & Command-Line Operations
> **Targeted File Search:** Using `grep -r`, `find`, and pattern matching to locate hidden flags across deeply nested directory structures.
> **Text Processing & Streams:** Combining Unix piping (`|`), `tr`, `strings`, `cut`, and `awk` to extract clean metadata and plain text out of complex or binary file formats (like SVG XML trees).
> **Archive & System Handling:** Managing file permissions (`chmod`), archive extraction (`unzip`, `tar`), and terminal-based file downloads (`wget`).
    
