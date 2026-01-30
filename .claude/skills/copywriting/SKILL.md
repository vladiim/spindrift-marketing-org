---
disable-model-invocation: true
argument-hint: /copywriting [format] [topic] — write copy (landing-page | packaging | ad | social | email | tagline)
---

# /copywriting — Brand Copywriting

Writes on-brand copy for Spindrift across all marketing formats. Every word must sound like Spindrift: real, warm, confident, ingredient-proud, and fun without trying too hard.

## Before Executing

**Mandatory:** Read the following memory files before writing a single word:

- `.claude/product-marketing-context.md` — company, product, competitive landscape
- `/memory/shared/voice.md` — brand voice guidelines (this is the source of truth for how Spindrift sounds)
- `/memory/shared/positioning.md` — positioning, messaging hierarchy, and competitive reframes
- `/memory/shared/icp.md` — ideal customer profile

Then check `/memory/content/` for existing copy on the same or similar topics to avoid repetition and maintain fresh angles.

## Supported Formats

| Format | Context | Key Constraints |
|--------|---------|-----------------|
| `landing-page` | Website pages: product, campaign, comparison | SEO-aware, scannable, benefit-led, clear CTA |
| `packaging` | On-can, box, shelf talker, POS | Ultra-concise, ingredient-proud, no wasted words |
| `ad` | Paid social, display, video scripts | Hook in first line/frame, benefit-led, multiple variants |
| `social` | Organic posts for Instagram, TikTok, X | Platform-native, within character limits, conversational |
| `email` | Marketing emails, newsletters | Warm, direct, single clear CTA, earns every paragraph |
| `tagline` | Campaign lines, slogans, headlines | Memorable, ownable, passes the "would a human say this" test |

## Spindrift Copy Principles

These are non-negotiable. Every piece of copy must honor them:

1. **The ingredient list is the headline.** Spindrift's biggest marketing asset is what's in the can. Lead with it, return to it, let it do the work.
2. **Say what's true.** No aspirational fluff. No "elevate your hydration." If you can't back it up with the label, cut it.
3. **Specificity over abstraction.** "Real squeezed lemon" beats "real fruit." "10 calories from grapefruit juice" beats "low calorie." Name the fruit.
4. **Confident, not loud.** The tone is a person who knows their product is good and doesn't need to shout. Think quiet conviction, not megaphone.
5. **Humor from honesty.** "Yes, there are calories. From fruit. It's fruit." — this is the model. Funny because it's plainly true, not because it's trying.
6. **Never disparage competitors by name.** We don't say "unlike LaCroix." We show our ingredient list and let the comparison make itself. In ads, never name competitors.
7. **One exclamation mark per piece, maximum.** Earn it. If the sentence needs an exclamation mark to have energy, the sentence is the problem.

## Execution Steps

1. **Read all memory files.** Internalize the voice guide — not as a checklist but as a personality. You are writing as Spindrift, not about Spindrift.
2. **Clarify the brief.** From the user's request, identify:
   - Format (from the table above)
   - Topic or product focus
   - Target audience segment (from ICP)
   - Goal (awareness, conversion, engagement, launch)
   - Any specific requirements (character limits, platform, campaign context)
3. **Write the first draft.** Follow format-specific guidance below.
4. **Run the voice check** (see Quality Gates). Read every line aloud mentally. Does it sound like the Spindrift voice samples in `voice.md`? If any line sounds like a generic CPG brand, a wellness brand, or Liquid Death, rewrite it.
5. **Run the positioning check.** Does the copy reinforce "real squeezed fruit" as the differentiator? Does it use words from the "Words We Use" list and avoid the "Words We Avoid" list?
6. **Produce the final output** with the primary version and at least one alternative angle.

## Format-Specific Guidance

