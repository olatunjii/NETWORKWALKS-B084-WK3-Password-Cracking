# 🔓 Password Cracking Lab: Recovering Locked PDF Passwords

**Using John the Ripper, hash extraction, and online cracking tools to recover passwords from locked PDFs**

![Skill](https://img.shields.io/badge/Skill-Password%20Cracking-E85D04?style=flat-square)
![Tool](https://img.shields.io/badge/Tool-John%20the%20Ripper-1E1E1E?style=flat-square&logo=linux&logoColor=white)
![Target](https://img.shields.io/badge/Target-PDF%20Files-C00000?style=flat-square&logo=adobeacrobatreader&logoColor=white)
![Method](https://img.shields.io/badge/Method-Dictionary%20Attack-2D6A4F?style=flat-square)
![Ethics](https://img.shields.io/badge/Use-Authorized%20Testing%20Only-0070C0?style=flat-square)

> Program: Cybersecurity at Networkwalks | Week: 3 | Author: **ABDULKADIRI ADARANIJO**
> 
> LinkedIn: https://www.linkedin.com/in/tj-adaranijo-02183a191/


---

## 📌 Project Overview

This project focused on recovering passwords from locked PDF files using two different approaches: a local command-line tool (**John the Ripper**) and web-based tools provided by Networkwalks (a hash calculator and an online password-cracking platform).

The goal was to understand how password hashes are extracted from protected files and how dictionary/word-list attacks are used to recover the original password.

> ⚠️ **Important:** These techniques were used only on PDFs provided for this lab. Never attempt to crack the password of a file you do not own or do not have explicit permission to test.

---

## 🎯 Objectives

- [x] Install and set up John the Ripper with Johny GUI
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
| 🐍 John the Ripper, Johny GUI | Password cracking | Local |
| 🌐 PDF Hash Extractor | Extract hash from a locked PDF | Web-based |
| 🧮 Networkwalks Hash Calculator | Extract hash directly from a PDF | Web-based |
| 🔑 Networkwalks Password Cracking Platform | Crack extracted hashes | Web-based |
| 📖 John the Ripper Bulk Word List | Larger dictionary for tougher passwords | Word list |

---

# 🪜 Procedure

## Method 1: John the Ripper (CLI)

### Step 1. Download and extract John the Ripper
Downloaded the John the Ripper package and extracted it for CLI use.

<img width="1920" height="1080" alt="Screenshot (53)" src="https://github.com/user-attachments/assets/22d12ce6-68ac-4db5-8ced-df68997191ce" />


### Step 2. Extract the hash from the locked PDF
Used the **PDF Hash Extractor** website: uploaded the locked PDF and generated its hash.

<img width="1920" height="1080" alt="Screenshot (28)" src="https://github.com/user-attachments/assets/4ecb4384-aad1-4465-9459-0766c25a2dbb" />


### Step 3. Save the hash to a text file
Copied the extracted hash into a `.txt` file for John the Ripper to read.

<img width="1920" height="1080" alt="Screenshot (54)" src="https://github.com/user-attachments/assets/68822dd4-f00e-4900-ae70-94649279d7c0" />


### Step 4. Run the crack
Uploaded/pointed the hash text file into John the Ripper and ran the cracking command.

<img width="1920" height="1080" alt="Screenshot (31)" src="https://github.com/user-attachments/assets/c9df1c6e-39ad-4122-9f01-f716256eaa0a" />


<img width="1920" height="1080" alt="Screenshot (43)" src="https://github.com/user-attachments/assets/4d3f464e-95cc-45b1-980b-a1473bbea01f" />


**Locked PDF 2**

<img width="1920" height="1080" alt="Screenshot (41)" src="https://github.com/user-attachments/assets/8cb38dc7-ba62-42a9-a48b-096653e25383" />

**Result:** ✅ Password recovered for My Locked PDF 1-3 using this method.

---

## Method 2: Networkwalks Hash Calculator + Cracking Platform

### Step 1. Extract the hash directly
Uploaded the locked PDF directly to the **Networkwalks Hash Calculator** (web-based) and copied the generated hash.

<img width="1920" height="1080" alt="Screenshot (46)" src="https://github.com/user-attachments/assets/a7382a64-e469-4942-a047-81b795c825e3" />


### Step 2. Submit the hash for cracking
Pasted the hash into the **Networkwalks Password Cracking Platform** and started the crack.

<img width="1920" height="1080" alt="Screenshot (48)" src="https://github.com/user-attachments/assets/3f266adb-a60b-4f51-be3d-5f6ae796920c" />

**Password Cracked**

<img width="1920" height="1080" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/0ab10c06-ff22-41c9-b57e-0768bfb360dd" />


**Result:** ✅ Worked for some PDFs on the first try. ⏳ Others needed a bigger word list (see below).

### Step 3. Use a larger word list for tougher passwords
For the PDFs that didn't crack on the first attempt, I uploaded the **John the Ripper bulk word list** to the same platform and restarted the crack.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/53bc12bd-2568-40c0-9769-d43e6a7925b0" />


 **Larger word list uploaded**

<img width="1920" height="1080" alt="Screenshot (57)" src="https://github.com/user-attachments/assets/a896c3ec-b415-4b87-b422-cc507bdd34bf" />


 **✅ Password cracked**
 

<img width="1908" height="1078" alt="image" src="https://github.com/user-attachments/assets/1bbcb2ac-82a8-4c2c-8224-96a668d9b13c" />


**Flag Captured**

<img width="1920" height="1080" alt="Screenshot (39)" src="https://github.com/user-attachments/assets/ee159ed9-5a04-4f4b-bd0f-8f566bbacbdd" />


**Result:** ✅ Password recovered after the larger word list was applied. Took longer, but succeeded.

---

## 📊 Results Summary

| PDF | Method Used | Word List | Outcome |
|---|---|---|---|
| PDF 1 | John the Ripper (GUI) | Default | ✅ Cracked |
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

- John the Ripper: https://www.openwall.com/john/
- PDF Hash Extractor: https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php#extract
- Networkwalks Hash Calculator: https://networkwalks.com/hash-calculator/
- Networkwalks Password Cracking Platform: https://networkwalks.com/password-cracker/
- JtR Bulk Word List: https://drive.google.com/file/d/1hwx0rbvEwIvBvSMxqWNVPrXwDa8PtRV8/view?usp=sharing

---

## 📎 Reference
Live Demo: https://drive.google.com/file/d/1PuFZGCFAKbx0E_7Cw2mRc_4jybtlwQYM/view?usp=sharing
