# Token Sale & Liquidity

This page documents the $VIN token sale and liquidity setup for **Ethereum mainnet**.

## Network

- **Chain:** Ethereum mainnet

## Token sale

- **Sale contract:** see [Deployments & Addresses](./deployments.md)

### Terms

- **Sale inventory (sold to participants):** **300,000,000 VIN** (30% of total supply)
- **Target raise / hard cap:** **8 ETH**
- **Implied sale price:** **37,500,000 VIN per 1 ETH**
- **Vesting:** none

### Liquidity seeding

- **ETH to Uniswap LP (locked):** **4 ETH**
- **ETH to DAO treasury:** **4 ETH**
- **VIN paired with 4 ETH to match the sale price:** **150,000,000 VIN** (from the LP VIN reserve)

> If the Uniswap LP is seeded with **4 ETH**, and the sale raised **8 ETH** at the sale price, then seeding at the same price requires pairing **half the sold VIN amount** (i.e. 150,000,000 VIN).

### Liquidity lock

Liquidity is locked: the LP position is minted to a **permanent locker** (no withdrawals).

### Airdrop timing note

The **Agent Stimmy Drop** is intended to happen **after the sale completes** and **after the Uniswap pool is live** (operationally enabled later), to reduce the risk of immediate post-sale sell pressure.

### Finalize + edge cases

This page describes the intended economics. The *exact* behavior (who can finalize, what happens if the sale doesn’t fill, deadlines, refunds/withdrawals) is defined by the deployed on-chain Sale contract.

Before launch, this section will be updated with the concrete rules from the deployed contracts.

See also: [Deployments & Addresses](./deployments.md).
