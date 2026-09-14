# TBH-CLI - Pure CLI Version (Menu + Command)

<p align="center">
  <img src="https://img.shields.io/badge/CLI-Pure-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Menu%20%2B%20Command-v1.1-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Termux-Ready-orange?style=for-the-badge">
</p>

> **Versi CLI saja** - Ringan, hanya terminal, tanpa JSON/HTML. Bisa pakai **menu interaktif** atau **command langsung**.

## ✨ Features CLI
- 🔍 **Headers** - Cek missing CSP/HSTS
- 🚪 **Ports** - Cek OPEN/CLOSED 80,443,8080
- 💻 **Pure Terminal** - Warna, tanpa file output
- 📱 **Menu + Command** - 2 cara jalanin

## 📦 Install (Termux / Kali / Linux)

**Langkah 1 - Install Python & Git:**
```bash
pkg update && pkg upgrade
pkg install python git
```

**Langkah 2 - Clone Repo:**
```bash
git clone https://github.com/TulungagungBlackHat/TBH-CLI
cd TBH-CLI
```

**Langkah 3 - Install Dependency:**
```bash
pip install requests
# atau: pip install -r requirements.txt (jika ada)
```

## 🚀 Cara Jalanin (2 Cara)

### Cara 1 - Menu Interaktif (Paling Gampang, Tanpa Hafal Command)
```bash
python3 tbh
```
Nanti muncul:
```
Pilih mode:
 1. Scan URL (ketik URL)
 2. Bantuan
 0. Keluar
Pilih [1/2/0]: 1
Masukkan URL (ex: https://example.com): https://example.com
```
Langsung scan, output di terminal.

### Cara 2 - Command Langsung (Untuk yang sudah hafal)
```bash
python3 tbh -u https://example.com
```
Atau pakai `./`:
```bash
chmod +x tbh
./tbh -u https://example.com
```

### Bantuan
```bash
python3 tbh -h
```

## 📸 Contoh Output
```
TBH-CLI v1.1 - Menu + Command
[*] example.com (172.66.147.243) | 2026-09-14 23:22
[!] Headers Missing: ['Content-Security-Policy']
    Status: 200 Server: cloudflare
OPEN 80
OPEN 443
OPEN 8080
[✓] CLI Scan Selesai
```

## vs AllScan
| | **TBH-CLI** | **TBH-AllScan** |
|---|---|---|
| **Cocok untuk** | Cek cepat, ringan | Laporan lengkap bug bounty |
| **Tools** | 2 (Headers, Ports) | 10 (Headers, SSL, Ports, dll) |
| **Output** | Terminal saja | JSON + HTML + Fix script |
| **Cara** | Menu + Command | Command `python3 allscan.py -u ...` |

## 🛠️ Troubleshooting
- `ModuleNotFoundError: requests` → `pip install requests`
- `Cannot resolve` → cek internet & URL

## 👥 TBH
- **uchil404 | Tulungagung Black Hat** - Always Smile :)
- GitHub: https://github.com/TulungagungBlackHat
- Portfolio: https://tulungagungblackhat.github.io

## 📄 License
MIT - Educational Only
