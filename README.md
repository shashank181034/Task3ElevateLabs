# 🛡️ Task 3 – Basic Vulnerability Scan using OpenVAS (Greenbone Vulnerability Management)

## 📌 Objective

Perform a **basic vulnerability scan** on a target machine (router) using **OpenVAS** in **Kali Linux**, identify any known vulnerabilities, and generate a professional security report.

---

## 🧰 Tools Used

- 🐧 Kali Linux (pre-installed OpenVAS/GVM 25.04)
- 🟢 Greenbone Vulnerability Management (GVM)
- 🌐 Greenbone Security Assistant (Web UI)
- 📄 PDF report generated from scan results

---

## 🎯 Target Details

| Parameter        | Value           |
|------------------|------------------|
| Target IP        | `192.168.**.*` *(Local router)* |
| Scan Profile     | Full and fast    |
| Total Scan Time  | ~5 hours         |

---

## 🧪 Vulnerabilities Identified

### ⚠️ Medium Severity (2 vulnerabilities):
1. **SSL/TLS: Renegotiation MITM Vulnerability (CVE-2009-3555)**
   - ❗ Risk: Man-in-the-middle attacks during TLS renegotiation.
   - ✅ Fix: Disable insecure renegotiation or ensure support for RFC5746.

2. **SSL/TLS: Renegotiation DoS Vulnerability (CVE-2011-1473, CVE-2011-5094)**
   - ❗ Risk: Denial-of-service via repeated renegotiation requests.
   - ✅ Fix: Disable client-initiated renegotiation or patch firmware.

> 🔐 No **High** or **Critical** severity vulnerabilities were found.

---
