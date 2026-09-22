# Functional Requirements — Lean Prototype

**Version:** 1.0  |  **Date:** September 2026
**Classification:** Confidential — For Qualified Development Partners

| ID | Requirement | Priority | Acceptance Summary |
|---|---|---|---|
| FR-01 | Connect MetaMask | P0 | Test wallet connects and address is displayed |
| FR-02 | Detect supported network | P0 | Unsupported network produces clear guidance |
| FR-03 | Read native ETH balance | P0 | Balance matches approved RPC/indexer source within documented timing |
| FR-04 | Read configured ERC-20 balances | P0 | Configured tokens display correctly |
| FR-05 | Display portfolio value | P1 | Price source and timestamp are visible |
| FR-06 | Display recent transactions | P0 | At least 20 recent supported transactions can be shown |
| FR-07 | Decode basic token transfers | P0 | Known ERC-20 movements are identified |
| FR-08 | Explain transactions with AI | P0 | Explanation is based on structured retrieved facts |
| FR-09 | Answer wallet questions | P0 | AI uses approved read-only tools for wallet facts |
| FR-10 | Reject unsupported requests | P0 | Unsupported action is not executed and user receives explanation |
| FR-11 | Parse swap request | P0 | Supported token/amount pair becomes structured intent |
| FR-12 | Obtain swap quote/transaction | P0 | Approved integration returns usable data or controlled demo response |
| FR-13 | Simulate transaction | P0 | Simulation result is displayed when supported |
| FR-14 | Apply policy checks | P0 | Chain/token/action/amount rules are evaluated deterministically |
| FR-15 | User confirmation | P0 | User sees action summary before wallet signing |
| FR-16 | Wallet signing | P0 | Application requests signature through wallet; server never receives private key |
| FR-17 | Transaction status | P1 | Submitted/confirmed/failed state is displayed |
| FR-18 | Basic error handling | P0 | RPC, AI, wallet, and integration failures produce safe messages |
| FR-19 | Conversation history | P1 | Current-session conversation can be viewed |
| FR-20 | Basic admin configuration | P1 | Authorized operator can configure supported tokens/rules without code change where practical |
| FR-21 | Mobile application access | P0 | iOS and Android users can access wallet intelligence features through supported mobile wallet connection flows |
| FR-22 | Mobile AI assistant | P1 | Mobile users can ask wallet questions and receive tool-grounded answers |
| FR-23 | Mobile transaction review | P0 | Mobile users see the same deterministic security review before wallet signing |
| FR-24 | Mobile notifications | P1 | Users receive transaction lifecycle updates where supported |

**P0** = mandatory for prototype. **P1** = included only if budget permits without delaying P0 scope.
