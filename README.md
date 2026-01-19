# 🛡️ SecCheckmate

> **Professional-Grade Security Assessment Framework - 200+ Tests Across 5 Domains**

<div align="center">

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/amitgy/seccheckmate)
[![GitHub Stars](https://img.shields.io/github/stars/amitgy/seccheckmate?style=social&label=Star%20us%21)](https://github.com/amitgy/seccheckmate)

**Industry-Standard Security Assessment Framework**

[🚀 Quick Start](#-quick-start) • [✨ Features](#-features) • [📥 Install](#-installation) • [⚖️ Legal](LICENSE) • [🤝 Contribute](#-contributing)

</div>

---

## ⚠️ LEGAL DISCLAIMER

**SecCheckmate is for AUTHORIZED SECURITY TESTING ONLY.**

- ✅ Use only on systems you own or have explicit written permission to test
- ✅ Comply with all applicable laws and regulations
- ✅ Use for defensive/authorized security purposes only

**Unauthorized testing is ILLEGAL.** Read [LICENSE](LICENSE) file for full legal terms before using.

---

## 🎯 Why SecCheckmate?

SecCheckmate solves a critical gap in security: **there's no standardized way to conduct security assessments.**

Every organization does it differently:
- ❌ Scattered spreadsheets
- ❌ Inconsistent methodologies
- ❌ Non-reproducible results
- ❌ Poor documentation
- ❌ Subjective severity ratings

**SecCheckmate changes this:**

✅ **Standardized** - Same framework, consistent results  
✅ **Comprehensive** - 200+ tests across 5 critical domains  
✅ **Offline-First** - 100% private, no data collection  
✅ **Professional** - Enterprise-grade reports  
✅ **Simple** - Just answer y/n/na questions  
✅ **Fast** - Complete assessment in minutes  

### 👥 Perfect For:

- 🔒 **Penetration Testers** - Comprehensive assessment checklists
- 👨‍💼 **Security Engineers** - Standardized security audits
- ☁️ **Cloud Architects** - AWS security compliance
- 📱 **Firmware Analysts** - Embedded systems security
- 🤖 **AI/ML Security** - LLM security testing
- 🌐 **Web Developers** - Application security reviews
- 🏢 **Security Auditors** - Compliance documentation

---

## ✨ Features at a Glance

### 📋 200+ Comprehensive Tests

| Category | Tests | Coverage |
|----------|-------|----------|
| 🌐 Web App Security | 35 | OWASP, APIs, Authentication |
| ☁️ AWS Cloud | 40 | IAM, EC2, S3, RDS, Lambda |
| 📡 WiFi Security | 38 | WPA2/3, Encryption, APs |
| 🔧 Firmware | 44 | Boot, Debug, Credentials |
| 🤖 LLM/AI Security | 44 | Prompts, Data, Privacy |


---

## 🚀 Quick Start (5 Minutes)

### Prerequisites
- **Python 3.10+** (required)
- **macOS, Linux, or Windows**

### Run Your First Assessment

```bash
python seccheckmate.py
```

**Then:**
1. Select assessment category (1-5)
2. Answer questions with: `y` / `n` / `na` (or press Enter for N/A)
3. Add evidence notes (optional)
4. Get professional report in `reports/` folder!

### Example Output

```
🛡️ SecCheckmate - Security Assessment Framework

Options:
  1. 🚀 Run Security Assessment
  2. 📚 View Available Assessments
  3. 📊 View Recent Reports
  4. ⚙️  Settings
  5. ❌ Exit

Select option (1-5): 1

Available Assessments:
  1. cloud_aws (40 tests)
  2. firmware (44 tests)
  3. llm (44 tests)
  4. web (35 tests)
  5. wifi (38 tests)

Select (1-5): 1

📊 AWS Cloud Security - 40 Tests

[  1/40] IAM Root Account Usage
Response [y/n/na]: n
Evidence: Root account has unused access keys

✅ Assessment Complete!
Pass Rate: 87.5%
Report: reports/report_20260119_143022.md
```

---

## 📥 Installation Details

### System Requirements

- **Python:** 3.10+ (required, not 3.9 or earlier)
- **OS:** macOS, Linux, or Windows
- **Disk:** ~50 MB
- **Internet:** Not required (100% offline)

### Installation Methods

**Method 1: Virtual Environment (Recommended)**

```bash
git clone https://github.com/amitgy/seccheckmate.git
cd seccheckmate

python3 -m venv venv
source venv/bin/activate  # macOS/Linux
# venv\Scripts\activate  # Windows

pip install --upgrade pip
pip install -r requirements.txt

python seccheckmate.py
```

**Method 2: Direct Installation**

```bash
git clone https://github.com/amitgy/seccheckmate.git
cd seccheckmate

pip install PyYAML>=6.0 colorama>=0.4.6
python seccheckmate.py
```

**Method 3: Development Setup**

```bash
git clone https://github.com/amitgy/seccheckmate.git
cd seccheckmate

python3 -m venv venv
source venv/bin/activate

pip install --upgrade pip
pip install -r requirements.txt

chmod +x seccheckmate.py  # macOS/Linux
```

### Platform-Specific Setup

**macOS**
```bash
# Using Homebrew
brew install python3

python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

**Linux (Ubuntu/Debian)**
```bash
sudo apt update
sudo apt install python3 python3-venv python3-pip

python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

**Windows (PowerShell)**
```powershell
python -m venv venv
venv\Scripts\Activate.ps1

pip install -r requirements.txt
python seccheckmate.py
```

**Windows (Command Prompt)**
```cmd
python -m venv venv
venv\Scripts\activate.bat

pip install -r requirements.txt
python seccheckmate.py
```

---

## 📊 Test Coverage

### 🌐 Web Application Security (35 tests)
Authentication & authorization, SQL injection, XSS, CSRF, CORS, API security, SSL/TLS, security headers, business logic, dependencies

### ☁️ AWS Cloud Security (40 tests)
IAM policies, EC2 security groups, S3 permissions, RDS encryption, CloudTrail, VPC, KMS, Lambda roles, DynamoDB

### 📡 WiFi Network Security (38 tests)
WPA2/WPA3, PSK testing, rogue APs, MITM prevention, deauth resilience, WPS/UPnP, guest networks, physical security, monitoring

### 🔧 Firmware Security (44 tests)
Secure boot, code integrity, rollback protection, hardcoded credentials, debug interfaces (JTAG/UART/SWD), buffer overflow, crypto, reverse engineering, supply chain

### 🤖 LLM/AI Security (44 tests)
Prompt injection, training data leakage, jailbreak resistance, RAG validation, API security, encryption, GDPR, model integrity, bias/fairness

---

## 🎯 Severity Classification

SecCheckmate classifies findings using this framework:

### 🔴 **CRITICAL** - Immediate Action (24-48 hours)
- Complete system compromise possible
- Examples: Unauthenticated access, hardcoded credentials, SQL injection
- **Assumption:** Allows full attacker control

### 🟠 **HIGH** - Urgent (1-2 weeks)
- Major security bypass or breach possible
- Examples: Weak authentication, missing encryption, privilege escalation
- **Assumption:** Bypasses major security controls

### 🟡 **MEDIUM** - Plan (1 month)
- Requires exploitation chain or conditions
- Examples: Missing headers, weak policies, info disclosure
- **Assumption:** Could chain with other vulnerabilities

### 🟢 **LOW** - Maintenance
- Minor impact, best practice gaps
- Examples: Outdated non-critical software, configuration hardening
- **Assumption:** Limited impact

### 🔵 **INFO** - Future Planning
- Recommendations and best practices
- Examples: Training, monitoring, documentation
- **Assumption:** Not a vulnerability

---

## 📄 Report Format

SecCheckmate generates professional markdown reports:

```markdown
# 🛡️ Security Assessment Report

**Category:** AWS Cloud Security
**Organization:** Your Org
**Date:** January 19, 2026
**Tool:** SecCheckmate v1.0.0

## Executive Summary

Assessment evaluated 40 security controls.

### Key Metrics
| Metric | Count | % |
|--------|-------|---|
| ✅ Passed | 35 | 87.5% |
| ❌ Failed | 3 | 7.5% |
| ⏭️ N/A | 2 | 5.0% |

### Risk Assessment
- **Critical:** 0
- **High:** 1

## Findings by Severity

### 🟠 High (1)
- AWS-15: S3 Bucket Public Access

### 🟡 Medium (2)
- AWS-08: CloudTrail Not Enabled
- AWS-12: VPC Flow Logs Missing
```

---

## 🔧 Configuration

Edit `config/settings.yaml`:

```yaml
organization: "Your Organization"
version: "1.0"
```

---

## 📁 Project Structure

```
seccheckmate/
├── seccheckmate.py           # Main application
├── requirements.txt          # Python dependencies
├── README.md                 # This file
├── LICENSE                   # MIT License + Legal Disclaimer
│
├── config/
│   └── settings.yaml         # Configuration
│
├── checklists/               # Assessment templates
│   ├── web.yaml              # Web security (35 tests)
│   ├── cloud_aws.yaml        # AWS security (40 tests)
│   ├── wifi.yaml             # WiFi security (38 tests)
│   ├── firmware.yaml         # Firmware security (44 tests)
│   └── llm.yaml              # LLM security (44 tests)
│
└── reports/                  # Generated reports
    └── report_*.md           # Dated reports
```

---

## ❓ FAQ

**Q: Is this an automated vulnerability scanner?**  
A: No. It's a checklist framework requiring professional judgment.

**Q: Can I test systems I don't own?**  
A: **No.** You need explicit written permission. Unauthorized testing is illegal.

**Q: What if a test doesn't apply?**  
A: Mark it "N/A" (press Enter). Metrics calculate only for applicable tests.

**Q: Can I modify checklists?**  
A: Yes! Edit YAML files in `checklists/` folder.

**Q: Does it send data online?**  
A: No. 100% offline, all reports stay on your machine.

**Q: What Python versions work?**  
A: Python 3.10+ only. Not compatible with 3.9 or earlier.

**Q: Can I contribute?**  
A: Yes! We welcome new checklists and improvements.

---

## 🤝 Contributing

We welcome:
- ✅ New security checklists
- ✅ Bug fixes and improvements
- ✅ Documentation enhancements
- ✅ Testing and validation

Please:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

See LICENSE file for contribution guidelines.

---

## 📄 License & Legal

This project is licensed under the **MIT License**.

**IMPORTANT:**
- For AUTHORIZED testing ONLY
- Read LICENSE file before use
- You assume all legal responsibility
- Unauthorized testing is illegal in all jurisdictions

---

## 📞 Support

- 🐛 **Bug Reports:** [GitHub Issues](https://github.com/amitgy/seccheckmate/issues)
- 💬 **Questions:** [GitHub Discussions](https://github.com/amitgy/seccheckmate/discussions)
- 📄 **Legal:** See LICENSE file

---

## 💡 Best Practices

1. **Read test descriptions** - Understand what each validates
2. **Document evidence** - Include URLs and configuration details
3. **Customize severity** - Adjust for your environment context
4. **Regular assessments** - Schedule quarterly reviews
5. **Track metrics** - Monitor improvements over time
6. **Share findings** - Present to relevant teams
7. **Act on recommendations** - Fix issues systematically

---

## ⭐ Like This Project?

Give it a **star** on GitHub!

[⭐ Star SecCheckmate](https://github.com/amitgy/seccheckmate)

---

**Made with ❤️ by the security community**

*Professional security assessment framework | Open source | MIT licensed | Privacy-first | Offline-only*

---

<div align="center">

**[Get Started Now →](#-quick-start)** | **[View Legal Terms →](LICENSE)** | **[Contribute →](#-contributing)**

Last Updated: January 19, 2026 | v1.0.0

</div>
