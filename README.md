# file-organizer
<h1 align="center">🗂️ File Organizer</h1>

<p align="center">
  <i>Messy folder? One command, and everything finds its place.</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Dependencies-None-success?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" />
</p>

---

## ✨ Features

- 🔍 Sorts files by extension into **Images, Documents, Audio, Videos, Archives, Scripts**
- 🛡️ **Never overwrites**: duplicate names become `file_1.png`, `file_2.png`
- 👀 **Dry-run mode** to preview changes before moving anything
- 🎨 Clean, colorful terminal output with a summary
- 📦 Zero dependencies, only `os`, `shutil` and `sys`

## 🚀 Usage

```bash
# organize the current folder
python organizer.py

# organize a specific folder
python organizer.py ~/Downloads

# preview only (nothing moves)
python organizer.py ~/Downloads --dry-run
```

## 🪄 Before → After

```text
📁 Downloads/                      📁 Downloads/
├── resume.pdf                     ├── 🖼️ Images/
├── photo.png                      │   └── photo.png
├── song.mp3               →       ├── 📄 Documents/
├── notes.txt                      │   ├── resume.pdf
├── movie.mp4                      │   └── notes.txt
└── backup.zip                     ├── 🎵 Audio/
                                   │   └── song.mp3
                                   ├── 🎬 Videos/
                                   │   └── movie.mp4
                                   └── 📦 Archives/
                                       └── backup.zip
```

## 🛠️ Customize

Add or edit categories in the `FILE_TYPES` dictionary at the top of `organizer.py`:

```python
FILE_TYPES = {
    "Images": [".jpg", ".png", ".webp"],
    "Ebooks": [".epub", ".mobi"],   # add your own!
}
```

## 🗺️ Roadmap

- [ ] `Others/` folder for unknown extensions
- [ ] Undo last run
- [ ] Sort by date option

## 👨‍💻 Author

**Vishal Tomar**
[LinkedIn](https://linkedin.com/in/vishal-tomar-34b640311) · [GitHub](https://github.com/vishalltomar)

<p align="center">⭐ If you found this useful, give it a star!</p>
