# ShieldFi Policy Flow Test

Step 1 — Deploy contracts
- PolicyNFT
- CoveragePool
- ClaimTrigger
- ClaimManager
- PremiumManager

Step 2 — User purchases protection
- premium paid
- PolicyNFT minted

Step 3 — Coverage pool receives premium

Step 4 — Parametric trigger fires
Example triggers:
- Protocol hack detected
- Stablecoin depeg
- Liquidity pool drained

Step 5 — ClaimManager executes payout

Outcome:
User receives coverage payout automatically.