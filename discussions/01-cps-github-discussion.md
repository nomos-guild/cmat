# CPS-0023 GitHub Discussion

Discussion from the CPS-0023 pull request: [cardano-foundation/CIPs#1103](https://github.com/cardano-foundation/CIPs/pull/1103)

## Community Concerns (Oct 27, 2025)

Collected from community feedback:

- Treasury action is usually too slow (which allows front-running treasury conversion)
- No good candidate for actively managing the CMAT
- The problem statement is too narrowly-scoped

### Response from CIP-159 Author (fallen-icarus)

> **On slow treasury actions:**
> IMO this is actually a feature, not a bug. *It should be hard to change what assets are supported!* I was thinking it would have to go through the full voting process to get the whitelist certificates approved which should be very difficult to prevent a fickle treasury. This means whatever CNTs end up being supported need ecosystem-wide support. This rules out all but possibly some stablecoins right now.

> **On active management:**
> What do you mean "actively managing"? Why should the CMAT be actively managed more than what it already does? IMO the only thing that should be added is the ability to hold whitelisted CNTs. The funds inside the treasury should not be actively managed. They should just sit there until a treasury withdrawal is made. If the current ADA should be diversified into a supported stablecoin, this would involve an approved treasury withdrawal + conversion + treasury deposit of the new stablecoin. Then it just sits there until the community approves another diversification conversion or withdrawal. I do not think the treasury should be actively rebalanced since this opens the door to possible abuse/mismanagement - the entities doing the rebalancing could effectively pick winners and losers in DeFi which is not a good thing right now.

## CIP Editors Meeting Discussion (Nov 28, 2025)

Key points from CIP editors:

- The "whitelisted assets to be included" is currently deemed "Out of Scope" although the first open question relates to just such a determination
- The "open questions" in general read more like a debate over administrative decisions for such a multi-asset treasury rather than considerations that would be useful to provide technical solutions
- We'd like to see a full, practical consideration of the problem rather than a CPS placeholder for a single CIP

### Author Response (HinsonSIDAN)

> **On "out of scope":**
> The "out of scope" doesn't mean this topic should not be addressed by the solution CIP. It only means the CIP should not choose which assets to be included directly as it introduces a partial problem of "choosing the winners" by a proposed CIP.

> **On open questions:**
> The open questions would determine how technically a proposed CIP should be written. For example:
> - If spam prevention is not important (aka no whitelisting), it is possible to use a typical Cardano address as treasury
> - If it is important, the proposed CIP might indicate use CIP159 like account, or implement a specific way to allow whitelisting
> - Similarly, allowing participate in DeFi means the proposed CIP should cover how it should be achieved

## Related References

- [CIP-159: Multi-Asset Stake Addresses](https://github.com/fallen-icarus/CIPs/blob/account-enhancement/CIP-0159/README.md) - Related proposal for account enhancements
- [CIP-1061](https://github.com/cardano-foundation/CIPs/pull/1061) - Cross-referenced for progress updates
