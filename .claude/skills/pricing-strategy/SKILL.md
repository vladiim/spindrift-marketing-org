---
disable-model-invocation: true
argument-hint: /pricing-strategy [scope] — scope: full-review|channel-pricing|promo-strategy|new-sku|competitive-benchmark
---

# /pricing-strategy — CPG Pricing Strategy

Develops pricing strategy for Spindrift across channels, SKUs, and competitive contexts. Covers channel pricing architecture, promotional strategy, price pack architecture, and competitive positioning — all grounded in Spindrift's premium real-ingredient positioning.

## Before Executing

Read the following memory files to ground pricing decisions in Spindrift's actual situation:

- `.claude/product-marketing-context.md` — company, product, price positioning, and competitive context
- `/memory/shared/positioning.md` — positioning framework and competitive comparison matrix (includes pricing data)
- `/memory/shared/icp.md` — ideal customer profile, purchase triggers, and objections (especially the price objection and reframe)

Also scan for additional context:

- `/memory/strategy/competitors/` — competitive pricing intelligence
- `/memory/analytics/` — sales velocity data, promo lift data, channel mix
- `/memory/strategy/` — strategic priorities that affect pricing decisions

## Spindrift Pricing Context

### Current Price Architecture

| SKU | DTC | Amazon | Grocery | Club (Costco) | Convenience |
|-----|-----|--------|---------|----------------|-------------|
| 8-pack (12oz cans) | $7.99 | $6.99-$7.49 | $5.49-$6.99 | N/A | N/A |
| 12-pack (12oz cans) | $10.99 | $9.99-$10.49 | $7.99-$9.99 | N/A | N/A |
| 24-pack (12oz cans) | N/A | $17.99-$19.99 | N/A | $16.99-$18.99 | N/A |
| Single can (12oz) | N/A | N/A | N/A | N/A | $1.99-$2.49 |
| Variety pack | $12.99 | $11.99 | N/A | $18.99 (24ct) | N/A |

*Note: Retail prices vary by region and retailer. These are approximate national averages. Update with actual data from `/memory/analytics/` when available.*

### Premium Positioning Rationale

Spindrift's $5-7/8-pack price point (vs. $3-5 for competitors) is justified by:

1. **Real squeezed fruit** — actual fruit juice costs more than "natural flavors" (synthetic flavoring). The COGS difference is real and significant.
2. **Ingredient transparency** — the premium signals quality to label-readers. Price IS a positioning tool.
3. **Category reframe** — Spindrift competes less against $0.40/can seltzer and more against $3-4 kombucha, $2-3 juice, and $5+ specialty coffee. Reframe the comparison set.
4. **ICP willingness to pay** — the target customer ($55K-$130K HHI) pays premiums for ingredient quality across categories (organic produce, specialty coffee, premium yogurt).

### Competitive Price Map

| Brand | Per-Can (approx.) | Price Index (Spindrift = 100) |
|-------|-------------------|-------------------------------|
| **Spindrift** | $0.85-$1.25 | 100 |
| Liquid Death (flavored) | $0.85-$1.10 | 85-90 |
| Topo Chico (flavored) | $0.75-$1.00 | 75-85 |
| LaCroix | $0.40-$0.55 | 40-50 |
| Polar | $0.35-$0.50 | 35-45 |
| Store brand | $0.25-$0.45 | 25-40 |

### Price Objection Reframe (from ICP document)

> **Objection:** "It's expensive vs. LaCroix/store brand"
> **Reframe:** It's cheaper than juice ($0.50-$1.00/oz), kombucha ($3-4/bottle), or a coffee ($5+). You're replacing those, not replacing water.

## Channel Pricing Principles

### DTC (spindrift.com)
- **Role:** Premium experience, highest margin, subscription driver
- **Strategy:** Price at or above retail. Never undercut retailers (channel conflict risk). Add value through bundles, exclusives, and subscription savings — not discounts.
- **Subscribe & Save:** 10-15% discount is the primary incentive. Frames as "member price," not "discount."

### Amazon
- **Role:** Convenience + bulk purchase + discovery
- **Strategy:** Match or slightly undercut DTC to reflect marketplace expectations. Subscribe & Save at 5-15% off. Monitor MAP (minimum advertised price) compliance. Win the "sparkling water" search Buy Box.
- **Risk:** Price erosion from 3P sellers. Monitor and enforce.

### Grocery (Whole Foods, Target, Kroger, etc.)
- **Role:** Primary volume channel, trial driver
- **Strategy:** Maintain premium shelf price. Promotional pricing (TPR) on a cadence that drives trial without training deal-seekers. Feature in weekly circulars for new flavor launches.
- **Promotion guardrails:** No more than 4-6 promoted weeks per year per retailer. Never more than 20% off. Promote multipacks over singles.

