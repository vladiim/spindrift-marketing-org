---
disable-model-invocation: true
argument-hint: [file] — path to the draft to edit using the seven-sweep framework
---

# /copy-editing [file] — Seven-Sweep Copy Editing

Applies a structured seven-sweep editorial framework to any Spindrift content draft. Each sweep targets a specific dimension of quality. The result is tighter, sharper, more on-brand copy with specific edits tracked.

## Before Executing

Read the following memory files to establish editorial standards:

- `.claude/product-marketing-context.md` — company, product, competitive landscape
- `/memory/shared/voice.md` — brand voice guidelines (critical for Sweep 2)
- `/memory/shared/positioning.md` — positioning and proof points (critical for Sweep 4)
- `/memory/shared/icp.md` — ideal customer profile (critical for Sweep 3)

Then read the draft file provided as the argument.

## The Seven Sweeps

Each sweep is a complete pass through the draft, focused on one dimension. Do not combine sweeps — complete one fully before moving to the next. Track every change.

---

### Sweep 1: Clarity
**Question:** Can a reader understand every sentence on first read?

- Eliminate ambiguity, jargon, and unnecessarily complex sentence structures
- Break long sentences into shorter ones where meaning is stacked
- Ensure logical flow between paragraphs — each paragraph should earn its position
- Remove any sentence that requires re-reading to parse
- Check that the opening line communicates the core idea within 10 words
- For Spindrift: plain language is brand-aligned. If it sounds like a marketing deck, simplify it.

### Sweep 2: Voice & Tone
**Question:** Does every line sound like Spindrift wrote it?

This sweep uses `/memory/shared/voice.md` as the standard. Check against all five voice attributes:

| Attribute | Check |
|-----------|-------|
| **Real (not raw)** | Is it honest without being chaotic? Would a smart friend say this? |
| **Warm (not soft)** | Is it approachable without being saccharine? Friendly without try-hard energy? |
| **Confident (not cocky)** | Does it state claims plainly without hedging OR bragging? |
| **Ingredient-proud (not preachy)** | Does it celebrate ingredients without lecturing? |
| **Fun (not trying too hard)** | Is humor grounded and observational, not forced or trend-chasing? |

**Word audit:** Flag and replace any words from the "Words We Avoid" list:
- natural flavors, clean, healthy, guilt-free, artisanal, craft, small-batch, disrupting, revolutionary, superfood, functional, beverage experience, hydration journey, wellness, hack, obsessed

**Punctuation check:**
- Maximum one exclamation mark per piece
- Sentence case for headlines (not Title Case unless platform requires)
- Emoji: fruit only, 1-2 max per social post, none in email body/packaging/ads
- Hashtags: #Spindrift and campaign-specific only

### Sweep 3: So What?
**Question:** Why should the reader care?

- Every claim must connect to a reader benefit or motivation
- Check against ICP jobs-to-be-done: Does this address what the Label Reader actually wants?
- Eliminate "so what?" moments — facts or features that aren't connected to value
- The reader is asking "what does this mean for me?" at every line. Answer it.
- For Spindrift: "We use real squeezed fruit" is a fact. "You can taste the difference because there is one" is the so-what.

### Sweep 4: Prove It
**Question:** Can every claim be substantiated?

This sweep is critical for Spindrift's positioning. The brand's entire differentiation rests on verifiable ingredient truth. Unsubstantiated claims undermine that foundation.

- **Ingredient claims:** Must be backed by the actual ingredient list. "Real squeezed fruit" — true. "Healthiest sparkling water" — cannot prove, remove.
- **Comparative claims:** Must be provable by public information. "Only national sparkling water with real squeezed fruit" — verifiable. "Better than LaCroix" — subjective, reframe.
- **Emotional claims:** Must be grounded in product truth. "Taste the difference" — supported by real ingredients. "Feel amazing" — ungrounded, cut.
- **Proof points from positioning.md:** Ingredient list transparency, visible cloudiness from real fruit, calorie honesty (5-15 cal from fruit), flavor variation batch-to-batch, sourcing transparency.
- Flag any claim that would not survive a skeptical consumer's scrutiny. Spindrift's audience is ingredient-literate and BS-sensitive.

