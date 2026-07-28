# First Grep

**Category:** General Skills  
**Difficulty:** Easy  
**Platform:** picoCTF 2021

## Challenge Description

The challenge provides a large text file containing random data. The objective is to locate the hidden flag using Linux command-line tools.

## Objective

Find the hidden flag inside the provided text file.

## Solution

First, I listed the available files to verify that the challenge file was present.

```bash
ls
```

Next, I checked the type of the file.

```bash
file file
```

The output showed that the file was an ASCII text file with very long lines.

```text
file: ASCII text, with very long lines (14545)
```

Since picoCTF flags begin with `picoCTF{`, I searched the file using the `grep` command.

```bash
grep "picoCTF" file
```

The command returned the line containing the hidden flag.

## Tools Used

- Kali Linux
- grep
- file

## Screenshot

<img width="2560" height="1600" alt="screenshot_20260725_171124" src="https://github.com/user-attachments/assets/690cf418-fbf2-41bc-a20c-76eb4742065e" />
<img width="2560" height="1600" alt="screenshot_20260725_171056" src="https://github.com/user-attachments/assets/7d53a6fa-1a3e-42f2-87c8-4f35dda145c6" />


## Skills Learned

- Linux command-line basics
- Using the `grep` command
- File inspection with the `file` utility
- Pattern searching in text files

## Key Takeaway

The `grep` command is an efficient way to search large files for specific patterns. Instead of manually inspecting thousands of lines, pattern matching allows you to quickly locate relevant information such as flags, credentials, or log entries.

> **Note:** The flag has been intentionally omitted from this write-up.
