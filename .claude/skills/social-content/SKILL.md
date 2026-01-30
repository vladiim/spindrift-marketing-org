---
disable-model-invocation: true
argument-hint: /social-content [platform] [topic] — create social content (instagram | tiktok | twitter | all)
---

# /social-content — Social Content Creation

Creates platform-native social content for Spindrift. Every post should feel like it was written by a person who genuinely loves this product, not a brand that hired a social media manager to "engage audiences."

## Before Executing

Read the following memory files:

- `.claude/product-marketing-context.md` — company, product, competitive landscape
- `/memory/shared/voice.md` — brand voice guidelines (pay special attention to Social Media tone section)
- `/memory/shared/positioning.md` — positioning and messaging hierarchy
- `/memory/shared/icp.md` — ideal customer profile (digital behavior and media habits sections)

Then check `/memory/content/` for recent social content to avoid repetition and maintain variety.

## Content Pillars (Pre-Loaded)

Every social post maps to one of these pillars. Default distribution: aim for roughly 40% Real Ingredients, 25% Taste, 20% Community, 15% Transparency.

| Pillar | Social Angle | Example Hooks |
|--------|-------------|---------------|
| **Real Ingredients** | Ingredient education, label literacy, "natural flavors" awareness | "Flip your can over. How many ingredients can you actually identify?" |
| **Taste Without Compromise** | Flavor moments, taste reactions, seasonal launches, recipes | "Raspberry Lime tastes like raspberries and limes. Controversial take, apparently." |
| **Transparency Culture** | Behind the scenes, sourcing, how it's made, company values | "Our lemons come from real lemon trees. This shouldn't be noteworthy but here we are." |
| **Community** | UGC, fan moments, occasions, "when do you Spindrift" | "Your fridge lineup is your personality test. Show us yours." |

## Platform-Specific Guidance

### Instagram
**Audience context:** Label Readers (27-42), curated feeds, stories > reels, visual-first.
**Content types:**
- **Feed posts:** Ingredient beauty shots — close-up of real fruit alongside the can. Clean, bright, appetizing. Copy is short, witty, ingredient-focused.
- **Reels:** 15-30 seconds. Behind-the-scenes (fruit sourcing, production), taste tests (real vs "natural flavors"), recipe content (Spindrift mocktails). Hook in first 2 seconds.
- **Stories:** Polls ("Can you name the fruit in our Mango Orange?"), quizzes ("How many ingredients in a Spindrift Lemon?"), casual behind-the-scenes.
- **Carousel:** Ingredient comparisons, "read the label" education, flavor guides.

**Instagram defaults:**
- Captions: 1-3 sentences max for feed. Let the image work.
- Emoji: Fruit emoji only, 1-2 max. No chains.
- Hashtags: #Spindrift + 1-2 campaign-specific max. In first comment if more than 2.
- Tone: Witty, casual, slightly knowing. Like a clever friend's post, not a brand.

### TikTok
**Audience context:** Younger tail of ICP (22-35), discovery-driven, raw/authentic, sound-on.
**Content types:**
- **Process videos:** How Spindrift is made, fruit squeezing, what happens in the facility. Satisfy curiosity.
- **Taste tests:** Side-by-side Spindrift vs "natural flavors" brand (never name the competitor on camera). Genuine reactions.
- **Ingredient reveals:** "Reading the ingredient list of popular sparkling waters" — let the comparison speak.
- **Recipe/hack:** Mocktail recipes, unexpected uses, Spindrift as a mixer.
- **Trend participation:** Only when the trend naturally fits. Never force Spindrift into a trend that doesn't align. The voice guide says: "Would we be embarrassed by this in 5 years?"

**TikTok defaults:**
- Hook in first 1-2 seconds. Text on screen + spoken.
- Conversational, unscripted feel even when scripted.
- No hard sell. The product truth IS the content.
- End with a soft CTA or a callback to the hook.

### X/Twitter
**Audience context:** Smallest but most vocal segment. Quick wit, sharp observations, conversations.
**Content types:**
- **Witty observations:** One-line takes on the sparkling water category, ingredient culture, food transparency.
- **Ingredient facts:** Quick, surprising facts about real fruit, "natural flavors," or the industry. Thread-worthy.
- **Engagement:** Replies, quote tweets, community interaction. Sound like a person, not a brand.
- **Threads:** Deep dives on ingredient topics, brand story moments, new flavor launches.

