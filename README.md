# Igor Koval

Senior blockchain engineer — Rust, Solana, DeFi protocols.

I build on-chain protocols end to end: account models, instruction APIs, PDA structure, security model, SDK, audit cycle, production. Most of that work is proprietary and lives in private repositories, so this profile is thinner than the work behind it. The public parts are below.

### Solana / DeFi

**Aldrin** — AMM, staking and farming protocols (2021–2022); token launch protocol with Raydium and Meteora liquidity graduation (2024–present).

- Protocol peaked at **$149.5M TVL** in December 2021 — [DefiLlama](https://defillama.com/protocol/aldrin)
- Cleared a **Kudelski Security** assessment with zero security findings — [public report](https://web.archive.org/web/20230519165819/https://dex.aldrin.com/877f900320eec44c13409814fe473fb7.pdf)
- Designed a curve abstraction allowing multiple AMM curve implementations to coexist in a single protocol — constant-product swaps and Balancer-style weighted single-asset withdrawals, verified against the Balancer specification during audit

### Upstream contributions

**[project-serum/serum-dex#143](https://github.com/project-serum/serum-dex/pull/143)** — my CPI calls into Serum were failing. The `cancel_order` and `cancel_order_by_client_order_id` instruction builders declared account mutability that contradicted the program's own `MarketInstruction` definitions, which breaks cross-program calls for any external integrator while leaving Serum's own paths unaffected. Brought the builders in line with the enum. Merged June 2021; closed [#139](https://github.com/project-serum/serum-dex/issues/139).

### Before blockchain

Co-founded a two-person game studio (2022–2024) — performance-critical simulation systems in C# and Unity: custom update scheduling, mesh baking, pathfinding, and an animation pipeline built for batching. Earlier, VR platform engineering at Varwin and decentralised storage prototyping at CasperAPI.

---

Rust · TypeScript · Anchor · SPL Token · Metaplex · Raydium · Meteora

[LinkedIn](https://linkedin.com/in/comradekoval) · igor.koval.dev@icloud.com
