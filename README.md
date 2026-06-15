# 🛡️ SOC Detection & Threat Hunting Rules

> **100+ Splunk + Sigma + KQL detection rules based on 50+ MITRE ATT&CK techniques**

[![MITRE ATT&CK](https://img.shields.io/badge/MITRE%20ATT%26CK-50%2B%20Techniques-blue)](https://attack.mitre.org/)
[![Splunk](https://img.shields.io/badge/Splunk-SPL-green)](https://www.splunk.com/)
[![ELK](https://img.shields.io/badge/ELK-KQL-orange)](https://www.elastic.co/)
[![Sigma](https://img.shields.io/badge/Sigma-Rules-red)](https://sigma-rules.io/)

## 👨‍💻 About Me

**x0Hunter** | Blue Team | Detection Engineer (Aspiring)

- 🎓 **BTL1 Gold** (Blue Team Level 1 - Gold Coin) – *In progress*
- 🎓 **CJDE** (Certified Junior Detection Engineer) – *Next target*
- 🎓 **OSDA** (OffSec Defense Analyst) – *Planned*

**What I do:**
- Write production-ready Splunk queries with FP reduction
- Develop Sigma rules for cross-SIEM detection
- Hunt threats using KQL on ELK Stack
- Map every detection to MITRE ATT&CK framework

**Why this repo?**
This repository contains my **personal detection engineering portfolio**. Every rule is:
- ✅ MITRE ATT&CK mapped (T1047, T1059, T1087, T1033, etc.)
- ✅ FP-tested with exclude filters (Chocolatey, Azure AD, SCCM, PRTG, Veeam)
- ✅ Production-ready (clean syntax, proper field usage)
- ✅ Cross-platform (Splunk SPL, KQL, Sigma)

---

## 📊 MITRE ATT&CK Coverage Summary (50+ Techniques)

| Tactic | Techniques | Rule Count |
|--------|-----------|-----------:|
| Initial Access | T1566.001, T1133, T1190 | 6(SPL) |
| Execution | T1204.002, T1059.001, T1059.003, T1059.005 | 8(SPL) |
| Persistence | T1053.005, T1547.001, T1543.003, T1078, T1136.001 | 10(SPL) |
| Defense Evasion | T1562.001, T1562.004, T1027, T1036.005, T1070.001 | 10(SPL) |
| Credential Access | T1003.001, T1110.001, T1110.003, T1555, T1558.003 | 10(SPL) |
| Discovery | T1082, T1083, T1057, T1018, T1069.001 | 10(SPL) |
| Lateral Movement | T1021.001, T1021.002, T1021.006, T1550.002, T1210 | 10(SPL) |
| Collection | T1005, T1114.001, T1056.001, T1560.001, T1074.001 | 10(SPL) |
| Exfiltration | T1048.003, T1041, T1567.002 | 6(SPL) |
| C2 | T1071.001, T1071.004, T1095, T1572, T1219 | 10(SPL) |
| Impact | T1486, T1490, T1489, T1485, T1498 | 10(SPL) |
| **Total** | **50+ Techniques** | **100+(SPL) Rules** |

---

## 📂 Repository Structure

`SOC-Detection-Rules/`
- `Splunk/` (50+ SPL queries - Detection + Hunting)
  -Invesgtigations
    - Lateral_Movement/
    - Execution/
    - Discovery/
    - Defense_Evasion/
    - Credential_Access/
    - Persistence/
    - Collection/
    - C2/
    - Impact/
- `KQL/` (50+ KQL queries - ELK Stack)
  - Lateral_Movement/
  - Execution/
  - Discovery/
- `README.md`


### Current Investigations
| Investigations ID | Techniques 
|--------|-----------:|
| **001** | **[./investigations/001-Encoded-PowerShell/Readme.md] T1569.001 Encoded PowerShell Execution** |
  - AMSI Bypass Analysis
  - PowerShell Deobfuscation
  - IOC Extraction
  - ATT&CK Mapping
  - Attack Flow Development


