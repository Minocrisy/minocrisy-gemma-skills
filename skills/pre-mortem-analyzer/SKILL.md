---
name: pre-mortem-analyzer
description: Conduct a structured pre-mortem: assume a plan or decision has failed in the future, then work backward to identify why it failed and what can be done now to prevent it. Use before committing to important plans or decisions.
version: 0.1.1
---

# Pre-Mortem Analyzer

## Role
Assume the plan has failed and identify why, then prevent it.

## Activation Conditions
Use when the user:
- Presents a plan or decision they're about to commit to
- Asks "what could go wrong?" or wants to find risks before starting
- Has a timeline-based initiative or high-stakes choice

Do not use for:
- Post-mortems of things that already happened
- Low-stakes or casual hypotheticals

## Instructions

1. Describe the specific future failure state.

2. List the most plausible reasons it failed, prioritizing ones that are easy to miss.

3. Trace causes back to today's controllable decisions.

4. Give concrete prevention steps.

5. Note what can't be fully controlled.

## Output Format

### Failure State
Clear description.

### Top Failure Modes
- Ranked
- Why
- Signals

### Prevention
Actionable steps.

### Residual Risk
What to watch.

## Examples

**User (founder launching in 8 weeks):** "Here's my go-to-market plan..."

**Good output:**

Failure State
Launch happens but zero customers and no revenue after 30 days.

Top Failure Modes
1. Built without validating real customer problems.
   - Why: Only talked to friends.
   - Signal: Low landing page signups.

Prevention
- 10 problem interviews this week.
- Test paid waitlist before building.

**Bad output:**
Vague risks like "competition or timing issues" without linking to the plan.

## Boundaries
- Not a replacement for real research.
- Use for real commitments only.

## Limitations
- Needs details about the actual plan to be effective.