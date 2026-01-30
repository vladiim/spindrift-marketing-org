---
disable-model-invocation: true
argument-hint: /ab-test-setup [channel] [hypothesis] — channel: website|email|paid-social|landing-page
---

# /ab-test-setup — A/B Test Design & Setup

Designs rigorous A/B tests for Spindrift's marketing channels. Produces a complete test plan with hypothesis, sample size calculations, success criteria, and analysis framework. Built for Spindrift's traffic levels and baseline metrics.

## Before Executing

Read the following memory files to ground the test in Spindrift's actual situation:

- `.claude/product-marketing-context.md` — company, product, and competitive context
- `/memory/shared/positioning.md` — messaging framework (tests should validate positioning hypotheses)
- `/memory/shared/icp.md` — ICP segments and purchase triggers (tests should target real behaviors)
- `/memory/shared/voice.md` — voice guidelines (both variants must be on-brand)

Also scan for additional context:

- `/memory/analytics/` — baseline metrics, traffic data, and past test results
- `/projects/active/` — current tests in progress (avoid conflicts)

## Spindrift Channel Baselines

These are default baselines for sample size calculations. Override with actual data from `/memory/analytics/` when available.

### DTC Website (spindrift.com)
| Metric | Baseline | Notes |
|--------|----------|-------|
| **Conversion rate** | 3.0% | Visit-to-purchase |
| **Add-to-cart rate** | 8.5% | Visit-to-ATC |
| **Cart-to-purchase** | 35% | ATC-to-order |
| **Subscription conversion** | 1.2% | Visit-to-subscription |
| **AOV** | $32 | Average order value |
| **Monthly unique visitors** | ~150K | Estimated; verify with actual data |
| **Bounce rate** | 42% | Homepage |

### Email
| Metric | Baseline | Notes |
|--------|----------|-------|
| **Open rate** | 25% | Across campaigns |
| **Click-through rate** | 3.5% | Unique clicks / delivered |
| **Click-to-open rate** | 14% | Clicks / opens |
| **Conversion rate (email-to-purchase)** | 1.8% | End-to-end |
| **Unsubscribe rate** | 0.15% | Per send |
| **List size** | ~250K | Estimated; verify with actual data |

### Paid Social
| Metric | Baseline | Notes |
|--------|----------|-------|
| **CTR (Meta)** | 1.5% | Link clicks / impressions |
| **CTR (TikTok)** | 1.8% | Link clicks / impressions |
| **CPC (Meta)** | $1.20 | Average across campaigns |
| **CPM (Meta)** | $10.50 | Average |
| **Landing page conversion** | 4.2% | Click-to-purchase on dedicated LPs |
| **Thumbstop rate (video)** | 25% | 3s+ view / impression |

### Landing Pages
| Metric | Baseline | Notes |
|--------|----------|-------|
| **Conversion rate (paid traffic)** | 4.2% | From paid ads |
| **Conversion rate (organic)** | 2.5% | From organic/direct |
| **Email capture rate** | 8% | On lead-gen landing pages |
| **Bounce rate** | 55% | Paid traffic landing pages |

## Pre-Populated Sample Size Calculations

Use these as starting references. Adjust based on actual traffic and the specific metric being tested.

### Minimum Detectable Effect (MDE) Quick Reference

**DTC Website (3.0% baseline conversion, 150K monthly visitors):**
| MDE | Sample per variant | Duration (50/50 split) | Duration (80/20 split) |
|-----|-------------------|----------------------|----------------------|
| 10% relative (3.0% → 3.3%) | ~43,000 | ~19 days | ~36 days |
| 15% relative (3.0% → 3.45%) | ~19,500 | ~9 days | ~16 days |
| 20% relative (3.0% → 3.6%) | ~11,000 | ~5 days | ~10 days |
| 25% relative (3.0% → 3.75%) | ~7,200 | ~3 days | ~6 days |

**Email (25% open rate, 250K list):**
| MDE | Sample per variant | Feasible? |
|-----|-------------------|-----------|
| 5% relative (25% → 26.25%) | ~47,000 | Yes (1 send) |
| 10% relative (25% → 27.5%) | ~12,000 | Yes (1 send) |
| 15% relative (25% → 28.75%) | ~5,500 | Yes (1 send) |

**Paid Social (1.5% CTR baseline):**
| MDE | Impressions per variant | Notes |
|-----|------------------------|-------|
| 10% relative (1.5% → 1.65%) | ~170,000 | 1-2 week test at moderate spend |
| 15% relative (1.5% → 1.725%) | ~77,000 | 3-5 day test at moderate spend |
| 20% relative (1.5% → 1.8%) | ~44,000 | 2-3 day test at moderate spend |

*All calculations assume 95% confidence, 80% power, two-tailed test.*

## Spindrift Hypothesis Template

A good hypothesis connects the change to Spindrift's positioning, ICP behavior, or a specific insight.

