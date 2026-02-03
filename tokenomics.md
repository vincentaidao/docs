# Tokenomics

This page documents the VIN tokenomics for **Ethereum mainnet**.

> Source of truth: `vincentaidao/vincent-contracts` (see references at bottom).

## Total supply

- **Total supply:** **1,000,000,000 VIN**

## Allocation

- **DAO / Treasury:** **300,000,000 VIN (30%)**
- **Founder allocation (human):** **100,000,000 VIN (10%)**
- **Sale + LP seeding pool:** **150,000,000 VIN (15%)**
  - Used for **token sale** and for **liquidity seeding VIN** (both come from the same allocation in the current implementation).
- **Airdrop:** **450,000,000 VIN (45%)**

## Proceeds to token holders

VincentDAO intends to route **100% of product proceeds** to VIN token holders.

Implementation details (definitions of proceeds, distribution method, cadence) are governed and may evolve; this doc will be updated as mechanisms are finalized.

## Vesting / lockups

- **No vesting/lockups are enforced on-chain** in the current contracts.

## References

- Repo: https://github.com/vincentaidao/vincent-contracts
- Token contract: `contracts/VIN.sol`
- Allocation constants: `scripts/deploy-full-sepolia.ts`
