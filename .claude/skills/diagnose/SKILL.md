---
disable-model-invocation: true
argument-hint: [challenge] — describe the marketing challenge to diagnose
---

# /diagnose [challenge] — Strategy Diagnosis

## Before Executing

Read the following memory files to ground the diagnosis in Spindrift's actual situation:

- `/memory/shared/positioning.md` — current positioning and differentiation
- `/memory/shared/icp.md` — ideal customer profile
- `/memory/shared/voice.md` — brand voice (relevant for communication-related challenges)

Also scan for additional context:

- `/projects/active/` — current initiatives that may relate to the challenge
- `/memory/analytics/` — recent performance data and past reviews
- `/memory/strategy/` — prior diagnoses for historical context

## What This Command Does

Applies Rumelt's full strategy kernel to a marketing challenge. A good strategy is not a list of goals — it is a coherent response to a specific challenge. This command produces that response.

## Execution Steps

### Step 1: Diagnosis — What Is Actually Happening

This is the most important step. Most strategy fails because the diagnosis is wrong.

- Restate the challenge as presented, then interrogate it. Is this the real problem, or a symptom of something deeper?
- Identify root causes. Use available data, positioning context, and competitive dynamics.
- Name the specific obstacles. Vague diagnoses produce vague strategies.
- State what makes this challenge hard — the crux. If it were easy, it would already be solved.

### Step 2: Guiding Policy — The Approach

The guiding policy is not a goal ("grow awareness") — it is a method of dealing with the challenge identified in the diagnosis.

- Define a clear approach that addresses the crux directly.
- The policy should channel effort — it should rule things out, not just rule things in.
- It must be consistent with Spindrift's positioning and resources.
- State what this policy means Spindrift will NOT do (this is as important as what it will do).

### Step 3: Coherent Actions — Specific, Reinforcing Steps

Actions must be:
- **Specific** — concrete enough to execute without further strategic thinking
- **Coherent** — they reinforce each other, not just a grab bag of tactics
- **Feasible** — achievable with available resources and within realistic timelines
- **Sequenced** — ordered by dependency and priority

For each action, state:
- What to do
- Why it follows from the guiding policy
- How it reinforces the other actions
- What success looks like

## Output Format

```
# Strategy Diagnosis — [Challenge Title]
Date: [Today's date]

## The Challenge
[Restatement of the challenge as provided]

## Diagnosis: What's Actually Happening

### Surface Symptoms
[What the challenge looks like from the outside]

### Root Causes
[What is actually driving the problem — evidence-based]

### The Crux
[The core difficulty — what makes this hard]

## Guiding Policy

[Clear statement of the approach — 2-3 paragraphs maximum]

### What This Means We Will NOT Do
- [Explicit exclusion and why]
- [Explicit exclusion and why]

## Coherent Actions

### 1. [Action Title]
- **Do:** [Specific action]
- **Because:** [How it follows from the guiding policy]
- **Reinforces:** [How it connects to other actions]
- **Success looks like:** [Observable outcome]

### 2. [Action Title]
...

### 3. [Action Title]
...

## Risks and Assumptions
- [Key assumption this strategy depends on]
- [Risk and mitigation]

## Review Trigger
[When or under what conditions this diagnosis should be revisited]
```

## Save Location

Save the completed diagnosis to:

```
/memory/strategy/diagnoses/[YYYY-MM-DD]-[short-slug].md
```
