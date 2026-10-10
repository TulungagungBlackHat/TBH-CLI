# TBH-CLI

<p align="center">
  <a href="https://github.com/TulungagungBlackHat/TBH-CLI/actions/workflows/ci.yml"><img src="https://github.com/TulungagungBlackHat/TBH-CLI/actions/workflows/ci.yml/badge.svg" alt="CI"></a>
  <img src="https://img.shields.io/badge/license-MIT-red.svg" alt="License">
  <img src="https://img.shields.io/badge/python-3.8%2B-blue.svg" alt="Python">
  <img src="https://img.shields.io/badge/modules-31-orange.svg" alt="Modules">
</p>

Terminal-only bug bounty menu with **31 security check modules** — no JSON files, no HTML reports, no dependencies beyond `requests`. Built for fast interactive hunting on Termux.

Part of the [Tulungagung Black Hat](https://github.com/TulungagungBlackHat) toolset.

## Modules

Recon: headers, ports, subdomains, directories, host info, backup files, 4xx bypass, tech/proxy detection

Web checks: XSS, open redirect, CORS, SQLi, SSRF, LFI, SSTI, IDOR, XXE, CRLF, clickjacking, CSRF, command injection, LDAP injection, XPath injection, HTTP parameter pollution, WebSocket, GraphQL, file upload, JWT, cache poisoning, subdomain takeover

## Install

```bash
git clone https://github.com/TulungagungBlackHat/TBH-CLI
cd TBH-CLI
python3 tbh --help
```

Single file (`tbh`), no `pip install` needed.

## Usage

**Interactive menu** — pick modules by number:

```bash
python3 tbh
```

**Direct command:**

```bash
python3 tbh -u https://example.com
```

## vs TBH-AllScan

| | **TBH-CLI** | [**TBH-AllScan**](https://github.com/TulungagungBlackHat/TBH-AllScan) |
|---|---|---|
| Modules | 31, terminal output only | 10, JSON + HTML reports |
| Best for | Interactive hunting | Report generation & submissions |

Need reports for a submission? Use AllScan. Need speed and volume while hunting? Use CLI.

## Authorized Use Only

Only against scopes you own or are authorized to test. Many modules send active probes — stay inside program rules. See [SECURITY.md](SECURITY.md).

## License

[MIT](LICENSE) — Tulungagung Black Hat, East Java, Indonesia. Always Smile :)
