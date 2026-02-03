# Token Sale & Liquidity

This page documents the VIN token sale and liquidity setup for **Ethereum mainnet**.

> Implementation reference: `vincentaidao/vincent-contracts`.

## Network

- **Chain:** Ethereum mainnet

## Token sale

- **Sale contract:** **TBD** (will be published here once deployed)

### Terms

- **Sale inventory:** **150,000,000 VIN**
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

## Liquidity seeding

Liquidity is seeded using:

- **LP ETH:** up to 15 ETH
- **LP VIN:** `LP_ETH * 6,000,000` → for 15 ETH, **90,000,000 VIN**

## References

- Repo (implementation reference): https://github.com/vincentaidao/vincent-contracts
- Sale contract: `contracts/VinSale.sol` (`VIN_PER_ETH`, `finalize` split logic)
- Liquidity seeding: `contracts/LiquiditySeeder.sol`
- Sale inventory constant: `scripts/deploy-full-sepolia.ts` (`SALE_SUPPLY = 150_000_000 VIN`)
