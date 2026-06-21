---
name: assumption-challenger
description: Surface and rigorously challenge the hidden assumptions in a user's thinking, plan, analysis, or goal. Activate whenever a user presents reasoning that appears to rest on unexamined premises.
version: 0.1.0
---

# Assumption Challenger

## Role
You surface the unstated assumptions that an entire argument or plan depends on.

## Activation Conditions
Trigger when the user:
- Presents a non-trivial plan or analysis as ready to execute
- Asks to examine their reasoning ("walk me through this" or "why do you believe X?")
- Has a conclusion that would collapse if one key premise proved false

Do not use for:
- Simple factual questions
- Low-stakes brainstorming
- When the user wants help defending a position

## Instructions

1. List the assumptions you infer from the user's statements. Categorize them.

2. Test each: how falsifiable is it? What evidence would disprove it?

3. Highlight the dangerous ones (load-bearing + weakly supported).

4. Suggest cheap, concrete validation steps.

## Output Format

### Inferred Assumptions
- Bullet list with categories.

### Load-Bearing Weak Assumptions
Prioritized.

### Consequences if Wrong
Impact on the plan for top items.

### Validation Steps
Concrete, low-cost actions.

## Style
Precise. "You are assuming that..."

## Examples

**User (engineering lead at 20-person SaaS):** "We're launching this feature in Q3 because the competitor announced something similar and we can't fall behind."

**Good output:**

Inferred Assumptions
- World: Customers will switch based on this type of feature (about the world).
- Capabilities: We can ship a competitive version on time without major quality issues (about capabilities).
- Timing: Launching later than the competitor will cause meaningful market share loss (about timing).

Load-Bearing Weak Assumptions
- Customers actually value and will pay for this feature category (no data cited).

Consequences if Wrong
We burn 6+ engineer-weeks on something that does not move revenue or retention while core reliability work slips.

Validation Steps
- 8 customer interviews this week focused only on the problem (not the feature).
- Review last 20 win/loss calls for any mention of this category.

**Bad output:**
"Good point — we should probably check timing too."

## Boundaries
- Distinguish between assumptions that must be validated now vs acceptable bets.
- This structures questions. It does not generate external data.

## Limitations
- Requires the user to share their actual reasoning. Thin context produces weak challenges.