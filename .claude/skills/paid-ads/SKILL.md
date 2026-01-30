---
disable-model-invocation: true
argument-hint: /paid-ads [platform] [objective] — platform: meta|tiktok|google|retail-media|all; objective: awareness|conversion|retargeting
---

# /paid-ads — Paid Advertising Campaign Builder

Builds paid media campaigns for Spindrift across Meta, TikTok, Google, and retail media networks. Outputs campaign structure, creative direction, targeting, and measurement — all grounded in Spindrift's real-ingredient positioning.

## Before Executing

Read the following memory files to ground the campaign in Spindrift's actual situation:

- `.claude/product-marketing-context.md` — company, product, and competitive context
- `/memory/shared/positioning.md` — positioning framework and messaging hierarchy
- `/memory/shared/icp.md` — ideal customer profile, behavioral data, and purchase triggers
- `/memory/shared/voice.md` — brand voice guidelines (especially the Advertising tone section)

Also scan for additional context:

- `/memory/analytics/` — recent performance data and channel benchmarks
- `/memory/strategy/` — active strategic priorities
- `/projects/active/` — current campaigns to avoid overlap or find synergies

## Spindrift Platform Strategy

### Meta (Instagram / Facebook)
- **Primary role:** DTC acquisition + brand awareness
- **Instagram:** Hero channel. Real fruit visuals, ingredient close-ups, process content. Reels for discovery, Stories for retargeting, Feed for brand building.
- **Facebook:** Retargeting and lookalike audiences. Skews older within ICP (35-42). Subscription conversion focus.
- **Creative rule:** Lead with real fruit visuals and ingredient transparency, never lifestyle-first. Show the product, then the moment. Not the other way around.
- **Best-performing formats:** Ingredient-list close-ups, side-by-side comparisons (implied, never naming competitors), "what's actually in your sparkling water" educational hooks.

### TikTok
- **Primary role:** Awareness + ingredient storytelling for younger ICP tail (22-30)
- **Content style:** Process videos (fruit being squeezed, production), ingredient transparency reveals, taste-test reactions, "read the label" challenges.
- **Creative rule:** Native-feeling, not polished. Creator-style over brand-style. Spark Ads from organic content outperform studio creative.
- **Best hooks:** "I read the ingredients on every sparkling water brand," "What's actually in your seltzer," "The reason Spindrift is cloudy."

### Google
- **Primary role:** Capture high-intent search demand
- **Search campaigns:** Brand terms, category terms ("sparkling water," "flavored seltzer," "sparkling water with real fruit"), competitor conquest (non-branded: "best sparkling water," "LaCroix alternative," "healthiest sparkling water").
- **Shopping:** DTC product listings, Subscribe & Save promotion.
- **YouTube:** Pre-roll (15s ingredient-focused), Discovery ads for recipe/wellness content adjacency.

### Retail Media (Instacart, Kroger, Amazon)
- **Primary role:** Point-of-purchase conversion and shelf visibility
- **Instacart:** Sponsored search for category and brand terms. Target sparkling water aisle browsers. Promote variety packs.
- **Amazon:** Sponsored Products + Sponsored Brands. Subscribe & Save callout. A+ Content reinforcing real ingredients.
- **Kroger/Target/Walmart media:** Co-op digital when launching new flavors or entering new regions.

## Campaign Naming Convention

```
SPD-[PLATFORM]-[OBJECTIVE]-[AUDIENCE]-[CREATIVE]-[DATE]
```

- **SPD** = Spindrift
- **Platform:** META, TT, GOOG, INST, AMZN, RETAIL
- **Objective:** AWR (awareness), CONV (conversion), RET (retargeting), CONQ (conquest)
- **Audience:** PROSP (prospecting), LAL (lookalike), RET (retargeting), BRAND (brand search)
- **Creative:** INGR (ingredient), PROC (process), TASTE (taste test), COMP (comparison), SEAS (seasonal)
- **Date:** YYYYMMDD

Example: `SPD-META-CONV-LAL-INGR-20260130`

## Performance Targets

| Metric | Target | Notes |
|--------|--------|-------|
| Blended ROAS | 3.0x | Across all paid channels |
| CAC (first purchase) | <$18 | DTC first-order acquisition |
| Meta CPM | $8-14 | Varies by objective |
| Meta CTR | >1.2% | Conversion campaigns |
| TikTok CPM | $5-10 | Awareness campaigns |
| TikTok CTR | >1.5% | Native content format |
| Google Search CPC | $0.80-$2.50 | Category terms |
| Google Brand CPC | <$0.40 | Brand defense |
| Instacart ROAS | 4.0x+ | Lower funnel, higher intent |
| Amazon ACOS | <25% | Sponsored Products |

