# Secure Cloud-Native Portfolio Infrastructure
A high-performance, hardened professional portfolio architected on **Azure Static Web Apps (SWA)** with automated **CI/CD** integration.

## 🏗️ Architecture Overview
This project goes beyond frontend design, focusing on **Cloud Infrastructure** and **Edge Security**. The site is hosted on Azure's global network to ensure sub-second latency and enterprise-grade protection.

- **Cloud Provider:** Azure (Static Web Apps)
- **Deployment Pipeline:** GitHub Actions (CI/CD)
- **Security Layer:** Azure Enterprise-grade Edge & Custom Security Headers
- **DNS Management:** [Insert your DNS Provider, e.g., Azure or Namecheap]

---

## 🛡️ Security Hardening & Compliance
To protect the site from common web vulnerabilities, I implemented a custom `staticwebapp.config.json` configuration to enforce strict security policies:

### 1. Security Headers (OWASP Best Practices)
I configured the following headers to harden the attack surface:
* **HSTS (Strict-Transport-Security):** Forces all browser communication over encrypted HTTPS for 1 year.
* **X-Frame-Options (DENY):** Prevents Clickjacking attacks by forbidding the site from being rendered in an iframe.
* **X-Content-Type-Options (nosniff):** Mitigates MIME-type sniffing vulnerabilities.

> **[INSERT SCREENSHOT: Your SecurityHeaders.com 'A' or 'B' Grade Here]**
> *Figure 1: Verified security audit showcasing successful header implementation.*

### 2. Secret Management
Used **GitHub Secrets** to securely store Azure Deployment Tokens. This ensures that no sensitive API keys or infrastructure credentials are exposed in the public source code, following the **Principle of Least Privilege**.

---

## 🚀 DevOps Workflow (CI/CD)
The project utilises a fully automated deployment pipeline. 
1. **Code:** Developed in Cursor AI.
2. **Push:** Git push triggers a **GitHub Action**.
3. **Build/Deploy:** Azure SWA automatically builds the production environment and applies security configurations.

> **[INSERT SCREENSHOT: Your GitHub Actions tab with a Green Checkmark]**
> *Figure 2: Automated CI/CD pipeline verifying successful builds.*

---

## 🛠️ Tech Stack
* **Hosting:** Azure Static Web Apps (Standard/PAYG Tier)
* **Framework:** HTML5 / CSS3 (Responsive Design) / JavaScript
* **Version Control:** Git & GitHub
* **Hardening:** JSON-based Infrastructure as Code (IaC)
