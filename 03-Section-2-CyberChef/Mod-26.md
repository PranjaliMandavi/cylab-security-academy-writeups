# Mod 26

**Category:** CyberChef  
**Difficulty:** Easy  
**Platform:** picoCTF 2021

## Challenge Description

The challenge provides text encrypted using the ROT13 cipher and requires recovering the original message.

## Objective

Decode the given ciphertext using the appropriate CyberChef operation.

## Solution

The provided text appeared to be encoded with the ROT13 cipher. I opened **CyberChef**, added the **ROT13** recipe, and pasted the ciphertext into the input panel.

CyberChef automatically decoded the message, revealing the flag.

## Tool Used

- CyberChef

## Recipe

```
ROT13
```

## Screenshot

![Mod 26] <img width="2560" height="1332" alt="screenshot_20260725_160800" src="https://github.com/user-attachments/assets/a4e88d2c-03a6-4899-89d5-21609b6a9e0f" />



## Skills Learned

- Identifying ROT13 encoded text
- Using CyberChef recipes
- Understanding Caesar cipher rotations

## Key Takeaway

ROT13 is a simple substitution cipher that shifts each alphabetic character by 13 positions. Applying the same operation twice restores the original text.

> **Note:** The flag has been intentionally omitted from this write-up.
