# 🦉 OCarve

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OForensics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-2.0-cyan?style=flat-square"/>
</p>

> **OCarve** — File Carving Suite

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OCarve is a file-carving suite that recovers embedded files from binaries, disk images, memory dumps and network captures. It streams data in chunks with mmap to carve files larger than RAM, deduplicates recovered objects by SHA-256 and parses GPT partition tables and EXT2/3/4 superblocks. Deep validators for PE and ELF, archive integrity checks and metadata extraction improve carving accuracy, with HTML reporting and a configurable output directory.

---

## ✨ Features

- Carves JPEG/PNG/PDF/ZIP/EXE/ELF/Office/video/audio from many source types
- Chunked streaming via mmap to carve files larger than RAM
- SHA-256 deduplication to skip identical carved files
- GPT partition table and EXT2/3/4 superblock detection
- Encrypted-volume (LUKS/VeraCrypt/BitLocker) detection and PE/ELF deep validation
- Metadata extraction, extended IOC patterns and HTML report export

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OCarve
./OCarve -o ./carved/
./OCarve --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