### Landing Page
- Open with the product truth, not a feeling
- Use short paragraphs, sentence fragments are fine
- Headers should be scannable and benefit-driven
- CTA language: plain ("Try it," "See the flavors," "Find near you") — never "Shop Now" or "Explore Our Collection"
- Include at least one ingredient callout that could stand alone as social copy

### Packaging
- Maximum economy of words. Every word on a can is prime real estate.
- Lead with the ingredient, follow with the implication
- Example rhythm: "Made with real squeezed [fruit]. Not 'natural flavors.' Not 'fruit essence.' [Fruit]."
- The can back panel should make someone want to photograph it and share it

### Ad Copy
- Hook in the first line (or first 3 seconds for video)
- Lead with product truth, then the feeling
- Provide 3 variants minimum: different hooks, same core message
- For video scripts: include visual directions in brackets, spoken word in plain text
- End on the ingredient list or the product, not a lifestyle vignette

### Social
- Write as a person, not a brand account
- Instagram: ingredient beauty, witty observations, real moments
- TikTok: conversational, hook-first, process or comparison angles
- X/Twitter: sharp, dry, one-idea-per-post
- Provide suggested visual direction alongside copy
- Emoji: fruit emoji only, 1-2 max, none if it doesn't add

### Email
- Subject lines: clear benefit or genuine curiosity, never clickbait
- Preview text: extends the subject, doesn't repeat it
- Body: conversational, purposeful, every paragraph earns its place
- Single CTA. "Try it" over "Shop Now."
- Sign-off should feel human, not corporate

### Tagline
- Must be ownable — could only be said by a brand with real fruit
- Test: would a person actually say this? If not, rewrite
- Provide 5+ options ranging from direct to clever
- Flag which ones work for campaign vs. evergreen use

## Quality Gates

Run every piece of copy through these checks before delivering:

1. **Voice alignment** — Read against `voice.md`. Does it match the core attributes (real, warm, confident, ingredient-proud, fun)? Check against the spectrum examples. Would it land between the "do" examples, not the "don't" examples?
2. **Word audit** — Scan for any words on the "Words We Avoid" list (natural flavors, clean, healthy, guilt-free, artisanal, disrupting, superfood, wellness, hack, obsessed, beverage experience, hydration journey). Remove and replace.
3. **Positioning proof** — Does the copy reinforce the messaging hierarchy from `positioning.md`? Can every claim be backed by the ingredient list or a product fact?
4. **ICP resonance** — Would the Label Reader persona (27-42, reads ingredients, values authenticity over performance) engage with this? Does it address their motivations?
5. **Competitive differentiation** — Does this copy differentiate from Liquid Death (substance over stunts), LaCroix (real vs "natural flavors"), and generic brands (premium justified by ingredients)?
6. **Exclamation mark count** — Maximum one per piece. Zero is usually better.
7. **Hashtag discipline** — #Spindrift and campaign-specific only. No #CleanEating #HealthyLifestyle chains.

## Output Format

```markdown
# Copy: [Format] — [Topic]
**Date:** [YYYY-MM-DD]
**Format:** [Format type]
**Target Segment:** [From ICP]
**Goal:** [What this copy should achieve]

---

## Primary Version

[Full copy in format-appropriate structure]

---

## Alternative Version

[Different angle or hook, same core message]

---

## Voice & Positioning Notes
- **Voice check:** [Pass/flag any adjustments made]
- **Key positioning element used:** [Which messaging hierarchy level]
- **Words avoided:** [Any near-misses caught and replaced]

## Suggested Next Steps
- Critique this draft → `/critique [file]`
- Repurpose to another format → `/repurpose [file] [format]`
- Edit and polish → use `copy-editing` skill
```

## Save Location

Output directly to the conversation. Save to `/projects/active/copy/[format]-[topic-slug]-[YYYY-MM-DD].md` if the user requests it.

## Related Skills

- `/critique` — Evaluate this copy against voice and positioning standards
- `copy-editing` — Seven-sweep editorial review for polish
- `/repurpose` — Adapt this copy to a different format
