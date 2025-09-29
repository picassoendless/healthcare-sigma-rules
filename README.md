# 🏥 Healthcare Sigma Rules

This repository contains **Sigma detection rules** tailored to protect the **healthcare sector** from cyber threats such as ransomware, phishing, and insider attacks.  

## 🎯 Purpose
Healthcare organizations are part of critical infrastructure and are frequent targets of ransomware campaigns. These Sigma rules provide defenders with ready-to-use detection content that can be applied in SIEM platforms like Splunk, Elastic, or Sentinel to improve security monitoring.

---

## 📂 Repository Structure
- `sigma-rules/healthcare/` → Healthcare-specific Sigma rules  
- `docs/` → Human-readable documentation for each rule  

---

## 📜 Rule Index

| Rule Name                                   | Category     | Description                                                             | Link |
|---------------------------------------------|--------------|-------------------------------------------------------------------------|------|
| Suspicious PowerShell Execution in Healthcare | Windows/Healthcare | Detects suspicious PowerShell usage often tied to ransomware campaigns | [YAML](sigma-rules/healthcare/powershell_suspicious_healthcare.yml) / [Docs](docs/powershell_suspicious_healthcare.md) |

---

## 🖼️ Example Screenshot
*(Optional, add after testing in Splunk/Elastic)*  
![screenshot](docs/images/powershell_rule_trigger.png)

---

## 🤝 Contribution
Pull requests are welcome. The goal is to build a free, open-source library that healthcare SOC teams can adopt quickly.  

---

## 🔗 References
- [MITRE ATT&CK T1059.001 - PowerShell](https://attack.mitre.org/techniques/T1059/001/)  
- [CISA Healthcare Ransomware Alerts](https://www.cisa.gov/news-events/alerts)  
