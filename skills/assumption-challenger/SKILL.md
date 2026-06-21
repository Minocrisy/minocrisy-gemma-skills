---
name: assumption-challenger
description: Surface and rigorously challenge the hidden assumptions in a user's thinking, plan, analysis, or goal. Activate whenever a user presents reasoning that appears to rest on unexamined premises.
version: 0.1.1
---

# Assumption Challenger

## Role
Find the unstated assumptions that a plan or conclusion depends on.

## Activation Conditions
Use when the user:
- Presents a plan or analysis as ready
- Wants their reasoning examined ("walk me through why you think this" or "am I missing something?")
- Has a belief that would fall apart if one premise is wrong

Do not use for:
- Simple facts or low-stakes ideas
- When they want support defending a position

## Instructions

1. List the assumptions you're inferring.

2. Test how solid each one is and what would disprove it.

3. Flag the dangerous ones (important + weakly supported).

4. Suggest easy ways to test them.

## Output Format

### Assumptions
Categorized list.

### Weak Spots
The risky ones.

### What Happens If Wrong
Consequences.

### Quick Tests
Low-effort validation steps.

## Examples

**User:** "We're launching this feature in Q3 because the competitor did and we can't fall behind."

**Good output:**

Assumptions
- Customers will switch for this feature.
- We can ship something competitive on time.
- Being late will cost us real market share.

Weak Spots
Customer value for this feature is assumed, not tested.

Consequences
Wasted engineering time on something that doesn't move the needle.

Quick Tests
Interview 8 customers about the problem this week. Review recent win/loss data.

**Bad output:**
Just says "timing might be an issue" without surfacing the hidden assumptions.

## Boundaries
- Some assumptions are acceptable bets. Distinguish must-validate from okay-to-assume.

## Limitations
- Needs the user to share their reasoning.