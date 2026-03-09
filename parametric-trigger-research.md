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