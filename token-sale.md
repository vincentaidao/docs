# Token Sale & Liquidity

This page documents the VIN token sale and liquidity setup for **Ethereum mainnet**.

> Implementation reference: `vincentaidao/vincent-contracts`.

## Network

- **Chain:** Ethereum mainnet

## Token sale

- **Sale contract:** **TBD** (will be published here once deployed)

### Terms

- **Sale inventory (sold to participants):** **60,000,000 VIN**
- **LP VIN reserve (used to seed liquidity):** **90,000,000 VIN**
- **Price:** **6,000,000 VIN per 1 ETH**
- **Hard cap:** **25 ETH**
- **Vesting:** none

## ETH allocation (sale proceeds)

On finalize, ETH raised is split between:

- **LP seeding ETH:** up to **15 ETH**
- **DAO runway / treasury ETH:** the remainder

For a **25 ETH** hard cap, that implies:

- **15 ETH** to seed liquidity
- **10 ETH** to the VincentDAO treasury

## Liquidity seeding (VIN source)

Liquidity is seeded using:

- **LP ETH:** up to 15 ETH
- **LP VIN:** `LP_ETH * 6,000,000` → for 15 ETH, **90,000,000 VIN**

**Important:** on-chain, VIN for both the sale and LP seeding is typically minted to (and transferred from) the Sale contract. In documentation we separate the intended buckets:

- **60,000,000 VIN** intended to be sold
- **90,000,000 VIN** reserved for LP seeding

## References

- Repo (implementation reference): https://github.com/vincentaidao/vincent-contracts
- Sale contract: `contracts/VinSale.sol` (`VIN_PER_ETH`, `finalize` split logic)
- Liquidity seeding: `contracts/LiquiditySeeder.sol`
- Sale inventory constant: `scripts/deploy-full-sepolia.ts` (`SALE_SUPPLY = 150_000_000 VIN`)
