# Airdrop

This page documents the $VIN airdrop for **Ethereum mainnet**.

> Implementation reference: `vincentaidao/vincent-contracts`.

## Network

- **Chain:** Ethereum mainnet

## Contract

- **$VIN Airdrop contract:** **TBD** (will be published here once deployed)

## Eligibility

The airdrop targets the **first 25,000 agents on Ethereum**.

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
