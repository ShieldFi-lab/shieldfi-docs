# ShieldFi Parametric Protection Layer

This diagram shows how ShieldFi delivers **real-time, automated DeFi coverage**:

---


┌───────────────────────────┐
 │       User Wallets        │
 │  (holds PolicyNFTs & LP) │
 └─────────────┬────────────┘
               │
               ▼
 ┌───────────────────────────┐
 │        PolicyNFTs         │
 │ - Coverage Amount         │
 │ - Trigger Type            │
 │ - Expiration Date         │
 │ - Risk Metadata           │
 └─────────────┬────────────┘
               │
               ▼
 ┌───────────────────────────┐
 │       Coverage Pool       │
 │ - Holds Premiums          │
 │ - Monitors Available Fund │
 │ - Dynamic Risk Metrics    │
 └─────────────┬────────────┘
               │
               ▼
 ┌───────────────────────────┐
 │     Parametric Triggers   │
 │ - On-chain Oracle Feeds   │
 │ - Protocol Liquidity Check│
 │ - Stablecoin Depeg Monitor│
 │ - Governance Admin Alerts │
 └─────────────┬────────────┘
               │
               ▼
 ┌───────────────────────────┐
 │      Claim Manager        │
 │ - Verifies Trigger Event  │
 │ - Executes Automatic Payout
 │ - Updates PolicyNFT Status│
 └───────────────────────────┘

---

## How It Works

1. **User buys coverage** → PolicyNFT minted with risk metadata.  
2. **Premium goes into Coverage Pool**, which tracks available liquidity.  
3. **Parametric Triggers continuously monitor**:  
   - Hacks/exploits  
   - Stablecoin depegs  
   - Sudden large transfers  
   - Governance/admin changes  
4. Trigger fires → **Claim Manager executes automatic payout**.  
5. PolicyNFT **updates status in real-time**, fully on-chain.

---

## Why This Layer is Unique

- Fully **automated** → no manual claim verification.  
- **Real-time monitoring**, preventing delayed payouts.  
- **Dynamic risk-based coverage** scales to institutions.  
- Transparent and verifiable **on-chain logic**.  
- Adds a **missing infrastructure layer** that almost no other DeFi project offers.

---

### ShieldFi Impact

This layer makes ShieldFi a **serious protocol** that:

- Retail users trust for automated coverage  
- Exchanges and DeFi protocols can integrate for risk mitigation  
- Institutions see as professional, scalable, and ready for real-world adoption