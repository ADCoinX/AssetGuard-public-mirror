# Data Flow — ADC AssetGuard (Public Mirror)

## 1. Overview
This document describes a **public** view of how data flows through ADC AssetGuard.  
Sensitive infrastructure details are removed for security reasons.

---

## 2. Process Flow
**Step 1 — User Input**  
- User submits wallet address, token ID, or NFT contract address.  
- Request sent via HTTPS to AssetGuard API.

**Step 2 — Pre-Validation**  
- Format & checksum check.  
- Remove invalid or malformed inputs.

**Step 3 — AI Risk Analysis**  
- Public mirror shows only high-level categories:
  - Scam Pattern Detection
  - Risk Score Calculation (0–100)
  - Suspicious Contract Interaction Alerts

**Step 4 — Aggregation & Output**  
- Risk score & summary returned to user.  
- Public logs store only anonymized metrics.

---

## 3. Public Data Flow Diagram
```mermaid
flowchart TD
    A[User Device] -->|HTTPS Request| B[AssetGuard API]
    B --> C[Input Validation]
    C --> D[AI Risk Analysis Engine]
    D --> E[Risk Score + Summary Output]
    E --> A
