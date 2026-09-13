<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=changshenhan&style=flat-square&color=blueviolet)

# Han Changshen

### *Between Protocols, Agents, and Money*

*High-performance code · Finance & quant · Blockchain · AI agents · Protocols*

</div>

**⭐ Featured: [mist](https://github.com/changshenhan/mist)** — settlement for the agent economy, live on Base mainnet · [gas ledger](https://github.com/changshenhan/mist/blob/main/docs/articles/02-x402-gas-ledger-en.md) · 488,738 payments/s

---

## Who I am

**CUHK** (computer engineering) · **Founder of [directwire](https://github.com/directwire)** — a Rust organization building public-key-native networking for autonomous agents · **Founder of [NeuralZoo](https://neuralzoo.com.cn)**

I write high-performance infrastructure at the seams of **protocols, agents, and money** — transport that beats TCP, portable AI identity, institutional-finance codecs, ZK-enabled machine learning, and the settlement layer for machine commerce.

---

## Foundation: directwire

> *Public-key native networking for autonomous agents — dial by public key, not by IP.*

| Repo | What it is |
|---|---|
| [**agent-transport**](https://github.com/directwire/agent-transport) | Message-oriented agent transport: single-packet round-trip, 8-level QoS, loss-resilient GRANT/SRPT scheduling over UDP. **5.2× lower P99 than TCP on short messages.** |
| [**directwire**](https://github.com/directwire/directwire) | Rust workspace: [p2p-mesh](https://github.com/directwire/p2p-mesh) (iroh-style mesh) + [gm-pq-stack](https://github.com/directwire/gm-pq-stack) (SM2 + ML-KEM-768 hybrid transport) |
| [**messaggero**](https://github.com/directwire/messaggero) | A2A-compatible high-performance multi-agent transport: bincode fast path over Unix sockets + A2A HTTP |
| [**culmen**](https://github.com/directwire/culmen) | persona/v1 — a portable format for AI personas that remember, grow, and relate; runs on **Claude Code · OpenClaw · Hermes · dsh** |
| [**fixfast**](https://github.com/directwire/fixfast) | High-performance Rust FIX/FAST reference implementation for institutional finance |

---

## Brick-laying in emerging ecosystems

I deliberately place first bricks into young ecosystems — work that yields **deterministic recognition and compounding value**, regardless of any single project's fate.

> 确定性认可 ｜ 绝对收获 ｜ 长期价值投资 ＋ 攀附初始生态添砖加瓦

| Upstream | PR | Contribution |
|---|---|---|
| **infiniflow/ragflow** (89k★) | [#18644](https://github.com/infiniflow/ragflow/pull/18644) | Precompile 17 regexes at package init — removes a fresh parse+compile per token/term from the retrieval hot path — **✅ merged** |
| **infiniflow/ragflow** (89k★) | [#18646](https://github.com/infiniflow/ragflow/pull/18646) | Closed the SubmitTo/StopWait TOCTOU race — send-on-closed-channel panic, lost in-flight tasks, and a full-queue send deadlock, all via active-sender counting *(2 commits)* — **✅ merged** |
| **infiniflow/ragflow** (89k★) | [#18648](https://github.com/infiniflow/ragflow/pull/18648) | Chunker: one BPE pass per hardSplitPiece iteration instead of two — Text 1.8×, CJK 2.0×, fewer allocations; review remediation in (seam-stubbed fallback test + split-contract invariants) — **✅ merged** |
| **fatedier/frp** (109k★) | [#5505](https://github.com/fatedier/frp/pull/5505) | nathole: multi-STUN discovery with per-server fallback — multi-server configs previously died on the first unreachable server (close #5504) *(OPEN)* |
| **pingcap/tidb** (40k★) | [#70616](https://github.com/pingcap/tidb/pull/70616) | Backported the #66897 planner fix to release-8.5 — IN-subquery join+agg duplication with implicitly casted keys returned wrong results (repro for #70546) *(OPEN)* |
| **vnpy/vnpy** (44.7k★) | [#3803](https://github.com/vnpy/vnpy/pull/3803) | `cs_rank` now returns cross-sectional percentile in [0,1] (was absolute rank [1,N]) — aligns with Alpha#1 centering and `ts_rank` semantics (close #3780) *(OPEN)* |
| **tikv/tikv** (16.8k★) | [#20016](https://github.com/tikv/tikv/pull/20016) | backup-stream `last_flush_time` use-after-free → `std::sync::RwLock` (close #19968) *(OPEN)* |
| **GreptimeTeam/greptimedb** (6.5k★) | [#8924](https://github.com/GreptimeTeam/greptimedb/pull/8924) | MySQL prepared-stmt now respects session timezone (Closes #8879) — **CLOSED**, superseded by [#8923](https://github.com/GreptimeTeam/greptimedb/pull/8923) |
| **GreptimeTeam/greptimedb** (6.5k★) | [#8925](https://github.com/GreptimeTeam/greptimedb/pull/8925) | WAL replay fail-closed — region open errors instead of silently skipping damaged WAL (Closes #8809) *(OPEN)* |
| **GreptimeTeam/greptimedb** (6.5k★) | [#8927](https://github.com/GreptimeTeam/greptimedb/pull/8927) | Anchor pending-rows flush to batch creation time, killing the (fi, 2fi) flush lag (Closes #8641) — superseded by upstream #8802 *(CLOSED)* |
| **milvus-io/milvus** (46k★) | [#52759](https://github.com/milvus-io/milvus/pull/52759) / [#52760](https://github.com/milvus-io/milvus/pull/52760) | TEI rerank test tolerance; proxy metrics cleanup via `DeletePartialMatch` — **CLOSED**, superseded by #52742 / #52691 (same fixes, merged) |
| **nautilus_trader** (26k★) | [#4799](https://github.com/nautechsystems/nautilus_trader/pull/4799) | Fixed the silent no-op in custom-data stream conversion — diagnosis confirmed by core maintainer ("spot on, both causes check out"), **CLOSED** as the old persistence path is being replaced by a new data catalog |
| **barter-rs** (2.2k★) | [#284](https://github.com/barter-rs/barter-rs/pull/284) | FIX protocol framing, parser & TCP/TLS transports — **built on my own [`fix-codec`](https://crates.io/crates/fix-codec)** *(OPEN)* |
| **semantica-agi** | [#1084](https://github.com/semantica-agi/semantica/pull/1084) | SHACL `#`-terminated namespace handling — **✅ merged** |
| **nervosnetwork/ckb** (1.2k★) | [#5309](https://github.com/nervosnetwork/ckb/pull/5309) | h2 → 0.4.17, closes RUSTSEC-2026-0258 HTTP/2 DoS — **✅ merged** |
| **cloudwego/volo** (2.6k★) | [#667](https://github.com/cloudwego/volo/pull/667) | h2 → 0.4.17, same RUSTSEC-2026-0258 HTTP/2 DoS *(OPEN)* |
| **zkonduit/ezkl** | [#1023](https://github.com/zkonduit/ezkl/pull/1023) / [#1021](https://github.com/zkonduit/ezkl/pull/1021) | Custom PWL lookup for nonlinear ops — **40× MAE improvement at zero proof overhead** *(OPEN)* |
| **akitaonrails/ai-memory** | [#413](https://github.com/akitaonrails/ai-memory/pull/413) | MCP `strip_root_combinators` — **✅ merged** |
| **EmilLindfors/a2a-rs** | [#50](https://github.com/EmilLindfors/a2a-rs/pull/50) | De-flaked ConnectRPC auth tests — **✅ merged** |
| **infinitefield/hypersdk** (211★) | [#80](https://github.com/infinitefield/hypersdk/pull/80) | Market orders now send `FrontendMarket` (were GTC — silent no-fill); `PriceTick::tick_for` correct at powers of ten — **✅ merged** |
| **agentclientprotocol/rust-sdk** | [#328](https://github.com/agentclientprotocol/rust-sdk/pull/328) | ACP v1 session load/resume restore builders — **CLOSED**: maintainer shipped the same builders in [#347](https://github.com/agentclientprotocol/rust-sdk/pull/347) |
| **zkonduit/LatentExchange** | [#1](https://github.com/zkonduit/LatentExchange/pull/1) | **First external PR** — Phase-1 benchmark harness for the AI-mediated barter protocol (match rate, completion, cold-start) *(OPEN)* |
| **Dominic789654/awesome-deepseek-harness** | [#159](https://github.com/Dominic789654/awesome-deepseek-harness/pull/159) | Listed **culmen** (dsh-plugin-persona) on the official dsh plugin list — cross-runtime personality memory — **✅ merged** |
| **joaquinbejar/OrderBook-rs** (513★) | [#220](https://github.com/joaquinbejar/OrderBook-rs/pull/220) → [**ironfix-orderbook-bridge**](https://github.com/directwire/ironfix-orderbook-bridge) | FIX bridge PR closed on scoping (engine stays codec-free); rebuilt per the maintainer's preferred shape as a standalone crate implementing IronFix's `Application` trait — per-session ClOrdID registry (cross-client cancel exposure closed), single fill path via trade listener, zero-float translation, replayable `execute()`; maintainer notified on the thread |
| **joaquinbejar/OptionStratLib** (240★) | [#426](https://github.com/joaquinbejar/OptionStratLib/pull/426) | Dividend carry bug family: 17 d1/d2 call-sites now pass `r-q`, θ discounted by `e^{-qT}` — all Greeks finite-difference verified — **✅ merged** |
| **x402-foundation/x402** | [#3321](https://github.com/x402-foundation/x402/pull/3321) | Mist listed in third-party extensions — mist-v1 scheme + EIP-3009 bridge *(OPEN)* |
| **google-agentic-commerce/a2a-x402** | [#172](https://github.com/google-agentic-commerce/a2a-x402/pull/172) | `scheme_exact_mist` payment scheme spec draft (exact/EIP-3009 byte-compatible) *(OPEN)* |
| **QuantumNous/new-api** (11w★) | [#7274](https://github.com/QuantumNous/new-api/pull/7274) | realtime (wss) double charge closed — per-segment pre-billing and session-end settlement now reconcile via incremental bookkeeping; users were being charged ~2× (fixes #7273) *(CLOSED — template-format, refiling)* |
| **QuantumNous/new-api** (11w★) | [#7276](https://github.com/QuantumNous/new-api/pull/7276) | Multi-key polling no longer persists a stale snapshot over `channel_info` — concurrent auto-disables were silently resurrected (fixes #7275) *(CLOSED — template-format, refiling)* |
| **rustdesk/rustdesk** (123k★) | [#16143](https://github.com/rustdesk/rustdesk/pull/16143) | quinn-proto 0.11.15 — two QUIC DoS advisories (RUSTSEC-2026-0037/-0185) — plus bytes 1.11.1 & crossbeam-epoch 0.9.20, Cargo.lock-only — **✅ merged** (same-day) |
| **meilisearch/meilisearch** (59.2k★) | [#6627](https://github.com/meilisearch/meilisearch/pull/6627) | h2 → 0.4.17 (RUSTSEC-2026-0258 HTTP/2 DoS) + crossbeam-epoch 0.9.20 — extended in-branch by meilisearch author Kerollmops (crossbeam-channel bump) *(OPEN)* |
| **databendlabs/databend** (9.4k★) | [#20472](https://github.com/databendlabs/databend/pull/20472) | h2 0.4.17 + quinn-proto + crossbeam-epoch + lz4_flex 0.11.6 — four RUSTSEC-2026 advisories, Cargo.lock-only *(OPEN — approved by sundy-li; CI rerun pending on runner infra)* |
| **risingwavelabs/risingwave** (9.3k★) | [#27024](https://github.com/risingwavelabs/risingwave/pull/27024) | rustls-webpki 0.103.13 closes four TLS-verification advisories + lru 0.18.2 + h2 0.4.17, Cargo.lock-only *(OPEN — approved)* |

---

## Mist — settlement for the agent economy

> *Agents will pay each other at machine volume. One transaction per payment doesn't survive that.*

[**mist**](https://github.com/changshenhan/mist) is a Delegated Spend Authority (DSA) authorization primitive + optimistic batch-settlement aggregator — **live on Base mainnet**:

- **Measured, not claimed**: an x402 payment costs 61,105–90,053 gas today; Mist amortizes settlement to **(246k + 78,958×R)/N per payment — 325 gas at N=1,000, R=1 (188× cheaper)**, honest negative cases included — full [gas ledger](https://github.com/changshenhan/mist/blob/main/docs/articles/02-x402-gas-ledger-en.md), every command reproducible
- **488,738 payments/s** measured in-process ingest, CI performance-gated on every push
- Contracts **deployed and exercised on Base mainnet** (commit → settle → 6-hour challenge window → claim), open source and permissionless — deploy your own `BatchSettler` and self-register
- x402 adapter: `mist-v1` scheme, EIP-3009 bridge, v1+v2 wire formats

---

## Personal projects

| Project | What it is |
|---|---|
| [**AI-Decentralized-Autonomous-Economy**](https://github.com/changshenhan/AI-Decentralized-Autonomous-Economy) | AIDE — an AI decentralized autonomous economy (research) |
| [**ANAI**](https://github.com/changshenhan/ANAI) | Native Android AI assistant (Kotlin, Jetpack Compose, Room) |
| [**STIP-MLX**](https://github.com/changshenhan/STIP-MLX) | Private LLM inference on Apple Silicon — the server only ever sees permuted tensors |
| [**ezkl-custom-lookup-experiment**](https://github.com/changshenhan/ezkl-custom-lookup-experiment) | Quantile-based PWL breakpoints with a full prove/verify pipeline |

---

## Toolbox

| Systems | Zero-Knowledge | AI / ML |
|---------|----------------|---------|
| **Rust** · Python · Kotlin · TypeScript · C# | Halo2 · ezkl · zk-SNARKs · custom PWL lookup | PyTorch · ONNX · MLX |

<p align="center">
  <img src="https://cdn.simpleicons.org/rust/000000" width="22" height="22" />
  <img src="https://cdn.simpleicons.org/kotlin/7F52FF" width="22" height="22" />
  <img src="https://cdn.simpleicons.org/python/3776AB" width="22" height="22" />
  <img src="https://cdn.simpleicons.org/typescript/3178C6" width="22" height="22" />
  <img src="https://cdn.simpleicons.org/csharp/239120" width="22" height="22" />
  <img src="https://cdn.simpleicons.org/pytorch/EE4C2C" width="22" height="22" />
  <img src="https://cdn.simpleicons.org/onnx/005CED" width="22" height="22" />
  <img src="https://cdn.simpleicons.org/apple/000000" width="22" height="22" />
</p>

---

## Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=changshenhan&show_icons=true&theme=github_dark&hide_border=true&hide_rank=true" alt="GitHub Stats" width="400" />

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=changshenhan&layout=compact&theme=github_dark&hide_border=true&exclude_repo=changshenhan" alt="Top Languages" width="350" />

</div>

---

<div align="center">

**[GitHub](https://github.com/changshenhan)** · [directwire](https://github.com/directwire) · [NeuralZoo](https://neuralzoo.com.cn)

*Wabi-sabi, Tengen — Between Verifiability and Unsayability*

</div>
