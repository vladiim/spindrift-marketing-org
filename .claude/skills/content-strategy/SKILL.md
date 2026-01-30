---
disable-model-invocation: true
argument-hint: /content-strategy [topic or campaign] — generates a content strategy document
---

# /content-strategy — Content Strategy Generator

Produces a comprehensive content strategy document for Spindrift, grounded in brand pillars, voice, positioning, and audience. Designed for a CPG beverage brand competing on ingredient transparency in a crowded sparkling water market.

## Before Executing

Read the following memory files to establish strategic context:

- `.claude/product-marketing-context.md` — company, product, competitive landscape
- `/memory/shared/voice.md` — brand voice guidelines
- `/memory/shared/positioning.md` — positioning and differentiation framework
- `/memory/shared/icp.md` — ideal customer profile and personas

Then check `/memory/content/` and `/memory/strategy/` for existing strategies, briefs, and published content to avoid duplication and ensure coherence with prior work.

## Content Pillars

Every Spindrift content strategy draws from four brand pillars. Each piece of content should map to at least one:

| Pillar | What It Covers | Example Topics |
|--------|---------------|----------------|
| **Real Ingredients** | What's in the can, sourcing, ingredient transparency, "natural flavors" education | Ingredient comparisons, farm-to-can stories, label literacy |
| **Taste Without Compromise** | Flavor, product experience, the visible difference, honest calories | Flavor profiles, taste tests, recipe content, seasonal launches |
| **Transparency Culture** | How Spindrift operates, behind-the-scenes, honest business practices | Sourcing transparency, supply chain, founder story, company values |
| **Community** | Customer stories, UGC, occasions, shared moments with Spindrift | Fan content, occasion-based content, family moments, hosting |

## Content Prioritization Framework

Prioritize content that is both **searchable** (SEO, discovery) and **shareable** (social, word-of-mouth). Use this 2x2:

```
                    High Shareability
                          |
        PRIORITY 1        |       PRIORITY 2
    (Search + Share)      |    (Share-first)
    "What are natural     |   "Our ingredient list
     flavors really?"    |    is the whole post"
                          |
   -----------------------------------------------
                          |
        PRIORITY 3        |       PRIORITY 4
    (Search-first)        |    (Internal/niche)
    "Best sparkling       |   "Q3 sourcing update"
     water brands"        |
                          |
                    Low Shareability
```

Always weight Priority 1 content highest. It earns traffic AND spreads organically.

## Execution Steps

1. **Read and internalize** all memory files listed above.
2. **Identify the strategic goal.** What is this content strategy trying to achieve? Options:
   - Brand awareness (top-of-funnel, new audience)
   - Competitive differentiation (vs. specific competitor or category)
   - Product launch (new flavor, seasonal, limited edition)
   - Community growth (engagement, UGC, loyalty)
   - Conversion (trial, repeat purchase, bulk upgrade)
3. **Map the topic to content pillars.** Which 1-2 pillars does this strategy activate?
4. **Select ICP segments.** Which audience segment(s) does this strategy target? Reference `/memory/shared/icp.md` for segments: Label Readers, parents, alcohol-reducers, etc.
5. **Define the content mix** across formats:
   - Long-form (blog, landing page, email sequence)
   - Short-form (social posts, stories, reels)
   - Visual (photography, video, infographics)
   - Interactive (quizzes, comparisons, UGC prompts)
6. **Build the editorial calendar skeleton** — themes by week/month, mapped to pillars and formats.
7. **Define distribution channels** — where each piece lives and how it's promoted.
8. **Set success metrics** — tied to the strategic goal, not vanity metrics.
9. **Assemble the strategy document** in the format below.
10. **Save** to `/projects/active/strategy-[topic-slug]-[YYYY-MM-DD].md`.

## Quality Gates

Before finalizing, verify:

- [ ] **Voice check:** Does every example headline/topic sound like Spindrift? Run against the decision filter in `voice.md` — is it true, would a real person say it, are we punching down, would we be embarrassed in 5 years?
- [ ] **Positioning alignment:** Does the strategy reinforce "real squeezed fruit" as the core differentiator? Does it avoid words on the avoid list (clean, healthy, guilt-free, disrupting)?
- [ ] **ICP resonance:** Would the Label Reader persona actually engage with this content? Does it address their motivations (ingredient truth, taste, trust) not just demographics?
- [ ] **Pillar mapping:** Is every content piece mapped to at least one pillar? Is the mix balanced or intentionally weighted?
- [ ] **Competitive awareness:** Does the strategy differentiate from Liquid Death (substance over stunts), LaCroix (real fruit vs natural flavors), and Topo Chico (independent vs corporate)?

## Output Format

Print the strategy to the conversation AND save to the path above.

```markdown
# Content Strategy: [Topic/Campaign]
**Date:** [YYYY-MM-DD]
**Author:** Claude
**Strategic Goal:** [One sentence]
**Primary Pillar(s):** [From the four pillars]
**Target Segment(s):** [From ICP]

---

## Strategic Context
[2-3 sentences: why this strategy, why now, what it responds to in the market or brand]

## Content Pillars Activated
[Which pillars this strategy draws from and why]

## Audience Insight
[Key insight about the target segment that this strategy exploits — from ICP or original analysis]

## Content Plan

### Searchable Content (SEO / Discovery)
| Piece | Format | Pillar | Target Keyword/Intent | Priority |
|-------|--------|--------|-----------------------|----------|
| [Title] | [Blog/Landing page/etc.] | [Pillar] | [Keyword] | [1-4] |

### Shareable Content (Social / WOM)
| Piece | Format | Platform | Pillar | Hook |
|-------|--------|----------|--------|------|
| [Title] | [Reel/Post/Thread/etc.] | [Platform] | [Pillar] | [1-line hook] |

### Supporting Content
| Piece | Format | Purpose |
|-------|--------|---------|
| [Title] | [Email/Infographic/etc.] | [How it supports the strategy] |

## Editorial Calendar
| Week | Theme | Key Pieces | Pillar |
|------|-------|-----------|--------|
| 1 | [Theme] | [Pieces] | [Pillar] |

## Distribution Plan
- **[Channel]:** [What goes here, frequency, approach]

## Success Metrics
| Metric | Target | Why It Matters |
|--------|--------|---------------|
| [Metric] | [Target] | [Connection to strategic goal] |

## Connected Next Steps
- Generate briefs for priority pieces → `/brief [topic]`
- Write copy for key assets → use `copywriting` skill
- Critique drafts against voice and positioning → `/critique [file]`
```

## Related Skills

- `/brief` — Generate detailed content briefs for individual pieces in this strategy
- `/critique` — Evaluate drafts against voice and positioning standards
- `copywriting` — Write the actual content pieces this strategy defines
