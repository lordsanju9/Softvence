# Assumptions, Risks & Dependencies — Lean Prototype

**Version:** 1.0  |  **Date:** September 2026
**Classification:** Confidential — For Qualified Development Partners

## Assumptions

- Client provides timely product decisions and access to required accounts.
- Vendor uses managed RPC/indexing services rather than building an indexing network.
- Only two testnet networks are mandatory.
- MetaMask is the mandatory wallet.
- Only one swap integration is required.
- No private-key custody is required.
- Third-party service fees are paid directly by Client and are outside engineering fees unless explicitly included.

## Key Risks

1. Testnet liquidity may be unavailable for a selected swap route.
2. Blockchain providers may impose rate limits.
3. AI responses may be inaccurate without strong tool grounding.
4. Transaction simulation behavior differs by chain/provider.
5. Additional wallets/chains can expand scope rapidly.

## Mitigation

Use a controlled integration, small allowlists, testnet assets, deterministic validation, and early technical spikes. If a live testnet swap cannot be reliably demonstrated, the vendor shall provide a controlled transaction-building demonstration rather than expand scope.

## Change Control

Any request outside this document requires written impact assessment for cost, schedule, and security.
