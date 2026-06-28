---
date:
tags:
  - MITRE
  - frameworks
category:
  - writeup
author: miniMinn
platform:
  - Blue Team Labs Online
banner: "[[ATT&CK - BTLO Walkthrough-1782631831506.webp]]"
---
![[ATT&CK - BTLO Walkthrough-1782631831506.webp]]

# 📓 Overview
This challenge is about researching attacks and techniques we will see in common, getting familiar with it will give insights to preparing defenses.

### Tools used
- [MITRE ATT&CK](https://attack.mitre.org/) framework to search specific attack techniques and tactics.

# 💻 Initial analysis

> [!quote]- Scenario
> *You are hired as a Blue Team member for a company. You are assigned to perform threat intelligence for the company. See how you can operationalize the MITRE ATT&CK framework to solve these scenario-based problems.*



# 👨‍💻 Q&A

### T-1. Your company heavily relies on cloud services like Azure AD, and Office 365 publicly. What technique should you focus on mitigating, to prevent an attacker performing Discovery activities if they have obtained valid credentials? (Hint: Not using an API to interact with the cloud environment!)

Under **Discovery** catalog, there's "Cloud Service Dashboard" tactic that the attacker will use cloud service dashboards with stolen victim's credentials to gather information about compromised cloud env:

![[ATT&CK - BTLO Walkthrough-1782632295773.webp]]

**Detection**: This can be mitigated by **User Account Management (M1018)** by enforcing **principle of least privilege** and restricting with **RBAC control**.

### T-2. You were analyzing a log and found uncommon data flow on port 4050. What APT group might this be?




# ⚔ MITRE tactics mapping

# 🛡 Detection rules

# 💭 Lessons learned
