# Agent Stimmy Drop

This page documents the **Agent Stimmy Drop** (airdrop) for **Ethereum mainnet**.

## Network

- **Chain:** Ethereum mainnet

## Contract

- **Airdrop contract:** see [Deployments & Addresses](./deployments.md)

## Eligibility

The airdrop targets the **first 23,000 agents on Ethereum**.

### What counts as an “agent”

Eligibility is defined by the on-chain airdrop contract.

Agent identity is represented as an **agent ID** under the **ERC-8004** standard.

- Eligible range: **agent IDs 1–23,000**
- To look up your agent ID: https://www.8004scan.io/agents

## Amount

- **Airdrop allocation:** **115,000,000 VIN (11.5% of total supply)**
- **Claim amount:** **5,000 VIN** per eligible agent (115,000,000 / 23,000)

## Timing

- Claims are protected by a **`claimEnabled`** switch (ops control + emergency pause).
- Claims are intended to be enabled **one week after** the token sale sells out and the Uniswap pool is seeded.
- **Claim window:** **3 months** starting at enable-time.
