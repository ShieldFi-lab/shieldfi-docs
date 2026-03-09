# Parametric Trigger Research

This document lists potential measurable on-chain events that could trigger automated protection mechanisms in ShieldFi.

---

## Exploit Detection

Event: Rapid TVL Drain  
Trigger: >40% protocol TVL lost within 10 blocks

Event: Emergency Contract Pause  
Trigger: pause() function executed

---

## Stablecoin Depeg

Event: Stablecoin price deviation  
Trigger: price < $0.95 for 30 minutes

Possible oracle sources:
- Chainlink price feeds
- DEX TWAP data

---

## Liquidity Pool Collapse

Event: Pool liquidity drop  
Trigger: >60% liquidity removed within 20 blocks

---

## Oracle Failure

Event: Oracle update failure  
Trigger: price feed not updated for >1 hour

Event: Oracle deviation  
Trigger: oracle price differs >15% from DEX TWAP

---

## Bridge Exploit Indicators

Event: Abnormal bridge withdrawals  
Trigger: withdrawals exceed historical average by 300%

---

## Contract Risk Events

Event: Contract implementation change  
Trigger: proxy implementation address changes

Event: Self-destruct executed  
Trigger: smart contract selfdestruct() called

---

## Example Historical Events

These events demonstrate why measurable on-chain triggers are important for automated protection systems.

- Ronin Bridge Hack (2022) – >$600M drained from the bridge contract.
- Euler Finance Hack (2023) – >$190M drained through a flash loan exploit.
- TerraUSD Depeg (2022) – algorithmic stablecoin lost its $1 peg and collapsed.

These incidents highlight the need for automatic detection of abnormal liquidity movements, price deviations, and rapid TVL losses.

---

## Trigger Reliability Considerations

Parametric triggers must be carefully designed to avoid false positives or manipulation.

Key considerations:

- Triggers should rely on multiple data sources where possible.
- Price triggers should compare oracle feeds and DEX TWAP prices.
- Liquidity events should be measured over several blocks to avoid flash loan distortions.
- Emergency protocol actions such as contract pauses may be used as confirmation signals.

---

## Potential Data Sources

ShieldFi triggers may rely on several on-chain and oracle data sources:

- Chainlink price feeds
- DEX TWAP price data
- Protocol TVL measurements
- Liquidity pool reserve balances
- Smart contract events (pause, upgrade, emergency functions)

---

## Future Research

Further work is required to refine trigger thresholds and test them against historical exploit data.

Areas of focus:

- backtesting triggers against past exploits
- identifying manipulation-resistant thresholds
- integrating multi-oracle validation
- designing automated payout mechanisms