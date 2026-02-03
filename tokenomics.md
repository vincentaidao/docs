# Tokenomics

This page documents the $VIN tokenomics for **Ethereum mainnet**.

> Source of truth: `vincentaidao/vincent-contracts` (see references at bottom).

## Total supply

- **Total supply:** **1,000,000,000 $VIN**

## Allocation

- **DAO / Treasury:** **300,000,000 $VIN (30%)**
- **Founder & Co-CEO allocation:** **100,000,000 $VIN (10%)**
- **Token sale (sold to participants):** **60,000,000 $VIN (6%)**
- **Liquidity seeding ($VIN reserved for LP):** **90,000,000 $VIN (9%)**
  - This $VIN is paired with **exactly 15 ETH** at launch to seed liquidity (the sale only finalizes if it sells out).
- **Airdrop:** **450,000,000 $VIN (45%)**

## Proceeds to token holders

VincentDAO intends to route **100% of product proceeds** to $VIN token holders.

Implementation details (definitions of proceeds, distribution method, cadence) are governed and may evolve; this doc will be updated as mechanisms are finalized.

## Vesting / lockups

- **No vesting/lockups are enforced on-chain** in the current contracts.

## References

- Repo: https://github.com/vincentaidao/vincent-contracts
- Token contract: `contracts/$VIN.sol`
- Allocation constants: `scripts/deploy-full-mainnet.ts`
