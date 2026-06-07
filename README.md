# LAB-4---Metadata-Analysis
# 📌 Metadata Analysis Report

---

### 🧭 Target Information

| Field | Value |
| :--- | :--- |
| **Name** | Metadata Analysis |
| **Tools Used** | exiftool, hexeditor, binwalk, strings, file |
| **Files Analyzed** | ocean.jpg, computer.jpg, dog.jpg, solitaire.exe, rubiks.jpg |

---

## 🔍 Task 1 - oceann.jpg

**Tools:** exiftool  
**Using:** Kali Linux  

**Command:**
```bash
exiftool -a -u -G1 -s -n ocean.jpg

RESULT:
<img width="931" height="763" alt="image" src="https://github.com/user-attachments/assets/cd763275-b529-4c65-aae5-ea167d0ec730" />

## 🕵️‍♂️ Task 1.1 - Flag Discovery

**Analysis Strategy:**  
Utilize command-line piping and case-insensitive filtering to target specific keywords embedded within the image metadata.

**Command Syntax:**
```bash
exiftool -a -u -G1 -s -n ocean.jpg | grep -i "flag\|ctf\|hint\|secret"
