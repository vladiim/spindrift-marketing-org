# Tool & Agent Discovery System

## Purpose

This system scans community directories weekly to find new agents, skills, and MCPs that can improve Spindrift's marketing system. The goal: the system gets smarter over time by discovering better ways to execute.

---

## Directories to Scan

### Primary Sources

1. **aitmpl.com/agents** — https://www.aitmpl.com/agents
   - Community Claude Code agent templates, skills, hooks, MCPs
   - Check weekly for new marketing-relevant entries
   - Focus: marketing automation, content tools, analytics agents

2. **Official Claude Code examples** — https://github.com/anthropics/claude-code
   - Official skill patterns and best practices
   - Check monthly for new patterns
   - Focus: skill architecture improvements, new capabilities

3. **Marketing Skills Library** — https://github.com/coreyhaines31/marketingskills
   - Dedicated marketing skills for Claude Code
   - Check weekly — this is the primary skills source
   - Pull latest, diff against installed, merge improvements

---

## Weekly Review Process

### Step 1: Scan Directories
For each directory:
- Fetch the latest listing
- Compare against `/tools/skills-index.md` (installed, deferred, skipped)
- Flag anything new or updated

### Step 2: Evaluate New Discoveries
For each new agent/skill/tool:
1. **What does it do?** — Clear description of capability
2. **Does it fit?** — Relevance to Spindrift's current needs and stage
3. **Does it overlap?** — Check against existing system for redundancy
4. **What's the effort?** — Installation complexity and customization needed
5. **Recommendation:** Install, defer (with trigger condition), or skip (with reason)

### Step 3: Install and Customize
For items recommended to install:
1. Copy to appropriate location (`.claude/skills/` for skills)
2. Customize with Spindrift brand context
3. Wire into existing command chains
4. Add to `/tools/skills-index.md`
5. Test with a real task

### Step 4: Maintain Existing
For already-installed items:
1. Check for updates in source repo
2. Merge improvements while preserving brand customizations
3. Review usage — prune unused (30+ days) to deferred

---

## Evaluation Criteria

### Install Now (meets all):
- [ ] Directly relevant to current challenges or active workflows
- [ ] Will be used within next 30 days
- [ ] Doesn't duplicate existing capability
- [ ] Installation effort justified by expected value

### Defer (meets any):
- [ ] Relevant but not urgent
- [ ] Requires capability we don't have yet (e.g., API access)
- [ ] Good for a phase we haven't reached
- [ ] Needs prerequisite skill installed first

### Skip (meets any):
- [ ] Not relevant to Spindrift's market or stage
- [ ] Fully duplicated by existing skill
- [ ] Quality too low to justify customization
- [ ] Requires tools/platforms we don't use

---

## Discovery Log

Track all discoveries in `/tools/discovery-log.md`:

```
| Date | Source | Item | Type | Decision | Reason |
|------|--------|------|------|----------|--------|
```

---

## Integration Points

- `/weekly-review` triggers the weekly scan
- New skills get mapped to divisions in CLAUDE.md
- Installed skills get added to `/tools/skills-index.md`
- Discovery insights feed into `/prompts/SYSTEMATIZATION.md`
