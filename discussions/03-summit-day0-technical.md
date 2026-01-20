# Cardano Summit Day0 - Technical Discussion

**Date**: November 11, 2025
**Event**: Cardano Summit 2025 Day 0 Governance Day
**Session**: Technical Breakout Group
**Moderator**: Hinson Wong
**Key Contributor**: Samuel Leathers (Input Output, Product Committee Chair)

## Key Technical Findings

### Smart Contract Approach

- Smart contract as treasury might not be easy to implement due to execution units limits
- You can't calculate a vote of everyone in the system instantaneously, which you have to do to validate a smart contract
- Smart contract validation can't span 48 hours - it would freeze the system

### Preferred Approach: CIP-159 Style

- CIP-159 approach is preferred
- We are NOT turning treasury into an address
- It is only for enabling users to withdraw from the treasury
- Implement the treasury in a simpler way of holding `Value` rather than `Coin`
- Add extra guardrails on whitelisting and de-whitelisting

### Implementation Details

1. **Reward Account Changes**
   - Augment the reward account (CIP-159) to be a multi-asset list instead of just a single value
   - Wallets opt-in to which tokens they accept in their reward account

2. **Whitelisting Mechanism**
   - Governance action to allow community to whitelist assets for treasury
   - Once whitelisted, anyone holding those tokens can donate to treasury
   - Tokens sit in treasury until governance action withdraws them

3. **Rollout Strategy**
   - Two hard forks approach (similar to CIP-1694 rollout)
   - Hard Fork 1: Introduce feature but deactivated
   - Window for: Constitution updates, guardrails, protocol parameters
   - Hard Fork 2: Intra-era hard fork to enable feature permanently

### Open Questions Raised

- How does NCL (Net Change Limit) work post-CMAT?
- Does NCL only apply to ADA or to other assets as well?
- NIGHT token can be a pathway to drive value back to Cardano ecosystem
- Groundwork for putting BTC at treasury

## Technical Rationale

> "The main reason why the treasury isn't a smart contract is because you can't calculate a vote of everyone in the system instantaneously which you have to do basically to validate a smart contract... The whole reason CIP-1694 put the treasury into the ledger is because it pulses that governance period over the course of 48 hours at the beginning of every epoch."
> — Sam Leathers
