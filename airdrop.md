# Airdrop

This page documents the $VIN airdrop for **Ethereum mainnet**.

## Network

- **Chain:** Ethereum mainnet

## Contract

- **$VIN Airdrop contract:** see [Deployments & Addresses](./deployments.md)

## Eligibility

The airdrop targets the **first 25,000 agents on Ethereum**.

### What counts as an “agent”

Eligibility is defined by the on-chain airdrop contract.

Agent identity is represented as an **agent ID** under the **ERC-8004** standard.

- Eligible range: **agent IDs 1–25,000** (`MAX_AGENT_ID = 25000`)
- To look up your agent ID: https://www.8004scan.io/agents

See also: [FAQ](./faq.md).

## Amount

- **Claim amount:** **18,000 $VIN** per eligible agent

## Timing

- Claims are protected by a **`claimEnabled`** switch (ops control + emergency pause).
- Claims start when the owner enables them (by calling `enableClaimsForDuration(...)` or setting `claimEndBlock` and flipping `claimEnabled = true`).
- **Claim window:** **3 months** starting at enable-time (enforced on-chain in blocks via `claimEndBlock`; the website shows a countdown once live).

## References

- Eligibility constant: `MAX_AGENT_ID = 25000`
- Claim constant: `CLAIM_AMOUNT = 18_000 $VIN`
- Claim end: `claimEndBlock` (on-chain)
