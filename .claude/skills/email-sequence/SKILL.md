---
disable-model-invocation: true
argument-hint: /email-sequence [type] [context] — design email sequence (welcome | nurture | win-back | launch)
---

# /email-sequence — Email Sequence Design

Designs multi-email sequences for Spindrift's marketing. Each email sounds like a warm, direct note from someone who genuinely believes in what's in the can — not a marketing automation platform.

## Before Executing

Read the following memory files:

- `.claude/product-marketing-context.md` — company, product, competitive landscape
- `/memory/shared/voice.md` — brand voice guidelines (pay special attention to Email Marketing tone section)
- `/memory/shared/positioning.md` — positioning and messaging hierarchy
- `/memory/shared/icp.md` — ideal customer profile (purchase triggers, objections, JTBD)

Then check `/memory/content/` for existing email content to avoid repetition.

## Sequence Types

### Welcome Sequence (New DTC Customers)
**Trigger:** First purchase on spindrift.com or subscription signup.
**Goal:** Turn a first buyer into a repeat buyer. Establish the brand relationship.
**Length:** 5 emails over 14 days.

| Email | Timing | Purpose | Core Message |
|-------|--------|---------|-------------|
| 1 | Immediately | Welcome + order confirmation | "Glad you're here. Here's what you ordered and what's actually in it." |
| 2 | Day 2 | The ingredient story | "Why we use real squeezed fruit (and why almost nobody else does)." |
| 3 | Day 5 | Product discovery | "You tried [flavor]. Here's what to try next." Based on purchase data if available, otherwise bestseller recs. |
| 4 | Day 9 | Social proof + community | "Here's what other Spindrift people say." UGC, reviews, community moments. |
| 5 | Day 14 | Repeat/subscribe CTA | "Running low? Here's the easy way to never run out." Subscription pitch without pressure. |

### Subscriber Nurture
**Trigger:** Email subscriber who hasn't purchased (or hasn't purchased recently).
**Goal:** Build relationship through value, drive first/next purchase organically.
**Length:** 4 emails over 21 days.

| Email | Timing | Purpose | Core Message |
|-------|--------|---------|-------------|
| 1 | Day 0 | Value-first welcome | "Here's what we're about: real squeezed fruit, short ingredient lists, and sparkling water that tastes like actual fruit." |
| 2 | Day 5 | Ingredient education | "What are 'natural flavors' anyway? Here's what we learned when we looked into it." Educational, not preachy. |
| 3 | Day 12 | Flavor guide | "Not sure which flavor to try first? Here's an honest guide." Personality-based or occasion-based recommendations. |
| 4 | Day 21 | Gentle CTA | "If you're curious, here's where to find us." Retail locator + online store. No pressure. |

### Win-Back Sequence
**Trigger:** Customer hasn't purchased in 60+ days (DTC) or hasn't opened in 45+ days (subscriber).
**Goal:** Re-engage without desperation. Remind them why they liked us.
**Length:** 3 emails over 14 days.

| Email | Timing | Purpose | Core Message |
|-------|--------|---------|-------------|
| 1 | Day 0 | Casual check-in | "Still here. Still real fruit. Just checking in." Low-key, no guilt. |
| 2 | Day 5 | What's new | "Here's what's happened since you've been away." New flavors, seasonal offerings, something genuinely interesting. |
| 3 | Day 14 | Last value offer | "If you want back in, here's a reason." Offer (if available) or just a warm reminder. If no engagement, gracefully reduce frequency. |

### New Flavor Launch
**Trigger:** New flavor announcement.
**Goal:** Drive trial of the new flavor. Build excitement through ingredient story.
**Length:** 3 emails over 7 days.

| Email | Timing | Purpose | Core Message |
|-------|--------|---------|-------------|
| 1 | Day 0 | Announcement | "New flavor: [Name]. Here's what's in it." Lead with the fruit, not the branding. |
| 2 | Day 3 | Behind the scenes | "How we made [flavor]. The sourcing, the process, the taste." Story-driven. |
| 3 | Day 7 | Availability + CTA | "Here's where to find it. Here's what people are saying." Reviews, retail availability, online ordering. |

## Spindrift Email Defaults

Apply these to every email in every sequence:

