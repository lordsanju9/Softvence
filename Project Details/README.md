# Client — AI Wallet Assistant Lean Prototype Vendor Package

**Version:** 2.0  
**Classification:** Confidential — For Qualified Development Partners  
**Target:** Lean prototype  
**Budget:** USD 200,000 maximum  
**Schedule:** Approximately 20 weeks

## Purpose

This package defines a deliberately constrained prototype designed to validate the core AI + wallet concept without attempting to build a full commercial Web3 platform. The USD 200,000 ceiling requires strict prioritization of P0 functionality and lean implementation choices.

## Core Demonstration

**Connect wallet → understand wallet → ask AI → explain transaction → prepare limited action → deterministic security checks → simulate → user reviews → user signs.**

## Mandatory Scope

- Web only.
- MetaMask.
- Ethereum Sepolia + Base Sepolia.
- Native ETH + selected ERC-20s.
- Basic transaction history/decoding.
- AI wallet Q&A.
- Transaction explanations.
- One limited swap/action integration.
- Policy validation.
- Simulation where supported.
- Explicit wallet signing.
- Basic QA, CI/CD, deployment, documentation.

## Major Exclusions

No custody, autonomous trading, broad DeFi, NFT platform, smart-account automation, multi-chain indexing, production mainnet execution, or formal third-party audit. Mobile applications are included only as a controlled companion experience for the prototype.

## Commercial Position

The vendor should quote this as a fixed-price lean prototype. Third-party API/RPC/LLM fees and independent audits should be separately identified.

## Client

Client-specific corporate information is intentionally omitted from this vendor package.

## Glossary

- **Non-custodial** — The application never holds, stores, or has access to the user's private keys or seed phrase; the wallet itself always signs.
- **Allowlist** — An explicit, pre-approved list (of chains, tokens, or transaction types) that the system will act on; anything not listed is rejected by default.
- **Policy engine** — Deterministic (non-AI) application code that checks a proposed transaction against rules (chain, token, amount, etc.) before it can proceed.
- **Simulation** — A dry-run of a transaction against current chain state to predict its outcome before the user signs, without broadcasting it.
- **Structured intent / structured action** — A user's natural-language request converted into a fixed, validated data format (e.g. token, amount, chain) that deterministic code — not the AI — acts on.
- **Tool calling** — The AI's ability to invoke a predefined, approved function (e.g. "get balance") to retrieve real data, rather than generating an answer from memory.
- **Testnet** — A blockchain network used for testing (Ethereum Sepolia, Base Sepolia) with no real monetary value, as opposed to mainnet.
- **RPC / Indexer** — Services used to read blockchain data (balances, transactions) without running your own blockchain node.

This document package is a vendor solicitation draft and does not replace legal, regulatory, or security advice.
