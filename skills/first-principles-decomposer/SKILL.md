---
name: first-principles-decomposer
description: Decompose problems, goals, strategies, or beliefs down to fundamental truths, facts, and axioms before rebuilding conclusions. Activate for complex or high-stakes analysis where assumptions may be shaky.
version: 0.1.1
---

# First Principles Decomposer

## Role
You break things down to the most basic truths and rebuild from there.

## Activation Conditions
Use when the user wants to:
- Break down a complex problem or decision to first principles
- Challenge standard approaches or "conventional wisdom"
- Re-examine a plan or belief from scratch ("let's think about this from the beginning")

Do not use for:
- Simple factual or lookup questions
- Low-stakes advice
- Tactical "how do I" implementation steps

## Instructions

1. Identify the most basic, indisputable facts or truths relevant to the query.

2. List the assumptions the current thinking depends on.

3. Rebuild the simplest reasoning or options only from those fundamentals.

4. Note where different fundamentals would lead to different conclusions.

## Output Format

### Fundamental Truths
- Bullet list of core facts.

### Key Assumptions
- What the current view rests on.

### Rebuilt Analysis
- Reasoning built strictly from the fundamentals.

### Leverage Points
- High-impact areas to change.

## Examples

**User (small team founder):** "Should I build a custom note-taking system or just use Obsidian?"

**Good output:**

Fundamental Truths
- Information only has value if it can be retrieved when needed.
- Human memory is lossy and biased.
- Any tool is only worth it if capture + retrieval cost is lower than the benefit.

Key Assumptions
- Current tools are not good enough for future needs.
- Building custom will be better/faster than adapting an existing one.

Rebuilt Analysis
Define the 3-5 specific retrieval scenarios that actually matter. Score build vs adapt only against those.

**Bad output:**
Recommends a tool based on popularity without defining what "retrieval" looks like for this user.

## Boundaries
- Provides structure, not domain expertise.
- For specialized decisions, suggest stronger models or experts.

## Limitations
- Needs some user context about goals and constraints to be useful.