# Client — AI Wallet Assistant Lean Prototype Project Brief

**Document status:** Vendor Solicitation Draft — Lean Prototype
**Version:** 2.0
**Date:** September 2026
**Commercial target:** **USD 200,000 maximum**
**Classification:** Confidential — For Qualified Development Partners

## 1. Executive Summary

The client is seeking a qualified technology partner to build a lean proof-of-product for an AI-powered cryptocurrency wallet assistant.

The prototype will demonstrate that a user can connect a non-custodial EVM wallet, understand wallet and transaction data through natural language, receive AI-assisted portfolio/transaction analysis, and safely prepare and simulate a limited transaction before explicit wallet approval.

This is intentionally **not** a full production Web3 platform. The goal is to validate product desirability, architecture, AI/tool orchestration, and secure transaction UX within a tightly controlled prototype scope and a maximum budget of USD 200,000.

## 2. Client Overview

The client is seeking a qualified technology partner to build the prototype.

Client-specific corporate profile details are intentionally omitted from this vendor package.

## 3. Business Problem

Crypto wallets expose powerful but complex information: balances, transactions, gas fees, token movements, contract interactions, and DeFi activity. Many users need a simpler way to understand this information without giving an AI unrestricted control over their assets.

## 4. Product Vision

> Let users understand their wallet and prepare safe blockchain actions using natural language, while keeping signing authority in the user's wallet.

Example prototype interactions:
- “How much ETH do I have?”
- “Explain my latest transaction.”
- “How much did I spend on gas?”
- “What are my biggest holdings?”
- “Show me my recent token activity.”
- “Prepare a swap of 25 USDC to ETH.”

## 5. Prototype Advantages

### User advantages
- Natural-language wallet intelligence.
- Plain-English transaction explanations.
- Faster access to portfolio information.
- Clear transaction previews before signing.

### Business advantages
- Demonstrates an AI-native Web3 product concept.
- Creates a reusable foundation for a future commercial product.
- Enables early user testing before a large production investment.

### Technical advantages
- Tool-based AI architecture instead of unrestricted agent access.
- Deterministic transaction validation.
- Simulation before signing where supported.
- Non-custodial signing flow.

## 6. Lean Prototype Scope

The fixed-price prototype shall include:

1. Cross-platform web application plus mobile companion applications (iOS and Android) using a shared backend and wallet-connect architecture.
2. EVM networks: **Ethereum Sepolia and Base Sepolia** for transaction workflows.
3. Wallet connection: **MetaMask** as the sole required wallet integration.
4. Native ETH and selected ERC-20 token balances.
5. Recent transaction history.
6. AI wallet Q&A using approved blockchain data tools.
7. Human-readable transaction explanations.
8. Basic portfolio summary.
9. One supported swap workflow on testnet or a mocked/controlled quote path if live testnet liquidity is unavailable.
10. Transaction simulation where technically supported.
11. Deterministic policy checks.
12. Explicit user approval and wallet signing.
13. Basic monitoring, logging, automated tests, and deployment.

## 7. Explicitly Out of Scope

- Custody or storage of private keys.
- Autonomous transaction execution.
- Production mainnet trading.

- NFT marketplace functionality.
- Broad DeFi position tracking.
- Multi-chain indexing platform.
- Smart-account automation.
- Session keys.
- Custom smart contracts unless specifically approved as a small prototype component.
- Tax, accounting, investment, or legal advice.
- Formal third-party smart-contract/security audit.
- Enterprise SLA/24×7 operations.

## 7A. Mobile Application Scope

The mobile prototype shall include:

- iOS and Android companion applications using React Native, Flutter, or equivalent cross-platform technology.
- Wallet connection support compatible with mobile wallet workflows (WalletConnect or equivalent).
- Secure mobile session management.
- Mobile dashboard for balances, portfolio summary, and recent activity.
- Mobile AI assistant chat experience.
- Push notifications for transaction status updates and important wallet events.
- Mobile transaction review screen before redirecting to wallet signing.
- Biometric/app-lock protection for local application access where supported.

The mobile application must maintain the same non-custodial security model as the web experience.

## 8. Prototype Success

The prototype is successful when a reviewer can connect a test wallet, retrieve reliable wallet information, ask meaningful questions, inspect an understandable transaction explanation, prepare a supported transaction, see deterministic security checks, simulate it where supported, and sign it explicitly through the wallet.
