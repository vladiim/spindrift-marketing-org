---
disable-model-invocation: true
argument-hint: (no arguments)
---

# /weekly-review — Strategic Weekly Review

## Before Executing

Read the following memory files to establish context:

- `/memory/shared/positioning.md`
- `/memory/shared/icp.md`
- `/memory/shared/voice.md`

Then scan the following directories and files:

- `/projects/active/` — all active project files for progress assessment
- `/projects/backlog/` — backlog items that may need promotion
- `/memory/` — all memory files, checking for staleness and gaps
- `/tools/skills-index.md` — current skill registry for maintenance audit
- `/prompts/SYSTEMATIZATION.md` — prompt audit framework

## What This Command Does

Produces a strategic weekly review applying Rumelt's strategy kernel. This is not a status update — it is a diagnosis of what is actually happening, identification of the crux, and planning of coherent actions for the coming week.

The review also audits the system itself to keep it sharp.

## Execution Steps

### Part 1: Strategic Diagnosis

1. **Diagnose** — Review all active projects and recent outputs. What is actually happening? Identify root causes, not symptoms. Look for patterns across projects: what is working, what is stalling, what is being avoided.
2. **Identify the Crux** — What is the single most important challenge or opportunity right now? What makes it hard?
3. **Guiding Policy** — Based on the diagnosis, what is the approach for next week? This should be a clear, focused direction — not a list of everything that could be done.
4. **Coherent Actions** — List specific, reinforcing actions for next week that follow from the guiding policy. Each action should be concrete enough to execute without further planning.

### Part 2: Project Review

For each project in `/projects/active/`:
- Current status and recent progress
- Blockers or stalls
- Whether it should remain active, move to backlog, or be closed

Check `/projects/backlog/` for items that should be promoted to active based on current strategic direction.

### Part 3: System Audit (Prompt Systematization)

1. **Prompt Patterns** — Identify any tasks that were performed repeatedly this week without a dedicated command. Recommend new slash commands where warranted.
2. **Command Refinement** — Flag any existing commands that produced suboptimal results or required manual correction. Suggest specific improvements.
3. **Workflow Gaps** — What workflows emerged organically that the system does not yet support?
4. **Memory Staleness** — Flag any memory files that appear outdated, contradictory, or incomplete. Recommend updates.
5. **Skills Maintenance** — Check `/tools/skills-index.md`. Flag any skills that should be added, updated, or pruned. Check community sources for new relevant skills.

## Output Format

```
# Weekly Review — [Date]

## Strategic Diagnosis

### What's Actually Happening
[Narrative diagnosis — patterns, root causes, honest assessment]

### The Crux
[The single most important challenge or opportunity]

### Guiding Policy for Next Week
[Clear, focused direction]

### Coherent Actions
1. [Specific action]
2. [Specific action]
3. [Specific action]

## Project Review

### Active Projects
| Project | Status | Progress | Recommendation |
|---------|--------|----------|----------------|
| ...     | ...    | ...      | ...            |

### Backlog Candidates for Promotion
- [Project and rationale, if any]

## System Audit

### New Commands to Consider
- [Pattern observed] → suggested command: `/command-name`

### Commands Needing Refinement
- [Command] — [Issue and suggested fix]

### Workflow Gaps
- [Gap description]

### Memory Maintenance
- [File] — [Issue: stale / incomplete / contradictory]

### Skills Index Status
- [Current / needs update — specifics]
```

## Save Location

Save the completed review to:

```
/memory/analytics/weekly-reviews/[YYYY-MM-DD].md
```
