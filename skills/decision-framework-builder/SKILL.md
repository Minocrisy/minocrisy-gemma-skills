---
name: decision-framework-builder
description: Apply structured decision frameworks to important choices. Clarify criteria, surface options, evaluate trade-offs, and produce a defensible recommendation or ranked set of options. Use for high-stakes or multi-factor decisions.
version: 0.1.1
---

# Decision Framework Builder

## Role
Bring structure to decisions instead of gut feel.

## Activation Conditions
Use when the user:
- Faces a real choice with consequences ("Should I take this job or that one?", "Which option?")
- Has multiple factors or conflicting priorities
- Wants a clear way to decide

Do not use for:
- Trivial choices
- Purely emotional decisions

## Instructions

1. Clarify the decision and timeframe.

2. List the criteria that matter and roughly weight them.

3. Generate real options (including doing nothing).

4. Score or compare them against the criteria.

5. Run sensitivity and recommend with next step.

## Output Format

### Decision
One sentence.

### Criteria
Weighted list.

### Comparison
How options score.

### Recommendation
Top choice + why + immediate next action.

## Examples

**User (engineer with family):** "Job A pays more but long hours and relocation. Job B is remote with better culture."

**Good output:**

Decision
Choose between higher-pay/high-hours Job A and lower-pay/remote Job B.

Criteria
1. Skill growth (35%)
2. Family time/energy (30%)
3. Pay/security (20%)
4. Balance (15%)

Recommendation
Take Job B and negotiate higher pay. Reconsider A only if runway <9 months.

**Bad output:**
Unweighted pros/cons list with no recommendation or next step.

## Boundaries
- Helps clarity but doesn't solve value conflicts.
- Big decisions may need expert input.

## Limitations
- Needs the user to define or accept criteria.