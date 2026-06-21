---
name: root-cause-analyzer
description: Move past symptoms to identify the underlying systemic or structural causes of a problem, failure, or undesirable outcome. Use for diagnosis of recurring issues or complex failures.
version: 0.1.1
---

# Root Cause Analyzer

## Role
You identify the real systemic causes behind recurring problems instead of accepting surface explanations.

## Activation Conditions
Use this when the user describes:
- A problem that keeps happening ("launches always slip", "this issue comes up again and again")
- Wants to understand why something fails repeatedly ("Why do our launches keep missing deadlines?" or "How do we stop this recurring?")
- Has tried fixes that only addressed symptoms

Do not use for:
- One-off problems or simple troubleshooting
- Questions about a single past event

## Instructions

1. Clearly define the recurring problem in specific terms.

2. Trace the causes step by step until you reach the root systemic issue (not just the immediate symptom).

3. Distinguish between one-time causes and recurring patterns (incentives, processes, missing feedback loops).

4. Suggest high-leverage interventions that address the root.

## Output Format

### Problem
Brief description of the recurring issue.

### Root Causes
1. Symptom
   - Why
   ...
   - Systemic root

### Interventions
- Specific changes that would prevent recurrence.

## Examples

**User:** "Our product launches always slip by several weeks no matter how carefully we plan."

**Good output:**

Problem
Product launches repeatedly miss committed dates by 3-6 weeks.

Root Causes
- Estimates do not account for integration and review work.
- No process to use historical accuracy data when planning.
- Team is incentivized to set aggressive dates rather than realistic ones (root).

Interventions
- Require using data from the last 3 launches when setting dates.
- Add mandatory buffer based on past slippage.
- Change review process so dates are set by someone measured on accuracy, not speed.

**Bad output:**
Just says "underestimated the work" or lists symptoms without identifying the incentive or process root.

## Boundaries
- Focus on systemic causes, not blaming individuals.
- End with actionable interventions.

## Limitations
- Works best when the user can describe the actual process and incentives honestly.