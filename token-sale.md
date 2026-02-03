# Token Sale & Liquidity

This page documents the current on-chain sale + liquidity seeding configuration for **VIN**.

## Network

- **Chain:** Sepolia

## Sale

- **VinSale contract:** `0x20102C4daF3FbE98fF5b761Bff3f7B58726FC8a5`

### Terms (current deployment)

- **Fixed price:** **6,000,000 VIN per 1 ETH** (`VIN_PER_ETH`)
- **Hard cap:** **0.001 ETH** (`HARD_CAP` in deploy script)
- **Delivery:** VIN is transferred on commit
- **Refunds:** refund path burns VIN via `saleBurn`
- **Finalize:** requires `totalRaised == totalCapWei`; then transfers enabled

## Liquidity seeding

- **LiquiditySeeder contract:** `0xDdc3d9496B75Cafe39801Bd3e6d0510fBd72a152`
- **Permanent locker:** `0x80d941c2850414a264acFa5823c50794221D72bd` (LP NFT minted to this locker)

### Method

`LiquiditySeeder.seed()` creates a Uniswap v4 full-range LP position (ETH + VIN) with:

- fee = 0
- tickSpacing = 10
- hooks = 0

## Uniswap v4 configuration (Sepolia)

- PoolManager: `0xE03A1074c86CFeDd5C142C4F04F1a1536e203543`
- PositionManager: `0x429ba70129df741B2Ca2a85BC3A2a3328e5c09b4`
- Permit2: `0x000000000022D473030F116dDEE9F6B43aC78BA3`

## Vesting / lockups

- **No vesting/lockups are enforced on-chain** for the sale or liquidity in the current contracts.

## References

- Repo: https://github.com/vincentaidao/vincent-contracts
- Sale contract: `contracts/VinSale.sol`
- Liquidity seeding: `contracts/LiquiditySeeder.sol`
- Deployment params: `scripts/deploy-full-sepolia.ts`
