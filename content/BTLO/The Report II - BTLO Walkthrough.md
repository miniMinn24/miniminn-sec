---
date: 2026-07-15
tags:
  - SecOps
category:
  - writeup
author: miniMinn
platform:
  - Blue Team Labs Online
status:
  - Writing in progress...
---
# 1. Overview
This challenge **The Report II** involves analyzing the **11 Strategies of a World Class Cybersecurity Operations Center** to answer specific tasks about day-to-day SOC operations.

> **BTLO challenge link**: https://blueteamlabs.online/home/challenge/the-report-ii-82ea7781c5

### Tools used
- **A browser** or **PDF viewer** to read the provided PDF report.

# 2. Analysis

> [!quote]- Scenario
> *This challenge is an extension for an existing 'The Report' challenge where you are working in a newly established SOC where there is still a lot of work to do to make it a fully functional one. As part of the SOC improvement process, you were assigned a task to study a report released by MITRE and suggest some useful outcomes for your SOC. Note: Answer the questions with the answers as the way you see in the document to avoid formatting issues. Report Link: https://www.mitre.org/sites/default/files/publications/11-strategies-of-a-world-class-cybersecurity-operations-center.pdf*

### T-1. Submit the name of the units/teams (in short form) that are responsible for maintaining network and other IT equipment, incident detection and response, and security compliance and risk measurement (Format: Team1, Team2, Team3)

The name of teams that are responsible for maintaining networks and other IT equipment is **NOC or IT operations**, incident detection and response is **SOC**, and security compliance and risk measurement is **ISCM** (Info Sec Continuous Monitoring):  

![[The Report II - BTLO Walkthrough-1784090567715.webp]]  

![[The Report II - BTLO Walkthrough-1784090593797.webp]]

### T-2. After investigation, what are the 4 suggested 'Response Options' mentioned in Basic SOC Workflow? (Format: Option1, Option2, Option3, Option4)

After investigation, the 4 suggested **'Response Options'** in Basic SOC Workflow are:
1. **Block Activity**
2. **Deactivate Account**
3. **Continue Watching**
4. **Refer to Outside Party**

![[The Report II - BTLO Walkthrough-1784090793114.webp]]

### T-3. What is the name of a military strategy used in SOCs to achieve a high level of situational awareness? (Format: Strategy Name)

The name of a military strategy used in SOCs to achieve a high level of situational awareness is **OODA loop** (Observe, Orient, Act, Decide).  

![[The Report II - BTLO Walkthrough-1784090902936.webp]]

### T-4. What is the name of the suggested organisational model if the constituency size is between 1000 to 10,000 employees (Format: Organisational Model Name)

The name of suggested organizational model if the **Constituency Size** is between 1,000 to 10,000 employees is **Distributed SOC**.  

![[The Report II - BTLO Walkthrough-1784091007426.webp]]

### T-5. In a Large Centralised SOC, who is responsible for generating SOC metrics, maintaining situational awareness, and conducting internal/external trainings? (Format: Role Name)

In the large SOC, the role **SOC Operations Lead** is responsible for generating SOC metrics, maintaining situational awareness, and conducting internal/external trainings.  

![[The Report II - BTLO Walkthrough-1784091118673.webp]]

### T-6. In Coordinating & National SOCs model what are the 2 functions mentioned as Optional Capability under Expanded SOC Operations Category? (Format: Function1, Function2)

Under Expanded SOC Operations Category, the functions **Deception and Insider Threat** are mentioned as optional capability in coordinating and national SOCs model.  

![[The Report II - BTLO Walkthrough-1784091425027.webp]]

### T-7. What are the two virtual console technologies (in short form) mentioned to support Virtual SOC/ Remote Work scenarios during pandemics? (Format: Technology1, Technology2)

The virtual consoles like **iLO** and **iDRAC** are mentioned to support virtual SOC/Remote work scenarios during pandemics.  

![[The Report II - BTLO Walkthrough-1784091743396.webp]]

### T-8. What is the name of the model used to distribute work load of SOC 24/7 across different timezones to eliminate working at night hours? (Format: Model Name)

The **Follow the Sun** model is used to distribute work load of 24/7 across different timezones to eliminate working at night hours.  

![[The Report II - BTLO Walkthrough-1784092019501.webp]]

### T-9. Submit the priorities(Low, Medium, High) assigned to Phishing, Insider Threat and Pre-incident Port Scanning activities respectively as per the Incident Prioritization mentioned in the document (Format: Priority1, Priority2, Priority3)

The priorities assigned by Incident Prioritization Table:
- **Phishing**: `Medium`
- **Insider Threat**: `High`
- **Pre-incident port scanning**: `Low`

![[The Report II - BTLO Walkthrough-1784092177708.webp]]

### T-10. Mention the name of the Open source Operating system mentioned, that can help in mobile incident investigations (Format: OS Name)

