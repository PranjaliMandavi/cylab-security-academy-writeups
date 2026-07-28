# Waved a Flag

**Category:** General Skills  
**Difficulty:** Easy  
**Platform:** picoCTF 2021

## Challenge Description

The challenge provides an executable file named `warm`. The objective is to execute the binary and retrieve the hidden flag.

## Objective

Make the binary executable and use its help option to reveal the flag.

## Solution

After downloading the challenge file, I listed the files in the current directory to verify that the `warm` binary was present.

```bash
ls
```

The binary did not have execute permission, so I added it using the `chmod` command.

```bash
chmod +x warm
```

Once the executable permission was granted, I ran the binary with the `-h` (help) option.

```bash
./warm -h
```

The program displayed its help message, which also contained the flag. I copied the flag and submitted it successfully.

## Commands Used

```bash
ls
chmod +x warm
./warm -h
```

## Tools Used

- Kali Linux Terminal
- `chmod`
- Linux Command Line

## Screenshot

![Warmed Up]<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/fe59e639-bdf3-4f0e-8ffc-92ff9ec9287f" />


## Skills Learned

- Linux file permissions
- Making files executable using `chmod`
- Running ELF executables
- Using help (`-h`) options to inspect program functionality

## Key Takeaway

Many Linux executables require execute permissions before they can be run. During CTF challenges, checking a program's help menu (`-h` or `--help`) can reveal useful information, hidden functionality, or even the flag itself.

> **Note:** The flag has been intentionally omitted from this write-up.
