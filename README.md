# Crypto Trust Standard

**A unified four-layer safety framework for cryptocurrency projects.**

> *The tools to prevent crypto scams already exist — separately. What doesn't exist is a single enforceable standard that coins must pass before going to market. This is that standard.*

---

## Overview

The Crypto Trust Standard (CTS) is an open initiative published and maintained by [NMA Consulting Group](https://nmaconsultinggroup.com) — a mandatory, verifiable safety framework for cryptocurrency projects.

The crypto market loses **$10 billion+ per year** to fraud — not because the blockchain hides it, but because no entity has bundled the available protections into a single enforced standard that exchanges require before listing.

This repository contains:
- The full CTS Whitepaper (v1.0)
- The technical specification for all four layers (in development)
- The TrustRegistry smart contract specification (in development)
- The public Safety Scorecard (launching soon)
- Community discussion and standard development

---

## The Four Layers

The CTS framework defines four layers every compliant coin must satisfy. There are no partial badges, no waivers.

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

Under the CTS framework, a coin earns the Trust Badge by:

1. Deploying using the CTS Token Template (open-source, non-upgradeable)
2. Passing an independent code audit confirming all four layers are active
3. Registering all named founders in the on-chain identity registry
4. Registering all balance-display platforms with signed attestation keys
5. Passing quarterly automated on-chain re-verification

The badge is **binary** — earned or not. It will be recorded on-chain in the `TrustRegistry` contract and queryable via public API. The verification platform is currently in development.

---

## Public Safety Scorecard

We are developing a public safety scorecard for existing coins — evaluated against the four-layer framework. Think of it as *Rotten Tomatoes for crypto safety.*

[→ View the Scorecard](https://nmaconsultinggroup.com/crypto-trust-standard/scorecard) *(launching soon)*

Coins will be scored 0–4 based on how many layers they currently satisfy. The scorecard will be free, public, and updated as coins evolve.

---

## Documents

| Document | Description |
|----------|-------------|
| [`whitepaper-v1.0.pdf`](./whitepaper-v1.0.pdf) | Full whitepaper: problem, technical spec, framework criteria, business model, roadmap |
| [`SPEC.md`](./SPEC.md) | Technical specification for the four layers (in development) |
| [`TrustRegistry.sol`](./contracts/TrustRegistry.sol) | Smart contract specification (in development) |
| [`SCORECARD.md`](./SCORECARD.md) | Public coin safety scores (launching soon) |

---

## Roadmap

| Phase | Timeline | Milestone |
|-------|----------|-----------|
| **1 — Credibility** | Months 1–4 | Whitepaper public; 20 coins scored; SEC submission |
| **2 — Platform** | Months 4–8 | TrustRegistry deployed; verification API live; first certifications |
| **3 — Exchange Partner** | Months 8–14 | First exchange commits to displaying the badge; 20+ compliant coins |
| **4 — Scale** | Months 14–18 | Coinbase / Binance outreach; MiCA engagement; 100+ coins; $1M ARR |

---

## Who This Is For

**Exchange compliance teams** — if your team spends resources on coin-by-coin listing decisions, the CTS framework is infrastructure that could systematize that decision. We want to understand what your compliance process would need from a standard to rely on it.

**Crypto projects & founders** — if you are building a legitimate coin and struggling to differentiate yourself from scammers, we want to hear from you. Early participants will help shape the standard before it is finalized.

**Regulators & policy teams** — if you are writing crypto safety rules and want an industry-originated framework to reference, this whitepaper is the starting point for that conversation.

**Technical contributors** — if you are a blockchain engineer, auditing firm, or identity provider, we are building the technical spec collaboratively and welcome your input.

---

## Get Involved

- **Discuss the standard:** Open a [Discussion](../../discussions) with questions, objections, or proposed amendments
- **Review the whitepaper:** Open an [Issue](../../issues) with specific feedback on any section
- **Contribute to the spec:** See `CONTRIBUTING.md` (coming soon)
- **Contact NMA directly:** [crypto-trust@nmaconsultinggroup.com](mailto:crypto-trust@nmaconsultinggroup.com)

---

## Background

The Crypto Trust Standard was developed and published in September 2026 by **NMA Consulting Group**, a management consulting firm focused on operational strategy and emerging technology. The framework emerged from a simple observation: every tool needed to prevent the four dominant scam types already exists — what's missing is the mandate and the bundle.

NMA Consulting Group publishes and maintains the CTS as an open framework. It is not a coin. It does not issue tokens.

The operational platform behind the CTS — the TrustRegistry smart contract, the trust badge issuance system, and the certification infrastructure — is operated by **CASHFLOW IQ**, the registered entity that runs and enforces the standard. The framework is open; the platform is the business.

---

## License

The CTS specification and documentation are published under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — free to use, share, and build on with attribution.

The TrustRegistry smart contract code will be published under [MIT License](./LICENSE).

---

*Crypto Trust Standard · NMA Consulting Group · September 2026*
