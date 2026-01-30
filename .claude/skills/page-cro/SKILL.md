---
disable-model-invocation: true
argument-hint: /page-cro [page] — page: homepage|flavor-page|subscription|about|landing-page|cart
---

# /page-cro — Conversion Rate Optimization for Spindrift DTC

Audits and optimizes pages on Spindrift's DTC website for conversion. Produces specific, prioritized recommendations grounded in CRO best practices and Spindrift's brand, positioning, and customer behavior.

## Before Executing

Read the following memory files to ground recommendations in Spindrift's actual situation:

- `.claude/product-marketing-context.md` — company, product, and competitive context
- `/memory/shared/positioning.md` — messaging hierarchy, proof points, and competitive reframes
- `/memory/shared/icp.md` — ideal customer profile, purchase triggers, objections, and JTBD
- `/memory/shared/voice.md` — brand voice guidelines (especially Website tone section and sample copy)

Also scan for additional context:

- `/memory/analytics/` — conversion data, traffic sources, page performance
- `/projects/active/` — any active CRO tests or website projects

## Spindrift DTC Page Strategy

### Homepage
**Purpose:** Brand story + product discovery + shop entry point
**Conversion goal:** Click-through to flavor pages or subscription

- **Hero section:** Real fruit imagery + ingredient transparency headline. Not lifestyle photography. The product and its ingredients are the hero.
- **Recommended hero copy:** "Sparkling water made with real squeezed fruit. Not 'natural flavors.' Not 'fruit essence.' Real fruit." (from voice.md website section)
- **Below-the-fold flow:** Bestsellers carousel > "What makes Spindrift different" (ingredient comparison, implied) > Social proof (reviews, press, UGC) > Subscription value prop > Where to buy (retail + DTC)
- **Primary CTA:** "Try Spindrift" / "Shop Flavors"
- **Secondary CTA:** "Subscribe & Save"
- **Trust signals:** "Real squeezed fruit. No artificial anything. [X] 5-star reviews."

### Flavor Pages (PDP)
**Purpose:** Ingredient education + conversion
**Conversion goal:** Add to cart or subscribe

