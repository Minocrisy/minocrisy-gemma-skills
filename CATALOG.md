# Catalog

All skills in this repository.

All skills use semantic versioning. Users should check the repository for newer versions before re-importing.

| Skill | Folder | Version | Type | Description | Status |
|-------|--------|---------|------|-------------|--------|
| First Principles Decomposer | `first-principles-decomposer` | 0.1.1 | Text | Breaks complex problems down to fundamental truths and axioms before building back up. | Shipped |
| Pre-Mortem Analyzer | `pre-mortem-analyzer` | 0.1.1 | Text | Forces identification of failure modes and risks before committing to a plan or decision. | Shipped |
| Devil’s Advocate Simulator | `devils-advocate-simulator` | 0.1.1 | Text | Systematically attacks your current line of thinking to surface weaknesses, counterarguments, and blind spots. | Shipped |
| Assumption Challenger | `assumption-challenger` | 0.1.1 | Text | Identifies and stress-tests the hidden assumptions underlying a plan, belief, or analysis. | Shipped |
| Decision Framework Builder | `decision-framework-builder` | 0.1.1 | Text | Applies structured decision frameworks (criteria, weighting, scenarios, trade-off analysis) to important choices. | Shipped |
| Root Cause Analyzer | `root-cause-analyzer` | 0.1.1 | Text | Moves past symptoms to identify underlying systemic causes of problems. | Shipped |
| Goal to Atomic Action Decomposer | `goal-to-atomic-action-decomposer` | 0.1.1 | Text | Converts vague goals and intentions into concrete, smallest possible next actions with clear ownership and timing. | Shipped |
| Skill Update Reminder | `skill-update-reminder` | 0.1.1 | Text | Helps users understand how to update skills from this repo when newer versions are released. | Shipped |

**Status legend**

- Proposed: Prioritized for implementation. Not yet shipped.
- In Review: Implemented and being tested on-device.
- Shipped: Available and passes QUALITY-STANDARDS.

All skills include a `version` field (semver) in frontmatter. Because Google AI Edge Gallery caches imported skills locally, to get an updated version of a skill you must remove it from the app and re-add it using the raw URL.

Skills are added only after they have been tested on Gemma 4 E2B in Google AI Edge Gallery and meet the bar in QUALITY-STANDARDS.md.

All current skills are text-only (SKILL.md) and follow the Google AI Edge Gallery format for activation via name + description in the frontmatter.