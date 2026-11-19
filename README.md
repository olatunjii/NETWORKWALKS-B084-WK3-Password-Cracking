# 🔓 Password Cracking Lab: Recovering Locked PDF Passwords

**Using John the Ripper, hash extraction, and online cracking tools to recover passwords from locked PDFs**

![Skill](https://img.shields.io/badge/Skill-Password%20Cracking-E85D04?style=flat-square)
![Tool](https://img.shields.io/badge/Tool-John%20the%20Ripper-1E1E1E?style=flat-square&logo=linux&logoColor=white)
![Target](https://img.shields.io/badge/Target-PDF%20Files-C00000?style=flat-square&logo=adobeacrobatreader&logoColor=white)
![Method](https://img.shields.io/badge/Method-Dictionary%20Attack-2D6A4F?style=flat-square)
![Ethics](https://img.shields.io/badge/Use-Authorized%20Testing%20Only-0070C0?style=flat-square)

> Program: Cybersecurity at Networkwalks | Week: [YOUR WEEK] | Author: **[YOUR NAME]**
> LinkedIn: [YOUR LINKEDIN URL]

<!-- PASTE: title/cover screenshot here, e.g. your desktop with JtR and the hash tools open -->

---

## 📌 Project Overview

This project focused on recovering passwords from locked PDF files using two different approaches: a local command-line tool (**John the Ripper**) and web-based tools provided by Networkwalks (a hash calculator and an online password-cracking platform).

The goal was to understand how password hashes are extracted from protected files and how dictionary/word-list attacks are used to recover the original password.

> ⚠️ **Important:** These techniques were used only on PDFs provided for this lab. Never attempt to crack the password of a file you do not own or do not have explicit permission to test.

---

## 🎯 Objectives

- [x] Install and set up John the Ripper (CLI version)
- [x] Extract password hashes from locked PDFs
- [x] Crack hashes using John the Ripper locally
- [x] Use a web-based hash calculator to extract PDF hashes
- [x] Crack hashes using an online password-cracking platform
- [x] Apply a larger word list for harder passwords
- [x] Document which method worked for which file

---

## 🧰 Tools Used

| Tool | Purpose | Type |
|---|---|---|
| 🐍 John the Ripper (CLI) | Hash extraction + password cracking | Local |
| 🌐 PDF Hash Extractor | Extract hash from a locked PDF | Web-based |
| 🧮 Networkwalks Hash Calculator | Extract hash directly from a PDF | Web-based |
| 🔑 Networkwalks Password Cracking Platform | Crack extracted hashes | Web-based |
| 📖 John the Ripper Bulk Word List | Larger dictionary for tougher passwords | Word list |

---

# 🪜 Procedure

## Method 1: John the Ripper (CLI)

### Step 1. Download and extract John the Ripper
Downloaded the John the Ripper package and extracted it for CLI use.

<!-- PASTE: screenshot of the extracted John the Ripper folder/files -->

### Step 2. Extract the hash from the locked PDF
Used the **PDF Hash Extractor** website: uploaded the locked PDF and generated its hash.

<!-- PASTE: screenshot of the PDF Hash Extractor site with the hash generated -->

### Step 3. Save the hash to a text file
Copied the extracted hash into a `.txt` file for John the Ripper to read.

<!-- PASTE: screenshot of the saved hash text file -->

### Step 4. Run the crack
Uploaded/pointed the hash text file into John the Ripper and ran the cracking command.

<!-- PASTE: screenshot of John the Ripper running and the cracked password output -->

**Result:** ✅ Password recovered for [X of Y] PDFs using this method.

---

## Method 2: Networkwalks Hash Calculator + Cracking Platform

### Step 1. Extract the hash directly
Uploaded the locked PDF directly to the **Networkwalks Hash Calculator** (web-based) and copied the generated hash.

<!-- PASTE: screenshot of the Hash Calculator with the PDF uploaded and hash shown -->

### Step 2. Submit the hash for cracking
Pasted the hash into the **Networkwalks Password Cracking Platform** and started the crack.

<!-- PASTE: screenshot of the cracking platform mid-run -->

**Result:** ✅ Worked for some PDFs on the first try. ⏳ Others needed a bigger word list (see below).

### Step 3. Use a larger word list for tougher passwords
For the PDFs that didn't crack on the first attempt, uploaded the **John the Ripper bulk word list** to the same platform and restarted the crack.

<!-- PASTE: screenshot of the word list being uploaded -->
<!-- PASTE: screenshot of the final cracked password result -->

**Result:** ✅ Password recovered after the larger word list was applied. Took longer, but succeeded.

---

## 📊 Results Summary

| PDF | Method Used | Word List | Outcome |
|---|---|---|---|
| PDF 1 | John the Ripper (CLI) | Default | ✅ Cracked |
| PDF 2 | Hash Calculator + Cracking Platform | Default | ✅ Cracked |
| PDF 3 | Hash Calculator + Cracking Platform | JtR Bulk List | ✅ Cracked |



---

## 💡 What I Learned

- How a password hash is extracted from a protected file before it can be attacked
- The difference between a local CLI tool (John the Ripper) and a web-based cracking workflow
- Why a dictionary/word-list attack can fail with a small list but succeed with a larger one
- That cracking time increases significantly with word-list size
- The importance of only running these tools against files you're authorized to test

---

## 🔐 Ethical Use

This lab is strictly for educational purposes using files provided for the course. Do not use these tools or techniques against any file or system without explicit permission.

---

## 🔗 Resources

- John the Ripper: [https://www.openwall.com/john/](https://www.openwall.com/john/)
- PDF Hash Extractor: [add the link you used]
- Networkwalks Hash Calculator: [add the link you used]
- Networkwalks Password Cracking Platform: [add the link you used]
- JtR Bulk Word List: [add the link provided in your course]

---

## 📎 Reference

