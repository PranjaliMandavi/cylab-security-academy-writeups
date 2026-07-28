# where are the robots

**Category:** General Skills  
**Difficulty:** Easy  
**Platform:** picoCTF 2021

## Challenge Description

The challenge provides a ZIP archive containing a deeply nested directory structure. The objective is to navigate through the directories, locate the executable file, and run it to obtain the flag.

## Objective

Navigate the extracted directories, identify the executable file, and execute it to reveal the flag.

## Solution

I first extracted the provided ZIP archive using the `unzip` command.

```bash
unzip Addadshashanammu.zip
```

After extraction, I manually navigated through each nested directory using the `cd` command until I reached the final directory containing the executable.

Once there, I listed the files to identify the executable.

```bash
ls
```

I verified the file type using the `file` command.

```bash
file fang-of-haynekhtnamet
```

The output showed that it was a 64-bit ELF executable.

Next, I granted execute permissions to the file.

```bash
chmod +x fang-of-haynekhtnamet
```

Finally, I executed the binary.

```bash
./fang-of-haynekhtnamet
```

The program displayed the flag, which I submitted successfully.

## Tools Used

- Kali Linux
- Linux Terminal
- `unzip`
- `cd`
- `ls`
- `file`
- `chmod`

## Steps Performed

1. Extracted the ZIP archive using `unzip`.
2. Navigated through each nested directory using `cd`.
3. Listed the contents of each directory using `ls`.
4. Located the executable file `fang-of-haynekhtnamet`.
5. Verified its type using the `file` command.
6. Made the file executable using `chmod +x`.
7. Executed the binary to obtain the flag.
8. Submitted the flag.

## Screenshot

### Extracting the ZIP Archive

![Extract ZIP] <img width="2560" height="1600" alt="screenshot_20260725_164018" src="https://github.com/user-attachments/assets/e3336ffe-85b7-4783-bc4e-fa1bee46d84f" />

### Navigating the Nested Directories

![Directory Navigation]
<img width="2560" height="1600" alt="screenshot_20260725_164030" src="https://github.com/user-attachments/assets/e756bf85-f633-4b3e-b348-4e96334918a8" />

### Executing the Binary

![Run Binary] <img width="2560" height="1600" alt="screenshot_20260725_164039" src="https://github.com/user-attachments/assets/7ac0fa4a-f6a7-4478-8b09-a3e10a22a0e0" />


## Skills Learned

- Linux file navigation
- Using `unzip` to extract archives
- Directory traversal with `cd`
- Listing files with `ls`
- Identifying file types using `file`
- Modifying file permissions with `chmod`
- Executing ELF binaries

## Key Takeaway

This challenge reinforces essential Linux command-line skills required for cybersecurity and CTFs. Understanding how to navigate directories, inspect files, change permissions, and execute binaries is fundamental for analysing and interacting with files in Linux environments.

> **Note:** The flag has been intentionally omitted from this write-up.
