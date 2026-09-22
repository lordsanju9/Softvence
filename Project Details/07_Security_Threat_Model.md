# Security Threat Model — Lean Prototype

**Version:** 1.0  |  **Date:** September 2026
**Classification:** Confidential — For Qualified Development Partners

## Primary Threats

| Threat | Control |
|---|---|
| Prompt injection causes unsafe action | AI cannot authorize transactions; deterministic policy layer |
| Hallucinated balance/transaction facts | AI must use authoritative read tools |
| Wrong network | Chain allowlist + wallet/network verification |
| Wrong token/address | Token and address validation/allowlists |
| Excessive transaction amount | Prototype spending threshold |
| Malicious contract interaction | Restrict to approved transaction types/integrations |
| Private-key exposure | Never request, transmit, or store seed/private keys |
| Wallet phishing UX | Clear domain/app identity and explicit wallet confirmation |
| Replay/duplicate submission | Track request state; no blind automatic retry |
| Third-party outage | Safe failure and clear user messaging |

## Prototype Transaction Policy

Default policy should allow only:
- Approved testnet chains.
- Approved token contracts.
- Approved transaction type(s).
- Amount below a configurable prototype limit.
- Successful or explicitly handled simulation result.
- Explicit user approval.

## Security Principle

**AI may propose; deterministic application code validates; the user signs.**

A formal independent security audit is outside the base USD 200,000 prototype budget and may be quoted separately as an optional service.
