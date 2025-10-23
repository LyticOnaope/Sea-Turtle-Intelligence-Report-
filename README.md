# 🕵️‍♂️ Sea Turtle Threat Intelligence Report (October 2025)

**Analyst:** Onaopemipo David Olugbemiro  
**Role:** Threat Intelligence Analyst 
**Report Type:** Advanced Threat Intelligence & IOC Analysis  
**Target Threat Actor:** Sea Turtle (Teal Kurma / Marbled Dust)  

---

## 🧠 Project Overview

This project is an **end-to-end threat intelligence investigation** conducted as part of my cybersecurity training with **10Alytics**, simulating a **National CERT response**.  
It focuses on analyzing the **Sea Turtle** espionage group — a **Turkish state-linked actor** known for **DNS hijacking, credential theft, and C2 operations** targeting **European government and telecom infrastructure**.  

**Key Deliverables:**
- IOC extraction and enrichment from **MISP**.  
- Threat infrastructure analysis using **VirusTotal** and **WHOIS/ASN lookups**.  
- TTP classification using the **MITRE ATT&CK** framework.  
- Risk and mitigation assessment for CERT recommendations.  
- Full technical and executive **Threat Intelligence Report & Presentation**.  

---

## 🛠️ Tools & Techniques Used

| Tool / Framework | Purpose |
|------------------|----------|
| **MISP** | IOC extraction and correlation |
| **VirusTotal** | IOC reputation and malware analysis |
| **WHOIS / ASN Lookup** | Hosting, geolocation, and network attribution |
| **MITRE ATT&CK** | TTP mapping and behavioral profiling |
| **MS Word** | Reporting and documentation |
| **PowerPoint** | Executive-level presentation design |

---

## 🚨 Key Findings

1. **Distributed Infrastructure Across Europe**  
   - Sea Turtle leveraged VPN and hosting services across **Belgium, Denmark, Netherlands, and Germany**.  
   - Providers included **M247**, **Arelion**, **Snel.com**, and **Vultr**.  

2. **Malware and Command & Control (C2)**  
   - Used custom **SnappyTCP malware** for HTTPS-based C2 communication.  
   - Domain `forward.boord.info` served as a C2 channel.  

3. **Credential Theft & DNS Hijacking**  
   - Compromised registrar **cPanel accounts** to redirect DNS traffic.  
   - Enabled long-term espionage access to government email systems.  

---

## 📊 Indicators of Compromise (IOCs)

| IOC | Hosting / Location | Description |
|:--|:--|:--|
| 82.102.19.88 | M247 Europe SRL – Belgium | VPN login infrastructure (**Medium**) |
| 193.34.167.245 | Snel.com BV – Netherlands | Malware host (**High**) |
| 95.179.176.250 | Vultr Holdings – Netherlands | C2 server (**High**) |
| forward.boord.info | Cloudflare – US | SnappyTCP C2 domain (**High**) |

---

## 🧩 MITRE ATT&CK Mapping

| Tactic | Technique | Technique ID |
|:--|:--|:--|
| Initial Access | Valid Accounts | T1078 |
| Command & Control | Application Layer Protocol: Web | T1071.001 |
| Persistence | Modify Authentication Process | T1556 |
| Defense Evasion | Use of Commercial Hosting | T1583.003 |
| Impact | DNS Hijack / Defacement | T1565.002 |

---

## 🚀 Mitigation & Recommendations

**Immediate Actions:**  
- Block identified IOCs and C2 domains.  
- Enforce **MFA** on registrar and admin accounts.  
- Monitor **VPN logins from foreign ASNs** (M247, Vultr, Arelion).  

**Preventive Measures:**  
- Enable **Registry Lock** and **DNSSEC** on domains.  
- Integrate **MISP & VirusTotal feeds** into SIEM for live threat updates.  
- Regularly **audit DNS configurations and SSL certificates**.  

**Long-Term Enhancements:**  
- Conduct periodic **threat hunting** for similar TTPs.  
- Improve **incident response playbooks** for DNS hijacking.  
- Strengthen collaboration with CERT partners for IOC sharing.  

---

## ✅ Learning Outcomes

Through this project, I gained hands-on experience in:  
- **Threat intelligence collection & IOC enrichment** (MISP, VirusTotal).  
- **MITRE ATT&CK mapping and behavioral analysis**.  
- **Technical & executive reporting** for CERT operations.  
- **DNS hijacking and C2 infrastructure analysis**.  
- **Developing actionable security mitigations** for real-world threats.  

---

## 📂 Project Deliverables

- `SeaTurtle_Final_Threat_Intelligence_Report_OnaopeOlugbemiro.docx`  
- `SeaTurtle_Threat_Intelligence_Presentation_OnaopeOlugbemiro.pptx`

---

## 🤝 Connect

If you’re a recruiter, SOC manager, or cybersecurity professional, feel free to connect:

📍 **[LinkedIn](https://www.linkedin.com/in/onaopemipo-olugbemiro-1b377828b/)**  
🐦 **[Twitter](https://x.com/itzonaope)**  
💻 **[GitHub](https://github.com/LyticOnaope)**  

---
