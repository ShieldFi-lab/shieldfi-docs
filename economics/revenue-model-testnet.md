ShieldFi

 — Simplified Revenue Model (Testnet Simulation)

Overview

ShieldFi introduces a parametric DeFi protection layer where users pay premiums to protect against measurable on-chain risks such as exploits, hacks, or stablecoin depegs.

During testnet, a simplified economic model will simulate how:
• Users pay coverage premiums
• Liquidity Providers (LPs) supply capital to the coverage pool
• Premiums generate yield for LPs
This allows testing of protocol sustainability before mainnet launch.

---


1. Coverage Premium Model

Users purchase protection policies for a defined coverage amount.

Example:
Coverage Amount
Duration
Premium Rate
Premium Paid
$1,000
30 days
2%
$20
$5,000
30 days
2%
$100
$10,000
30 days
2%
$200
Premium formula:
Premium = Coverage Amount × Premium Rate
For testnet simulation:
Premium Rate = 2%
Premiums are deposited into the coverage pool smart contract.

---


2. Liquidity Provider (LP) Yield

Liquidity providers deposit capital into the ShieldFi coverage pool to fund potential payouts.

Example:
LP Deposit
Share of Pool
$10,000
10%
$25,000
25%
$65,000
65%
LPs earn yield from user premiums.
Example scenario:
Total Pool Liquidity = $100,000
Total Premiums Collected = $5,000
LP yield distribution:
LP Yield = Premiums Collected × LP Pool Share

Example:
LP Share
Yield Earned
10%
$500
25%
$1,250
65%
$3,250

---


3. Protocol Fee

A small percentage of premiums is allocated to the protocol treasury to support development and operations.

Example:
Protocol Fee = 10% of premiums
Revenue split:
Allocation
Percentage
Liquidity Providers
90%
Protocol Treasury
10%
Example:
Premiums collected = $5,000
Protocol fee = $500
LP yield = $4,500

---

4. Parametric Payout Event (Simulation)

If a trigger event occurs (exploit, hack, or depeg), payouts are automatically executed from the coverage pool.

Example trigger:
Protocol exploit detected
Loss threshold exceeded
Policy payout example:
Policy Holder
Coverage
Payout
User A
$1,000
$1,000
User B
$5,000
$5,000

Payouts are executed automatically by the smart contract.

---


5. Testnet Simulation Goals

The testnet economic model will help validate:
• Premium sustainability
• Liquidity provider incentives
• Pool solvency during payout events
• Parametric trigger execution
These simulations will guide parameter adjustments before mainnet deployment.

---


6. Future Economic Expansion

Future iterations of ShieldFi may include:
• Dynamic premium pricing based on risk scoring
• Risk-adjusted LP yield models
• Multi-pool coverage markets
• Governance-based parameter adjustments
