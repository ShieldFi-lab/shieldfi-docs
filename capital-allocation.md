# ShieldFi Coverage Pool Capital Allocation

Coverage pools provide liquidity for protection payouts.

## Liquidity Providers

LPs deposit stablecoins (USDT / USDC / DAI).

Example:

LP1 deposits: 10,000 USDT  
LP2 deposits: 5,000 USDT  

Total Pool: 15,000 USDT

## Coverage Allocation

Policies reserve capital based on coverage amount.

Example:

Policy A coverage: 1,000 USDT
Policy B coverage: 2,000 USDT

Reserved Capital = 3,000 USDT

Available Liquidity = Pool - Reserved

15,000 - 3,000 = 12,000 available

## Risk Limit

Max coverage = 30% of pool liquidity.

This prevents insolvency during large exploits.