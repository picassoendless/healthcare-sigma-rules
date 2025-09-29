# Suspicious PowerShell Execution in Healthcare Systems

## 📌 Overview
This rule detects suspicious PowerShell activity that is commonly used in **ransomware attacks targeting hospitals and healthcare organizations**.  

Hackers often use PowerShell to:
- Download malware from the internet (`Invoke-WebRequest`, `DownloadString`)
- Hide commands using encoding (`Base64`)
- Execute the downloaded script immediately (`IEX`)

## 🔍 Rule Logic
- Watch for any process where `powershell.exe` is started.  
- Check the command line for keywords that match attacker behavior.  
- Exclude known safe scripts (like internal IT automation).  

## 🏥 Relevance to Healthcare
Hospitals and clinics are high-value targets for ransomware gangs.  
A successful attack could:
- Lock doctors out of patient records.  
- Delay surgeries or critical care.  
- Put patient lives at risk.  

By detecting malicious PowerShell use early, this rule helps **stop ransomware before it spreads**.  

## ⚠️ False Positives
- IT administrators using PowerShell for updates or automation.  
- Backup or monitoring tools.  

## ✅ Example
Alert triggered when:
