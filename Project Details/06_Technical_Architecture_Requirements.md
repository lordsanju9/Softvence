# Technical Architecture Requirements — Lean Prototype

**Version:** 1.0  |  **Date:** September 2026
**Classification:** Confidential — For Qualified Development Partners

## 1. Required Architecture

```text
Web UI
  -> Backend API
      -> AI Orchestrator
          -> Approved Read Tools
          -> Structured Action Builder
      -> Blockchain Service
          -> RPC / Indexer Provider
      -> Policy & Validation Engine
      -> Simulation Service
      -> Approved Swap Integration

Wallet <-> Web UI for signing
```

## 2. Architecture Principles

- Non-custodial.
- Server never receives private keys.
- LLM is not the security boundary.
- Deterministic code validates every action.
- Transaction construction is separate from AI interpretation.
- Provider dependencies are isolated behind service interfaces.

## 3. Recommended Technology Direction

Vendor may propose alternatives. A reasonable baseline is React/Next.js, TypeScript, Node.js, PostgreSQL or equivalent, an EVM library such as viem/ethers, managed RPC/indexing, and a mainstream LLM API.

## 4. Blockchain Scope

- Ethereum Sepolia.
- Base Sepolia.
- Mainnet support is out of scope for the fixed prototype; all transaction workflows shall use Ethereum Sepolia and Base Sepolia.

## 5. AI Architecture

AI may select from a small, explicitly defined tool set. Tools should return structured data. The model should not be trusted to calculate balances, validate addresses, enforce limits, or determine authorization.

## 6. Data

A persistent database is required only for application/session configuration and minimum necessary history. Blockchain remains the authoritative source for on-chain state.

## 7. Infrastructure

One staging/demo environment is sufficient. Infrastructure-as-code is optional; enterprise-grade infrastructure complexity is out of scope.
