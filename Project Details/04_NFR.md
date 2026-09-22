# Non-Functional Requirements — Lean Prototype

**Version:** 1.0  |  **Date:** September 2026
**Classification:** Confidential — For Qualified Development Partners

## Performance
- Normal read-only API requests should target <3 seconds excluding third-party latency.
- AI responses should target <10 seconds under normal conditions.
- UI should remain responsive during asynchronous blockchain requests.

## Security
- No private keys or seed phrases may enter Client/vendor servers.
- Secrets must be stored in environment/secret management systems, not source control.
- Server-side transaction tools must use an explicit allowlist.
- AI output must never directly authorize a transaction.
- All transaction parameters must be validated outside the LLM.

## AI Usage Controls
- Rate limiting and/or usage caps on AI/LLM calls per session to control cost and abuse.
- Basic logging of AI tool-call volume for cost monitoring.

## Reliability
- Graceful handling of wallet rejection, RPC failure, quote failure, simulation failure, and AI outage.
- Failed external calls must not result in automatic retries that could duplicate a transaction.

## Privacy
- Collect only data required for the prototype.
- Document what conversation and wallet-address data is retained.
- Do not store seed phrases/private keys.

## Accessibility
- Target WCAG 2.1 AA for core flows (wallet connect, dashboard, transaction review, sign) where practical for a prototype.
- Keyboard-navigable core flows; no critical action reachable only by mouse.

## Browser & Device Support
- Supported: latest stable Chrome, Firefox, and Edge on desktop.
- Responsive web experience plus dedicated cross-platform mobile applications for iOS and Android prototype acceptance.

## Maintainability
- Type-safe APIs where practical.
- Environment-specific configuration.
- Clear README and setup instructions.
- Basic architecture and ADR documentation.

## Availability
- Prototype target: 99% monthly availability excluding planned maintenance and third-party outages.
- No 24/7 SLA is required.
