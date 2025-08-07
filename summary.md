# Task 3 - Vulnerability Scan Summary

## 🔍 Target
- IP: 192.168.31.1 (Router)
- Scan Type: Full vulnerability scan using OpenVAS (GVM)

## 🧪 Tools Used
- Kali Linux
- OpenVAS / GVM
- Greenbone Security Assistant (GSA) Web Interface

## 🕵️ Vulnerabilities Found
1. **SSL/TLS: Renegotiation MITM Vulnerability (CVE-2009-3555)**
   - Threat: Medium (CVSS 5.8)
   - Risk: MITM attacks through improper SSL/TLS renegotiation
   - Fix: Disable renegotiation or apply vendor patches (RFC5746)

2. **SSL/TLS: Renegotiation DoS Vulnerability (CVE-2011-1473, CVE-2011-5094)**
   - Threat: Medium (CVSS 5.0)
   - Risk: Resource exhaustion via repeated SSL handshakes
   - Fix: Disable client-initiated renegotiation

## 📌 Conclusion
While no high-risk vulnerabilities were detected, medium-risk TLS issues indicate a need to harden router SSL/TLS configurations. This task demonstrates proactive threat detection using OpenVAS.