- **Hero:** Can image + actual fruit imagery side by side. Ingredient list prominently displayed — this IS the selling point.
- **Must-include elements:**
  - Full ingredient list (hero-level prominence, not footer fine print)
  - Fruit sourcing info ("Made with real squeezed [fruit] from [origin]")
  - Taste description in Spindrift voice ("Tastes like [fruit]. Because it is [fruit].")
  - Nutrition facts (lean into the calories — "10 calories from real fruit")
  - Customer reviews (filterable, real)
  - "Compare ingredients" section (show Spindrift's list vs. generic "natural flavors" — no competitor names)
- **Primary CTA:** "Add to Cart" / "Subscribe & Save [X]% off"
- **Cross-sell:** "You might also like" with other flavors. Variety pack upsell.

### Subscription Page
**Purpose:** Convert single-purchasers to subscribers
**Conversion goal:** Subscription sign-up

- **Value prop hierarchy:**
  1. Savings (Subscribe & Save X%)
  2. Convenience (delivered on your schedule, never run out)
  3. Flexibility (skip, swap flavors, cancel anytime)
  4. Exclusives (subscriber-only flavors or early access)
- **Objection handling on page:**
  - "Can I cancel anytime?" — Yes, prominently stated
  - "Can I change flavors?" — Yes, show the swap feature
  - "What if I have too much?" — Skip a delivery, easy
- **Social proof:** Subscriber count or testimonials. "Join [X] people who never run out of Spindrift."
- **CTA:** "Start Your Subscription" / "Subscribe & Save"

### About Page
**Purpose:** Origin story + brand credibility
**Conversion goal:** Brand affinity (soft conversion to email sign-up or shop)

- **Story arc:** Founder's question ("Why doesn't sparkling water use real fruit?") > The answer (Spindrift) > The difference (real ingredients, transparent process) > Where we are today (national brand, same simple ingredients)
- **Tone:** Warmer and more personal than other pages. Founder voice acceptable.
- **Key elements:** Founding story, ingredient philosophy, team/founder photo, timeline of growth, press logos, email sign-up
- **Avoid:** Corporate-speak, mission statements, buzzwords. Keep it real.

### Landing Pages (Paid Traffic)
**Purpose:** Convert paid traffic from specific campaigns
**Conversion goal:** Purchase or email capture

- **Rule:** Match the ad promise. If the ad was about ingredients, the landing page opens with ingredients. If it was about a specific flavor, land on that flavor.
- **Structure:** Headline (mirrors ad hook) > Product/ingredient visual > 3 proof points > Social proof > CTA > FAQ
- **Remove friction:** No navigation bar (or minimal). Single clear CTA. Short form for email capture.
- **CTA:** "Try Spindrift" (acquisition) / "Get [X]% Off Your First Order" (promo)

### Cart / Checkout
**Purpose:** Complete the purchase
**Conversion goal:** Reduce abandonment

- **Key optimizations:** Subscription upsell in cart, free shipping threshold (prominently displayed and progress-barred), order summary with product images, trust badges (secure checkout, satisfaction guarantee), variety pack suggestion if single flavor in cart.
- **Abandonment recovery:** Exit-intent email capture, cart abandonment email sequence (see email-sequence skill).

## CRO Principles for Spindrift

### The Ingredient-First Hierarchy
Every page should follow this visual and information hierarchy:
1. **Product + real fruit** (what it is)
2. **Ingredient list / ingredient truth** (why it's different)
3. **Social proof** (others agree)
4. **CTA** (take action)

Never lead with lifestyle imagery, brand attitude, or abstract benefit claims. The product truth is the most compelling thing Spindrift has. Put it first.

### Trust Signal Framework
| Signal | Where to Use | Spindrift-Specific |
|--------|-------------|-------------------|
| Ingredient transparency | Every product page, homepage | "Real squeezed [fruit]. That's it." |
| No artificial anything | Homepage, about, subscription | "No artificial sweeteners, no natural flavors, no concentrates" |
| Customer reviews | Product pages, homepage | Star ratings + written reviews, especially ingredient-focused ones |
| Press mentions | Homepage, about | Food/beverage editorial (Bon Appetit, NYT, etc.) |
| Subscriber count | Subscription page | "Join [X] subscribers" |
| Satisfaction guarantee | Cart, checkout | "Love it or we'll make it right" |

### Spindrift CTA Language
| Do | Don't |
|----|-------|
| "Try Spindrift" | "Shop Now" |
| "Subscribe & Save" | "Explore Our Collection" |
| "Add to Cart" | "Purchase" |
| "See the Ingredients" | "Learn More" |
| "Find in Store" | "Locate a Retailer" |
| "Start Your Subscription" | "Begin Your Hydration Journey" |

## Execution Steps

### Step 1: Identify the Page

Based on the provided `[page]`, focus the audit. If no page specified, prioritize by revenue impact: flavor pages > subscription > homepage > cart > about.

### Step 2: Audit the Current State

Assess the page against:
- **Ingredient-first hierarchy:** Is the product truth the hero?
- **Message-to-positioning alignment:** Does the copy follow the messaging hierarchy from positioning.md?
- **Voice compliance:** Does the copy sound like Spindrift (real, warm, confident, ingredient-proud)?
- **CTA clarity:** Is the primary action obvious? Is the CTA language on-brand?
- **Trust signals:** Are they present, relevant, and well-placed?
- **Friction points:** What might cause hesitation, confusion, or abandonment?
- **Mobile experience:** Is the hierarchy preserved on mobile?
- **Page speed:** Note if relevant data is available.

### Step 3: Generate Recommendations

For each recommendation:
- **What to change** (specific element on the page)
- **Current state** (what it is now, or what's missing)
- **Recommended state** (what it should be, with example copy if relevant)
- **Why** (CRO principle + Spindrift positioning rationale)
- **Expected impact** (High / Medium / Low)
- **Effort** (Quick win / Medium / Major project)

### Step 4: Prioritize

Rank recommendations using ICE scoring:
- **Impact:** How much will this move the conversion needle?
- **Confidence:** How confident are we this will work (based on data, best practices, or testing)?
- **Ease:** How easy is this to implement?

## Output Format

```
# CRO Audit — [Page Name]
**Date:** [YYYY-MM-DD]
**Page:** [Specific page or URL]
**Current baseline:** [Conversion rate if known, or "baseline TBD"]

## Page Assessment

### Ingredient-First Hierarchy
[Is the product truth the hero? What's above the fold?]
**Score:** [Strong / Needs Work / Weak]

### Message-Positioning Alignment
[Does the copy align to Spindrift's messaging hierarchy?]
**Score:** [Strong / Needs Work / Weak]

### Voice Compliance
[Does it sound like Spindrift?]
**Score:** [Strong / Needs Work / Weak]

### CTA Clarity
[Is the primary action obvious and on-brand?]
**Score:** [Strong / Needs Work / Weak]

### Trust Signals
[Are they present and effective?]
**Score:** [Strong / Needs Work / Weak]

## Recommendations

### 1. [Recommendation Title]
- **Element:** [What on the page]
- **Current:** [What it is now]
- **Recommended:** [What it should be]
- **Example copy:** [If applicable]
- **Why:** [CRO principle + Spindrift rationale]
- **Impact:** [High / Medium / Low]
- **Ease:** [Quick win / Medium / Major]
- **ICE Score:** [X/30]

### 2. [Recommendation Title]
...

[Continue for all recommendations]

## Prioritized Action Plan

| Priority | Recommendation | ICE Score | Type |
|----------|---------------|-----------|------|
| 1 | [Name] | [Score] | Quick win |
| 2 | [Name] | [Score] | Quick win |
| 3 | [Name] | [Score] | Medium effort |
| ... | ... | ... | ... |

## A/B Test Candidates
[Which recommendations should be tested rather than shipped directly?]
- **Test 1:** [What to test and why]
- **Test 2:** [What to test and why]

## Quality Checklist
- [ ] All copy recommendations follow Spindrift voice guidelines
- [ ] Ingredient truth is the hero of the page (not lifestyle)
- [ ] CTAs use Spindrift-approved language (not generic marketing-speak)
- [ ] No words from the "Words We Avoid" list in recommended copy
- [ ] Trust signals are specific and substantiatable
- [ ] Recommendations address ICP purchase triggers and objections
- [ ] Mobile experience considered
- [ ] A/B test candidates identified for highest-impact changes
```

## Save Location

Save to: `/projects/active/cro/[page-slug]-audit-[YYYY-MM-DD].md`

## Related Skills

- `/ab-test-setup` — Design experiments for CRO recommendations
- `/brief` — Create content briefs for new page sections or copy rewrites
- Use voice.md website copy examples as reference for all copy recommendations
