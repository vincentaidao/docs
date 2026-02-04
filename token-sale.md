# Token Sale & Liquidity

This page documents the $VIN token sale and liquidity setup for **Ethereum mainnet**.

## Network

- **Chain:** Ethereum mainnet

## Token sale

- **Sale contract:** see [Deployments & Addresses](./deployments.md)

### Terms

- **Sale inventory (sold to participants):** **60,000,000 $VIN**
- **LP $VIN reserve (used to seed liquidity):** **90,000,000 $VIN**
- **Price:** **6,000,000 $VIN per 1 ETH**
- **Hard cap:** **25 ETH**
- **Vesting:** none

### ETH allocation (sale proceeds)

- Up to **15 ETH** is used for liquidity.
- The remainder goes to the DAO treasury (at the **25 ETH** cap: **10 ETH**).

### Liquidity lock

Liquidity is locked: the LP position is minted to a **permanent locker** (no withdrawals).

### Finalize + edge cases

This page describes the intended economics. The *exact* behavior (who can finalize, what happens if the sale doesn’t fill, deadlines, refunds/withdrawals) is defined by the deployed on-chain Sale contract.

Before launch, this section will be updated with the concrete rules from the deployed contracts.

See also: [Deployments & Addresses](./deployments.md).
