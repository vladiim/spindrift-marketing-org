---
disable-model-invocation: true
argument-hint: /brief [topic]
---

# /brief — Content Brief Generator

Produces a strategic content brief grounded in Spindrift's voice, positioning, and audience.

## Steps

1. **Read memory files for context:**
   - `/memory/shared/voice.md`
   - `/memory/shared/positioning.md`
   - `/memory/shared/icp.md`

2. **Check past content for overlap:**
   - Scan `/memory/content/` for existing briefs and published content
   - Identify any previous angles on the same or adjacent topics
   - If overlap exists, note it and differentiate the new angle explicitly

3. **Generate the brief using the provided topic:**
   - Select the most relevant ICP segment for this topic
   - Align key messages to Spindrift's positioning (real squeezed fruit, transparency, taste)
   - Match tone and language to the voice guidelines
   - Choose distribution channels appropriate to the audience segment

4. **Assemble the brief in the format below.**

5. **Save the brief:**
   - Save to `/projects/active/brief-[topic-slug]-[YYYY-MM-DD].md`
   - Use a lowercase, hyphenated slug derived from the topic

## Output Format

Print the brief to the conversation AND save to the path above.

```
# Content Brief: [Topic]
**Date:** [YYYY-MM-DD]
**Author:** Claude

## Topic Angle
[1-2 sentences: the specific angle, not just the broad topic]

## Target Audience Segment
[Which ICP segment and why this topic matters to them]

## Key Messages
1. [Primary message]
2. [Supporting message]
3. [Supporting message]

## Differentiation from Past Content
[How this differs from previous content on similar topics, or "No prior overlap found"]

## Distribution Channels
- [Channel]: [rationale]
- [Channel]: [rationale]

## Success Metrics
- [Metric 1]
- [Metric 2]
- [Metric 3]

## Draft Outline
1. [Section]
2. [Section]
3. [Section]
4. [Section]
```
