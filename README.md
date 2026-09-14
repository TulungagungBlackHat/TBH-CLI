# TBH-CLI v1.4 - Bug Bounty 10 Tools Full

<p align="center">
  <img src="https://img.shields.io/badge/CLI-Bug%20Bounty%2010%20Tools-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/Version-v1.4-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/AllScan-Equivalent-green?style=for-the-badge">
</p>

> **Full 10 Tools** sama kayak AllScan, tapi **pure CLI** tanpa JSON/HTML.

## ✨ Features 10 Tools
1. Headers 2. Ports 3. Subdomains 4. Dirs 5. XSS 6. OpenRedirect 7. CORS 8. SQLi 9. SSRF 10. LFI

## 📦 Install
```bash
pkg update && pkg install python git
git clone https://github.com/TulungagungBlackHat/TBH-CLI
cd TBH-CLI
pip install requests
```

## 🚀 Cara Jalanin

### Menu
```bash
python3 tbh
# Pilih 1. Scan All 10 Tools -> Masukkan URL
```

### Command
```bash
python3 tbh -u https://example.com
```

## 📸 Contoh
```
[*] Bug Bounty 10 Tools: example.com (172.66.147.243)
[1] Headers -> Missing CSP
[2] Ports -> OPEN 80,443,8080
[3] Subdomains -> FOUND www.example.com
[4] Dirs -> NOT 404
[5] XSS -> tidak reflected
[6] OpenRedirect -> tidak vulnerable
[7] CORS -> OK
[8] SQLi -> tidak terdeteksi
[9] SSRF -> tidak terdeteksi
[10] LFI -> tidak terdeteksi
[✓] Bug Bounty CLI 10 Tools Selesai
```

## 👥 TBH
uchil404 - Tulungagung Black Hat
