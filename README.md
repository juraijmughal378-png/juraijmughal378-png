<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=RECON%20TOOLKIT&fontSize=60&fontColor=ffffff&animation=twinkling&fontAlignY=38&desc=Automated%20OSINT%20%26%20Attack%20Surface%20Intelligence%20Platform%20v3.0&descSize=18&descAlignY=60&descColor=ffffff"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Version-3.0.0-C0392B?style=for-the-badge&logo=github&logoColor=white"/>
  <img src="https://img.shields.io/badge/Platform-Kali%20Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white"/>
  <img src="https://img.shields.io/badge/License-MIT-27AE60?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Modules-10-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge"/>
</p>
<p align="center">
  <img src="https://img.shields.io/github/stars/juraijmughal378-png/recon-toolkit?style=social"/>
  &nbsp;
  <img src="https://img.shields.io/github/forks/juraijmughal378-png/recon-toolkit?style=social"/>
</p>
██████╗ ███████╗ ██████╗ ██████╗ ███╗   ██╗    ████████╗ ██████╗  ██████╗ ██╗
██╔══██╗██╔════╝██╔════╝██╔═══██╗████╗  ██║       ██╔══╝██╔═══██╗██╔═══██╗██║
██████╔╝█████╗  ██║     ██║   ██║██╔██╗ ██║       ██║   ██║   ██║██║   ██║██║
██╔══██╗██╔══╝  ██║     ██║   ██║██║╚██╗██║       ██║   ██║   ██║██║   ██║██║
██║  ██║███████╗╚██████╗╚██████╔╝██║ ╚████║       ██║   ╚██████╔╝╚██████╔╝███████╗
╚═╝  ╚═╝╚══════╝ ╚═════╝ ╚═════╝ ╚═╝  ╚═══╝       ╚═╝    ╚═════╝  ╚═════╝ ╚══════╝
                                                               v3.0 — 10 Modules
<p align="center">
  <b>🔴 10-Module Automated OSINT & Attack Surface Intelligence Framework</b><br/>
  <i>Built for ethical hackers, red teamers & security researchers</i>
</p>
<p align="center">
  <a href="#-overview">📌 Overview</a> •
  <a href="#-modules">⚡ Modules</a> •
  <a href="#-installation">🚀 Install</a> •
  <a href="#-usage">📖 Usage</a> •
  <a href="#-output">📊 Output</a> •
  <a href="#️-project-structure">🗂️ Structure</a> •
  <a href="#️-roadmap">🗺️ Roadmap</a> •
  <a href="#-author">👨‍💻 Author</a>
</p>

📌 Overview
Recon Toolkit v3.0 is a modular, multi-threaded Python reconnaissance framework built for the information gathering phase of authorized penetration tests.
With 10 independent modules, an interactive terminal menu, and CLI support, it automates the full recon pipeline — from passive OSINT and subdomain enumeration to CVE correlation and SSL analysis — and outputs clean HTML, JSON, and Markdown reports.

🎓 Built during the Cyberster Red Team Internship (CSI-B1-617) as a hands-on offensive security project.

bash# Just run it — interactive menu appears!
python3 main.py

📸 Screenshots
Interactive Terminal Menu
Show Image
HTML Visual Report
Show Image

⚡ Modules

v3.0 ships with 10 modules — 3 more than the previous release.

#ModuleKey Capabilities1🔍 Subdomain Enumerationcrt.sh passive recon, multi-threaded DNS brute-force, auto IP resolution, subdomain takeover detection2🔌 Port ScannerTCP connect scan (100+ ports), service & banner grabbing, risk classification, configurable threads & timeout3🌐 WHOIS & DNS IntelligenceFull DNS records (A/MX/NS/TXT), WHOIS data, reverse DNS, IP geolocation (country, ISP, org)4🎯 Google Dork Generator30+ dorks across 7 categories — admin panels, sensitive files, credentials, API key exposure5🛡️ WAF DetectionFingerprints 12+ WAF vendors (Cloudflare, AWS, Akamai, Imperva), header/cookie/body analysis, payload triggering6📧 Email HarvesterPage scraping, DNS TXT/MX analysis, email pattern prediction, false-positive filtering7🔎 Shodan IntegrationIP intelligence via Shodan API, exposed services, CVE listing, OS fingerprinting8🧬 Technology Fingerprinting ⭐ NEWDetects frameworks, CMS, servers, JS libraries from headers & response body9🔐 SSL/TLS Analyzer ⭐ NEWCertificate info, expiry, cipher suites, TLS version, misconfiguration detection10💀 CVE Correlator ⭐ NEWCorrelates detected banners & technologies against known CVEs for instant vuln intelligence88⚡ Full ScanRuns all 10 modules sequentially99🎯 Custom ScanPick any combination: 1,3,5 or 1-5 ranges

📄 Triple Report Generator
Every scan auto-generates 3 report formats:
FormatUse Case📄 MarkdownTerminal-friendly, paste into reports🗃️ JSONRaw structured data for automation & pipelines🌐 HTMLDark-theme visual report — open in browser

🚀 Installation
bash# 1. Clone the repo
git clone https://github.com/juraijmughal378-png/recon-toolkit.git
cd recon-toolkit

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run!
python3 main.py

Recommended OS: Kali Linux / Parrot OS / Ubuntu
Python: 3.8+


