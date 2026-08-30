# Emmanuel Ajayi — Security Engineer

Cloud security, application security, and detection engineering — with a focus on building controls that work, automating what can be automated, and leaving systems better documented than I found them.

I work across the full security stack: designing AWS detection pipelines, hardening AI-driven SaaS platforms, threat modelling APIs and LLM integrations, shipping CI/CD security controls, and building GRC programmes from the ground up. I care about signal quality, measurable outcomes, and security that developers can actually work with.

---

## Areas of Focus

- Cloud security engineering (AWS) and detection engineering
- AI & LLM security — threat modelling agentic systems, scoping third-party model exposure, securing AI-driven SaaS platforms
- Application security — STRIDE threat modelling, API security, secrets lifecycle, multi-tenant data isolation
- SIEM operations — Splunk, Microsoft Sentinel, KQL, MITRE ATT&CK-mapped detections
- DevSecOps — CI/CD hardening, secrets detection, secure-by-default developer workflows
- GRC — ISO 27001:2022, PCI DSS, SOC 2, UK GDPR, risk registers, runbook authoring

---

## Featured Work

### 🏗️ Secure Multi-Tenant BaaS / Lending Platform — Reference Architecture
🔗 https://github.com/Emmy241/secure-multitenant-baas-lending

A secure-by-design reference architecture for a fictional multi-tenant Banking-as-a-Service and lending platform. Built as a teaching artifact — every finding is framed as a reusable, explainable pattern.

Covers:
- Six trust boundaries with STRIDE-per-boundary threat modelling
- Tenant isolation: demonstrates why PostgreSQL RLS enforces nothing while the app connects as an owner role — specifies the correct non-privileged connection role + FORCE RLS as the true enforcement mechanism, with a CI check that fails the build if the effective role is over-privileged
- LLM scoping: keeps cardholder data out of the third-party LLM path to hold the provider outside PCI DSS scope; threat models the agentic API surface for prompt injection and data exfiltration risks
- Money-movement controls: deterministic maker-checker authorization gating all transfers
- GRC overlay: PCI DSS, GLBA, AML/KYC, fair lending — formula-driven risk register with inherent → residual CIA scoring

---

### 🔍 SIEM Monitoring & Incident Response (Microsoft Sentinel)
🔗 https://github.com/Emmy241/SIEM-Monitoring-Incident-Response-Microsoft-Sentinel-

SOC-style detection environment built to detect and investigate:
- Credential abuse and brute-force authentication attempts
- Privilege escalation via administrative logons
- Network reconnaissance using Azure NSG flow telemetry

Includes custom analytics rules, MITRE ATT&CK mapping (T1110, T1078, T1049), and professional incident reports with structured triage documentation.

---

### 🔐 OAuth Abuse Detection & Incident Response
🔗 https://github.com/Emmy241/oauth-abuse-incident-response

Detection and investigation of authentication abuse scenarios involving valid OAuth tokens — focusing on post-compromise misuse rather than initial credential theft. Includes alert triage, log correlation, and incident documentation aligned with real-world SOC workflows.

---

## Selected Projects

- **SIEM Log Monitoring — Splunk**  
  Detection and analysis of suspicious activity using correlated system and authentication logs, with investigative queries and structured alert context.  
  🔗 https://github.com/Emmy241/SIEM-Log-Monitoring-Splunk

- **Vulnerability Assessment — DVWA & Nessus**  
  Web application assessment aligned with OWASP Top 10 — findings prioritization, impact analysis, and developer-facing remediation guidance.  
  🔗 https://github.com/Emmy241/DVWA-Vulnerability-Assessment

- **Web Application Security Testing — OWASP ZAP**  
  Identification of XSS, authentication flaws, and insecure configurations through active scanning and analysis.  
  🔗 https://github.com/Emmy241/OWASP-ZAP-WebTest

---

## Tooling & Domains

**Cloud & Infrastructure**  
AWS (IAM, CloudTrail, CloudWatch, EventBridge, SNS, EC2, ECS) · least-privilege IAM · cloud detection engineering · misconfiguration review

**AI & LLM Security**  
LLM API exposure scoping · prompt injection threat modelling · agentic workflow authorization · keeping sensitive data out of third-party model paths · OWASP LLM Top 10

**SIEM & Detection**  
Microsoft Sentinel · Splunk · KQL · MITRE ATT&CK · detection authoring and tuning · response playbook authoring

**Application & API Security**  
Burp Suite · OWASP Top 10 · OWASP ZAP · STRIDE threat modelling · OAuth/JWT hardening · PostgreSQL RLS · secrets management

**Vulnerability Management**  
Nessus · Nmap · CVE/CVSS triage · remediation tracking to verified closure

**DevSecOps**  
Pre-commit secrets detection · SAST/DAST pipeline integration · dependency scanning · CI/CD security controls · GitHub Actions

**Programming & Automation**  
Python · JavaScript/TypeScript · Bash · SQL · Git

**GRC & Frameworks**  
ISO 27001:2022 · NIST CSF · PCI DSS · SOC 2 · UK GDPR · risk registers · runbook authoring

---

## Certifications

- CompTIA Security+ (SY0-701)

---

## Connect

- LinkedIn: https://www.linkedin.com/in/emmanuelajayi241
- TryHackMe: https://tryhackme.com/p/ajayiemmy241
