# Obedient Cat

**Category:** General Skills  
**Difficulty:** Easy  
**Platform:** picoCTF 2021

## Challenge Description

> This file has a flag in plain sight (aka "in-the-clear").

## Objective

Retrieve the flag from the provided file.

## Solution

The challenge provided a file named `flag`. Since the description indicated that the flag was "in plain sight", I first listed the contents of the working directory to verify that the file had been downloaded successfully.

```bash
ls
```

Output:

```text
flag
```

Next, I displayed the contents of the file using the `cat` command.

```bash
cat flag
```

The command printed the flag directly to the terminal, confirming that the file contained plain text and required no additional decoding or analysis.

## Commands Used

```bash
ls
cat flag
```

## Screenshot

![Solution Screenshot] <img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/64093b6e-200b-430c-b637-7f5877031c18" />


## Skills Learned

- Basic Linux file navigation
- Listing directory contents using `ls`
- Reading text files using `cat`
- Understanding and following challenge descriptions

## Key Takeaway

Not every CTF challenge requires advanced techniques. Reading the challenge description carefully can often provide enough information to solve introductory problems quickly.

> **Note:** The flag has been intentionally omitted from this write-up.<img width="2560" height="1600" alt="screenshot_20260725_160145" src="https://github.com/user-attachments/assets/b1df5ff8-d554-4110-8d3b-c5b1016103f9" />
