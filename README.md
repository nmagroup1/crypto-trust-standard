# Crypto Trust Standard

**A unified four-layer safety framework for cryptocurrency projects.**

> *The tools to prevent crypto scams already exist — separately. What doesn't exist is a single bundled framework that exchanges can require before listing. CTS is our proposed answer to that gap.*

---

## Overview

The Crypto Trust Standard (CTS) is a research-based proposal from [NMA Consulting Group](https://nmaconsultinggroup.com) — an open, verifiable safety framework that any exchange can choose to adopt as a listing requirement.

The crypto market loses **$10 billion+ per year** to fraud — not because the blockchain hides it, but because no one has bundled the available protections into a single framework that exchanges can point to when making listing decisions.

This repository contains:
- The full CTS Whitepaper (v1.0)
- The technical specification for all four layers (in development)
- The TrustRegistry smart contract specification (in development)
- The public Safety Scorecard (launching soon)
- Community discussion and standard development

---

## The Four Layers

The CTS framework proposes four layers a participating coin satisfies to earn the Trust Badge. The badge is all-or-nothing — no partial credit.

| Layer | Name | Solves | Specification |
|-------|------|--------|---------------------|
| **L1** | Liquidity Lock | Rug Pull | Founder tokens locked 24+ months in non-upgradeable VestingVault; max 4%/month release |
| **L2** | Anti-Whale Enforcement | Pump & Dump | No wallet >1% of supply; 0.25% daily sell cap per wallet; requires 67% governance vote to modify |
| **L3** | On-Chain Verification | Fake Platforms | All balance displays source live from blockchain via signed RPC; no private database balances |
| **L4** | Cryptographic Endorsement Registry | Fake Celebrity Scams | Promoters register identity via zk-proof KYC; all promotional content is wallet-signed |

---

## The Problem We're Addressing

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
| Unicrypt / Team.Finance | Liquidity locking | Voluntary, not bundled with other protections |
| CertiK / Hacken | Smart contract audits | Checks code correctness, not scam-resistance; one-time, not ongoing |
| ENS Domains | Wallet identity names | No real-world ID verification, no signing requirement |
| Anti-whale mechanisms | Supply controls in some coins | Non-standard, removable by founders, inconsistent |

**The gap:** No one has bundled all four protections into a single framework that exchanges can point to as a listing benchmark. CTS is our proposed solution to that gap.

---

## The Trust Badge

Under the CTS framework, a coin earns the Trust Badge by:

1. Deploying using the CTS Token Template (open-source, non-upgradeable)
2. Completing an independent code audit confirming all four layers are active
3. Registering all named founders in the on-chain identity registry
4. Registering all balance-display platforms with signed attestation keys
5. Completing quarterly automated on-chain re-verification

The badge is **binary** — earned or not. It will be recorded on-chain in the `TrustRegistry` contract and queryable via public API. The verification platform is currently in development.

---

**Disclaimer:** The Trust Badge reflects verifiable on-chain criteria at the time of verification only. It is not a guarantee of investment safety, project legitimacy, or future performance. NMA Consulting Group and CASHFLOW IQ make no warranties, express or implied, regarding the accuracy, completeness, or reliability of any verification result. The CTS framework is a proposed open standard — participation is voluntary, verification is technical and limited in scope, and no verification process eliminates all risk. The Trust Badge is not financial advice, not an endorsement of any project or team, and not a representation that any coin is free from fraud or loss. Neither NMA Consulting Group nor CASHFLOW IQ assumes any liability for losses, damages, or adverse outcomes arising from reliance on the Trust Badge, the CTS framework, or any associated verification tools.

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
| **3 — Exchange Partner** | Months 8–14 | First exchange commits to displaying the badge; 20+ participating coins |
| **4 — Scale** | Months 14–18 | Coinbase / Binance outreach; MiCA engagement; 100+ coins; $1M ARR |

---

## Who This Is For

**Exchange compliance teams** — if your team spends resources on coin-by-coin listing decisions, the CTS framework is a proposed benchmark that could help systematize that process. We want to understand what your compliance process would need from a framework like this.

**Crypto projects & founders** — if you are building a legitimate coin and struggling to differentiate yourself from scammers, we want to hear from you. Early participants will help shape the framework before it is finalized.

**Regulators & policy teams** — if you are writing crypto safety rules and want an industry-originated framework to reference, this whitepaper is the starting point for that conversation.

**Technical contributors** — if you are a blockchain engineer, auditing firm, or identity provider, we are building the technical spec collaboratively and welcome your input.

---

## Get Involved

- **Discuss the framework:** Open a [Discussion](../../discussions) with questions, objections, or proposed amendments
- **Review the whitepaper:** Open an [Issue](../../issues) with specific feedback on any section
- **Contribute to the spec:** See `CONTRIBUTING.md` (coming soon)
- **Contact NMA directly:** [crypto-trust@nmaconsultinggroup.com](mailto:crypto-trust@nmaconsultinggroup.com)

---

## Background

**NMA Consulting Group** is a management consulting firm focused on operational strategy and emerging technology. In September 2026, after researching the existing cryptocurrency safety ecosystem and finding no bundled framework addressing the four dominant scam types, NMA Consulting Group put forward the Crypto Trust Standard — an open framework the industry can rally around, available for any exchange to adopt.

NMA Consulting Group contributed this framework to the industry as an open proposal. It is not a coin. It does not issue tokens.

**CASHFLOW IQ** is building the tools that make the framework verifiable — the TrustRegistry smart contract, the trust badge issuance system, and the verification infrastructure. The framework is open; the platform is the business.

---

## License

The CTS specification and documentation are published under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — free to use, share, and build on with attribution.

The TrustRegistry smart contract code will be published under [MIT License](./LICENSE).

---

*Nothing in this repository constitutes financial, legal, or investment advice. The Crypto Trust Standard is a proposed open framework — not a regulated product, not a certification body, and not a guarantee of any outcome. NMA Consulting Group and CASHFLOW IQ make no representations regarding the suitability of this framework for any particular purpose.*

*Crypto Trust Standard · NMA Consulting Group · September 2026*
