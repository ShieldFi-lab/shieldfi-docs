# ShieldFi Testnet Deployment Plan

Network: Polygon Testnet

Contracts to deploy:
1. PolicyNFT
2. CoveragePool
3. ClaimTrigger
4. ClaimManager
5. PremiumManager

Deployment Order:
1. Deploy PolicyNFT
2. Deploy CoveragePool
3. Link CoveragePool to PolicyNFT
4. Deploy ClaimTrigger
5. Deploy ClaimManager
6. Deploy PremiumManager

Test Scenario:
1. User buys protection policy
2. PolicyNFT is minted
3. Premium is sent to CoveragePool
4. Parametric trigger is simulated
5. ClaimManager processes payout