📖 Usage
Interactive Menu
╔══════════════════════════════════════════════════════════════╗
║           RECON TOOLKIT v3.0  —  SELECT MODULE              ║
╠══════════════════════════════════════════════════════════════╣
║  [1]   🔍  Subdomain Enumeration + Takeover Detection        ║
║  [2]   🔌  Advanced Port Scanner                             ║
║  [3]   🌐  WHOIS & DNS Intelligence                          ║
║  [4]   🎯  Google Dork Generator                             ║
║  [5]   🛡️   WAF & Firewall Detection                          ║
║  [6]   📧  Email Harvesting                                   ║
║  [7]   🔎  Shodan Intelligence                                ║
║  [8]   🧬  Technology Fingerprinting          ← NEW v3.0     ║
║  [9]   🔐  SSL/TLS Analyzer                   ← NEW v3.0     ║
║  [10]  💀  CVE Correlation & Vuln Intelligence ← NEW v3.0    ║
║                                                              ║
║  [88]  ⚡  Full Scan  (All 10 Modules)                       ║
║  [99]  🎯  Custom Scan (Pick your modules)                   ║
║  [0]   ❌  Exit                                              ║
╚══════════════════════════════════════════════════════════════╝
  Enter choice [0-99]:
CLI Mode (Advanced)
bash# Full scan
python3 main.py --target example.com --full

# Combo scans
python3 main.py --target example.com --waf --ports --ssl
python3 main.py --target example.com --subdomains --emails --shodan

# With Shodan API key
python3 main.py --target example.com --full --shodan-key YOUR_API_KEY
FlagDescription--targetTarget domain or IP--fullRun all 10 modules--subdomainsSubdomain enumeration + takeover check--portsPort scanning--whoisWHOIS & DNS--dorksGoogle dorks--wafWAF detection--emailsEmail harvesting--shodanShodan lookup--techTechnology fingerprinting--sslSSL/TLS analysis--cveCVE correlation--shodan-keyShodan API key

📊 Output
reports/
├── example.com_20260517_140210.md      ← Markdown report
├── example.com_20260517_140210.json    ← Raw JSON (automation-ready)
└── example.com_20260517_140210.html    ← Visual HTML ← Open in browser!

🗂️ Project Structure
recon-toolkit/
│
├── 📄 main.py                    ← CLI entry point + Interactive Menu
├── 📄 requirements.txt
├── 📄 README.md
│
├── 📁 modules/
│   ├── 🐍 subdomain.py           ← crt.sh + DNS brute-force + takeover check
│   ├── 🐍 portscan.py            ← TCP scanner + banner grab
│   ├── 🐍 whois_info.py          ← WHOIS + DNS + GeoIP
│   ├── 🐍 dorking.py             ← Google dork generator (30+ dorks)
│   ├── 🐍 waf_detect.py          ← WAF fingerprinting (12+ vendors)
│   ├── 🐍 email_harvest.py       ← Email harvester
│   ├── 🐍 shodan_lookup.py       ← Shodan API integration
│   ├── 🐍 fingerprint.py         ← Technology fingerprinting ⭐ NEW
│   ├── 🐍 ssl_scan.py            ← SSL/TLS analyzer ⭐ NEW
│   ├── 🐍 cve_check.py           ← CVE correlator ⭐ NEW
│   └── 🐍 banner.py              ← ASCII banner
│
├── 📁 ui/
│   └── 🐍 rich_ui.py             ← Rich terminal UI (menus, colors, progress)
│
├── 📁 reports/
│   ├── 🐍 report_gen.py          ← HTML + JSON + Markdown generator
│   └── 📄 sample_report.md       ← Real scan output sample
│
├── 📁 wordlists/
│   └── 📄 subdomains.txt         ← DNS brute-force wordlist
│
└── 📁 screenshots/
    ├── 🖼️  terminal_scan.png
    └── 🖼️  html_report.png

📁 Sample Report
👉 View Sample Scan Report
Real scan against scanme.nmap.org — Nmap's official authorized test target

🗺️ Roadmap
✅ Completed — v3.0

 Subdomain enumeration + takeover detection
 Port scanner + banner grabbing
 WHOIS & DNS + GeoIP
 Google dork generator (30+ dorks)
 WAF detection (12+ vendors)
 Email harvesting
 Shodan API integration
 HTML visual dark-theme report
 Interactive terminal menu (Rich UI)
 Technology fingerprinting
 SSL/TLS analysis
 CVE correlation engine

🔜 Coming — v4.0

 Nuclei template integration
 Slack / Discord webhook alerts
 Docker support
 GitHub Actions CI workflow
 Web UI dashboard


⚠️ Disclaimer

Strictly for authorized security research, CTF competitions, and penetration testing where explicit written permission has been granted. Unauthorized use against systems you do not own or have permission to test is illegal. The author takes no responsibility for misuse of this tool.

🔴 Always hack ethically. Always get written permission first.

👨‍💻 Author
🎓 InternshipCyberster Red Team Internship — CSI-B1-617🔴 TrackRed Team / Offensive Security🌐 GitHub@juraijmughal378-png💼 LinkedInJuraij Sadaqat📧 Emailjuraijmughal378@gmail.com🌍 Portfoliojuraij-cyber-portfolio
<p align="center">
  <a href="https://github.com/juraijmughal378-png">
    <img src="https://img.shields.io/badge/GitHub-juraijmughal378--png-181717?style=for-the-badge&logo=github"/>
  </a>
  <a href="https://linkedin.com/in/juraij-sadaqat-b92a4939a">
    <img src="https://img.shields.io/badge/LinkedIn-Juraij_Sadaqat-0077B5?style=for-the-badge&logo=linkedin"/>
  </a>
</p>
<p align="center"><i>🔍 Open to: Cybersecurity Internships · Junior Pentester Roles · Bug Bounty</i></p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer"/>
</p>
<p align="center">
  <b>⭐ Star this repo if it helped you!</b> &nbsp;|&nbsp; <b>🍴 Fork it and build on top!</b>
</p>
