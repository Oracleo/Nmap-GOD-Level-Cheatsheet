<div align="center">

```
███╗   ██╗███╗   ███╗ █████╗ ██████╗     ███╗   ███╗ █████╗ ███████╗████████╗███████╗██████╗ ██╗   ██╗
████╗  ██║████╗ ████║██╔══██╗██╔══██╗    ████╗ ████║██╔══██╗██╔════╝╚══██╔══╝██╔════╝██╔══██╗╚██╗ ██╔╝
██╔██╗ ██║██╔████╔██║███████║██████╔╝    ██╔████╔██║███████║███████╗   ██║   █████╗  ██████╔╝ ╚████╔╝ 
██║╚██╗██║██║╚██╔╝██║██╔══██║██╔═══╝     ██║╚██╔╝██║██╔══██║╚════██║   ██║   ██╔══╝  ██╔══██╗  ╚██╔╝  
██║ ╚████║██║ ╚═╝ ██║██║  ██║██║         ██║ ╚═╝ ██║██║  ██║███████║   ██║   ███████╗██║  ██║   ██║   
╚═╝  ╚═══╝╚═╝     ╚═╝╚═╝  ╚═╝╚═╝         ╚═╝     ╚═╝╚═╝  ╚═╝╚══════╝   ╚═╝   ╚══════╝╚═╝  ╚═╝   ╚═╝   
```

**God-Level Interactive Reference for SOC Analysts & Penetration Testers**

