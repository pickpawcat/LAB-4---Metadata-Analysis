#LAB4
# 📌Metadata Analysis Report

---

 🧭 Target Information
| Field        | Value            | 
|--------------|----------------------|
|Name          |  Metadata Analysis  | 
|Tools Used   |   exiftool, hexeditor, binwalk, strings, file     |
|Files Analyzed | ocean.jpg, computer.jpg, dog.jpg, solitaire.exe, rubiks.jpg|

---

## 🔍 Task 1 - oceann.jpg  

Tools: exiftool

Using kali linux:

Command:
```bash
exiftool -a -u -G1 -s -n ocean.jpg
```
✅ Result

<img width="931" height="763" alt="image" src="https://github.com/user-attachments/assets/710dbfed-cb33-43a3-bd63-0b20a2fecdf5" />

---
 Find Flag:
 
Command:
```bash
exiftool -a -u -G1 -s -n ocean.jpg | grep -i "flag\|ctf\|hint\|secret"
```
✅ Result

<img width="805" height="82" alt="image" src="https://github.com/user-attachments/assets/a00439ad-b3f3-47f4-8805-345d061554fd" />

---
Using online tools:

Command:
```bash
https://exif.tools/
```

✅ Result

<img width="922" height="682" alt="image" src="https://github.com/user-attachments/assets/425034c6-2299-43e4-ba17-7e018c3954f4" />
---

## 🔍Task 2 - computer.jpg 

Tools: hexeditor

Using kali linux:

Command:
```bash
hexeditor computer.jpg
```
✅ Result

<img width="931" height="868" alt="image" src="https://github.com/user-attachments/assets/06659976-3359-48d1-aeb9-32c40444cfbc" />

---

Using online tools:

Command:
```bash
https://hexed.it/
```

✅ Result

<img width="1882" height="835" alt="image" src="https://github.com/user-attachments/assets/79e9b13d-a440-4b03-ab0f-b76c43997bb4" />

---

## 🔍Task 3: dog.jpg 

Tools: binwalk

Using kali linux:

Command:
```bash
binwalk dog.jpg
binwalk -e dog.jpg
cd _dog.jpg.extracted/
cat hidden_text.txt
```

✅ Result

<img width="945" height="526" alt="image" src="https://github.com/user-attachments/assets/adee960d-572e-4602-99e8-d55865976df5" />

---

## 🔍Task 4: computer.jpg

Tools: binwalk

Using kali linux:

Command:
```bash
strings computer.jpg
```

✅ Result

<img width="937" height="736" alt="image" src="https://github.com/user-attachments/assets/d0e3a09f-93ee-45e9-861e-032dc834256a" />

---
Using online tools:

Command:
```bash
https://www.dcode.fr/strings-extractor
```

✅ Result

<img width="700" height="438" alt="image" src="https://github.com/user-attachments/assets/873d0c08-6f74-40f7-a73b-5b6a14c97800" />

Findings:

| String        | Meaning                         |
|---------------|----------------------------------|
| JFIF          | JPEG file format confirmed       |
| ICC_PROFILE   | Color profile embedded           |
| lcms          | Little CMS color management      |
| mntr          | RGB XYZ RGB color space info     |

---
## 🔍Task 5- solitaire.exe 

Tools:
file

Command:
```bash
file solitaire.exe
```
✅ Result:

<img width="678" height="73" alt="image" src="https://github.com/user-attachments/assets/15579c8f-5a6f-46fb-ba45-714190037d67" />

---

## 🔍Task 6- rubiks.jpg 

Tools:
file

Command:
```bash
file rubiks.jpg
```

✅ Result:

<img width="748" height="73" alt="image" src="https://github.com/user-attachments/assets/87b5a01b-a35a-4ef9-8983-950b2484cde6" />

