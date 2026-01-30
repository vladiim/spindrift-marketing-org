---
disable-model-invocation: true
argument-hint: (no arguments)
---

# /wip — Work in Progress Dashboard

Session-start ritual. Shows what's active, what's stuck, and what to do next.

## Steps

1. **Read memory files for context:**
   - `/memory/shared/positioning.md`
   - `/memory/shared/icp.md`

2. **Scan active projects:**
   - Read all files in `/projects/active/`
   - For each project, extract: name, status, last modified date, next milestone, owner if listed

3. **Identify recent changes:**
   - Check git log or file modification times across the repo for the last 48 hours
   - Note any new files, significant edits, or completed deliverables

4. **Detect blockers and overdue items:**
   - Flag any project with no updates in 7+ days
   - Flag any task past its stated deadline
   - Flag any draft content that has been in draft state for 5+ days

5. **Recommend next action:**
   - Prioritize: overdue items first, then items closest to completion, then highest-impact work based on ICP and positioning alignment
   - Provide a single clear recommendation for what to work on right now, with reasoning

## Output Format

Print the dashboard directly to the conversation. Do not save to a file.

```
## WIP Dashboard — [today's date]

### Active Projects
| Project | Status | Last Updated | Next Step |
|---------|--------|--------------|-----------|
| ...     | ...    | ...          | ...       |

### Overdue / Stalled
- [item]: [days overdue or days since last update] — [what's needed]

### Draft Content
- [draft name]: [status, age] — [next action]

### Recent Activity (48h)
- [summary of changes]

### Recommended Next Action
[Single clear recommendation with reasoning tied to priorities]
```