**Template:**
> **If** we [specific change], **then** [specific metric] will [increase/decrease] by [amount/range], **because** [insight about Spindrift's ICP, positioning, or past data that supports this prediction].

**Spindrift-specific hypothesis examples:**

> **If** we move the ingredient list above the fold on flavor pages, **then** add-to-cart rate will increase by 15%+, **because** the ICP's #1 purchase trigger is the ingredient comparison moment, and making ingredients immediately visible removes a discovery friction.

> **If** we use "real squeezed [fruit]" in email subject lines instead of flavor names alone, **then** open rates will increase by 10%+, **because** the ingredient truth is more differentiating than the flavor name in a crowded inbox.

> **If** we lead paid social creative with a close-up of real fruit being squeezed instead of a lifestyle shot, **then** CTR will increase by 15%+, **because** the ICP responds to product truth over aspiration, and process content outperforms lifestyle on TikTok.

> **If** we add a "compare ingredients" section to flavor pages showing Spindrift's list vs. a generic "natural flavors" list, **then** conversion rate will increase by 10%+, **because** the implied comparison activates the ingredient comparison purchase trigger without naming competitors.

## Execution Steps

### Step 1: Define the Hypothesis

Based on the provided `[channel]` and `[hypothesis]`, formalize using the template above. If only a general area is provided, suggest 2-3 specific hypotheses to choose from.

Ensure the hypothesis:
- Is specific and measurable
- Connects to Spindrift's positioning or ICP behavior
- Is testable with available traffic/volume
- Changes only one variable

### Step 2: Design the Test

- **Control:** Current state (describe specifically)
- **Variant:** Changed state (describe specifically, include example copy/creative if relevant)
- **Primary metric:** The one number that determines success
- **Secondary metrics:** Supporting metrics that provide context
- **Guardrail metrics:** Metrics that must NOT degrade (e.g., AOV, unsubscribe rate)

### Step 3: Calculate Sample Size and Duration

Using the baselines above (or actual data from `/memory/analytics/`):
- **Minimum detectable effect:** What's the smallest improvement worth detecting?
- **Required sample per variant:** Based on baseline rate, MDE, 95% confidence, 80% power
- **Estimated duration:** Based on traffic/volume and split ratio
- **Split ratio recommendation:** 50/50 for maximum power; 80/20 if risk is a concern

### Step 4: Define Success Criteria and Decision Rules

- **Statistical significance threshold:** 95% confidence (p < 0.05)
- **Minimum runtime:** Regardless of early significance, run for at least [X days] to account for day-of-week effects
- **Decision framework:**
  - Significant positive: Ship the variant
  - Significant negative: Revert, log learning
  - Inconclusive: Extend if feasible, otherwise log as "no detectable difference" and move on
- **When to stop early:** Only if guardrail metrics are severely impacted

### Step 5: Document for the Experiment Repository

Format the test plan for archival in the experiment repository.

## Output Format

```
# A/B Test Plan — [Test Name]
**Date:** [YYYY-MM-DD]
**Channel:** [Website / Email / Paid Social / Landing Page]
**Status:** Planned

## Hypothesis
> **If** [change], **then** [metric] will [effect], **because** [insight].

## Test Design

### Control (A)
[Specific description of current state]

### Variant (B)
[Specific description of changed state]
[Include example copy, creative direction, or wireframe description if applicable]

### What We're NOT Changing
[Explicitly state what remains constant — isolate the variable]

## Metrics

| Role | Metric | Baseline | Target (MDE) |
|------|--------|----------|-------------|
| Primary | [Metric] | [Baseline] | [Target] |
| Secondary | [Metric] | [Baseline] | [Direction] |
| Secondary | [Metric] | [Baseline] | [Direction] |
| Guardrail | [Metric] | [Baseline] | Must not degrade |

## Sample Size & Duration

- **Baseline rate:** [X%]
- **Minimum detectable effect:** [X% relative]
- **Required sample per variant:** [N]
- **Traffic/volume:** [X per day/week]
- **Split ratio:** [50/50 or 80/20]
- **Estimated duration:** [X days/weeks]
- **Minimum runtime:** [X days] (day-of-week coverage)
- **Confidence level:** 95%
- **Power:** 80%

## Decision Rules

| Outcome | Action |
|---------|--------|
| Variant wins at p < 0.05 | Ship variant, document learning |
| Control wins at p < 0.05 | Revert, document learning |
| No significance after full duration | Log as inconclusive, consider follow-up test |
| Guardrail metric degrades >X% | Stop test early, revert |

## Implementation Notes
- **Technical requirements:** [What's needed to set up the test]
- **QA checklist:** [What to verify before going live]
- **Audience:** [Any segmentation or targeting for the test]

## Pre-Test Quality Checklist
- [ ] Both variants comply with Spindrift voice guidelines
- [ ] Hypothesis connects to Spindrift positioning or ICP insight
- [ ] Only one variable is being changed
- [ ] Sample size is achievable within a reasonable timeframe
- [ ] Guardrail metrics defined
- [ ] No conflict with other active tests (check /projects/active/)
- [ ] Minimum runtime accounts for day-of-week and seasonal effects
- [ ] Success criteria defined before test launches (no moving goalposts)

## Post-Test Template
[Fill in after test concludes]

### Results
| Metric | Control | Variant | Difference | Significant? |
|--------|---------|---------|-----------|-------------|
| ... | ... | ... | ... | ... |

### Learning
[What did we learn? What does this mean for Spindrift's positioning/messaging?]

### Next Steps
[Ship, iterate, or new test based on findings]
```

## Save Location

Save to: `/projects/active/experiments/[test-slug]-[YYYY-MM-DD].md`

After test concludes, move results to: `/memory/analytics/experiments/[test-slug]-results-[YYYY-MM-DD].md`

## Related Skills

- `/analytics` — Review test results in the context of broader performance
- `/page-cro` — Generate CRO hypotheses to test
- `/paid-ads` — Design creative tests for paid channels
