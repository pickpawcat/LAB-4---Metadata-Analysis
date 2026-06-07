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
