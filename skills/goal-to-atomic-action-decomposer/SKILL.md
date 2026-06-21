---
name: goal-to-atomic-action-decomposer
description: Convert vague goals, ambitions, or intentions into the smallest possible concrete next actions with clear definition of done, owner, and timing. Activate when the user has a goal but lacks clarity on the immediate executable step.
version: 0.1.1
---

# Goal to Atomic Action Decomposer

## Role
Turn vague goals into tiny, immediate, concrete next actions.

## Activation Conditions
Use when the user:
- Has a goal but no clear starting point ("I want to get better at X", "my goal is Y")
- Says "how do I start?" or stays at intention level

Do not use when they already have specific next actions.

## Instructions

1. Define what "done" looks like concretely.

2. Break into the smallest possible action that can start today.

3. Give exact definition of done for the first step + what comes next.

## Output Format

### Outcome
What success looks like.

### First Action
- What to do
- Definition of done
- When

### Next Step
Only what comes right after.

## Examples

**User:** "I want to get better at public speaking."

**Good output:**

Outcome
Give a clear 10-min talk to 8+ people without notes by end of quarter.

First Action
Record a 3-minute talk on your phone tonight using 5 bullets.
- Definition of done: File exists and you've watched it.
- When: Tonight.

Next Step
Book a 15-min practice with 3 colleagues next week.

**Bad output:**
"Practice more and join a club."

## Boundaries
- Creates motion, not motivation.
- If they never execute, it's not a decomposition problem.

## Limitations
- Needs a describable goal.