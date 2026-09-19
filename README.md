# Hi, I'm Brayden 👋

`Application Security Analyst` · `Aspiring Application Security Engineer` · `Independent Security Researcher`

I work in application security day-to-day and spend my own time finding and reporting real vulnerabilities in open source software, building DevSecOps tooling, and leveling up toward an AppSec Engineer role. Two of my findings have been assigned CVEs. I write up the interesting ones on my [blog](https://builtbybrayden.github.io).

---

## 🔍 Independent Security Research

- **CVE-2026-86765** — Snipe-IT: checkout authorization bypass via the asset update endpoint. A role with only asset-edit rights (and checkout explicitly denied) could still check out equipment by pushing assignment fields through a different endpoint than the one that was actually gated. CVSS 6.5.
  - 📝 [Write-up](https://builtbybrayden.github.io/blog/snipeit-asset-update-checkout-bypass/) · [Advisory (GHSA-6g2g-83pc-6365)](https://github.com/grokability/snipe-it/security/advisories/GHSA-6g2g-83pc-6365)

- **CVE-2026-55516** — Snipe-IT: cross-tenant data exposure in multi-company mode. A missing ownership check on maintenance records let a user in one company attach or re-point records onto another company's equipment. CVSS 7.7 (High).
  - 📝 [Write-up](https://builtbybrayden.github.io/blog/snipeit-maintenance-cross-tenant/) · [Advisory (GHSA-575r-357h-fhch)](https://github.com/grokability/snipe-it/security/advisories/GHSA-575r-357h-fhch)

Both found and reproduced in an isolated lab, reported through coordinated disclosure, and fixed by the maintainer.

---

## 🛠️ AppSec Engineering

- **Self-hosted DevSecOps pipeline** — GitHub Actions (self-hosted runner) triggers SAST (Semgrep) and SCA (OWASP Dependency-Check) scans on every push/PR. An event-driven ingestion service watches for new scan output and automatically imports findings into DefectDojo, tagging them by product/scan type so they land in the right vulnerability-management workflow without manual upload. Currently a personal lab project, being hardened toward something I'd run against real repos.

- **CVE-hunting labs** — Practice environments for fingerprinting real-world software and matching it against known CVEs with Nuclei (detect-then-match workflow), plus hands-on work against intentionally vulnerable applications to sharpen web exploitation skills.

---

## 🎓 Certifications

**Application & Web Security**
- Burp Suite Certified Practitioner (BSCP) — PortSwigger, Apr 2026
- Certified Web Exploitation Specialist (CWES) — Hack The Box, Feb 2026
- Practical Web Pentest Associate — TCM Security, Apr 2024

**Offensive Security & Analysis**
- CompTIA PenTest+ — Dec 2025
- CompTIA CySA+ — Nov 2025
- CompTIA Advanced Security Practitioner (CASP+) — Dec 2025

**Security Management & Governance**
- Certified Information Security Manager (CISM) — ISACA, Dec 2025
- Certified in Cybersecurity (CC) — ISC2, Nov 2025

**IT Service Management**
- ITIL 4 Leader: Digital & IT Strategy — Nov 2025
- ITIL Foundation — Jan 2024

---

## 💻 Technologies & Tools

**AppSec / Security:**
`Burp Suite` · `Semgrep` · `OWASP Dependency-Check` · `Nuclei` · `DefectDojo` · `SIEM` · `EDR`

**Languages:**
`Python` · `PowerShell` · `SQL` · `Java`

**DevOps & Cloud:**
`Docker` · `GitHub Actions` · `Azure` · `Microsoft 365` · `Windows Server`

**IT & Identity:**
`Active Directory` · `Firewalls` · `Ticketing Systems (Freshservice / ServiceNow)`

---

## 🎯 Current Focus

- 📚 Studying for CPTS, OSCP, and CISSP
- 🎯 Targeting Application Security Engineer roles
- 🔍 Continuing independent vulnerability research and coordinated disclosure
- 🛠️ Hardening the DevSecOps pipeline project for real-world use

---

## 🤝 Connect with Me

- 📝 Blog: https://builtbybrayden.github.io
- 💼 LinkedIn: https://www.linkedin.com/in/brayden-arnold-5387b3199/
- 📺 YouTube: https://www.youtube.com/@builtbybrayden1

---

### ✉️ Contact

For collaboration, questions, or just to say hi:
**Email:** brayden@builtbybrayden.com
