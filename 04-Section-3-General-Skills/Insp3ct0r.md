# Insp3ct0r

**Category:** Web Exploitation  
**Difficulty:** Easy  
**Platform:** picoCTF 2021

## Challenge Description

The challenge presents a simple webpage with no visible flag. The objective is to inspect the webpage and its associated files to locate the hidden flag.

## Objective

Inspect the webpage source and linked resources to recover the complete flag.

## Solution

I opened the challenge website in my browser.

First, I opened the browser's **Developer Tools** by pressing **F12** and inspected the HTML source. In the HTML comments, I found the **first part** of the flag.

Next, I switched to the **Sources** tab and opened the linked CSS file (`mycss.css`). At the bottom of the file, I found the **second part** of the flag inside a CSS comment.

Finally, I opened the JavaScript file (`myjs.js`). A comment at the end of the file contained the **third part** of the flag.

After combining the three parts obtained from the HTML, CSS, and JavaScript files, I reconstructed the complete flag and submitted it successfully.

## Files Inspected

- `index.html`
- `mycss.css`
- `myjs.js`

## Tools Used

- Google Chrome
- Chrome Developer Tools (F12)

## Steps Performed

1. Open the challenge website.
2. Press **F12** to open Developer Tools.
3. Inspect the HTML source and locate the first part of the flag in an HTML comment.
4. Open `mycss.css` from the **Sources** tab and locate the second part in a CSS comment.
5. Open `myjs.js` and locate the final part in a JavaScript comment.
6. Combine all three parts to obtain the complete flag.
7. Submit the flag.

## Screenshot

### HTML Source

![HTML Source] <img width="2560" height="1600" alt="screenshot_20260725_164357" src="https://github.com/user-attachments/assets/ed88cb58-d3ad-44ce-8300-524154047a9e" />


### CSS File

![CSS File] <img width="2560" height="1600" alt="screenshot_20260725_165029" src="https://github.com/user-attachments/assets/8d353d78-6476-4613-b885-169e9313843c" />


### JavaScript File

![JavaScript File] <img width="2560" height="1600" alt="screenshot_20260725_165103" src="https://github.com/user-attachments/assets/c065f84d-ea64-4a47-9147-186fdc7ee995" />


## Skills Learned

- Inspecting HTML source code
- Using Chrome Developer Tools
- Analyzing CSS and JavaScript files
- Finding sensitive information hidden in client-side code

## Key Takeaway

Client-side files such as HTML, CSS, and JavaScript are publicly accessible to every user visiting a website. Developers should never store sensitive information such as secrets, credentials, or flags in these files because they can easily be discovered through browser Developer Tools.

> **Note:** The flag has been intentionally omitted from this write-up.
