# What's a Net Cat?

**Category:** General Skills  
**Difficulty:** Easy  
**Platform:** picoCTF 2021

## Challenge Description

> Using Netcat (nc) is an essential networking skill. Can you connect to the given server and retrieve the flag?

## Objective

Use Netcat (`nc`) to connect to the remote server and obtain the flag.

## Solution

The challenge provided a hostname and a port number. Using the `nc` (Netcat) command, I connected to the remote service.

```bash
nc fickle-tempest.picoctf.net 51437
```

After establishing the connection, the server immediately displayed a welcome message followed by the flag.

## Commands Used

```bash
nc fickle-tempest.picoctf.net 51437
```

## Screenshot

![What's a Net Cat Solution] <img width="1835" height="273" alt="image" src="https://github.com/user-attachments/assets/5cb1ce6a-6297-441b-8582-37efd70fae91" />


## Skills Learned

- Using Netcat (`nc`) to connect to remote TCP services.
- Understanding how to specify a hostname and port.
- Retrieving data from a remote server through a terminal connection.

## Key Takeaway

Netcat is a versatile networking utility used to establish TCP/UDP connections, transfer data, perform port testing, and interact with remote services. It is one of the most commonly used tools in CTF competitions for communicating with challenge servers.

> **Note:** The flag has been intentionally omitted from this write-up.
