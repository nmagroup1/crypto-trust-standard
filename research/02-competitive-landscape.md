# Competitive Landscape — Existing Tools and Frameworks

**Prepared by:** NMA Consulting Group  
**Date:** September 2026  
**Purpose:** Document every existing tool, standard, and framework identified during prior art research, with a factual description of what each does and what it does not do.

> This document is the basis for NMA's public acknowledgement of prior art in the CTS whitepaper and README. It demonstrates that CTS credits all existing tools accurately and does not misrepresent what came before.

---

## Category 1: Liquidity Locking Platforms

### Unicrypt
- **URL:** unicrypt.network
- **What it does:** Allows token developers to lock liquidity pool tokens in a smart contract for a specified duration. Once locked, the tokens cannot be withdrawn until the lock period expires.
- **What it does not do:** Unicrypt is a voluntary tool. No exchange mandates its use as a listing requirement. There is no minimum lock duration standard, no maximum release rate specification, no audit of the underlying contract by Unicrypt, and no integration with a broader multi-layer scam-prevention framework.
- **Status relative to CTS:** Addresses L1 only, voluntarily, with no enforceable standard behind it.

### Team.Finance
- **URL:** team.finance
- **What it does:** Similar to Unicrypt — allows vesting and locking of tokens and liquidity. Includes some governance features.
- **What it does not do:** Same limitations as Unicrypt. Voluntary, single-layer, no exchange mandate, no connection to anti-whale or identity verification.
- **Status relative to CTS:** Addresses L1 only, voluntarily.

### DxLock / PinkLock
- **What they do:** Additional liquidity locking services in the DeFi ecosystem.
- **What they do not do:** Same as above — voluntary, single-layer, no standard.
- **Status relative to CTS:** Addresses L1 only, voluntarily.

**Overall finding on this category:** Liquidity locking is a well-developed tool category with multiple providers. None of these providers publish or enforce a minimum standard for lock duration, release rates, or the non-upgradeability of the locking contract. None of them connect to the other three scam vectors CTS addresses.

---

## Category 2: Smart Contract Audit Firms

### CertiK
- **URL:** certik.com
- **What it does:** Audits smart contract code for vulnerabilities, bugs, and security risks. Publishes audit reports publicly. Operates a "Skynet" monitoring system for ongoing alerts.
- **What it does not do:** A CertiK audit verifies that the code is correct and secure — it does not verify that the project is scam-resistant at the business level. A rug pull can pass a CertiK audit if the liquidity is not locked. A pump-and-dump scheme can pass if there are no whale restrictions. CertiK does not audit off-chain promotional activity or verify founder identities. Audits are one-time or periodic, not continuous. No exchange requires CertiK certification as a mandatory listing standard.
- **Status relative to CTS:** Partially overlaps with L3 (code correctness) but does not address L1, L2, or L4. Not an exchange-mandated standard.

### Hacken
- **URL:** hacken.io
- **What it does:** Smart contract security audits, penetration testing, bug bounties. Also operates HackenAI as a security rating system.
- **What it does not do:** Same limitations as CertiK. Code security, not scam-resistance. No exchange mandate.
- **Status relative to CTS:** Same as CertiK.

### Quantstamp / Trail of Bits / OpenZeppelin
- **What they do:** High-end smart contract audit firms serving institutional and major DeFi projects.
- **What they do not do:** Same limitations — code review only, no scam-prevention bundle, no exchange mandate.
- **Status relative to CTS:** Code security only.

**Overall finding on this category:** Smart contract audits address code correctness. They are valuable but explicitly do not address the four scam types CTS targets. The audit industry itself acknowledges this: a passed audit does not mean a project is safe to invest in. CTS's L3 (on-chain verification) is categorically different from a smart contract audit — it specifies how live balance data must be sourced and displayed, not whether the contract code is bug-free.

---

## Category 3: Blockchain Analytics and Compliance

### Chainalysis
- **URL:** chainalysis.com
- **What it does:** Transaction monitoring and analytics for exchanges, regulators, and law enforcement. Tracks fund flows, identifies high-risk wallets, supports AML compliance. Provides the Reactor investigation tool and Kryptos compliance platform.
- **What it does not do:** Chainalysis operates on existing transactions after they happen. It does not prevent scam coin listings. It does not specify technical requirements for token projects. It does not address liquidity locking, anti-whale enforcement, platform verification, or promotional identity. It is a forensics and monitoring tool, not a pre-listing safety standard.
- **Status relative to CTS:** No overlap with CTS's function. Complementary rather than competitive.

### Elliptic
- **URL:** elliptic.co
- **What it does:** Similar to Chainalysis — blockchain analytics, AML compliance, transaction risk scoring.
- **Status relative to CTS:** Same as Chainalysis. Forensics, not prevention framework.

### TRM Labs
- **URL:** trmlabs.com
- **What it does:** Blockchain intelligence for financial crime compliance.
- **Status relative to CTS:** Same as Chainalysis.

**Overall finding on this category:** Blockchain analytics firms are surveillance and compliance tools for after-the-fact detection. They are not pre-listing safety standards and do not address the four scam types CTS targets.

