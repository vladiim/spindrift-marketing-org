---
disable-model-invocation: true
argument-hint: /marketing-ideas [focus area] — e.g., "brand awareness", "retail activation", "DTC growth", "sampling", "partnerships"
---

# /marketing-ideas — Marketing Ideas Generator

Generates actionable marketing ideas for Spindrift, pre-filtered for a CPG beverage brand at growth stage with national distribution. Ideas are grounded in Spindrift's positioning, ICP, and current strategic priorities — not generic marketing playbooks.

## Before Executing

Read the following memory files to ground ideation in Spindrift's actual situation:

- `.claude/product-marketing-context.md` — company, product, and competitive context
- `/memory/shared/positioning.md` — positioning framework, competitive reframes, messaging hierarchy
- `/memory/shared/icp.md` — ideal customer profile, purchase triggers, discovery channels, JTBD
- `/memory/shared/voice.md` — brand voice guidelines

Also scan for additional context:

- `/memory/strategy/` — current strategic priorities and past diagnoses
- `/projects/active/` — active initiatives (avoid duplicating, find synergies)
- `/memory/analytics/` — recent performance data to identify opportunities
- `/memory/strategy/competitors/` — competitive landscape for differentiation angles

## Spindrift Ideation Filters

### Include (Prioritize Ideas That...)
- **Build the brand around ingredient truth.** The "real squeezed fruit" story is Spindrift's moat. Every idea should reinforce it.
- **Drive trial.** Spindrift converts at a high rate once someone tastes it. Ideas that get the product into hands are disproportionately valuable.
- **Work across retail and DTC.** Spindrift sells in both channels. The best ideas drive traffic to wherever the customer prefers to buy.
- **Leverage the ingredient comparison moment.** The ICP's #1 purchase trigger is reading the label and seeing real fruit vs. "natural flavors." Ideas that create this moment — in-store, online, or in content — are high-value.
- **Scale nationally.** Spindrift has national distribution. Ideas should work at scale, not just in one market.
- **Strengthen the brand long-term.** At $100M+ revenue, brand building compounds. Short-term tactics should also serve long-term brand equity.

### Exclude (Filter Out Ideas That...)
- **Are SaaS-specific.** No free trials, freemium models, PLG motions, or B2B lead gen tactics. This is a physical consumer product.
- **Require copying Liquid Death's edge.** Spindrift's voice is warm and confident, not irreverent or provocative. Ideas that require attitude over substance are off-brand.
- **Depend on health claims.** Spindrift makes ingredient claims, not health claims. No "superfood," "functional," or "wellness" positioning.
- **Are one-market stunts.** PR stunts in a single city don't move the needle at Spindrift's scale unless they generate earned media nationally.
- **Require celebrity endorsement.** Spindrift's ICP trusts micro-influencers and ingredient transparency over celebrity. Big endorsement deals are low-ROI for this brand.
- **Involve discounting the core product.** Premium pricing is strategic. Ideas should drive value perception, not train customers to wait for sales.

## Idea Categories for Spindrift

### 1. Brand Building & Storytelling
Ideas that deepen the "real squeezed fruit" narrative and build long-term brand equity.
- Ingredient sourcing stories (where do our lemons come from?)
- Process transparency (how Spindrift is made)
- Founder story activations
- Brand documentary / docu-series content
- "Real vs. Natural Flavors" educational content

