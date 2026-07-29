# Python Wrangling

## Challenge Information

| Category | Python |
|----------|---------|
| Difficulty | Easy |
| Platform | picoCTF |

---

## Objective

The challenge provides an encrypted flag (`flag.txt.en`), a Python decryption script (`ende.py`), and a password file (`password.txt`). The goal is to decrypt the encrypted flag using the provided script and the correct password.

---

## Skills Learned

- Linux command-line usage
- Python script execution
- File inspection
- Working with encrypted files
- Understanding command-line arguments

---

## Tools Used

- Kali Linux
- Python 3
- Linux Terminal

---

## Files Provided

```text
ende.py
flag.txt.en
password.txt
```

---

## Methodology

### Step 1: Verify the Files

List the contents of the directory.

```bash
ls
```

Output:

```text
ende.py
flag.txt.en
password.txt
```

This confirms that the Python decryption script, encrypted flag, and password file are present.

---

### Step 2: Execute the Decryption Script

Run the Python script with the encrypted file using the `-d` option.

```bash
python3 ende.py -d flag.txt.en
```

The program prompts for the password.

```text
Please enter the password:
```

Enter the password stored in `password.txt`.

The script decrypts the encrypted file and prints the flag.

---

## Commands Used

```bash
ls

python3 ende.py -d flag.txt.en
```

---

## Explanation

The challenge supplies everything required for decryption:

- `ende.py` performs the decryption.
- `flag.txt.en` contains the encrypted flag.
- `password.txt` stores the password needed by the script.

Instead of reverse engineering the encryption algorithm, simply execute the script and provide the correct password when prompted. The script then decrypts the encrypted flag and displays it on the terminal.

---

## Learning Outcome

This challenge helped reinforce:

- Executing Python programs from the command line.
- Understanding command-line arguments.
- Inspecting challenge files before attempting complex analysis.
- Using provided resources effectively during CTF challenges.

---

## Screenshot

**Successful decryption of the encrypted flag using the provided Python script.**

> <img width="2560" height="469" alt="image" src="https://github.com/user-attachments/assets/73827fb2-ebd4-4fcc-861e-a91302eb1d24" />


---

## References

- picoCTF
- Python 3 Documentation
- Kali Linux Documentation

---

> **Note:** The actual flag has been intentionally hidden in this write-up to preserve the integrity of the challenge.
