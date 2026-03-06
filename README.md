# 🛡️ ExoShade's Nuclei Arsenal (11/11)

Welcome to the official **ExoShade** custom Nuclei template collection. This repository contains high-precision templates engineered for vulnerability discovery and automated reconnaissance.

---

## 🚀 Arsenal Overview

This collection focuses on 11 critical attack vectors optimized for Bug Bounty hunting and professional Penetration Testing.

| ID | Template Name | Primary Objective | Severity |
|:---|:---|:---|:---|
| 1 | `sqli-check` | Error-based & Boolean SQL Injections | **Critical** |
| 2 | `auth-bypass` | Login Form Bypass (Admin/User) | **High** |
| 3 | `idor-check` | Unauthorized Data Access via ID Manipulation | **High** |
| 4 | `xss-fuzz` | Reflected XSS (Context-aware) | **High** |
| 5 | `sensitive-files` | `.env`, `.git`, `.htaccess` & Config Exposure | **High** |
| 6 | `exposed-backups` | SQL Dumps, ZIP Archives & Backup Scripts | **High** |
| 7 | `ssti-polyglot` | Server-Side Template Injection (RCE) | **Critical** |
| 8 | `admin-panel` | Discovering Hidden Admin Entry Points | **Medium** |
| 9 | `debug-leak` | PHP/Python Stack Trace & Debug Leakage | **Medium** |
| 10 | `open-redirect` | Phishing Vectors via URL Parameters | **Medium** |
| 11 | `cors-misconfig` | Insecure CORS (Credential Reflection) | **Medium** |

---

## 🛠️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/exoshade-arch/nuclei-templates.git](https://github.com/exoshade-arch/nuclei-templates.git)
   cd nuclei-templates

## 🛠️ Validation:
**Verify that all templates are correctly formatted:**
```bash
nuclei -t . -validate

## ⚔️ Usage Guide
**Scan a single target using the entire arsenal:**
```bash
nuclei -u [https://target.com](https://target.com) -t . -v

nuclei -l targets.txt -t . -o results_exoshade.txt

nuclei -u [https://target.com](https://target.com) -t . -severity critical,high

## 🛡️ Security Disclaimer
 This arsenal is provided for educational purposes and authorized security testing only. ExoShade (exoshade-arch) is not responsible for   any misuse or damage caused by these templates on unauthorized systems.

 Happy Hacking! 💻🔥
