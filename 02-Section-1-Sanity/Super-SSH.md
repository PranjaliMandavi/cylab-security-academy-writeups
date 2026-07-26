# Super SSH

**Category:** General Skills  
**Difficulty:** Easy  
**Platform:** picoCTF 2021

## Challenge Description

> Using a Secure Shell (SSH) is going to be pretty important. Can you log in to this server?

## Objective

Connect to the remote server using the provided SSH credentials and retrieve the flag.

## Solution

The challenge provided the following information:

- **Host:** `titan.picoctf.net`
- **Port:** `52857`
- **Username:** `ctf-player`
- **Password:** *(provided by the challenge)*


```bash
ssh ctf-player@titan.picoctf.net -p 52857
```

On the first connection, SSH prompted me to verify the server's authenticity. After accepting the host key, I entered the password provided by the challenge.

Once authenticated, the server displayed the flag.

## Commands Used

```bash
ssh ctf-player@titan.picoctf.net -p 52857
```

## Screenshot

![Super SSH Solution] ![Uploading image.png…]()


## Skills Learned

- Connecting to remote systems using SSH
- Using the `-p` option to specify a custom port
- Verifying an SSH host key
- Understanding common SSH connection errors

## Key Takeaway

SSH uses **port 22** by default. When a service runs on a different port, the `-p` option must be used to specify the correct port. Reading the challenge instructions carefully and understanding SSH syntax helps avoid common connection errors.

> **Note:** The flag has been intentionally omitted from this write-up.
