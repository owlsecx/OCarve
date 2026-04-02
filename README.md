# 🪓 OCarve

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-OForensics%20%2F%20File%20Carving-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-None%20(Standalone)-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v1.0-cyan?style=flat-square"/>
</p>

> **OCarve** is a powerful file carving tool. It recovers deleted, hidden, or fragmented files from raw binary data, disk images, memory dumps, and forensic evidence using signature-based carving (header/footer, header+max, header+size).

---

## 📌 Overview

OCarve scans any binary stream for over 50 file types including images (JPEG, PNG, GIF), documents (PDF, DOCX, RTF), archives (ZIP, RAR, GZIP), executables (EXE, ELF, Mach-O), media (MP3, MP4, AVI, MKV), databases (SQLite), scripts, certificates, and more.

It supports three carving methods:
- **Header + Footer** (most accurate)
- **Header + Max Size**
- **Header + Embedded Size Field**

---

## 🖥️ Modules

| # | Module                        | Description |
|---|-------------------------------|-------------|
| **[1]** | **Auto Carve**                | Carve all supported file types automatically |
| **[2]** | **Selective Carve**           | Choose specific categories to carve |
| **[3]** | **Deep Scan**                 | Full signature scan + carving |
| **[4]** | **Disk Image Analyzer**       | MBR, FAT, NTFS detection + carving |
| **[5]** | **String Harvest**            | Extract ASCII, UTF-8, UTF-16LE strings + IOCs |
| **[6]** | **Entropy Map**               | Visualize file structure with entropy blocks |
| **[7]** | **Signature Scanner**         | Detect all embedded signatures |
| **[8]** | **Fragment Recovery**         | Recover partial/truncated files |

---

## 📊 Key Features

- **50+ File Signatures** — JPEG, PNG, PDF, ZIP, EXE, ELF, MP4, SQLite, PEM keys, etc.
- **Three Carving Methods** — Header-Footer, Header-Max, Header-Size
- **Entropy Analysis** — Detects encrypted/packed regions
- **IOC Extraction** — URLs, IPs, emails, paths, secrets, hashes, registry keys
- **Disk Image Support** — MBR, FAT32, NTFS detection
- **String Harvesting** — ASCII, UTF-8, UTF-16LE with minimum length filter
- **Fragment Recovery** — Handles incomplete or truncated files
- **Detailed Reports** — JSON export with offsets, sizes, entropy, hashes

---

## ⚙️ Requirements

- **Linux or Windows**
- **No additional dependencies** — pure Python with standard library

---

## 🚀 Usage

```bash
./OCarve

📁 Output

Carved Files — Saved to ocarve_*/ folders with numbered names
Rich Terminal Reports — Colored findings, entropy map, signature hits
JSON Export — Complete forensic report with offsets, entropy, hashes
Entropy Map — Visual representation of high/low entropy regions


📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.

AUTHORISED FORENSIC ANALYSIS & DATA RECOVERY USE ONLY
