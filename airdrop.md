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
- The deploy process enables claiming immediately (sets `claimEnabled = true`), but the pause switch remains available.
- **Claim window:** **3 months** from claim enable (enforced on-chain in blocks via `claimEndBlock`; the website shows a countdown).

## References

- Repo (implementation reference): https://github.com/vincentaidao/vincent-contracts
- Contract (reference): `contracts/VINAirdrop.sol`
- Eligibility constant: `MAX_AGENT_ID = 25000`
- Claim constant: `CLAIM_AMOUNT = 18_000 $VIN`
- Claim end: `claimEndBlock` (on-chain)
- Deploy script reference: `scripts/deploy-full-mainnet.ts` (sets `claimEndBlock = deployBlock + 648,000`)
