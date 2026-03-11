# ShieldFi MVP Workflow

This document describes the full end-to-end MVP testing process for the ShieldFi protocol.

The goal is to validate the complete system flow:

Policy Mint → Premium Payment → Trigger Event → Claim → LP Payout

---

## 1. Deploy Contracts

Deploy the following contracts to Polygon testnet:

1. MockUSDT
2. CoveragePool
3. PolicyNFT
4. PremiumManager
5. ClaimManager
6. TriggerManager (mock parametric trigger)

Deployment order matters because contracts must reference each other.

---

## 2. Initialize Coverage Pool

Liquidity providers deposit stablecoins.

Example:

LP1 deposits 10,000 mUSDT  
LP2 deposits 5,000 mUSDT

Total pool liquidity = 15,000 mUSDT

CoveragePool now holds the protection capital.

---

## 3. User Buys Coverage

User interacts with frontend.

Steps:

1. Connect wallet
2. Choose coverage amount
3. Pay premium in mUSDT

PolicyNFT contract mints an NFT containing:

- coverage amount
- expiration date
- trigger type
- policy ID

Example:

Coverage = 1000 mUSDT  
Premium = 10 mUSDT  
Duration = 30 days

---

## 4. Premium Allocation

PremiumManager splits the premium:

Example distribution:

70% → Coverage pool rewards  
20% → Protocol treasury  
10% → Risk oracle funding

---

## 5. Trigger Event Simulation

Parametric trigger is activated.

Example triggers:

- stablecoin depeg
- protocol TVL drop
- bridge exploit

Mock trigger contract emits event.

---

## 6. Claim Execution

ClaimManager validates:

- policy exists
- policy active
- trigger matches policy condition

If valid:

CoveragePool releases payout.

---

## 7. LP Payout

CoveragePool transfers funds to the policy holder.

Example:

Coverage amount = 1000 mUSDT

User receives payout automatically.

Policy NFT becomes inactive.

---

## 8. Frontend Integration Testing

Frontend should support:

1. Connect wallet
2. Buy coverage
3. View policy NFT
4. Submit claim
5. View payout status
6. LP staking interface

---

## 9. Test Scenarios

Run these tests:

Test 1 – Policy mint  
Test 2 – Premium payment  
Test 3 – Capital allocation  
Test 4 – Trigger activation  
Test 5 – Claim validation  
Test 6 – LP payout

---

## 10. Success Criteria

The MVP is considered functional if:

- policies mint correctly
- premiums transfer correctly
- triggers activate correctly
- claims validate correctly
- payouts execute automatically