# strings it

**Category:** General Skills  
**Difficulty:** Easy  
**Platform:** picoCTF 2021

## Challenge Description

The challenge provides an executable file that contains a hidden flag. The objective is to inspect the file and extract the flag using basic Linux command-line utilities.

## Objective

Identify the file type and retrieve the hidden flag without executing the binary.

## Solution

First, I listed the files in the challenge directory.

```bash
ls
```

Next, I identified the file type using the `file` command.

```bash
file strings
```

The output showed that the file was a **64-bit ELF executable**.

I then extracted all printable strings from the executable and filtered the output for the picoCTF flag using `grep`.

```bash
strings strings | grep pico
```

The command displayed the hidden flag, which was then submitted to complete the challenge.

## Tools Used

- Kali Linux
- `file`
- `strings`
- `grep`

## Screenshot

![strings it]
<img width="2560" height="585" alt="screenshot_20260725_165804" src="https://github.com/user-attachments/assets/08a37f6c-0dc0-472d-b199-a61615260a7e" />



## Skills Learned

- Identifying executable file types using `file`
- Extracting printable strings from binaries
- Searching command output with `grep`
- Performing basic static analysis of executables

## Key Takeaway

Many executable files contain readable strings such as error messages, configuration values, or even flags. The `strings` utility is a quick and effective technique for extracting printable text from binaries, making it a valuable tool during CTFs, reverse engineering, and malware analysis.

> **Note:** The flag has been intentionally omitted from this write-up.