[![Live Demo](https://img.shields.io/badge/🚀_LIVE_DEMO-View_Cheatsheet-00ff9d?style=for-the-badge&labelColor=050a0f)](https://oracleo.github.io/Nmap-GOD-Level-Cheatsheet/Nmap-GOD-Level-Cheatsheet.html)
[![License](https://img.shields.io/badge/LICENSE-MIT-00d4ff?style=for-the-badge&labelColor=050a0f)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-WELCOME-ff6b35?style=for-the-badge&labelColor=050a0f)](CONTRIBUTING.md)

![nmap](https://img.shields.io/badge/NMAP-7.94-00ff9d?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0iIzAwZmY5ZCIgZD0iTTEyIDJMMiA3bDEwIDUgMTAtNUwxMiAyem0wIDE1bC0xMC01djVsMTAgNSAxMC01di01bC0xMCA1eiIvPjwvc3ZnPg==&labelColor=050a0f)
![SOC](https://img.shields.io/badge/ROLE-SOC_ANALYST-00d4ff?style=flat-square&labelColor=050a0f)
![Pentest](https://img.shields.io/badge/ROLE-PENETRATION_TESTER-ff6b35?style=flat-square&labelColor=050a0f)
![HTML](https://img.shields.io/badge/BUILT_WITH-HTML_·_CSS_·_JS-ffd700?style=flat-square&labelColor=050a0f)

</div>

---

## What Is This?

A **single-file, fully interactive NMAP cheatsheet** built for cybersecurity professionals preparing for SOC analyst, penetration tester, and blue team interviews. No frameworks, no dependencies, no internet required — open the HTML file and it just works.

> *"Most candidates know nmap flags. You know the WHY behind each flag, what TCP handshake state it exploits, how IDS detects it, and how to chain flags for specific scenarios. That's what gets you hired."*

---

## Preview

<div align="center">

| Overview Tab | Scan Types | Interview Scenarios |
|:---:|:---:|:---:|
| Quick-reference flag grid | Deep-dive with TCP logic | 12 real interview combos |

</div>

---

## What's Inside

| Tab | Contents |
|-----|----------|
| **⚡ Overview** | Master quick-reference grid — every flag group at a glance |
| **🔍 Host Discovery** | Ping sweeps, ARP, ICMP, -Pn, -PS/PA — find live hosts first |
| **🔫 Scan Types** | SYN vs TCP Connect vs UDP, Null/FIN/Xmas stealth scans with handshake logic |
| **🎯 Port Selection** | Single ports, ranges, all 65535, UDP+TCP combos, --min-rate tricks |
| **🔬 Version & OS** | -sV, -O, -A, --osscan-guess, version intensity control |
| **📜 NSE Scripts** | EternalBlue, Heartbleed, DNS zone transfer, FTP anon, HTTP enumeration |
| **⏱️ Timing** | -T0 through -T5 explained, --min-rate, --max-rate, parallelism |
| **💾 Output** | -oA as the professional standard, --reason, --packet-trace |
| **🛡️ Firewall Evasion** | Decoys (-D), fragmentation (-f), source port spoofing, MAC spoofing |
| **🎯 Interview Scenarios** | 12 real-world command combos with full explanations of WHY |

---

## Quick Start

**Option 1 — Just open it:**
```bash
git clone https://github.com/Oracleo/Nmap-GOD-Level-Cheatsheet.git
cd nmap-mastery-cheatsheet
open nmap-cheatsheet.html   # macOS
xdg-open nmap-cheatsheet.html  # Linux
```

**Option 2 — Live on GitHub Pages:**

Visit the live demo → **[oracleo.github.io/Nmap-GOD-Level-Cheatsheet](https://oracleo.github.io/Nmap-GOD-Level-Cheatsheet/Nmap-GOD-Level-Cheatsheet.html)**

---

## Commands Covered


```
HOST DISCOVERY    │  SCAN TYPES       │  PORT CONTROL     │  VERSION & OS
──────────────────┼───────────────────┼───────────────────┼──────────────────
-sn  ping sweep   │  -sS  SYN stealth │  -p-  all ports   │  -sV  versions
-Pn  skip ping    │  -sT  TCP connect │  -F   top 100     │  -O   OS detect
-PS  SYN ping     │  -sU  UDP         │  --top-ports N    │  -A   aggressive
-PR  ARP (LAN)    │  -sA  ACK/fw map  │  -p U:,T: combo   │  --version-all
-PE  ICMP echo    │  -sN/F/X stealth  │  --min-rate 5000  │  --osscan-guess

NSE SCRIPTS       │  TIMING           │  EVASION          │  OUTPUT
──────────────────┼───────────────────┼───────────────────┼──────────────────
-sC  defaults     │  -T0  paranoid    │  -f   fragment    │  -oN  normal
--script=vuln     │  -T1  sneaky      │  -D   decoys      │  -oX  XML
smb-vuln-ms17-010 │  -T3  normal      │  --source-port 53 │  -oG  grepable
ssl-heartbleed    │  -T4  aggressive  │  --spoof-mac      │  -oA  all formats
dns-zone-transfer │  -T5  insane      │  --data-length    │  --open  --reason
```


---

## Interview Scenarios Included

Real command combinations you'll be asked to demonstrate:

```bash
# 1. Full port scan, fast (CTF standard)
nmap -p- --min-rate 5000 -T4 10.10.10.5

# 2. Full enumeration after finding open ports
nmap -sV -sC -O -p 22,80,443 -oA full_enum target

# 3. Maximum stealth — evade IDS
nmap -sS -T1 -f -D RND:10 --source-port 53 --data-length 25 target

# 4. Check for EternalBlue (MS17-010)
nmap -p 445 --script=smb-vuln-ms17-010 10.10.10.5

# 5. Scan target that blocks ping
nmap -Pn -sS -p- -T4 target

# 6. SOC incident response triage
nmap -F -sV -T4 --open suspicious_ip -oN ir_triage.txt

# ... 6 more inside the cheatsheet
```

---

## Features

- **🔎 Live Search** — Filter any command, flag, or keyword instantly across all categories
- **📑 Tabbed Navigation** — 9 organized sections, zero clutter
- **🎨 Terminal Aesthetic** — Dark, hacker-themed UI built with pure HTML/CSS/JS
- **📱 Responsive** — Works on desktop and mobile
- **⚡ Zero Dependencies** — Single HTML file, works fully offline
- **🏷️ Severity Badges** — Commands tagged as STEALTH / LOUD / RECON / CRITICAL / PRO
- **💡 Guru Tips** — Contextual interview insights throughout each section

---

## Who Is This For?

```
✅ SOC Analyst candidates preparing for technical interviews
✅ Penetration tester trainees (OSCP, CEH, eJPT prep)
✅ Blue teamers who want to think like red teamers
✅ CTF players (HackTheBox, TryHackMe)
✅ Security engineers needing a quick reference
✅ Anyone learning network reconnaissance fundamentals
```

---

## 🛠️ Tech Stack

| Layer | Choice | Why |
|-------|--------|-----|
| Structure | Pure HTML5 | Zero build step, instant open |
| Styling | CSS3 + Custom Properties | No framework bloat |
| Logic | Vanilla JavaScript | Live search, tab switching |
| Fonts | Google Fonts (Orbitron, Share Tech Mono, Rajdhani) | Terminal aesthetic |
| Hosting | GitHub Pages | Free, fast, permanent URL |

---

## 📂 Repository Structure

```
Nmap-GOD-Level-Cheatsheet/
│
├── Nmap-GOD-Level-Cheatsheet.html    # ← The entire app. One file.
├── README.md                         # ← You are here
└── LICENSE                           # MIT
```

---

## 🤝 Contributing

Found a missing command? Know a better interview answer? PRs are welcome.

```bash
# Fork → Clone → Edit → PR
git clone https://github.com/yourusername/nmap-mastery-cheatsheet.git
```

Open an issue if you want to suggest a new section (e.g., Metasploit integration, masscan comparison, Nmap vs RustScan).

---

## 📜 License

MIT — use it, share it, build on it. Credit appreciated but not required.

---

## 🌐 Connect

If this helped you land a role or pass an interview, I'd love to know.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077b5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dr-niladri-biswas/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Oracleo)

---

<div align="center">

**Built for the security community. Master the tool, master the interview.**

`nmap` · `cybersecurity` · `soc` · `penetration-testing` · `blue-team` · `red-team` · `ctf` · `interview-prep`

</div>
