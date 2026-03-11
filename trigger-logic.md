# ShieldFi Parametric Trigger Logic

Parametric triggers automatically execute payouts based on on-chain events.

## Example Triggers

### 1 Depeg Event

Trigger if:

USDC price < $0.97 for 10 minutes.

### 2 Smart Contract Exploit

Trigger if:

Protocol TVL drops > 30% within 5 blocks.

### 3 Bridge Hack

Trigger if:

Bridge contract emits abnormal withdrawal event.

## Execution Flow

1 Oracle detects anomaly
2 Trigger contract confirms condition
3 ClaimManager validates policy
4 CoveragePool executes payout