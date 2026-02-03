# Airdrop

This page documents the current on-chain airdrop configuration for **VIN**.

## Network

- **Chain:** Sepolia

## Contract

- **VINAirdrop:** `0xA52423A5394fCDF4a4E88F3bc3EB423BA69bC494`

## Eligibility

Eligibility is determined on-chain as:

- `agentId < 25000` (i.e., agent IDs **0–24,999**)
- the agent must have a registered wallet in the IdentityRegistry: `registry.getAgentWallet(agentId)`
- claiming is gated by `claimEnabled`

## Amount

- **Claim amount:** **18,000 VIN** per eligible agent (`CLAIM_AMOUNT`)

## Snapshot / timing

- **No snapshot block/time is enforced on-chain**.
- **No claim window (start/end) is enforced on-chain**.

These parameters may be enforced off-chain (UI/policy) or added in future contract versions.

## References

- Repo: https://github.com/vincentaidao/vincent-contracts
- Contract: `contracts/VINAirdrop.sol`