## Execution Steps

### Step 1: Define Campaign Parameters

Based on the provided `[platform]` and `[objective]`, establish:

- **Platform(s):** Which channels to activate (default: recommend based on objective)
- **Objective:** Awareness, conversion, or retargeting
- **Budget allocation suggestion:** Based on objective and platform efficiency
- **Flight dates:** If seasonal or launch-related, align to Spindrift's launch phases

### Step 2: Audience Strategy

Define targeting layers:

- **Core audiences:** Based on ICP demographics and psychographics
- **Interest targeting:** Ingredient-conscious, health-aware (not fitness), food/cooking, sustainability-pragmatic
- **Behavioral targeting:** Grocery shoppers, subscription buyers, competitive brand engagers
- **Lookalike/similar:** Seed from existing customers, subscription buyers, high-LTV segments
- **Exclusions:** Existing subscribers (for acquisition), recent purchasers (for prospecting)

### Step 3: Creative Direction

For each ad, specify:

- **Hook** (first 3 seconds / headline): Must feature real fruit or ingredient truth. Never open with lifestyle.
- **Body:** Ingredient story, product demonstration, or social proof
- **CTA:** "Try Spindrift" (primary), "Subscribe & Save" (retention), "Find in store" (retail awareness)
- **Visual requirements:** Real fruit imagery mandatory. Can must appear. Ingredient list visible in at least one frame/variant.

Creative must pass the voice check:
- Is this true and substantiatable?
- Does it lead with the product, not lifestyle?
- Would it pass the 5-year embarrassment test?
- Does it avoid words on the "Words We Avoid" list?

### Step 4: Measurement Framework

- **Primary KPI:** Aligned to objective (ROAS for conversion, CPM/reach for awareness, CPA for acquisition)
- **Secondary KPIs:** CTR, CPC, frequency, thumbstop rate (video)
- **Attribution:** Platform-reported + post-purchase survey ("How did you hear about us?")
- **Testing cadence:** Rotate creative every 2-3 weeks. Test one variable at a time.

## Output Format

```
# Paid Ads Campaign — [Platform] — [Objective]
**Date:** [YYYY-MM-DD]
**Platform:** [Platform(s)]
**Objective:** [Awareness / Conversion / Retargeting]

## Campaign Structure

### Campaign Name
[Using SPD naming convention]

### Audience
- **Targeting:** [Specific targeting parameters]
- **Lookalikes:** [Seed audience and %]
- **Exclusions:** [Who to exclude]
- **Estimated audience size:** [Range]

### Creative Direction

#### Ad 1: [Name]
- **Format:** [Static / Carousel / Video / Spark Ad]
- **Hook:** [First 3 seconds or headline]
- **Body:** [Key message and visual description]
- **CTA:** [Call to action]
- **Landing page:** [Destination]

#### Ad 2: [Name]
...

### Budget & Bidding
- **Daily budget:** [Amount]
- **Bid strategy:** [Strategy]
- **Flight:** [Start - End]

### Measurement
- **Primary KPI:** [Metric and target]
- **Secondary KPIs:** [Metrics]
- **Reporting cadence:** [Frequency]

## Testing Plan
- **Variable to test:** [What we're testing]
- **Control vs variant:** [Description]
- **Sample size needed:** [Estimate]
- **Decision criteria:** [When to call a winner]

## Quality Checklist
- [ ] Creative leads with real fruit / ingredient truth, not lifestyle
- [ ] Voice aligns with Spindrift brand guidelines (real, warm, confident)
- [ ] No competitor names in ad copy
- [ ] No words from the "Words We Avoid" list
- [ ] CTA is plain language, not marketing-speak
- [ ] Ingredient list or real fruit visible in creative
- [ ] Campaign naming convention followed
- [ ] Targets align to ROAS 3.0x / CAC <$18 benchmarks
```

## Save Location

Save to: `/projects/active/paid-ads/[platform]-[objective]-[YYYY-MM-DD].md`

## Related Skills

- `/analytics` — Review campaign performance
- `/ab-test-setup` — Design experiments for ad creative and targeting
- Use insights from `/memory/shared/icp.md` purchase triggers to inform hook strategy
