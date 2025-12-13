# Blackhaven Final

# Overview

Blackhaven is a reserve-backed treasury that functions as a liquidity engine for the MegaETH ecosystem. It grows by putting deposited capital to work in vetted DeFi strategies, then shares the returns with participants while building up its reserves.

Users deposit assets and receive principal-protected notes or fixed-term bonds. These instruments earn yield as the treasury deploys capital into approved MegaETH protocols. Returns flow back to participants, and any surplus gets reinvested to grow the reserve.

The treasury also expands by capturing its own trading premium. When the treasury token trades above its backing value, the protocol mints new tokens and sells them at that premium. This adds more assets to the reserve without diluting existing holders, since each new token is backed by more than it should be.

---

**Core Objectives**

Blackhaven is designed to achieve five core objectives that define its function within the MegaETH ecosystem:

| **Objective**                                                    | **Description**                                                                                                    |
| ---------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| **Protect Principal**                                            | Note depositors' capital stays fully backed and redeemable, with verifiable on-chain reserves.                     |
| **Capture On-Chain Value**                                       | Earn rewards from approved MegaETH DeFi strategies that balance capital efficiency with risk-adjusted performance. |
| **Accumulate Reserve Value**                                     | Grow treasury assets through bonds, fees, forfeits, and ecosystem rewards.                                         |
| **Anchor Liquidity Across the MegaETH Ecosystem**                | Support and stabilize key MegaETH protocols by directing reserves into ecosystem pools                             |
| **Function as a Digital Asset Treasury (DAT) Layer for MegaETH** | Build a foundational, sustainable treasury backbone that powers MegaETH's long-term infrastructure.                |

<aside>
💡

**Blackhaven is the reserve-backed liquidity engine powering sustainable rewards and treasury growth across the MegaETH ecosystem.**

</aside>

---

# HVN (Governance Token)

## Governance

HVN is the governance token of Blackhaven. It gives holders direct influence over key parameters and strategic direction. Governance is fully on-chain and open to all HVN holders.

Contributors and core participants initiate proposals, while HVN holders vote to approve or reject them. This keeps decision-making efficient and informed while still reflecting the community's will.

Proposals may include adjustments to:

- Treasury composition, deployment strategy, and reserve parameters
- Reward distribution rates and emission schedules
- Approval or removal of MegaETH DeFi strategies
- Allocation of Blackhaven's staked MEGA within the Proximity Market

Each HVN token represents one vote. This keeps the process transparent, data-driven, and aligned with long-term ecosystem growth.

## **Staking & Rewards (sHVN)**

sHVN represents staked HVN and serves as the governance-linked token that anchors participation and reward distribution across Blackhaven.

sHVN holders earn rewards from treasury growth and other incentives accumulated through treasury management. Rewards will be distributed to stakers based on the available reward pool, which will be configured after the treasury growth phase through a governance proposal.

The system rewards participants who demonstrate long-term alignment with Blackhaven's growth, not short-term speculation.

## Fee Structure and Value Accrual

Blackhaven's fee structure is designed to create a sustainable, self-reinforcing flywheel that rewards both RBT and HVN holders for their distinct contributions to the ecosystem.

**Revenue Sources**

The Blackhaven treasury generates revenue from six primary sources:

1. **Yield from DeFi Strategies:** Returns generated from deploying HPN deposits into whitelisted MegaETH protocols.
2. **Early Exit Fees:** Penalties collected from users who exit HPNs or bonds before maturity.
3. **Premium Capture Module Fees (PCM):** Fees generated from arbitraging RBT when it trades above its backing.
4. **Sequencer Staking Rewards:** Yield earned from staking the treasury's MEGA holdings.
5. **Trading Fees from RBT Pool:** Fees generated from the RBT-USDM liquidity pool.
6. **Trading Fees from HVN Pool:** Fees generated from the HVN-USDM liquidity pool.

**Fee Split and Bootstrap Period**

To ensure the treasury has sufficient resources to build a strong foundation, there will be a bootstrap period following the launch of the HVN token. During this period, 100% of all net treasury revenue will be directed to the protocol treasury to build Protocol-Owned Liquidity (POL) and fund operations. After the bootstrap period, revenue sharing will be activated.

> Fees from net treasury revenue will be allocated to sHVN holders in the form of buybacks, while a portion will continue to flow to the protocol treasury.

## **Proximity Influence (MegaETH Integration)**

> MegaETH’s Proximity Market allows market makers and dApps to bid for sequencer-adjacent floorspace, improving execution speed and liquidity efficiency across DeFi.

Blackhaven will actively participate in the MegaETH sequencer and proximity markets using MEGA accumulated through treasury operations. HVN governance controls how this MEGA is deployed to strengthen Blackhaven's position within the ecosystem and align with yield opportunities and network utility.

### **Blackhaven Bribe Market**

External parties could bribe Blackhaven into directing existing staked MEGA toward their floorspace. This lets external parties access the proximity market without taking on the price risk and liquidity constraints of buying and staking MEGA directly.

For HVN holders, bribes flow into the treasury to further increase reserve backing, creating another revenue stream on top of treasury performance. The more MEGA Blackhaven accumulates, the more valuable HVN voting power becomes to external parties competing for proximity market allocation.

