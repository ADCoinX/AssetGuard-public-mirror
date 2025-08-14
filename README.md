# ADC AssetGuard (Public Overview)

**Security-first Web3 asset validation tool**  
This is a public mirror repository for grant reviewers and the community.  
It contains non-sensitive documentation and example files only.  
Core implementation, API keys, and infrastructure details are kept private for security reasons.

---

## 🔍 Overview
**AssetGuard** validates tokens, coins, and NFTs across multiple chains using AI-powered risk scoring.

---

## 🛡 Security-first Design
- **Stateless**: No PII stored; all processing done in-memory.
- **Aggregate Logging Only**: Counts & metrics, no wallet or asset addresses stored.
- **Multi-layer Security**:
  - TLS enforced
  - Security headers (HSTS, CSP, X-Frame-Options, Referrer-Policy)
  - CORS allowlist
  - Rate limiting + WAF

For more, see:
- [`docs/security/SECURITY.md`](docs/security/SECURITY.md)
- [`docs/security/DATAFLOW.md`](docs/security/DATAFLOW.md)
- [`docs/security/ISO-sample.xml`](docs/security/ISO-sample.xml)

---

## 📊 Example Aggregate Metrics
*(Dummy data for illustration)*

{
“date”: “2025-01-01”,
“total_requests”: 1250,
“unique_assets_hashed_rotating”: 732,
“chains_touched”: 4,
“high_risk_flags”: 37
}

---

## 📢 Security Disclosure
If you discover a vulnerability, please report it responsibly:  
**Email:** security@example.com *(dummy address)*

---

# Public Mirror Disclaimer

This repository is a **public mirror** intended for transparency with grant reviewers and the community.
It includes only non-sensitive documentation and example files.

- No production credentials, private keys, or personal data are present.
- Core implementation (AI scoring logic, infrastructure, configurations) is kept **private** to protect users and prevent abuse.
- We can provide restricted access to the full source code **upon request under NDA** for formal security review.

For security matters: security@example.com (dummy address).
