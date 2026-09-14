# TBH-CLI v1.3 - Bug Bounty 8 Tools

<p align="center">
  <img src="https://img.shields.io/badge/CLI-Bug%20Bounty%208%20Tools-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/Version-v1.3-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Menu%20%2B%20Command-v1.3-green?style=for-the-badge">
</p>

> **Bug Bounty System 8 Tools** dalam 1 CLI - Menu + Command.

## ✨ Features 8 Tools
1. **Headers** - Missing CSP/HSTS (Low)
2. **Ports** - 80,443,8080 (Info)
3. **Subdomains** - www,api,admin,test
4. **Dirs** - .env/.git/admin (High)
5. **XSS** - Reflected `<svg/onload=alert(1)>` (High)
6. **OpenRedirect** - `?redirect=evil.com` (Medium)
7. **CORS** - `Origin: evil.com` (High)
8. **SQLi** - `' OR '1'='1` (High)

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
# Pilih 1. Scan All 8 Tools -> Masukkan URL
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
[6] OpenRedirect -> tidak vulnerable
[7] CORS -> OK
[8] SQLi -> tidak terdeteksi
[✓] Bug Bounty CLI 8 Tools Selesai
```

## 👥 TBH
uchil404 - Tulungagung Black Hat

## 📄 License
MIT
