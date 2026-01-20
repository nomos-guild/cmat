# Cardano Summit Day0 - CMAT Roundtable

**Date**: November 11, 2025
**Event**: Cardano Summit 2025 Day 0 Governance Day
**Recording**: [YouTube](https://www.youtube.com/watch?v=b-Vimpso3qw)

## Panelists

- **Hinson Wong** - Moderator
- **Shunsuke Murasaki** - GM of Ecosystem, Emurgo (Economics)
- **Samuel Leathers** - Input Output, Product Committee Chair (Technical)
- **Nicolas Cerny** - Governance Lead, Cardano Foundation (Governance)

## Overall Sentiment

No strong opposition to CMAT itself. Each stakeholder group sees strong benefits from the initiative.

---

## 1. Economics Perspective

*Moderated by Shunsuke Murasaki*

### Short-Term Objectives

- **Hedging**: Convert necessary funds for annual budget into stablecoins
- Secure runway for 1-2 years in stable value
- Reduce exposure to ADA volatility for predictable funding

### Long-Term Objectives

- **Active Treasury Management**: Generate yield from treasury assets
- Consider Cardano-native RWAs and gold-backed tokens
- Explore yield-bearing assets while keeping value on-chain

### Key Takeaways

- **Hedging & stability** – Use multi-asset treasury to shift some ADA into stablecoins for predictable funding
- **Yield & upside** – Over time hold yield-bearing RWAs and equity-like project tokens to grow the treasury
- **Cardano-native focus** – Prioritize Cardano-native stablecoins and RWAs to keep value on-chain
- **Phased risk** – Start with simple hedging, then consider higher-yield strategies and off-chain managers later
- **Less ADA dependence** – Diversify away from sole ADA exposure to improve financial resilience

---

## 2. Governance Perspective

*Moderated by Nicolas Cerny*

### Constitutional Changes Required

- Current guardrail states treasury withdrawals must be denominated in ADA
- Constitutional amendment required (75% DRep approval + CC approval)

### Asset Selection Approach

- Constitution should NOT hard-code specific assets (avoid picking winners/losers)
- Constitution should set principles and guardrails
- DReps choose which assets to whitelist via governance actions

### Key Takeaways

- **Constitution must change** – ADA-only withdrawal rule needs amendment for multi-asset treasury
- **Principles, not tickers** – Constitution should set guardrails, leaving asset selection to governance
- **DReps choose assets** – New governance actions let DReps whitelist tokens for the treasury
- **Extra load, cautious voters** – Multi-asset adds work, but DReps have shown conservative spending so far
- **Managing token politics** – Clear objectives and criteria are needed to handle meme-token and lobbying pressure

---

## 3. Technical Perspective

*Summary from technical breakout and Sam Leathers*

### Implementation Approach

- Extend reward accounts and treasury to hold lists of native assets (CIP-159 style)
- Keep treasury logic in ledger's epoch-based governance model, not smart contracts
- Wallets opt-in to which tokens they can receive in reward accounts

### Governance Integration

- Donations and withdrawals governed on-chain
- Hooks to verify off-chain swaps
- Whitelisting via governance action (simple majority may be sufficient)

### Key Takeaways

- **Multi-asset ledger support** – Extend rewards accounts and treasury to hold lists of native assets
- **Ledger-level governance** – Keep treasury logic in the ledger's epoch-based governance model
- **Wallet opt-in** – Wallets let users opt into which tokens they can receive
- **Governance-driven flows** – Donations and withdrawals governed on-chain with hooks for off-chain swaps
- **Two-step rollout** – Feature-introducing hard fork, then activation fork once guardrails are set

---

## Notable Quotes

### On Conservative DReps

> "DReps are way more conservative than anticipated. There's way less funds flowing out of the Treasury. We have an exchange limit in 2025 of 350 million ADA and currently only 272 million ADA was withdrawn."
> — Nicolas Cerny

### On Killer Feature

> "I think the killer feature is this basically allows projects that are being built within the ecosystem to give a commitment to the ecosystem that, hey, I'm providing you some equity in what I'm doing."
> — Sam Leathers

### On Phased Approach

> "Keep it simple in the beginning, only allow for stablecoins because that actually really addresses the pain point we're trying to solve - predictability."
> — James (Gimbal Labs), via Nicolas

### On Parallel Experimentation

> "We can still experiment with off-chain fund management currently. We have the stablecoin DeFi liquidity proposal. We should not just stop and do nothing until the hard forks potentially get implemented."
> — Nicolas Cerny

---

## Next Steps Identified

1. Finalize CPS revisions incorporating workshop feedback
2. Submit open pull request for CPS
3. Draft skeleton CIP for community contribution
4. Submit info action for community sense-check
5. Follow with constitution change and hard fork initiation

---

## Full Transcript

*See the [community-discussion.md](https://github.com/sidan-lab/CIPs/blob/cardano-multi-asset-treasury/CPS-0023/community-discussion.md) in the CPS repository for the complete transcript.*
