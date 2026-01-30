# DVWA SQL Injection Lab

A beginner-friendly cybersecurity project demonstrating SQL injection vulnerabilities in a safe, controlled environment.

## Overview

This project documents a hands-on penetration testing exercise using DVWA (Damn Vulnerable Web Application) on an isolated lab setup. The goal was to identify and exploit a SQL injection vulnerability, understand the attack vectors, and learn defensive coding practices.

**Author:** Muhammad Khubaib Asif  
**Date:** September 29, 2025  
**Institution:** University of Engineering and Technology, Lahore

## Repository Contents

```
├── README.md              # Project overview
├── lab-setup.md          # Lab environment setup instructions
├── PERMISSIONS.md        # Ethical and legal compliance statement
├── findings/
│   └── VULN-001.md      # SQL injection vulnerability report
└── media/
    └── screenshots/      # Documentation screenshots
```

## Lab Environment

- **Attack Machine:** Kali Linux / Host OS
- **Target Machine:** Metasploitable2 running DVWA
- **Network:** Host-only adapter (isolated from internet)
- **Vulnerability:** SQL Injection on DVWA login page

## Quick Start

1. Clone this repository
2. Follow setup instructions in `lab-setup.md`
3. Review the vulnerability findings in `findings/VULN-001.md`

## Key Learnings

- Setting up isolated penetration testing environments
- Identifying and exploiting SQL injection vulnerabilities
- Understanding tautology-based SQL injection techniques
- Documenting security findings professionally
- Importance of parameterized queries and input validation

## Ethical Notice

⚠️ **All testing was performed on personally owned virtual machines in an isolated environment.**

This project is for educational purposes only. Attempting these techniques on systems you do not own or have explicit permission to test is illegal and unethical.

See `PERMISSIONS.md` for detailed ethical guidelines.

## License

MIT License - See LICENSE file for details.

---

**Contact:** Muhammad Khubaib Asif | [LinkedIn](https://linkedin.com/in/khubaib-asif) | [GitHub](https://github.com/khubaib-asif)
