---
disable-model-invocation: true
argument-hint: /analytics [period] (default: "last 7 days")
---

# /analytics — Performance Summary

Synthesizes available metrics into an executive summary: what's working, what's not, what changed, and what to do about it. Not a data dump — interpretation and recommendations.

## Steps

1. **Read memory files for context:**
   - `/memory/shared/positioning.md`
   - `/memory/shared/icp.md`

2. **Read historical analytics context:**
   - Read all files in `/memory/analytics/`
   - Identify prior benchmarks, trends, and past recommendations

3. **Determine the reporting period:**
   - Use the provided `[period]` argument (e.g., "last 7 days", "January", "Q4")
   - If no period is provided, default to "last 7 days"

4. **Pull and synthesize available metrics:**
   - Look for any data files, reports, or logged metrics in `/memory/analytics/` and `/projects/active/`
   - Organize by channel or initiative
   - Compare to prior periods where data exists

5. **Interpret the data:**
   - Identify what is working and why
   - Identify what is underperforming and possible causes
   - Note any significant changes from prior periods
   - Formulate 2-3 specific, actionable recommendations

## Output Format

Print the summary directly to the conversation. Do not save to a file.

```
## Performance Summary — [period]

### Executive Summary
[2-3 sentences: the headline takeaway for a busy marketing lead]

### What's Working
- [Insight]: [supporting evidence]
- [Insight]: [supporting evidence]

### What's Not Working
- [Insight]: [supporting evidence and possible cause]
- [Insight]: [supporting evidence and possible cause]

### Notable Changes
- [Change]: [comparison to prior period]

### Recommendations
1. [Action]: [rationale]
2. [Action]: [rationale]
3. [Action]: [rationale]

### Data Gaps
[List any metrics that were unavailable or incomplete — be honest about what we don't know]
```