### Sweep 5: Specificity
**Question:** Is every detail as specific as it can be?

- Replace generic language with specific details
- "Real fruit" → "real squeezed lemon" (name the fruit)
- "Low calorie" → "10 calories from grapefruit juice" (name the number and source)
- "Our sparkling water" → "Spindrift Raspberry Lime" (name the product)
- "Available everywhere" → "At Target, Whole Foods, and Costco" (name the stores)
- Specificity builds trust. Vagueness erodes it. For a brand built on ingredient transparency, every vague word is a missed opportunity.

### Sweep 6: Heightened Emotion
**Question:** Does this make the reader feel something?

- After sweeps 1-5 have made the copy clear, on-voice, relevant, provable, and specific, this sweep adds emotional resonance
- Look for moments where a factual statement could land with more impact through rhythm, contrast, or surprise
- Spindrift's emotional range: quiet pride, genuine warmth, dry humor, confident simplicity, pleasant surprise
- Spindrift's emotional boundaries: never fear, shame, anxiety, FOMO, or manufactured urgency
- Example: "We use real fruit" (factual) → "There's real lemon juice in here. That's why it's a little cloudy." (same fact, more feeling)
- The best Spindrift copy makes people feel respected and delighted, not pressured or preached at

### Sweep 7: Zero Risk
**Question:** Could any line cause brand, legal, or reputational harm?

- **Legal:** No unsubstantiated health claims. No naming competitors in ads. No claims about competitor ingredients that aren't publicly verifiable.
- **Brand:** Nothing that sounds like Liquid Death (edgy, aggressive), a wellness brand (preachy, prescriptive), or a luxury brand (exclusive, aspirational). Nothing we'd be embarrassed by in 5 years.
- **Tone:** No punching down at consumers' choices. No fear-mongering about "natural flavors" — educate, don't scare. No shaming people who drink other brands.
- **Accuracy:** Double-check any specific numbers, ingredient claims, or availability statements.
- **Sensitivity:** Avoid language that could be read as elitist ("you should know better") or dismissive ("it's just water").

---

## Execution Steps

1. **Read all memory files** and the draft file.
2. **Execute each sweep in order** (1 through 7). Complete one sweep before starting the next.
3. **Track every change** — what was changed, which sweep caught it, and why.
4. **Produce the edited version** — clean, complete, ready to use.
5. **Produce the change log** — organized by sweep.

## Output Format

```markdown
# Copy Edit: [Draft filename]
**Date:** [YYYY-MM-DD]
**Sweeps completed:** 7/7

---

## Change Log by Sweep

### Sweep 1: Clarity
- **[Change]:** [Original] → [Edited] — [Why]

### Sweep 2: Voice & Tone
- **[Change]:** [Original] → [Edited] — [Why]

### Sweep 3: So What?
- **[Change]:** [Original] → [Edited] — [Why]

### Sweep 4: Prove It
- **[Change]:** [Original] → [Edited] — [Why]

### Sweep 5: Specificity
- **[Change]:** [Original] → [Edited] — [Why]

### Sweep 6: Heightened Emotion
- **[Change]:** [Original] → [Edited] — [Why]

### Sweep 7: Zero Risk
- **[Change]:** [Original] → [Edited] — [Why]

---

## Edited Version

[Complete edited draft — full text, ready to use]

---

## Summary
- **Total changes:** [Number]
- **Most active sweep:** [Which sweep caught the most issues]
- **Overall assessment:** [1-2 sentences on the draft's quality and what the edits accomplished]
```

## Save Location

Output directly to the conversation. Do not save to a file unless the user requests it.

## Related Skills

- `/critique` — Higher-level strategic evaluation (voice, positioning, ICP alignment) — use before copy-editing for structural issues
- `copywriting` — Generate new copy from scratch if the draft needs a full rewrite rather than editing
