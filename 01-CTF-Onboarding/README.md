# 🚀 01 — CTF Onboarding & Environment Setup

Welcome to the **CTF Onboarding** section! This module serves as the foundation for navigating Capture The Flag (CTF) environments, setting up necessary tools, and mastering essential Linux terminal skills required throughout the CyLab Security Academy.

---

## 🎯 Objectives & Learning Outcomes

By completing the onboarding module, you will learn how to:
- Access and navigate the **Linux WebShell** / command-line environment.
- Download and inspect challenge files safely using terminal utilities.
- Understand standard flag formats (`picoCTF{...}`) and submission workflows.
- Organize local files and writeups for systematic documentation.

---

## 🧰 Essential Terminal Tools & Commands

Here are the primary Linux commands used during onboarding and daily CTF navigation:

### 1. Navigating & Inspecting Files
| Command | Usage | Description |
| :--- | :--- | :--- |
| `pwd` | `pwd` | Print working directory (shows current location). |
| `ls -la` | `ls -la` | List all files, including hidden files (`.filename`), with permissions. |
| `cd <dir>` | `cd 01-CTF-Onboarding` | Change directory to the target path. |
| `cat <file>` | `cat flag.txt` | Display the full text contents of a file in the terminal. |
| `file <file>` | `file executable` | Determine file type (ASCII text, ELF binary, PNG image, zip archive). |

### 2. Fetching & Downloading Resources
| Command | Usage | Description |
| :--- | :--- | :--- |
| `wget <url>` | `wget https://.../file` | Download a challenge file directly to the current terminal directory. |
| `curl <url>` | `curl https://...` | Fetch web page contents or API responses via command line. |

### 3. File Permissions
| Command | Usage | Description |
| :--- | :--- | :--- |
| `chmod +x` | `chmod +x script.sh` | Grant executable permissions to a script or binary file. |

---

## 🔁 Standard CTF Challenge Workflow

When starting any challenge, follow this standard step-by-step workflow:

1. **Environment Initialization:** Launch your terminal or picoCTF WebShell.
2. **File Acquisition:** Download provided challenge assets using `wget <URL>`.
3. **File Inspection:** Verify file properties with `file` and check plain text contents using `cat`.
4. **Solve & Extract:** Execute necessary terminal commands or scripts to reveal the flag.
5. **Document:** Copy the flag, record commands used, and update the writeup document.

---

## 📂 Section Directory Layout

```text
01-CTF-Onboarding/
│
├── 📜 README.md                 # Module overview & command cheat sheet (this file)
└── 📁 Writeups/                 # Step-by-step documentation for onboarding tasks
