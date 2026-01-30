# Prompt Systematization System

## Purpose

This system ensures the slash command library grows organically from actual usage, not from theoretical planning. Every repeated workflow becomes a command. Every unused command gets pruned. The library mirrors how we actually work.

---

## The Weekly Prompt Audit

Built into `/weekly-review`. Every week, answer:

### 1. What prompts did I type more than twice this week?
Each becomes a candidate for a new slash command.
- Review conversation history for repeated patterns
- Identify the core workflow being repeated
- Draft the command name and argument structure
- Create the SKILL.md in `.claude/skills/[command-name]/`

### 2. Which existing commands need refinement?
Update the SKILL.md with lessons learned.
- Which commands produced output that needed heavy editing?
- Which commands missed context they should have read?
- Which commands had unclear output formats?
- Update the SKILL.md, don't create a new command

### 3. What new workflows emerged that I didn't plan?
Name them, even before building the command.
- Document the workflow in `/prompts/emerging-workflows.md`
- Track how often each emerges
- Promote to command when used 3+ times

### 4. What's the system missing?
Where are gaps between what I do and what's automated?
- What manual work am I doing that feels repetitive?
- What context am I re-explaining in every session?
- What decisions am I making that follow a pattern?

---

## The Emergence Principle

The command library evolves in phases:

### Week 1: Foundation (5-8 starter commands)
- `/wip` — session start ritual
- `/brief` — content brief generation
- `/analytics` — performance summary
- `/competitor` — competitive analysis
- `/weekly-review` — strategic review
- `/critique` — content quality check
- `/diagnose` — strategy diagnosis
- `/repurpose` — content reshaping

### Weeks 2-3: Refinement + Extension
- Refine starters based on actual usage
- Add 2-3 new commands from repeated patterns
- Start connecting commands (output of one feeds input of another)

### Month 2: Chains Emerge
- Commands start referencing each other naturally
- `/brief` → `/critique` → `/repurpose` becomes a content pipeline
- `/competitor` → `/diagnose` → strategy update becomes an intelligence loop
- `/analytics` → `/diagnose` → `/weekly-review` becomes the review cycle

### Month 3: Library = Playbook
- The command library IS the marketing playbook
- New team members learn by reading SKILL.md files
- Workflows are documented as command chains

### Month 6: Evolved System
- The system has evolved into something you couldn't have designed upfront
- Commands reflect actual workflows, not theoretical ones
- Pruned commands reveal what didn't matter
- Active commands reveal what does

---

## Command Design Standards

### Naming
- Verb or noun, never both (prefer nouns for dashboards, verbs for actions)
- Max 2 words, prefer 1
- Must be instantly recognizable after first use

### Arguments
- First argument is the most common variable
- Defaults should work for 80% of cases
- Optional arguments for customization

### Context Loading
- Every command reads relevant memory files before executing
- Always check: voice, positioning, ICP (the trinity)
- Load division-specific memory as needed

### Output
- Clear structure: summary → detail → action items
- Save location defined in the SKILL.md
- Output should be usable without editing for 80% of cases

### Chain Compatibility
- Output of one command should be valid input for another
- Use consistent file formats
- Save to predictable locations

---

## Tracking

### Command Usage Log
Track in `/prompts/usage-log.md`:
```
| Date | Command | Modifications Needed | Rating (1-5) |
|------|---------|---------------------|---------------|
```

### Emerging Workflows
Track in `/prompts/emerging-workflows.md`:
```
| Workflow | Times Used | Last Used | Promoted? |
|----------|-----------|-----------|-----------|
```

---

## The Compound Effect

Each new command multiplies the value of existing commands:
- `/brief` creates better input for `/critique`
- `/competitor` feeds context into positioning updates
- `/analytics` provides data for `/weekly-review`
- `/diagnose` improves the quality of `/brief` recommendations
- `/weekly-review` identifies when to run `/competitor` updates
- `/repurpose` extends the value of every piece of content

The system gets smarter the more you use it. That's the point.
