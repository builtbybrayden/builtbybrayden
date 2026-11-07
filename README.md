# Hi, I'm Brayden 👋

`Application Security Analyst` · `Aspiring Application Security Engineer` · `Independent Security Researcher`

I work in application security day-to-day and spend my own time finding and reporting real vulnerabilities in open source software, building DevSecOps tooling, and leveling up toward an AppSec Engineer role. Six of my findings have been assigned CVEs. I write up the technical details on my [blog](https://builtbybrayden.github.io).

---

## 🔍 Independent Security Research

- **CVE-2026-116201** — Snipe-IT: SAML single sign-on assertion replay. A non-atomic nonce check with no database uniqueness constraint let one captured SAML assertion be replayed into multiple concurrent sessions, so revoking one session left the others alive. Moderate.
  - 📝 [Write-up](https://builtbybrayden.github.io/blog/snipeit-saml-assertion-replay/) · [Advisory (GHSA-w49g-f2jc-qxhg)](https://github.com/grokability/snipe-it/security/advisories/GHSA-w49g-f2jc-qxhg)

- **CVE-2026-116200** — Snipe-IT: LDAP StartTLS downgrade to cleartext. The login code never checked whether the StartTLS upgrade succeeded, so a failed or attacker-stripped handshake sent the directory service-account and every user password across the wire in cleartext while login still looked normal. Moderate.
  - 📝 [Write-up](https://builtbybrayden.github.io/blog/snipeit-ldap-starttls-downgrade/) · [Advisory (GHSA-wx48-r3qh-jvh5)](https://github.com/grokability/snipe-it/security/advisories/GHSA-wx48-r3qh-jvh5)

- **CVE-2026-116199** — Snipe-IT: Google SSO accepted deactivated users. The active-account check was enforced on every login path except Google sign-in, so a deactivated user whose Google identity was still live could log back in at their original permission level. Moderate.
  - 📝 [Write-up](https://builtbybrayden.github.io/blog/snipeit-google-sso-deactivated-user/) · [Advisory (GHSA-xf36-wx48-5rqp)](https://github.com/grokability/snipe-it/security/advisories/GHSA-xf36-wx48-5rqp)

- **CVE-2026-116198** — Snipe-IT: plaintext written to encrypted custom fields. One asset-creation API path skipped encryption but still wrote the value when the caller lacked the encrypted-fields permission, storing plaintext in a column flagged as encrypted and breaking encryption at rest. Low.
  - 📝 [Write-up](https://builtbybrayden.github.io/blog/snipeit-encrypted-field-plaintext-write/) · [Advisory (GHSA-jh4g-98fm-jcqc)](https://github.com/grokability/snipe-it/security/advisories/GHSA-jh4g-98fm-jcqc)

- **CVE-2026-86765** — Snipe-IT: checkout authorization bypass via the asset update endpoint. A role with only asset-edit rights (and checkout explicitly denied) could still check out equipment by pushing assignment fields through a different endpoint than the one that was actually gated. CVSS 6.5.
  - 📝 [Write-up](https://builtbybrayden.github.io/blog/snipeit-asset-update-checkout-bypass/) · [Advisory (GHSA-6g2g-83pc-6365)](https://github.com/grokability/snipe-it/security/advisories/GHSA-6g2g-83pc-6365)

- **CVE-2026-55516** — Snipe-IT: cross-tenant data exposure in multi-company mode. A missing ownership check on maintenance records let a user in one company attach or re-point records onto another company's equipment. CVSS 7.7 (High).
  - 📝 [Write-up](https://builtbybrayden.github.io/blog/snipeit-maintenance-cross-tenant/) · [Advisory (GHSA-575r-357h-fhch)](https://github.com/grokability/snipe-it/security/advisories/GHSA-575r-357h-fhch)

All found and reproduced in an isolated lab, reported through coordinated disclosure, and fixed by the maintainer.

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
- Certified Penetration Testing Specialist (CPTS) — Hack The Box, Oct 2026
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

- 📚 Studying for OSCP and CISSP
- 🎯 Targeting Application Security Engineer roles
- 🔍 Continuing independent vulnerability research and coordinated disclosure
- 🛠️ Hardening the DevSecOps pipeline project for real-world use

---

## 🤝 Connect with Me

- 📝 Blog: https://builtbybrayden.github.io
- 💼 LinkedIn: https://www.linkedin.com/in/builtbybrayden
- 📺 YouTube: https://www.youtube.com/@builtbybrayden1

---

### ✉️ Contact

For collaboration, questions, or just to say hi:
**Email:** brayden@builtbybrayden.com
