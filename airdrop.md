# Airdrop

This page documents the $VIN airdrop for **Ethereum mainnet**.

> Implementation reference: `vincentaidao/vincent-contracts`.

## Network

- **Chain:** Ethereum mainnet

## Contract

- **$VIN Airdrop contract:** see [Deployments & Addresses](./deployments.md)

## Eligibility

The airdrop targets the **first 25,000 agents on Ethereum**.

### What counts as an “agent”

Eligibility is defined by the on-chain airdrop contract.

In the reference implementation, eligibility is expressed as an **agent ID** with `MAX_AGENT_ID = 25000`. The specific mechanism that maps users → agent IDs (registry, NFT, etc.) is part of the deployed system and will be linked in [Deployments & Addresses](./deployments.md).

See also: [FAQ](./faq.md).

## Amount

- **Claim amount:** **18,000 $VIN** per eligible agent

## Timing

- Claims are protected by a **`claimEnabled`** switch (ops control + emergency pause).
- Claims start when the owner enables them (by calling `enableClaimsForDuration(...)` or setting `claimEndBlock` and flipping `claimEnabled = true`).
- **Claim window:** **3 months** starting at enable-time (enforced on-chain in blocks via `claimEndBlock`; the website shows a countdown once live).

## References

- Repo (implementation reference): https://github.com/vincentaidao/vincent-contracts
- Contract (reference): `contracts/VINAirdrop.sol`
- Eligibility constant: `MAX_AGENT_ID = 25000`
- Claim constant: `CLAIM_AMOUNT = 18_000 $VIN`
- Claim end: `claimEndBlock` (on-chain)
- Deploy script reference: `scripts/deploy-full-mainnet.ts` (does not auto-enable; you enable manually with `enableClaimsForDuration(648000)`)
