---
disable-model-invocation: true
argument-hint: [file] [format] — source content path + target format (thread | video | post | email | social | ad)
---

# /repurpose [file] [format] — Content Repurposing

## Before Executing

Read the following memory file:

- `/memory/shared/voice.md` — brand voice guidelines (every format must sound like Spindrift)

Then read the source content file provided as the first argument.

## What This Command Does

Takes existing Spindrift content and reshapes it for a different format. This is not summarization or shortening — it is re-angling the core ideas for a new medium, audience context, and consumption pattern.

## Supported Formats

| Format   | Description                        | Key Characteristics                                                                 |
|----------|------------------------------------|-------------------------------------------------------------------------------------|
| `thread` | Social media thread (X/Twitter)    | Hook in first post, one idea per post, builds momentum, ends with CTA or callback   |
| `video`  | Video script                       | Visual directions + spoken word, hook in first 3 seconds, conversational tone        |
| `post`   | Blog post                          | Structured with headers, scannable, SEO-aware, deeper exploration of the topic       |
| `email`  | Newsletter edition                 | Personal tone, single clear CTA, subject line + preview text, skimmable structure    |
| `social` | Single social media post           | One sharp idea, platform-native feel, stops the scroll, under character limits       |
| `ad`     | Ad copy                            | Headline + body + CTA, benefit-led, concise, multiple variants                       |

## Execution Steps

1. **Read the source content.** Identify the core insight, key supporting points, and any proof points or data.
2. **Read the voice guide.** The repurposed piece must sound like Spindrift regardless of format.
3. **Analyze the target format.** Consider:
   - How does the audience encounter this format? (Scrolling, searching, inbox, mid-video)
   - What is the attention window? (2 seconds for social, 2 minutes for email, 5+ minutes for blog)
   - What action should the audience take after consuming?
4. **Re-angle, don't just resize.** Find the angle within the source content that is most native to the target format. A blog post about ingredient sourcing becomes a thread about "what most sparkling water brands won't tell you." An email about a new flavor becomes an ad about the specific fruit.
5. **Produce the repurposed content** following the format-specific structures below.

## Format-Specific Structures

### thread
```
[Post 1 — Hook: provocative claim, question, or surprising fact]
[Post 2 — Context or setup]
[Post 3-N — One idea per post, building on the previous]
[Final Post — CTA, callback to hook, or memorable closer]
```

### video
```
HOOK (0-3s): [Visual + spoken word to stop scrolling]
SETUP (3-10s): [Establish the topic and why it matters]
BODY (10-45s): [Core content — visual directions in brackets, spoken word in plain text]
CTA (45-60s): [Clear next step for viewer]
---
Suggested B-roll / visuals: [List]
Music/tone direction: [Description]
```

### post
```
# [SEO-friendly headline]
**Meta description:** [155 characters max]
[Opening paragraph — hook the reader]
## [Section headers]
[Body — scannable, short paragraphs]
## [Conclusion / CTA]
```

### email
```
**Subject line:** [Primary]
**Subject line alt:** [Alternative]
**Preview text:** [40-90 characters]
---
[Opening — personal, one clear hook]
[Body — 2-3 short sections, skimmable]
[CTA — single, clear action]
[Sign-off]
```

### social
```
[Post text — platform-native, within character limits]
---
Alt versions:
1. [Different angle]
2. [Different hook]
Suggested visual: [Description]
```

### ad
```
**Variant 1**
Headline: [Benefit-led, concise]
Body: [1-2 sentences]
CTA: [Action text]

**Variant 2**
[Different angle]

**Variant 3**
[Different angle]
---
Target audience note: [Who this is optimized for]
```

## Output Format

```
# Repurposed: [Source title] → [Format]

**Source:** [File path]
**Target format:** [Format name]
**Core insight carried forward:** [One sentence]

---

[Format-specific content]

---

## Repurposing Notes
- **Angle chosen:** [Why this angle works for the target format]
- **What was left out:** [Key points not included and why]
- **Suggested next repurpose:** [Another format this content would work in]
```

## Save Location

Save to `/projects/active/repurposed/[source-slug]-[format].md`