### 2. Ingredient Storytelling & Education
Ideas that turn ingredient transparency into a competitive weapon.
- Label-reading campaigns
- Ingredient comparison content (what's in our can vs. theirs — implied, not named)
- "What are natural flavors?" educational series
- Seasonal fruit sourcing stories
- Calorie-as-proof-point content (our 10 calories come from fruit)

### 3. Retail Activation
Ideas that drive trial and velocity at retail.
- In-store sampling programs (the highest-converting tactic for Spindrift)
- End-cap displays with ingredient story
- Shelf talkers and POS materials
- Retailer-specific promotions (Costco roadshows, Whole Foods features)
- Cross-merchandising (place near produce, not just beverage aisle)
- Seasonal retail activations (summer cooler, holiday entertaining)

### 4. DTC Growth
Ideas that grow Spindrift's direct-to-consumer business.
- Subscription acquisition and retention
- Variety pack strategy (discovery packs for new customers)
- Gifting programs (send a friend a pack)
- Unboxing experience as content
- Loyalty / rewards program
- Limited-edition DTC exclusives

### 5. Sampling & Trial Programs
Ideas that get the product into new mouths — Spindrift's highest-ROI activity.
- Office/workplace sampling (companies that stock good beverages)
- Event sampling (farmers markets, food festivals, fitness events)
- Subscription box inserts (meal kits, snack boxes)
- Hotel/airline partnerships (in-room, in-flight)
- "Side-by-side" tasting events (blind taste test: Spindrift vs. "natural flavor" brand)
- New mover / new parent welcome packs

### 6. Partnership Opportunities
Ideas that leverage complementary brands and audiences.
- Co-branded content with premium food brands (cheese, snacks, meal kits)
- Recipe collaborations with food creators
- Mocktail partnerships with spirit brands or bars
- Fitness studio / gym partnerships (post-workout hydration)
- Corporate wellness partnerships
- Music/food festival sponsorships (sampling + brand presence)

### 7. Community & UGC
Ideas that turn customers into advocates.
- Referral program (see `/referral-program` skill)
- UGC campaigns (share your Spindrift moment)
- Customer story features
- Flavor voting / co-creation for new flavors
- Brand ambassador program (micro-influencer seeding)

## Execution Steps

### Step 1: Understand the Focus Area

Based on the provided `[focus area]`, narrow ideation to the most relevant categories. If no focus area is provided, generate ideas across all categories weighted by current strategic priorities.

### Step 2: Review Current Context

- What is Spindrift already doing? (Check `/projects/active/`)
- What has worked before? (Check `/memory/analytics/`)
- What strategic challenges exist? (Check `/memory/strategy/`)
- What are competitors doing that Spindrift should counter? (Check `/memory/strategy/competitors/`)

### Step 3: Generate Ideas

Produce 8-12 ideas. For each idea:

- **Name it** clearly (not cleverly)
- **Describe it** in 2-3 sentences
- **Connect it to Spindrift's positioning** — how does it reinforce "real squeezed fruit"?
- **Identify the ICP trigger** — which purchase trigger or JTBD does it activate?
- **Estimate effort and impact** (Low/Medium/High for each)
- **Note channel fit** — where does this live (retail, DTC, social, email, events, PR)?

### Step 4: Prioritize

Rank ideas using a 2x2 of Impact vs. Effort. Recommend the top 3 for immediate action with brief implementation notes.

## Output Format

```
# Marketing Ideas — [Focus Area]
**Date:** [YYYY-MM-DD]
**Strategic context:** [1-2 sentences on current priorities informing ideation]

## Ideas

### 1. [Idea Name]
**What:** [2-3 sentence description]
**Positioning connection:** [How it reinforces "real squeezed fruit"]
**ICP trigger:** [Which purchase trigger it activates]
**Channels:** [Where it lives]
**Effort:** [Low / Medium / High]
**Impact:** [Low / Medium / High]

### 2. [Idea Name]
...

[Continue for 8-12 ideas]

## Prioritization Matrix

| Idea | Impact | Effort | Priority |
|------|--------|--------|----------|
| [Name] | [H/M/L] | [H/M/L] | [1-12] |
| ... | ... | ... | ... |

## Top 3 Recommendations

### 1. [Idea Name]
**Why now:** [Strategic rationale]
**First steps:** [2-3 concrete next actions]
**Timeline:** [Estimated time to launch]
**Resources needed:** [Team, budget, tools]

### 2. [Idea Name]
...

### 3. [Idea Name]
...

## Ideas Filtered Out (and Why)
[Brief note on any ideas considered but rejected per the Spindrift filters above]

## Quality Checklist
- [ ] Every idea reinforces Spindrift's real-ingredient positioning
- [ ] No SaaS-specific tactics included
- [ ] No ideas requiring edge/attitude inconsistent with brand voice
- [ ] No health claims — ingredient claims only
- [ ] Ideas work at national scale
- [ ] ICP triggers and JTBD explicitly connected
- [ ] Top 3 include concrete first steps, not just concepts
```

## Save Location

Save to: `/projects/active/ideas/[focus-area-slug]-[YYYY-MM-DD].md`

## Related Skills

- `/diagnose` — If ideation reveals a deeper strategic challenge, run a diagnosis
- `/brief` — Turn a selected idea into a full content brief
- `/launch-strategy` — If an idea becomes a launch initiative
