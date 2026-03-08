## ShieldFi Architecture

```mermaid
flowchart LR

A[User Wallet] --> B[Protocol / dApp]

B --> C[ShieldFi API Gateway]

C --> D[Wallet Scoring Engine]
C --> E[Cluster Intelligence Engine]
C --> F[Blockchain Data Layer]

F --> G[Ethereum]
F --> H[BNB Chain]
F --> I[Solana]
F --> J[TRON]

D --> K[Shield Score 0–100]
E --> L[Cluster Risk Analysis]

K --> M[Risk Recommendation]
L --> M

M --> N{Protocol Decision}

N --> O[Allow Transaction]
N --> P[Warn User]
N --> Q[Block Transaction]
