🗂️ Traditional CTF Challenge Categories
Capture The Flag (CTF) competitions split challenges into distinct categories based on the security domain, skill set, and technical tools required to solve them. Understanding these categories helps structure writeups and choose the right tools for the job.

1. 🔬 Reverse Engineering (Rev / RE)
Reverse Engineering involves analyzing compiled binaries, bytecode, or scripts without having the original source code. The goal is to understand the program's underlying logic, control flow, and input validation routines to extract the flag or bypass checks.

Key Concepts: Control flow analysis, function tracing, dynamic key generation, deobfuscation, keygenning, patching.

Common File Types: .pyc, Executable files (ELF/PE), .class, .apk.

Essential Tools: Ghidra, IDA Free, GDB, pdb, dis, uncompyle6, Binary Ninja.

2. 🔐 Cryptography (Crypto)
Cryptography challenges test your ability to break broken encryption algorithms, exploit weak key generation, or reverse custom mathematical ciphers. Unlike real-world encryption (like modern AES-256), CTF crypto challenges intentionally implement flawed mathematics or misconfigured parameters.

Key Concepts: Classical ciphers (Caesar, Vigenère, Substitution), RSA parameter attacks, AES modes (ECB/CBC IV reuse), XOR bitwise operations, frequency analysis.

Key Tools: CyberChef, Python (hashlib, pycryptodome), SageMath, RsaCftTool.

3. 🌐 Web Exploitation (Web)
Web challenges focus on finding and exploiting vulnerabilities in web applications, REST APIs, databases, and web servers. Participants interact with web interfaces or proxy HTTP requests to gain unauthorized access or leak hidden data.

Key Concepts: SQL Injection (SQLi), Cross-Site Scripting (XSS), Command Injection, Local/Remote File Inclusion (LFI/RFI), Session Hijacking/Cookie Tampering, Insecure Direct Object References (IDOR).

Essential Tools: Burp Suite, OWASP ZAP, sqlmap, curl, Browser Developer Tools (F12).

4. 🧩 Forensics & Steganography
Forensics challenges involve investigating digital artifacts, memory dumps, network traffic, or hidden data inside media files. It simulates real-world Digital Forensics and Incident Response (DFIR).

Key Concepts: Hidden file extraction, metadata analysis, network packet analysis, memory inspection, file carvers, steganography (hiding data inside images or audio).

Common File Types: .pcap/.pcapng, .png, .jpg, .wav, .raw (memory dumps).

Essential Tools: Wireshark, exiftool, binwalk, steghide, zsteg, Volatilty.

5. 💥 Binary Exploitation (Pwn)
Pwn challenges involve exploiting vulnerabilities in compiled programs (usually written in C/C++) running on a remote server. The goal is typically to corrupt program memory, divert control flow, and spawn a remote shell (/bin/sh) to read the flag from the target server.

Key Concepts: Buffer overflows, Format string vulnerabilities, Return-Oriented Programming (ROP), Heap exploitation, Integer overflows.

Essential Tools: pwntools (Python library), GDB + pwndbg / GEF, checksec, ropper, one_gadget.

6. 🛠️ General Skills / Miscellaneous (Misc)
Misc challenges cover broad technical competencies that don't fit neatly into the core categories. They often test command-line efficiency, scripting speed, OSINT (Open Source Intelligence), or problem-solving.

Key Concepts: Linux shell navigation, regex matching, audio manipulation, esoteric programming languages (Esolangs), automated web scraping.

Essential Tools: grep, find, awk, sed, Bash scripting, Python automation.
