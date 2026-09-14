# TBH-CLI v1.2 - Bug Bounty System

<p align="center">
  <img src="https://img.shields.io/badge/CLI-Bug%20Bounty-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/Version-v1.2-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Tools-5%20in%201-green?style=for-the-badge">
</p>

> **Versi CLI dengan Bug Bounty System** - 5 tools dalam 1 menu.

## ✨ Features Bug Bounty
1. **Headers** - Missing CSP/HSTS (Low)
2. **Ports** - OPEN 80,443,8080 (Info)
3. **Subdomains** - www,api,admin,test
4. **Dirs** - .env/.git/admin (High)
5. **XSS** - Reflected `<svg/onload=alert(1)>` (High)

## 📦 Install
```bash
pkg update && pkg install python git
git clone https://github.com/TulungagungBlackHat/TBH-CLI
cd TBH-CLI
pip install requests
```

## 🚀 Cara Jalanin

### Menu (Gampang)
```bash
python3 tbh
```
Pilih:
```
Bug Bounty System:
 1. Scan Bug Bounty (All 5)
 2. Scan Cepat (Headers+Ports)
 3. Bantuan
 0. Keluar
Pilih [1/2/3/0]: 1
URL: https://example.com
```

### Command
```bash
python3 tbh -u https://example.com
```

## 📸 Contoh
```
[*] Bug Bounty Scan: example.com (104.20.23.154)
[1] Headers -> Missing CSP
[2] Ports -> OPEN 80,443,8080
[3] Subdomains -> FOUND www.example.com
[4] Dirs -> NOT 404
[5] XSS -> tidak reflected
[✓] Bug Bounty CLI Selesai
```

## 👥 TBH
uchil404 - Tulungagung Black Hat - Always Smile :)

## 📄 License
MIT