### Club (Costco, Sam's)
- **Role:** Volume, loyalty milestone, household penetration
- **Strategy:** Larger pack size at lower per-unit cost. The 24-pack at Costco is where a casual buyer becomes a household staple. Price per can should be 15-25% below grocery single-pack equivalent.

### Convenience (7-Eleven, gas stations, bodegas)
- **Role:** Impulse, single-serve premium, new occasion
- **Strategy:** Highest per-unit price. Single-serve premium justified by impulse and immediate consumption. $1.99-$2.49 per can. Placement next to premium water and energy drinks, not value seltzer.

## Execution Steps

### Step 1: Define Scope

Based on the provided `[scope]`, focus the analysis:

- **Full review:** Comprehensive pricing audit across all channels and SKUs
- **Channel pricing:** Deep dive on a specific channel's pricing strategy
- **Promo strategy:** Promotional calendar, depth, and frequency recommendations
- **New SKU:** Pricing recommendation for a new product or pack size
- **Competitive benchmark:** Updated competitive pricing analysis and positioning

### Step 2: Gather Data

- Pull current pricing from available data sources
- Review competitive pricing (update the competitive map if new data exists)
- Check promotional history and lift data
- Review channel mix and margin contribution

### Step 3: Apply Pricing Frameworks

**For new SKU or full review — Van Westendorp Price Sensitivity:**
- Define the four price points: too cheap (quality concern), cheap (good deal), expensive (but would consider), too expensive (out of consideration)
- For Spindrift ICP, the "too cheap" threshold is real — if Spindrift costs the same as LaCroix, the ICP questions whether the ingredients are actually different.

**For competitive benchmark — Value-Based Pricing:**
- Map price vs. perceived value for Spindrift and competitors
- Identify white space (underpriced relative to value, or competitor vulnerability)
- Calculate price premium justification using ingredient cost differential

**For promo strategy — Promotional Effectiveness:**
- Base velocity vs. promoted velocity lift
- Post-promotion dip analysis (do sales crater after the promo?)
- Promotional ROI: incremental revenue vs. margin erosion
- Frequency optimization: how often can you promote without conditioning deal-seeking?

### Step 4: Develop Recommendations

- Channel-specific pricing recommendations
- Promotional calendar with depth, frequency, and duration
- Price pack architecture recommendations
- Competitive response scenarios

## Output Format

```
# Pricing Strategy — [Scope]
**Date:** [YYYY-MM-DD]
**Scope:** [Full review / Channel / Promo / New SKU / Competitive benchmark]

## Executive Summary
[2-3 sentences: the headline pricing recommendation and rationale]

## Current State Assessment

### Price Architecture
| SKU | [Channel 1] | [Channel 2] | [Channel 3] | Margin Notes |
|-----|-------------|-------------|-------------|--------------|
| ... | ... | ... | ... | ... |

### Competitive Position
| Brand | Per-Unit Price | Price Index | Value Perception | Vulnerability |
|-------|---------------|-------------|------------------|---------------|
| ... | ... | ... | ... | ... |

## Analysis

### [Framework Applied]
[Van Westendorp results, competitive benchmark analysis, promo effectiveness analysis, etc.]

### Key Findings
1. [Finding with evidence]
2. [Finding with evidence]
3. [Finding with evidence]

## Recommendations

### 1. [Recommendation]
- **What:** [Specific pricing action]
- **Why:** [Strategic rationale grounded in Spindrift's positioning]
- **Impact:** [Expected effect on volume, revenue, margin, brand perception]
- **Risk:** [What could go wrong and mitigation]

### 2. [Recommendation]
...

### Promotional Calendar (if applicable)
| Period | Retailer/Channel | Promo Type | Depth | Duration | Objective |
|--------|-----------------|-----------|-------|----------|-----------|
| ... | ... | ... | ... | ... | ... |

### Price Pack Architecture (if applicable)
| Pack Size | Channel | Price | Per-Unit | Role | Margin |
|-----------|---------|-------|----------|------|--------|
| ... | ... | ... | ... | ... | ... |

## Scenarios

### If competitor cuts price:
[Response framework]

### If COGS increase:
[Pass-through vs. absorb decision framework]

### If entering new channel:
[Pricing approach for new distribution]

## Quality Checklist
- [ ] Premium positioning maintained — no recommendations that erode brand perception
- [ ] Channel conflict avoided — DTC not undercutting retail
- [ ] Promotional depth stays within guardrails (never >20% off)
- [ ] Price objection reframes reinforced (compare to juice/kombucha/coffee, not seltzer)
- [ ] Ingredient cost premium acknowledged as real COGS difference, not just brand markup
- [ ] ICP willingness-to-pay aligned with recommendations
- [ ] Competitive response doesn't trigger race-to-bottom
```

## Save Location

Save to: `/projects/active/pricing/[scope-slug]-[YYYY-MM-DD].md`

## Related Skills

- `/competitor` — Run updated competitive analysis including pricing
- `/diagnose` — If pricing challenges reveal deeper strategic issues
