# 🛡️ Security Operations Dashboard

**Enterprise SOC Simulator | Threat Detection | Incident Response | Security Analytics**

---

[![Kaggle](https://img.shields.io/badge/Kaggle-Notebook-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/code/mrrogueknight/security-operations-dashboard)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MrRogueKnight/security-operations-dashboard)
[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mrrogueknight/)

---

## 📊 Enterprise Security Operations Center (SOC) Simulator

**A comprehensive Python-based security analytics platform simulating real-world SOC operations, threat detection, and incident response.**

---

## 🎯 Project Overview

The **Security Operations Dashboard** is an educational cybersecurity project that simulates a complete Security Operations Center environment. It demonstrates the full security data pipeline – from synthetic log generation and threat detection to incident response and executive reporting.

This project was developed as the primary deliverable for an **8-week Ethical Hacking Internship** with Edu Skills, complemented by the **Google Cybersecurity Professional Certificate**.

---

## ✨ Key Features

| Feature | Description |
| :--- | :--- |
| **SIEM-like Log Collection** | Generates 18,600+ synthetic security events (auth, network, malware, firewall) |
| **Threat Detection Engine** | 5 detection rules mapped to MITRE ATT&CK framework |
| **Alert Generation** | 71+ alerts with severity classification |
| **Incident Response** | 4 playbooks with full incident lifecycle (Detection → Recovery) |
| **Analytics Dashboard** | 9 interactive visualizations for security posture analysis |
| **Executive Reporting** | Auto-generated professional security reports with recommendations |
| **Unit Testing** | 8 comprehensive tests ensuring system reliability |
| **Framework Alignment** | NIST CSF, MITRE ATT&CK, OWASP Top 10, CISSP |

---

## 🏗️ System Architecture

```mermaid
flowchart TD
    A[Data Sources Synthetic] --> B[SQLite Database 10 Tables]
    
    B --> C[Threat Detection Engine 5 Rules]
    C --> D[Alert Correlation]
    D --> E[Incident Response 4 Playbooks]
    E --> F[Visualization Dashboard 9 Charts]
    F --> G[Executive Report]

    subgraph B[Database Tables]
        B1[Assets]
        B2[Users]
        B3[Auth Logs]
        B4[Network Traffic]
        B5[Firewall Logs]
        B6[Malware Events]
        B7[Vulnerabilities]
        B8[Alerts]
        B9[Incidents]
        B10[Playbooks]
    end

    subgraph C[Detection Rules]
        C1[Brute Force<br>T1110]
        C2[Impossible Travel<br>T1078]
        C3[Port Scanning<br>T1046]
        C4[Malware Activity<br>T1203]
        C5[SQL Injection<br>T1190]
    end

    subgraph E[Incident Response]
        E1[Detection]
        E2[Analysis]
        E3[Containment]
        E4[Eradication]
        E5[Recovery]
    end

    subgraph F[Dashboard Charts]
        F1[Authentication Status]
        F2[Threat Type Distribution]
        F3[Attack Timeline]
        F4[Vulnerability Severity]
        F5[MFA Adoption Rate]
        F6[Malware Detections]
        F7[Incident Severity]
        F8[Asset Criticality]
        F9[NIST CSF Assessment]
    end
```

---

## 🛠️ Technologies Used

<div align="center">
  
| Category | Technologies |
| :--- | :--- |
| **Language** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) |
| **Database** | ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) |
| **Data Processing** | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) |
| **Visualization** | ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=python&logoColor=white) ![Seaborn](https://img.shields.io/badge/Seaborn-1273B3?style=flat-square&logo=python&logoColor=white) |
| **Security Frameworks** | NIST CSF, MITRE ATT&CK, OWASP Top 10, CISSP |

</div>

---

## 📁 Project Structure

```
security-operations-dashboard/
│
├── 📓 security-operations-dashboard.ipynb   # Main Jupyter Notebook
├── 📄 executive_security_report.txt         # Generated security report
├── 🖼️ security_dashboard.png                # Dashboard visualization
├── 📖 README.md                             # Project documentation
└── 📜 LICENSE                               # MIT License
```

---

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/MrRogueKnight/security-operations-dashboard.git
cd security-operations-dashboard
```

### 2. Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn sqlite3 bcrypt
```

### 3. Run the Notebook
```bash
jupyter notebook security-operations-dashboard.ipynb
```

### 4. Or Run on Kaggle
Click the badge below to run directly on Kaggle:

[![Kaggle](https://img.shields.io/badge/Run_on_Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/code/mrrogueknight/security-operations-dashboard)

---

## 📊 Dashboard Preview

The dashboard includes 9 key visualizations:

| Chart | Purpose |
| :--- | :--- |
| **Authentication Status** | IAM health monitoring (success/failure rates) |
| **Threat Type Distribution** | Most common attack types |
| **Attack Timeline** | 24-hour attack pattern analysis |
| **Vulnerability Severity** | OWASP classification of open vulnerabilities |
| **MFA Adoption Rate** | IAM best practice assessment |
| **Malware Detections** | Malware type distribution |
| **Incident Severity** | Incident response workload assessment |
| **Asset Criticality** | High-value asset identification |
| **NIST CSF Assessment** | Framework implementation status |

---

## 🧪 Unit Tests

8 comprehensive tests ensure system reliability:

| Test | Status |
| :--- | :---: |
| Database Connection | Pass |
| Schema Creation | Pass |
| Data Population | Pass |
| Brute Force Detection | Pass |
| Configuration Validation | Pass |
| Metrics Calculation | Pass |
| Incident-Playbook Linkage | Pass |
| MITRE ATT&CK Mapping | Pass |

---

## 📐 Framework Alignment

| Framework | Implementation |
| :--- | :--- |
| **NIST CSF v2.0** | All 6 functions: Govern, Identify, Protect, Detect, Respond, Recover |
| **MITRE ATT&CK** | 5 tactics: T1110, T1046, T1190, T1203, T1078 |
| **OWASP Top 10** | 5 categories: A03, A05, A07, A08, A02 |
| **CISSP Domains** | All 8 domains represented |
| **CIA Triad** | Confidentiality, Integrity, Availability |

---

## 📈 Sample Output

### Executive Security Report
```
================================================================================
EXECUTIVE SECURITY SUMMARY REPORT
================================================================================

Generated: August 01, 2026 at 14:00
Organization: Enterprise SOC Simulator (Educational)
Report Type: Security Posture Assessment

================================================================================
1. EXECUTIVE SUMMARY
================================================================================

Overall Security Score: 77% (Heuristic)
Security Posture: Moderate

================================================================================
2. SECURITY METRICS
================================================================================

Assets Managed: 50
Patch Compliance: 40.0%
Users with MFA: 66.0%
Open Vulnerabilities: 39
Critical Vulnerabilities: 11
Total Incidents: 5
Open Incidents: 0
Total Alerts: 71

================================================================================
6. RECOMMENDATIONS
================================================================================

Immediate Actions (0-30 days):
  - Patch all 30 systems with Critical Patch Required status
  - Remediate 11 Critical vulnerabilities
  - Enable MFA for 17 users currently without it
```

---

## 🛡️ Security Concepts Demonstrated

| Category | Concepts |
| :--- | :--- |
| **Core Principles** | CIA Triad, Least Privilege, Defense in Depth |
| **Operations** | Incident Response, SIEM Operations, Threat Intelligence |
| **Management** | Vulnerability Management, IAM, Framework Alignment |

---

## 📚 References

- **Google Cybersecurity Professional Certificate (2026)**
- **NIST Cybersecurity Framework v2.0**
- **MITRE ATT&CK Framework**
- **OWASP Top 10 (2021)**
- **CISSP Common Body of Knowledge**

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Prashant Ranjan**
- [![Kaggle](https://img.shields.io/badge/Kaggle-@MrRogueKnight-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/mrrogueknight)
- [![GitHub](https://img.shields.io/badge/GitHub-@MrRogueKnight-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/MrRogueKnight)
- [![LinkedIn](https://img.shields.io/badge/LinkedIn-@MrRogueKnight-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mrrogueknight/)

---

## ⭐ Acknowledgments

- **Edu Skills** – For the internship opportunity
- **Google Cybersecurity Certificate** – For the theoretical foundation
- **Open-source community** – For tools and libraries

---

<div align="center">
  
### ⭐ If you found this project useful, please give it a star!

---

**Built with ❤️ during the Ethical Hacking Internship (8 Weeks) | August 2026**

</div>
