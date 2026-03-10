# ShieldFi Policy NFT Structure

ShieldFi policies are represented as ERC-721 NFTs.  
Each NFT represents an active protection policy for a user.

## Core Fields

- policyId  
- ownerAddress  
- protocolCovered  
- coverageAmount  
- coverageAsset  
- premiumPaid  
- triggerType  
- triggerThreshold  
- startTimestamp  
- expirationTimestamp  
- policyStatus  

## Field Descriptions

**policyId**

Unique identifier for the policy.

**ownerAddress**

Wallet address that owns the policy NFT.

**protocolCovered**

The DeFi protocol covered by the policy.

Examples:
- Uniswap
- Aave
- Lido

**coverageAmount**

Amount insured by the policy.

Example:
10,000 USDC coverage.

**coverageAsset**

Asset used for coverage.

Examples:
- USDC
- ETH
- DAI

**premiumPaid**

Amount paid by the user for the coverage.

Example:
120 USDC premium.

**triggerType**

Defines the event that triggers a payout.

Examples:
- smart contract exploit
- liquidity drain
- oracle manipulation
- stablecoin depeg

**triggerThreshold**

Objective condition for triggering the policy.

Example:
TVL drop greater than 40%.

**startTimestamp**

Time when coverage begins.

**expirationTimestamp**

Time when coverage expires.

Examples:
- 30 days
- 90 days
- 180 days

**policyStatus**

Current status of the policy.

Possible values:

ACTIVE  
TRIGGERED  
EXPIRED  
CLAIMED  

## Policy Lifecycle

1. User purchases coverage.
2. Policy NFT is minted.
3. Monitoring system watches the protected protocol.
4. If trigger conditions occur, payout is activated.
5. Policy NFT status updates to CLAIMED.