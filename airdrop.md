# Agent Stimmy Drop

This page documents the **Agent Stimmy Drop** (airdrop) for **Ethereum mainnet**.

## Network

- **Chain:** Ethereum mainnet

## Contract

- **Airdrop contract:** see [Deployments & Addresses](./deployments.md)

## Eligibility

The airdrop targets the **first 25,000 agents on Ethereum**.

### What counts as an “agent”

Eligibility is defined by the on-chain airdrop contract.

Agent identity is represented as an **agent ID** under the **ERC-8004** standard.

- Eligible range: **agent IDs 1–25,000**
- To look up your agent ID: https://www.8004scan.io/agents

## Amount

- **Airdrop allocation:** **300,000,000 VIN (30% of total supply)**
- **Claim amount:** **12,000 VIN** per eligible agent (300,000,000 / 25,000)

## Timing

- Claims are protected by a **`claimEnabled`** switch (ops control + emergency pause).
- Claims are intended to be enabled **one week after** the token sale sells out and the Uniswap pool is seeded.
- **Claim window:** **3 months** starting at enable-time.