## Baseline Utilization

Blackhaven will launch HVN on Baseline Markets, a token market built around real, locked liquidity where the system handles price discovery and liquidity (not market makers). Baseline establishes an on-chain Baseline Value (BLV) that acts as a guaranteed price floor, backed by reserves for every token. Buyers get a protected, transparent entry from day one.

**How Baseline works for HVN**

- The BLV sets the lowest tradable price on-chain and rises with trading activity and liquidity depth
- Liquidity is autonomous and value-retentive, with no custom deals, private spreads, or silent extraction
- Capital-efficient, liquidation-free borrowing and leverage scales liquidity with demand, supporting deeper markets and fairer participation

**Why this matters**

- Clear downside definition at launch
- Liquidity that cannot be pulled by third parties
- Growth tied to real market activity rather than emissions

By combining a guaranteed price floor (BLV) with capital-efficient borrowing and non-liquidatable leverage, Baseline automatically scales liquidity to support higher prices, deeper markets, and fairer participation. [Baseline Market Docs](https://docs.baseline.markets/).

### Tokenomics [add after announcing raise]

---

# RBT Overview

The Reserve-Backed Token (RBT) represents the underlying backing of the Blackhaven treasury. Its value is supported by on-chain reserves that grow through bond issuance, Haven Protected Note (HPN) forfeits, early redemptions, and treasury yields.

Users receive RBT through Bonds, by redeeming Haven Protected Notes against RBT, or by purchasing on the open market. As treasury inflows increase, additional RBT is issued proportionally to preserve the reserve ratio. All backing assets are held and managed by the Blackhaven treasury with full transparency and verifiable on-chain accountability.

RBT can be used across the MegaETH DeFi ecosystem in various products and liquidity strategies, allowing users to engage with on-chain markets while maintaining alignment with Blackhaven's treasury growth.

## RBT NOTES

RBT Notes are fixed-term lockup instruments issued as ERC-721 NFTs that let holders earn guaranteed yield by committing their RBT for a set period. Unlike liquid staking where rewards vary and capital can leave at any time, Notes offer a simple proposition: lock now, know your exact return, collect at maturity.

**How Notes Work**

1. Choose your term
2. Deposit RBT into the contract
3. Receive an NFT representing your position
4. Your yield is calculated and locked in from day one
5. At maturity, burn the NFT and claim principal plus yield

**Early Exit**

You can redeem before maturity, but it comes with two costs:

1. **Forfeited yield:** You receive zero yield regardless of how long you held
2. **Principal penalty:** Up to 10% of your deposit, scaling linearly with time remaining

The penalty decreases proportionally with time held. Exit at the start of your term and pay the full 10%. Exit halfway through and pay 5%. Exit near maturity and pay close to nothing.

<aside>
💡

Penalties flow back into the contract, funding future yields for holders who complete their terms.

</aside>

### RBT Notes Yield Curve

Yield scales quadratically with term length, rewarding longer commitments disproportionately more than linear scaling.

$$
\text{APY}(t) = r_{\min} + (r_{\max} - r_{\min}) \times \left(\frac{t - t_{\min}}{t_{\max} - t_{\min}}\right)^2
$$

Where:

- _t_ = term length in weeks
- _t_min_ = 2 weeks, _t_max_ = 52 weeks
- _r_min_ = 2.5%, _r_max_ = 100%

### **Enhanced Bond Discounts**

Active RBT Notes unlock scaled bond discounts based on term length and amount locked. The discount bonus applies automatically when purchasing bonds, with longer commitments and larger positions earning greater advantages.

**Formula:**

```jsx
Eligibility:
- Note Term > 12 weeks
- RBT Amount ≥ Minimum Threshold

Thresholds (governance-adjustable):
- Min Threshold = sqrt(Total RBT Supply) × K1
- Max Threshold = sqrt(Total RBT Supply) × K2
- Initial values: K1 = 0.01, K2 = 0.1

Bonus Calculation:
- Term Factor = (Note Term - 12) / (52 - 12)
- Amount Factor = min((RBT Amount - Min Threshold) / (Max Threshold - Min Threshold), 1)
- Combined Factor = (Term Factor + Amount Factor) / 2
- Bonus Discount = Combined Factor × 2.5%

Final Bond Discount = Base Discount (from debt ratio) + Bonus Discount
```

As total RBT supply grows, thresholds scale proportionally via the square root function. Governance may adjust K1 and K2 parameters to maintain appropriate dollar-value requirements as market conditions evolve:

$$
D_{\text{final}} = D_{\text{base}} + \left[\frac{1}{2}\left(\frac{t - 12}{52 - 12} + \min\left(\frac{A - K_1\sqrt{S}}{(K_2 - K_1)\sqrt{S}}, 1\right)\right) \times 0.025\right]
$$

where:

- _D_final_ = final bond discount
- _D_base_ = base discount from debt ratio
- _t_ = Note term in weeks
- _A_ = RBT amount locked in Note
- _S_ = total RBT circulating supply
- _K1_ = 0.01, _K2_ = 0.1
