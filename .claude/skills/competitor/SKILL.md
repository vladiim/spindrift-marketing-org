---
disable-model-invocation: true
argument-hint: /competitor [name]
---

# /competitor — Competitive Analysis

Runs a focused competitive analysis using April Dunford's positioning framework. Produces actionable intelligence, not a generic overview.

## Steps

1. **Read memory files for context:**
   - `/memory/shared/positioning.md` — understand Spindrift's own positioning before analyzing the competitor

2. **Check for existing analysis:**
   - Look in `/memory/strategy/competitors/` for any prior analysis on this competitor
   - If prior analysis exists, note what has changed or needs updating

3. **Run the Dunford positioning framework against the competitor:**
   - **Competitive Alternatives:** What would customers use if the competitor didn't exist?
   - **Unique Capabilities:** What does the competitor offer that alternatives don't?
   - **Value:** What value do those capabilities deliver to customers?
   - **Target Customers:** Who cares most about that value?
   - **Market Category:** What category does the competitor position themselves in?

4. **Extend the analysis:**
   - **Messaging Analysis:** How does the competitor talk about themselves? What claims do they make? What emotional territory do they occupy?
   - **Pricing Comparison:** How does their pricing compare to Spindrift's across comparable SKUs?
   - **Strengths:** Where are they genuinely strong?
   - **Gaps:** Where are they weak or vulnerable?
   - **Spindrift's Angle:** Based on this analysis and our own positioning, what is Spindrift's strongest differentiator against this competitor?

5. **Save the analysis:**
   - Save to `/memory/strategy/competitors/[competitor-slug]-[YYYY-MM-DD].md`
   - Use a lowercase, hyphenated slug derived from the competitor name

## Output Format

Print the analysis to the conversation AND save to the path above.

```markdown
# Competitive Analysis: [Competitor Name]
**Date:** [YYYY-MM-DD]
**Analyst:** Claude

## Dunford Positioning Framework

### Competitive Alternatives
[What customers would use instead of this competitor]

### Unique Capabilities
[What they do that alternatives don't]

### Value Delivered
[What customer value those capabilities create]

### Target Customers
[Who cares most about this value]

### Market Category
[How they frame their market]

## Messaging Analysis
[How they talk about themselves — tone, claims, emotional territory]

## Pricing Comparison
| Product | Competitor Price | Spindrift Price | Notes |
|---------|-----------------|-----------------|-------|
| ...     | ...             | ...             | ...   |

## Strengths
- [Strength with evidence]

## Gaps
- [Weakness or vulnerability]

## Spindrift's Angle
[Our strongest differentiator against this competitor, grounded in our positioning]

## Changes from Prior Analysis
[What changed since last review, or "No prior analysis on file"]
```