**X/Twitter defaults:**
- One idea per tweet. Sharp, complete, standalone.
- Dry humor over loud humor. Observation over announcement.
- No hashtags in tweet body (exception: campaign-specific).
- Reply to genuine fans with genuine responses. No template replies.

## Hook Formulas (Adapted for Spindrift Voice)

These are starting points, not templates. Adapt the voice — never use them verbatim if they sound generic.

| Formula | Spindrift Adaptation | Example |
|---------|---------------------|---------|
| **Surprising fact** | Lead with an ingredient truth that reframes expectations | "Most sparkling water doesn't contain any fruit. At all. Zero." |
| **Challenge** | Invite the audience to verify something themselves | "Flip your favorite sparkling water over. Read the ingredients. We'll wait." |
| **Contrast** | Put Spindrift's reality against category norms | "'Natural flavors' can mean almost anything. Our ingredient list means exactly what it says." |
| **Casual flex** | State a product truth with understated confidence | "Ingredients: sparkling water, real squeezed lemon juice. That's the whole list. That's the whole post." |
| **Humor from honesty** | Find the funny in being straightforwardly real | "Yes, Spindrift has calories. From fruit. Because there's fruit in it. Hope this helps." |
| **UGC prompt** | Ask a genuine question that invites participation | "What flavor are you reaching for at 3pm? Be honest." |

## Execution Steps

1. **Read all memory files.** Absorb the voice guide deeply — social is where voice matters most.
2. **Identify the platform and topic** from the user's request. If "all" is specified, create platform-specific versions of the same core idea.
3. **Select the content pillar** this post maps to.
4. **Choose the hook approach** — which formula or original angle will stop the scroll?
5. **Write the post(s).** Follow platform-specific defaults above.
6. **Write visual direction** — what the image/video should show (even if we're only writing copy, the visual context matters).
7. **Create 2-3 variants** — different hooks or angles on the same topic.
8. **Run quality gates.**

## Quality Gates

- [ ] **Voice check:** Read the post out loud. Does it sound like a real person who works at Spindrift and loves the product? Or does it sound like a brand account? If the latter, rewrite.
- [ ] **Platform-native check:** Would this post blend naturally into the platform's feed? Or does it feel like an ad dropped into organic content?
- [ ] **Pillar check:** Which content pillar does this map to? If none, it shouldn't exist.
- [ ] **Word audit:** No words from the "Words We Avoid" list. No #CleanEating or similar.
- [ ] **Exclamation mark check:** Max one per post. Zero is usually right for X/Twitter.
- [ ] **Emoji check:** Fruit emoji only, 1-2 max. None if it doesn't add.
- [ ] **Competitor check:** Never name competitors in posts. Implication is fine. Direct comparison content should be educational, not combative.
- [ ] **5-year test:** Would we be embarrassed by this in 5 years? If it relies on a trend or meme with a short shelf life, flag it.

## Output Format

```markdown
# Social Content: [Platform] — [Topic]
**Date:** [YYYY-MM-DD]
**Platform:** [Instagram/TikTok/X/All]
**Content Pillar:** [Real Ingredients / Taste / Transparency / Community]
**Content Type:** [Feed post / Reel / Story / Tweet / Thread / etc.]

---

## Post — Version 1

**Copy:**
[Post text]

**Visual Direction:**
[What the image/video should show]

**Format Notes:**
[Any platform-specific notes — reel length, carousel slides, etc.]

---

## Post — Version 2

[Alternative angle]

---

## Post — Version 3

[Another alternative]

---

## Scheduling Notes
- **Best posting context:** [Time of day, day of week, or cultural moment that fits]
- **Engagement plan:** [How to respond to likely comments/questions]
- **Repurpose potential:** [Could this be adapted for another platform?]
```

## Save Location

Output to conversation. Save to `/projects/active/social/[platform]-[topic-slug]-[YYYY-MM-DD].md` if requested.

## Related Skills

- `/repurpose` — Adapt this content for a different platform or format
- `/brief` — Generate a content brief for a larger campaign this post supports
- `content-strategy` — See how this fits into the broader content plan