---

## Category 4: Identity and Wallet Verification

### Ethereum Name Service (ENS)
- **URL:** ens.domains
- **What it does:** Maps human-readable names to Ethereum wallet addresses. Allows wallets to have a public name (e.g., vitalik.eth).
- **What it does not do:** ENS provides naming, not identity verification. There is no real-world KYC tied to an ENS name. Anyone can register any name. There is no mechanism to verify that a promotional claim is authorized by the wallet owner. ENS does not connect to any promotional content signing or scam prevention framework.
- **Status relative to CTS:** Does not address L4. L4 requires zk-proof KYC (real-world identity verified without exposing it), a registry of authorized promoters, and a requirement that all promotional content be wallet-signed. ENS does none of this.

### Proof of Humanity / Worldcoin
- **What they do:** Attempt to create verified human identity on-chain.
- **What they do not do:** Neither is a promotional endorsement registry. Neither addresses crypto scam promotion specifically. Neither is connected to exchange listing requirements.
- **Status relative to CTS:** Conceptually adjacent to L4's identity verification component, but not a framework for promotional content accountability in the crypto context.

**Overall finding on this category:** No existing identity or wallet verification tool addresses the specific L4 problem: cryptographically verifying that promotional content for a token was created by a real, KYC-verified person who is authorized by the token project.

---

## Category 5: Standards Bodies and Published Standards

### CCSS — Cryptocurrency Security Standard
- **URL:** cryptoconsortium.org
- **Published by:** CryptoCurrency Certification Consortium (C4)
- **What it does:** Defines security requirements for organizations that hold or transact cryptocurrency — exchanges, wallets, custodians. Covers key management, authentication, data sanitization, and operational security. Has three levels of compliance.
- **What it does not do:** CCSS is entirely about the security of cryptocurrency businesses and their operations. It has no provisions for token project safety, liquidity locking, anti-whale enforcement, on-chain verification of balance displays, or promotional identity verification. CCSS is not an exchange listing requirement for token projects — it is a security framework for the exchange itself.
- **Status relative to CTS:** Categorically different target. CCSS governs crypto businesses; CTS governs token projects. No substantive overlap.

### MiCA — Markets in Crypto-Assets Regulation (EU)
- **What it does:** EU regulatory framework for crypto asset issuers and service providers. Requires whitepapers for most crypto assets, defines categories, establishes reserve requirements for stablecoins, and mandates certain disclosures.
- **What it does not do:** MiCA is a disclosure and registration framework. It does not specify technical requirements for liquidity locking, anti-whale mechanisms, on-chain balance verification, or endorsement registries. MiCA compliance does not prevent rug pulls, pump-and-dumps, fake platforms, or fake celebrity scams.
- **Status relative to CTS:** Regulatory disclosure framework vs. technical scam-prevention standard. Complementary — CTS could be referenced in MiCA compliance strategy, but the two are not the same thing.

### IOSCO Crypto Policy Recommendations (2023)
- **What it does:** High-level policy recommendations for regulators on oversight of crypto asset markets.
- **What it does not do:** Not a technical standard. Not enforceable. Does not address the four scam types CTS targets at a technical level.
- **Status relative to CTS:** Regulatory policy, not a technical framework.

---

## Category 6: Anti-Whale Mechanisms in Existing Coins

Some token projects implement their own anti-whale mechanisms. Examples include transfer limits, wallet size caps, and sell taxes. These vary widely and share the following characteristics:

- **Non-standard:** Every implementation is different. There is no shared specification.
- **Removable:** Typically controlled by the token's owners and can be modified or removed.
- **Unverified:** No third party verifies that the mechanism is active or properly implemented.
- **No exchange mandate:** No exchange requires anti-whale mechanisms as a listing condition.

**Status relative to CTS:** CTS's L2 is a specified, external, proposed standard for how anti-whale mechanisms must be implemented and governed — one any exchange can choose to adopt as a listing requirement. It requires supermajority governance vote to modify and automated verification. This is categorically different from a coin implementing its own informal cap.

---

## Summary Table

| Tool / Standard | L1: Liquidity Lock | L2: Anti-Whale | L3: On-Chain Verify | L4: ID Registry | Exchange-Adoptable Design | Bundled Standard |
|----------------|:-:|:-:|:-:|:-:|:-:|:-:|
| Unicrypt / Team.Finance | Partial ✓ | — | — | — | — | — |
| CertiK / Hacken | — | — | Partial ✓ | — | — | — |
| Chainalysis / Elliptic | — | — | — | — | — | — |
| ENS | — | — | — | Partial ✓ | — | — |
| CCSS | — | — | — | — | — | — |
| MiCA | — | — | — | — | — | — |
| Anti-whale (in-coin) | — | Partial ✓ | — | — | — | — |
| **Crypto Trust Standard (CTS)** | **✓** | **✓** | **✓** | **✓** | **✓** | **✓** |

*Partial ✓ = the tool addresses a related concern but does not meet CTS's specification for that layer.*

---

*Document Version 1.0 · NMA Consulting Group · Private & Confidential · September 2026*
