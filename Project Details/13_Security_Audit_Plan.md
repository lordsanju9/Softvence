# Security & Audit Plan — Lean Prototype

**Version:** 1.0  |  **Date:** September 2026
**Classification:** Confidential — For Qualified Development Partners

This engagement is a prototype, not a production financial-service launch. Security controls are nevertheless mandatory for all transaction-related functionality.

## Required Reviews
- Threat-model review.
- Dependency/security scan.
- API authorization review.
- Wallet-signing flow review.
- AI prompt-injection/tool-authorization tests.
- Transaction validation tests.

## Release Gate

No critical security issue may remain open in the prototype acceptance build. High-risk findings affecting transaction authorization must be fixed before demonstration of signing functionality.

## Explicit Exclusion

Independent penetration testing, formal smart-contract audit, SOC/ISO certification work, and production financial-service compliance are outside the base USD 200,000 scope. Vendors may price independent penetration testing or audit work separately as optional services.
