---
date:
tags:
category:
  - writeup
author: miniMinn
platform:
  - HackTheBox
banner: "[[Diagnostic - HTB Walkthrough-1782531644360.webp]]"
---
![[Diagnostic - HTB Walkthrough-1782531644360.webp]]

# 📓 Overview
The "Diagnostic" lab is a #forensic challenge and rated as #easy difficulty. It's about investigating how the phishing links are directing to the same server, and compromising the victim's systems by using the Microsoft Windows Support Diagnostics Tool's (MSDT) flaw.

### Tools used
- [VirusTotal](https://www.virustotal.com/gui/home/upload) to analyze known malformed files and CVEs.
- `curl` (Client URL) to fetch server data and information.
- [CyberChef](https://gchq.github.io/CyberChef/) to decode obfuscated codes.

# 💻 Initial analysis

> [!quote]- Challenge Scenario
> Our SOC has identified numerous phishing emails coming in claiming to have a document about an upcoming round of layoffs in the company. The emails all contain a link to diagnostic.htb/layoffs.doc. The DNS for that domain has since stopped resolving, but the server is still hosting the malicious document (your docker). Take a look and figure out what's going on.

# 👨‍💻 Q&A

### T-1.

# ⚔ MITRE tactics mapping

# 🛡 Detection rules

# 💭 Lessons learned
