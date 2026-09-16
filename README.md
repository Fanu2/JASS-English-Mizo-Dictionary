<img width="1902" height="925" alt="image" src="https://github.com/user-attachments/assets/a865dab1-8631-4e30-a179-bb18d3223aca" />

<img width="1902" height="925" alt="image" src="https://github.com/user-attachments/assets/cd0131a4-d10b-4174-a5ae-ba0028cd6814" />

# JASS English–Mizo Dictionary Pro

A beautiful, fast, offline desktop dictionary built with **Python + PySide6**, designed for English–Mizo language lookup and local dictionary management.

The application converts dictionary source material into a searchable **SQLite + FTS5** database and provides a modern dictionary-style interface for everyday use.

## ✨ Features

### 🔎 Powerful Dictionary Search

- English → Mizo lookup
- Mizo → English search
- Smart lookup
- Exact English search
- English prefix / starts-with search
- Full-text search
- Fuzzy spelling suggestions
- Fast local SQLite/FTS5 searching
- Multiple results for words with different parts of speech or meanings

### 📖 Dictionary Entry Display

Each entry can display:

- English headword
- Pronunciation
- Part of speech
- Mizo definition
- Book page
- Scan page
- OCR confidence
- Original source information

The application keeps source/provenance information so entries can be checked against the original material.

### ⭐ Personal Dictionary Tools

- Favorites
- Search history
- A–Z dictionary browser
- Random Word
- Copy definition
- Adjustable definition text size
- Previous / Next result navigation

### 🎨 Modern User Interface

- Clean dictionary-style layout
- Light theme
- Dark theme
- Responsive two-panel design
- Search suggestions
- Large, readable definition area
- Keyboard shortcuts
- Source information displayed below definitions

### 📚 Source Import

The application supports dictionary source importing from:

- DjVuXML
- TXT
- EPUB
- PDF

For the original English–Mizo source, **DjVuXML is preferred** because it can preserve useful page and OCR information.

PDF importing requires **PyMuPDF**.

DRM-protected books are not supported.

### 💾 Database

The dictionary uses:

- SQLite
- SQLite FTS5 full-text search
- Local database storage
- Favorites/history storage
- Source and page metadata
- OCR confidence information

The current prepared database contains approximately **16,534 dictionary records** extracted from the supplied English–Mizo source.

## 🖥️ Requirements

- Windows, Linux, or another desktop platform supported by PySide6
- Python 3
- PySide6

Optional:

- PyMuPDF — for PDF importing
- `python-docx` — if additional DOCX importing is added in your local version

No GPU is required.

No PyTorch is required.

No cloud service is required.

No internet connection is required for normal dictionary use.

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/JASS-English-Mizo-Dictionary.git
cd JASS-English-Mizo-Dictionary
```

Install the main dependency:

```bash
pip install PySide6
```

For PDF import:

```bash
pip install PyMuPDF
```

Run:

```bash
python jass_english_mizo_dictionary_pro_v2.py
```

Keep the database file in the same directory as the application:

```text
JASS-English-Mizo-Dictionary/
│
├── jass_english_mizo_dictionary_pro_v2.py
├── english_mizo_dictionary.db
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
└── assets/
```

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl + L` | Focus search |
| `Ctrl + O` | Import dictionary source |
| `Ctrl + Shift + R` | Random Word |
| `Ctrl + Shift + C` | Copy definition |
| `Ctrl + D` | Add/remove favorite |
| `Ctrl + +` | Increase text size |
| `Ctrl + -` | Decrease text size |
| `Ctrl + 0` | Reset text size |
| `←` | Previous result |
| `→` | Next result |

## 📂 Recommended Repository Structure

```text
JASS-English-Mizo-Dictionary/
│
├── jass_english_mizo_dictionary_pro_v2.py
├── english_mizo_dictionary.db
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
│
└── assets/
    └── icon.png
```

### Source files

The original downloaded source files such as large EPUB, PDF, DjVuXML, and OCR files do not need to be stored in the Git repository.

For example:

```text
dli.language.0175.epub
dli.language.0175.pdf
dli.language.0175_djvu.txt
dli.language.0175_djvu.xml
```

These should normally remain outside the repository unless redistribution of the particular source material is permitted.

## 📊 Current Dictionary Database

The prepared database was built from the supplied English–Mizo dictionary source material.

Current database characteristics:

- ~16,534 dictionary records
- SQLite database
- FTS5 search index
- English headwords
- Mizo definitions
- Pronunciation information where available
- Parts of speech where detected
- Page information where available
- OCR confidence information where available
- Source attribution

The database is designed to allow future cleaning and enhancement without losing the original source information.

## 🧹 Future Dictionary Improvement

The next development stage can focus on turning the extracted data into a more comprehensive lexical resource.

Possible future improvements:

- Group multiple senses under one headword
- Better part-of-speech classification
- Cleaner pronunciation formatting
- OCR correction workflow
- Verified/corrected entry status
- Example sentences
- Phrases and idioms
- Synonyms
- Antonyms
- Cross-references
- Clickable related words
- English ↔ Mizo reverse lookup
- Better Mizo full-text search
- Source-page viewer
- Audio pronunciation
- User-created dictionary entries
- Import/export of dictionary corrections
- Database backup and restore
- Portable Windows application
- Professional application icon and branding

## 🔐 Offline & Privacy

JASS English–Mizo Dictionary is designed as a **local-first, offline application**.

Normal dictionary searches do not require:

- Internet access
- Cloud APIs
- User accounts
- External AI services
- GPU hardware

Your dictionary database remains on your computer.

## ⚖️ Source Material & Licensing

The application software and the dictionary source/database are separate matters.

Before redistributing the supplied dictionary database or original source material, verify that the applicable copyright and licensing terms permit redistribution.

If redistribution rights for the source-derived database are uncertain, distribute the application/importer separately and instruct users to create their own database from source material they are legally entitled to use.

The repository should clearly state the license that applies to the **software itself**.

## 🛠️ Development Philosophy

The project is intentionally lightweight.

The core dictionary engine does not depend on large AI frameworks. The goal is to provide:

- Fast search
- Low memory usage
- Reliable local storage
- Unicode/Mizo support
- Source traceability
- Simple installation
- Long-term maintainability

## 📌 Project Status

**Current status: Working / Stable Baseline**

The current v2 application is considered a stable foundation for future improvements.

Future development should preferably add features incrementally while preserving:

- Existing database compatibility
- Existing dictionary entries
- Existing search functionality
- Favorites
- History
- Source metadata
- Current UI stability

## ❤️ Project

**JASS English–Mizo Dictionary Pro**

A local dictionary project focused on making English–Mizo language resources easier to search, study, preserve, and use.

---

### Version

**v2 — Stable Baseline**

Built with:

**Python • PySide6 • SQLite • FTS5**
