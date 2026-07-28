# where are the robots

**Category:** General Skills  
**Difficulty:** Easy  
**Platform:** picoCTF 2021

## Challenge Description

The challenge provides a website and requires finding the hidden flag. The title suggests checking the `robots.txt` file, which is commonly used to tell web crawlers which pages or directories should not be indexed.

## Objective

Inspect the website and locate the hidden flag by exploring the `robots.txt` file.

## Solution

I opened the challenge website in a web browser.

Since the challenge title hinted at robots, I navigated to the `robots.txt` file by appending `/robots.txt` to the website URL.

```
https://<challenge-url>/robots.txt
```

The file contained a disallowed directory.

```
User-agent: *
Disallow: /<hidden-directory>/
```

I then visited the hidden directory mentioned in the `robots.txt` file.

```
https://<challenge-url>/<hidden-directory>/
```

The directory contained the page displaying the flag.

## Tools Used

- Web Browser
- robots.txt

## Screenshot

<img width="2560" height="1600" alt="screenshot_20260725_171536" src="https://github.com/user-attachments/assets/755d72e1-7967-4ee8-a2cc-726b513cca6c" />
<img width="2560" height="548" alt="screenshot_20260725_171545" src="https://github.com/user-attachments/assets/e58c48ab-dd65-4ce7-9ce4-43dd64960772" />


## Skills Learned

- Web enumeration
- Understanding `robots.txt`
- Directory discovery
- Basic web reconnaissance

## Key Takeaway

The `robots.txt` file is publicly accessible and can reveal hidden directories or resources that developers do not want search engines to index. During web security assessments and CTFs, checking `robots.txt` is a simple but effective reconnaissance technique.

> **Note:** The flag has been intentionally omitted from this write-up.
