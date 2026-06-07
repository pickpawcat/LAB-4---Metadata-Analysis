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
<img width="931" height="763" alt="574215555-710dbfed-cb33-43a3-bd63-0b20a2fecdf5" src="https://github.com/user-attachments/assets/7cfa1bef-3905-4b25-aeb4-ab11feda58fd" />


