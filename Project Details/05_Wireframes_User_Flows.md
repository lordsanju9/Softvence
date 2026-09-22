# Wireframes & User Flows — Lean Prototype

**Version:** 1.0  |  **Date:** September 2026
**Classification:** Confidential — For Qualified Development Partners

## Screen Inventory

1. Landing / Connect Wallet
2. Wallet Dashboard
3. AI Assistant
4. Transaction Detail / Explanation
5. Swap Preparation
6. Transaction Review & Risk Check
7. Result / Transaction Status
8. Basic Error / Unsupported Network State

## Dashboard Structure

```text
+--------------------------------------------------+
| AI Wallet Assistant              [Wallet: 0x...] |
+--------------------------------------------------+
| Portfolio Value | ETH Balance | Network         |
+--------------------------------------------------+
| Assets                         | Recent Activity |
| ETH                            | Tx #1           |
| USDC                           | Tx #2           |
| ...                            | Tx #3           |
+--------------------------------------------------+
| Ask your wallet...                               |
+--------------------------------------------------+
```

## Transaction Review

```text
Requested action: Swap 25 USDC -> ETH
Network: Base Sepolia
From: 0x...
Estimated result: ...
Estimated fee: ...
Simulation: PASS / FAIL / UNAVAILABLE
Policy: PASS / BLOCKED
Risk notes: ...

[Cancel]                         [Approve in Wallet]
```

The vendor may improve the visual design, but the prototype must preserve this safety sequence.
