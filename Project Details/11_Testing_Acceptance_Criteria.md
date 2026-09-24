# Testing & Acceptance Criteria — Lean Prototype

**Version:** 1.0  |  **Date:** September 2026
**Classification:** Confidential — For Qualified Development Partners

## Test Levels
- Unit tests for business-critical logic.
- API/integration tests for blockchain and AI tool boundaries.
- End-to-end tests for wallet connection and core user journeys.
- Security-focused tests for authorization and transaction validation.
- Manual exploratory testing.

## Mandatory Acceptance Tests

### AT-01 Wallet
A test wallet connects, disconnects, and displays the correct address/network.

### AT-02 Portfolio
Native and configured token balances are retrieved and displayed from approved sources.

### AT-03 AI Grounding
A wallet-balance question causes an approved data tool call rather than an invented answer.

### AT-04 Transaction Explanation
A known test transaction is decoded and explained with correct token movement and fee information.

### AT-05 Unsafe Action
An unsupported chain/token/action or over-limit transaction is blocked before signing.

### AT-06 Simulation
A supported transaction displays simulation status or a clear “simulation unavailable” state without falsely claiming success.

### AT-07 User Approval
No blockchain signing occurs until the user explicitly approves the review screen.

### AT-08 Key Safety
Testing confirms the application never receives or stores the wallet seed phrase/private key.

### AT-09 Failure Handling
Wallet rejection, RPC failure, AI failure, and quote failure produce safe recoverable states.

### AT-10 Handover
Client can run the project from the supplied documentation and repository.
