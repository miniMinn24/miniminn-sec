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

# 💻 Forensic

## 1. Initial analysis

> [!quote]- Challenge Scenario
> Our SOC has identified numerous phishing emails coming in claiming to have a document about an upcoming round of layoffs in the company. The emails all contain a link to diagnostic.htb/layoffs.doc. The DNS for that domain has since stopped resolving, but the server is still hosting the malicious document (your docker). Take a look and figure out what's going on.

Looking at the first, there seems to be no challenge files provided but only the target host. Accessing the target server on the browser responds with "404 Not found", though it's active:

![[Diagnostic - HTB Walkthrough-1782533344914.webp]]

I move on to scan network service information and specific port `154.57.164.69:31308` using `nmap`:

```bash
# Aggressive network scanning
> sudo nmap -sV -sC -O -T4 --min-rate 5000 154.57.164.69 -p 31308

PORT      STATE SERVICE VERSION
31308/tcp open  http    Werkzeug httpd 2.1.2 (Python 3.9.13)
|_http-title: 404 Not Found
|_http-server-header: Werkzeug/2.1.2 Python/3.9.13
Aggressive OS guesses: Linux 4.15 - 5.19...

```

So the results shows that it's a Python web-server **Werkzeug HTTP daemon 2.1.2** running on port `31308`. It possibly looks like a **development server** running for production use due to the presence of Werkzeug (a WSGI utility library for python).

## 2. Evidence triage

The scenario mentions that all phishing emails direct link to `http://diagnostic.htb:31308/layoffs.doc`, which seems the attacker's hosting a suspicious file:

```bash
# Downloading the suspicious file
> curl 154.57.164.69:31308/layoffs.doc --output layoffs.doc

# Finding useful file meta info
> exiftool diagnostic.doc

File Name                       : diagnostic.doc
Warning                         : Install Archive::Zip to decode compressed ZIP information
File Type                       : ZIP
File Type Extension             : zip
MIME Type                       : application/zip
...
```

All the `.doc` files are basically **Office Open XML** (OOXML) and are simply ZIP archives containing **XML files and medias**. Attackers often manipulate those internal file hierarchy by replacing legitimate files with malicious ones:

```bash
# Extracting .docx's XML files
> unzip diagnostic.doc -d output
Archive:  diagnostic.doc
   creating: output/_rels/
   creating: output/docProps/
   creating: output/word/
  inflating: output/[Content_Types].xml  
  ...
```

Before inspecting each XML manually, I uploaded `layoffs.doc` file on **VirusTotal** to gather any known CVE information or Mitre's signatures:

![[Diagnostic - HTB Walkthrough-1782545023614.webp]]

Looking at the [CVE-2022-30190](https://www.cvedetails.com/cve/CVE-2022-30190/), it's a RCE that takes advantage of **Microsoft Windows Support Diagnostic Tool** (MSDT) vuln, then run arbitrary code with the privileges of the calling application (Word, for this scenario):

![[Diagnostic - HTB Walkthrough-1782545240178.webp]]

## 3. Examination

I used a vulnerable sandbox to fully execute the malware on **Any.Run** for dynamic analysis:  

![[Diagnostic - HTB Walkthrough-1782549404690.webp]]

> Though it's not required, you can still rely on static analysis using **VirusTotal** or manually inspecting the XML files.  

During the execution, the malware tried to retrieve malicious file from `http://diagnostic.htb:30510/223_index_style_fancy.html!`. 




# 👨‍💻 Q&A

### T-1.

# ⚔ MITRE tactics mapping

# 🛡 Detection rules

# 💭 Lessons learned
