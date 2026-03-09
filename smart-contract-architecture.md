# ShieldFi Smart Contract Architecture

ShieldFi uses a modular smart contract system to provide parametric DeFi protection.

## Core Components

1. Coverage Pool
2. Policy NFT
3. Trigger Engine
4. Payout Manager
5. Oracle Interface

---

## Coverage Pool

The coverage pool holds liquidity provided by capital providers.

Functions:
- deposit liquidity
- withdraw liquidity
- allocate liquidity to protection pools

---

## Policy NFT

Each protection policy is represented by an NFT.

Policy contains:
- wallet address
- protected protocol
- coverage amount
- protection duration
- trigger conditions

---

## Trigger Engine

The trigger engine monitors on-chain events.

Responsibilities:
- detect trigger conditions
- verify oracle data
- activate payouts

---

## Oracle Interface

ShieldFi integrates oracle networks for data feeds.

Data sources may include:
- price feeds
- liquidity pool data
- TVL measurements

---

## Payout Manager

If a trigger event is confirmed:

- affected policies are identified
- payout amounts are calculated
- funds are distributed automatically