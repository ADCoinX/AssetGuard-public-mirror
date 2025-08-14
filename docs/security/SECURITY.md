# Security Policy — ADC AssetGuard (Public Mirror)

## 1. Overview
This document outlines the **public** security posture for ADC AssetGuard.  
It does **not** contain sensitive production details.

---

## 2. Data Handling Principles
- **No Sensitive Data Stored**: Wallet addresses, token IDs, and NFT metadata are never persisted in logs or databases.
- **Hashed Identifiers**: Temporary, rotating hashes are used for in-memory processing.
- **Aggregate Metrics Only**: Public reports contain only counts and anonymized statistics.

---

## 3. Infrastructure Security
*(Generalised for public disclosure)*  
- Encrypted transport via TLS 1.3.
- API Gateway with WAF (Web Application Firewall).
- IP allowlist for admin endpoints.
- Regular dependency scans & patching.

---

## 4. Threat Mitigation
- **AI Risk Scoring**: Detects patterns linked to known scams or high-risk behaviour.
- **Rate Limiting**: Prevents brute-force or abuse.
- **CORS Restrictions**: API access limited to allowlisted origins.
- **Security Headers**: CSP, HSTS, X-Content-Type-Options, Referrer-Policy.

---

## 5. Compliance
- **ISO 20022-Inspired XML Audit Export**: Standardized export format for integration with compliant systems.
- GDPR-friendly: No personal data is collected.

---

## 6. Reporting Vulnerabilities
If you discover a vulnerability:
1. Email: security@example.com *(dummy for public mirror)*
2. Provide description & steps to reproduce (if safe).
3. Do not publicly disclose until confirmed & patched.

---

## 7. Disclaimer
This document is a **public mirror** version.  
Production environment uses additional controls not listed here.
