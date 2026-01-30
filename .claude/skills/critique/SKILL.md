---
disable-model-invocation: true
argument-hint: [file] — path to the draft content to critique
---

# /critique [file] — Content Quality Critique

## Before Executing

Read the following memory files to establish evaluation criteria:

- `/memory/shared/voice.md` — brand voice guidelines
- `/memory/shared/positioning.md` — positioning and differentiation
- `/memory/shared/icp.md` — ideal customer profile

Then read the draft file provided as the argument.

## What This Command Does

Evaluates a content draft against Spindrift's voice guide, positioning, ICP alignment, and quality standards. Provides specific issues with concrete fixes, organized by severity. Then produces a complete revised version incorporating all fixes.

## Execution Steps

1. **Read and internalize** the three memory files. These are the evaluation criteria — not suggestions, but standards.
2. **Read the draft** provided as the argument.
3. **Evaluate the draft** against each standard:
   - **Voice alignment** — Does it sound like Spindrift? Check tone, word choice, sentence rhythm against the voice guide.
   - **Positioning alignment** — Does it reinforce Spindrift's differentiation? Does it make claims that are ownable and true?
   - **ICP resonance** — Would this land with the target audience? Does it address their motivations, not just demographics?
   - **Craft quality** — Is the writing sharp? Check for: flabby phrasing, cliches, passive voice, buried leads, weak openings/closings, unclear structure.
4. **Organize issues by severity**:
   - **Blocking** — Must fix before publishing. Misaligned positioning, wrong voice, factual issues, anything that would actively hurt the brand.
   - **Important** — Should fix. Weakens the piece but does not break it. Missed opportunities, soft language where strong is needed, structural issues.
   - **Nice-to-have** — Polish items. Would improve the piece but acceptable as-is.
5. **Produce a complete revised version** that addresses all blocking and important issues, and as many nice-to-have items as possible.
6. **Summarize changes** between the original and revised version.

## Output Format

```
# Content Critique — [Draft filename]

## Issues

### Blocking
1. **[Issue title]**
   - Location: [Quote or line reference]
   - Problem: [What's wrong and why it matters]
   - Fix: [Specific, concrete fix — not "make it better"]

### Important
1. **[Issue title]**
   - Location: [Quote or line reference]
   - Problem: [What's wrong and why it matters]
   - Fix: [Specific, concrete fix]

### Nice-to-Have
1. **[Issue title]**
   - Location: [Quote or line reference]
   - Suggestion: [Specific improvement]

---

## Revised Version

[Complete revised draft — full text, ready to use]

---

## Summary of Changes

- [Change 1 — what was done and why]
- [Change 2 — what was done and why]
```

## Save Location

Output directly to the conversation. Do not save to a file unless the user requests it.
