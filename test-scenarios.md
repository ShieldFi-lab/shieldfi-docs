# ShieldFi Test Scenarios

## Test 1 Policy Purchase

User buys policy for 1000 USDT coverage.

Expected:

PolicyNFT minted.

## Test 2 Premium Payment

User pays 10 USDT premium.

Expected:

Funds transferred to PremiumManager.

## Test 3 Trigger Event

Mock depeg event triggered.

Expected:

ClaimManager validates policy.

## Test 4 Payout

CoveragePool sends payout to policy holder.