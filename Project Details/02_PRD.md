# Product Requirements Document — Lean AI Wallet Assistant

**Version:** 2.1  | **Target budget:** USD 200,000  | **Release:** Lean Prototype

## 1. Product Goal

Validate a conversational wallet assistant that combines authoritative blockchain data with an AI interface while preserving user-controlled signing.

## 2. Primary Personas

- **Beginner:** wants balances and transactions explained simply.
- **Active wallet user:** wants quick portfolio and activity answers.
- **Web3 evaluator:** wants to test AI-assisted transaction preparation safely.

## 3. Core User Journeys

### A. Connect Wallet
1. Open web app.
2. Connect MetaMask.
3. Detect network and wallet address.
4. Retrieve supported assets.
5. Display dashboard.

### B. Ask a Question
1. User asks a natural-language question.
2. AI determines intent.
3. AI calls an approved read-only tool.
4. Tool retrieves blockchain data.
5. AI explains the result.

### C. Explain a Transaction
1. User selects a transaction.
2. Backend decodes known fields and token movements.
3. AI receives structured facts.
4. UI displays plain-English explanation, fees, assets moved, and risk indicators.

### D. Prepare and Sign a Swap
1. User requests a supported swap.
2. AI converts the request into structured parameters.
3. Backend validates parameters.
4. Quote/transaction data is obtained from the approved integration.
5. Simulation is attempted.
6. Policy engine evaluates the action.
7. User sees the exact action summary.
8. User explicitly approves.
9. Wallet performs signing.
10. UI reports submission and confirmation status.

## 4. Functional Scope

### Wallet
- Connect/disconnect MetaMask.
- Display address and chain.
- Request network switch.
- Handle rejection, timeout, and wrong-network states.

### Portfolio
- Native ETH balance.
- Up to 10 configured ERC-20 tokens per network.
- Approximate USD valuation using an approved price source.
- Simple allocation view.

### Transactions
- Last 20 supported wallet transactions.
- Transaction hash, status, timestamp, gas/fee, token movements.
- Basic known-contract decoding.

### AI
- Natural-language Q&A.
- Tool calling for wallet data.
- Transaction explanation.
- Missing-parameter clarification.
- Structured action extraction for supported swap requests.

### Swap prototype
- One swap integration selected during discovery.
- One or two configured token pairs.
- Testnet or controlled demo path.
- No autonomous execution.

### Security
- Deterministic allowlist for supported chains, tokens, and actions.
- Spending/amount threshold for prototype.
- Simulation before signing where available.
- User confirmation screen.
- No private-key access by application servers.

## 5. Product Non-Goals

No mobile app, no custodial wallet, no autonomous agent, no unrestricted DeFi actions, and no production financial-service launch are part of this release.

## 6. Prototype Acceptance

A feature is accepted when it works in the agreed staging environment, has automated coverage appropriate to its risk, has documented limitations, and passes the relevant acceptance test.