### Subject Lines
- **Clear benefit or genuine curiosity.** Never clickbait.
- **Never:** "You Won't BELIEVE What's Inside!" / "LAST CHANCE" / "Don't Miss Out!"
- **Do:** "What's actually in your sparkling water?" / "New flavor. Real fruit. No surprises." / "The ingredient list is short. On purpose."
- Preview text extends the subject, never repeats it.
- A/B test subject lines where possible. Provide two options per email.

### Body Copy
- **Warm and direct.** Get to the point, but make the point interesting.
- **Conversational but purposeful.** Every paragraph earns its place. If you remove a paragraph and nothing is lost, remove it.
- **Short paragraphs.** 1-3 sentences max. White space is your friend in email.
- **One CTA per email.** Singular, clear, plain language. "Try it" over "Shop Now." "See what's new" over "Explore Our Collection."
- **No corporate sign-offs.** "Thanks for reading" over "Warm regards, The Spindrift Team." Or just end on the CTA.

### Design Direction
- Clean, minimal. Let the copy and product photography do the work.
- Real fruit imagery alongside product — not lifestyle stock photography.
- Mobile-first. Most of the ICP reads email on their phone.
- Ingredient list as a design element, not hidden in fine print.

### Tone Guardrails
- Never create artificial urgency ("Only 3 left!" / "Sale ends tonight!") unless it's genuinely true.
- Never guilt-trip for not opening/purchasing. No "We miss you" in subject lines.
- Never use health claims. Spindrift is a sparkling water with real fruit, not a wellness product.
- Never talk down to the reader. They're smart — they read ingredients. Respect that.

## Execution Steps

1. **Read all memory files.**
2. **Identify the sequence type** from the argument.
3. **Gather context** from the user — any specific product focus, offer, timing constraints, or audience segment.
4. **Design the sequence structure** using the templates above as a starting point. Customize based on context.
5. **Write each email in full** — subject line (2 options), preview text, body copy, CTA.
6. **Run quality gates** on every email.
7. **Save** the sequence.

## Quality Gates (Per Email)

- [ ] **Voice check:** Does this email sound like a real person at Spindrift wrote it? Or does it sound like a marketing automation platform? Read it aloud.
- [ ] **Subject line test:** Is the subject line clear and genuinely interesting? Would you open this email? Is it free of clickbait patterns?
- [ ] **Single CTA check:** Is there exactly one clear action the reader should take?
- [ ] **Paragraph audit:** Does every paragraph earn its place? Try removing each one — if nothing is lost, cut it.
- [ ] **Word audit:** No words from the "Words We Avoid" list. No corporate jargon.
- [ ] **Positioning alignment:** Does the email reinforce real-squeezed-fruit differentiation?
- [ ] **Pressure check:** Is this email respectful of the reader's time and inbox? No false urgency, no guilt, no desperation.
- [ ] **ICP check:** Would the Label Reader persona appreciate receiving this email? Would they read it or delete it?

## Output Format

```markdown
# Email Sequence: [Type] — [Context]
**Date:** [YYYY-MM-DD]
**Sequence type:** [Welcome / Nurture / Win-Back / Launch]
**Emails in sequence:** [Number]
**Total duration:** [X days]

---

## Sequence Overview
[2-3 sentences: the strategic logic of this sequence — what it's trying to accomplish and how]

## Audience
[Target segment from ICP, key motivations this sequence addresses]

---

## Email 1: [Title]
**Send timing:** [Trigger or day]
**Goal:** [What this email should accomplish]

**Subject line A:** [Option 1]
**Subject line B:** [Option 2]
**Preview text:** [40-90 characters]

---

[Full email body copy]

---

**CTA:** [Button/link text]
**CTA destination:** [Where it goes]

---

[Repeat for each email in the sequence]

---

## Sequence Notes
- **Key metric to watch:** [Open rate, click rate, conversion, etc. and why]
- **Suggested A/B tests:** [Beyond subject lines — timing, length, CTA placement]
- **Exit conditions:** [When someone should leave this sequence — e.g., they purchase, they unsubscribe, they enter another sequence]
```

## Save Location

Print to conversation AND save to `/projects/active/email/sequence-[type]-[YYYY-MM-DD].md`.

## Related Skills

- `copywriting` — Write individual emails or email campaigns outside of sequences
- `/critique` — Evaluate email drafts against voice and positioning standards
