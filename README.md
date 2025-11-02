# MP3Tag-Reader_Editor
<!-- Stylish Header -->
<h1 align="center">🎶 MP3 Tag Reader & Editor in C</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Language-C-blue.svg" alt="Language"/>
  <img src="https://img.shields.io/badge/Concept-File Handling-yellow.svg" alt="File Handling"/>
  <img src="https://img.shields.io/badge/Topic-ID3 Tag Reader & Editor-orange.svg" alt="ID3 Tag Reader & Editor"/>
  <img src="https://img.shields.io/badge/IDE-VS Code-lightgrey.svg" alt="IDE"/>
</p>

<p align="center">
  <b>Developed by <a href="https://github.com/Rushikesh0311">Rushikesh Gore</a></b>  
</p>

---

## 🧩 Overview
The **MP3 Tag Reader & Editor** is a C-based mini project designed to **read, view, and modify ID3v2 tags** inside MP3 files.  
It allows you to extract key metadata — such as **Title, Artist, Album, Year, and Genre** — and even **edit or update** this information directly through the terminal.

---

## 📘 Project Description
Each MP3 file contains a header with **ID3 tags**, storing metadata that music players display.  
This project reads these tags using **binary file handling** and provides a simple **menu-driven interface** to display or modify them.  

🔹 **Reader Mode:** Displays all existing MP3 tag details.  
🔹 **Editor Mode:** Allows updating specific tag values safely within the file.

---

## 🌟 Features
✅ Read MP3 ID3v2 metadata (Title, Artist, Album, Year, Genre)  
✅ Edit or update existing tags (Title, Artist, etc.)  
✅ Display metadata in a clean, formatted output  
✅ Works on both Linux and Windows  
✅ Simple, menu-driven interface  
✅ Modular and easy-to-understand code  

---

## 📂 File Structure
```
MP3TagReader/
│
├── mp3_tag_reader.c       # Main source code file
├── sample.mp3             # Sample MP3 file for testing
├── README.md              # Project documentation
└── assets/                # Screenshots or demo images
```

---

## 🗂️ Understanding ID3 Tags
An MP3 file starts with a **10-byte ID3v2 header**, followed by frames that hold metadata.  
Each frame has a specific identifier for a data type.

| Frame ID | Description | Example |
|-----------|--------------|----------|
| TIT2 | Title | Shape of You |
| TPE1 | Artist | Ed Sheeran |
| TALB | Album | ÷ (Divide) |
| TDRC | Year | 2017 |
| TCON | Genre | Pop |

---

## ⚙️ Build and Run
### ▶️ Compile the Program
```bash
gcc mp3_tag_reader.c -o mp3editor
```

### ▶️ Run the Executable
```bash
./mp3editor sample.mp3
```

---

## 🖥️ Demo Outputs

### 🎧 **1. Read MP3 Tag Details**
```bash
========= MP3 TAG READER =========
Title : Shape of You
Artist: Ed Sheeran
Album : Divide
Year  : 2017
Genre : Pop
==================================
```

### ✏️ **2. Edit MP3 Tag Example**
```bash
========= MP3 TAG EDITOR =========
Enter the tag you want to edit:
1. Title
2. Artist
3. Album
4. Year
5. Genre
----------------------------------
Enter your choice: 1
Enter new Title: Perfect
----------------------------------
✅ Title updated successfully!

========= UPDATED TAG INFO =========
Title : Perfect
Artist: Ed Sheeran
Album : Divide
Year  : 2017
Genre : Pop
====================================
```

---

## 💡 Ideal For
- Students learning **File Handling in C**
- Mini projects for **College or Internship Submissions**
- Understanding **binary data parsing**
- Beginners exploring **media file structures**

---

## 🧠 Key Concepts Used
- **Binary File I/O:** `fopen`, `fread`, `fseek`, `fclose`  
- **Structures:** Used for storing tag data cleanly  
- **String Manipulation:** Handling text-based tag fields  
- **Menu-driven Interface:** Interactive program control  

---

## 🧰 Tools & Environment
- **Language:** C  
- **Compiler:** GCC  
- **IDE Used:** VS Code / Code::Blocks  
- **OS Tested On:** Windows / Linux  

---

## 🔍 Real-World Applications
- 🎵 Used in **music players** and **MP3 library managers** to display and modify song info  
- 💻 Helps in developing **media management tools** for file organization  
- ☁️ Used in **upload systems** (e.g., music platforms) to auto-read song metadata  

---

## 🚀 Future Enhancements
- Add support for **ID3v1 tag reading (end of file)**  
- Implement **album art (APIC frame)** extraction  
- Add **UTF-16 and multilingual text** support  
- Include a **GUI interface** using C/GTK for advanced editing  

---

## 👨‍💻 Author
**Rushikesh Gore**  
📧 Email: [rushikeshgore0311@gmail.com](mailto:rushikeshgore0311@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/rushikeshgore11) | [GitHub](https://github.com/Rushikesh0311)

---

