# Crypto Trust Standard

**A unified four-layer safety certification framework for cryptocurrency projects.**

> *The tools to prevent crypto scams already exist — separately. What doesn't exist is a single enforceable standard that coins must pass before going to market. This is that standard.*

---

## Overview

The Crypto Trust Standard (CTS) is an open initiative originated by [NMA Consulting Group](https://nmaconsultinggroup.com) to establish a mandatory, verifiable safety certification framework for cryptocurrency projects.

The crypto market loses **$10 billion+ per year** to fraud — not because the blockchain hides it, but because no entity has bundled the available protections into a single enforced standard that exchanges require before listing.

This repository contains:
- The full CTS Whitepaper (v1.0)
- The technical specification for all four layers
- The TrustRegistry smart contract specification
- The public Safety Scorecard (ongoing)
- Community discussion and standard development

---

## The Four Layers

Every certified coin must satisfy all four layers. There are no partial badges, no waivers.

| Layer | Name | Solves | Minimum Requirement |
|-------|------|--------|---------------------|
| **L1** | Liquidity Lock | Rug Pull | Founder tokens locked 24+ months in non-upgradeable VestingVault; max 4%/month release |
| **L2** | Anti-Whale Enforcement | Pump & Dump | No wallet >1% of supply; 0.25% daily sell cap per wallet; requires 67% governance vote to modify |
| **L3** | On-Chain Verification | Fake Platforms | All balance displays must source live from blockchain via signed RPC; no private database balances |
| **L4** | Cryptographic Endorsement Registry | Fake Celebrity Scams | Promoters must register identity via zk-proof KYC; all promotional content must be wallet-signed |

---

## The Problem We're Solving

| Scam Type | Annual Loss | How It Works |
|-----------|-------------|--------------|
| Rug Pull | $2.8B+ | Creators drain liquidity pool and disappear within 24–48 hours of launch |
| Pump & Dump | $80M+ | Coordinated hype → retail buys → whales dump → price collapses |
| Fake Platform | $3.96B | Fabricated profit dashboards backed by a private database, not any blockchain |
| Fake Celebrity | 700% ↑ (2023) | AI deepfakes of real people used to promote scam coins with no way to verify |

---

## What Already Exists (And Why It's Not Enough)

| Tool | What It Does | What's Missing |
|------|-------------|----------------|
| Unicrypt / Team.Finance | Liquidity locking | Voluntary, unenforced, no exchange mandate |
| CertiK / Hacken | Smart contract audits | Checks code correctness, not scam-resistance; one-time, not ongoing |
| ENS Domains | Wallet identity names | No real-world ID verification, no signing enforcement |
| Anti-whale mechanisms | Supply controls in some coins | Non-standard, removable by founders, inconsistent |

**The gap:** No single entity has bundled all four protections into one enforceable standard with an exchange mandate behind it.

---

## The Trust Badge

A coin earns the CTS Trust Badge by:

1. Deploying using the CTS Token Template (open-source, non-upgradeable)
2. Passing an independent code audit confirming all four layers are active
3. Registering all named founders in the on-chain identity registry
4. Registering all balance-display platforms with signed attestation keys
5. Passing quarterly automated on-chain re-verification

The badge is **binary** — earned or not. It is recorded on-chain in the `TrustRegistry` contract and queryable via public API.

---

## Public Safety Scorecard

We are publishing public safety scores for existing coins — audited manually against the four-layer standard — before the certification platform is formally operational. Think of it as *Rotten Tomatoes for crypto safety.*

[→ View the Scorecard](https://nmaconsultinggroup.com/crypto-trust-standard/scorecard) *(launching soon)*

Coins are scored 0–4 based on how many layers they currently satisfy. The scorecard is free, public, and updated as coins change their architecture.

---

## Documents

| Document | Description |
|----------|-------------|
| [`whitepaper-v1.0.pdf`](./whitepaper-v1.0.pdf) | Full whitepaper: problem, technical spec, certification criteria, business model, roadmap |
| [`SPEC.md`](./SPEC.md) | Technical specification for the four layers (in development) |
| [`TrustRegistry.sol`](./contracts/TrustRegistry.sol) | Smart contract specification (in development) |
| [`SCORECARD.md`](./SCORECARD.md) | Public coin safety scores |

---

## Roadmap

| Phase | Timeline | Milestone |
|-------|----------|-----------|
| **1 — Credibility** | Months 1–4 | Whitepaper public; 20 coins scored; SEC submission |
| **2 — Platform** | Months 4–8 | TrustRegistry deployed; verification API live; first paying certifications |
| **3 — Exchange Partner** | Months 8–14 | First exchange commits to displaying the badge; 20+ certified coins |
| **4 — Scale** | Months 14–18 | Coinbase / Binance outreach; MiCA engagement; 100+ coins; $1M ARR |

---

## Who This Is For

**Exchange compliance teams** — if your team spends resources on coin-by-coin listing decisions, the Trust Badge is infrastructure that systematises that decision. We want to understand what your compliance process would need from a badge to rely on it.

**Crypto projects & founders** — if you are building a legitimate coin and struggling to differentiate yourself from scammers, early certification at a founding-partner rate is available. You will shape the standard before it is set.

**Regulators & policy teams** — if you are writing crypto safety rules and want an industry-built framework to reference, this document is the starting point for that conversation.

**Technical contributors** — if you are a blockchain engineer, auditing firm, or identity provider with a role in the four-layer architecture, we want to build the technical spec together.

---

## Get Involved

- **Discuss the standard:** Open a [Discussion](../../discussions) with questions, objections, or proposed amendments
- **Review the whitepaper:** Open an [Issue](../../issues) with specific feedback on any section
- **Contribute to the spec:** See `CONTRIBUTING.md` (coming soon)
- **Contact NMA directly:** [crypto-trust@nmaconsultinggroup.com](mailto:crypto-trust@nmaconsultinggroup.com)

---

## Background

This standard was originated in September 2026 by **Shamz** at **NMA Consulting Group**, a minority-owned consulting firm with four years of government contracting experience. The idea emerged from a simple observation: every tool needed to prevent the four dominant scam types already exists — what's missing is the mandate and the bundle.

NMA Consulting Group is the founding organisation of the Crypto Trust Standard. It is not a coin. It does not issue tokens. It certifies projects against a safety standard.

---

## License

The CTS specification and documentation are published under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — free to use, share, and build on with attribution.

The TrustRegistry smart contract code is published under [MIT License](./LICENSE).

---

*Crypto Trust Standard · NMA Consulting Group · September 2026*
