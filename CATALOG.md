# Catalog

All skills in this repository.

All skills use semantic versioning. Users should check the repository for newer versions before re-importing.

| Skill | Folder | Version | Type | Description | Status |
|-------|--------|---------|------|-------------|--------|
| First Principles Decomposer | `first-principles-decomposer` | 0.1.1 | Text | Breaks complex problems down to fundamental truths and axioms before building back up. | Shipped - Tested & Validated |
| Pre-Mortem Analyzer | `pre-mortem-analyzer` | 0.1.1 | Text | Forces identification of failure modes and risks before committing to a plan or decision. | Shipped - Tested & Validated |
| Devil’s Advocate Simulator | `devils-advocate-simulator` | 0.1.1 | Text | Systematically attacks your current line of thinking to surface weaknesses, counterarguments, and blind spots. | Needs Improvement - Triggering issues |
| Assumption Challenger | `assumption-challenger` | 0.1.1 | Text | Identifies and stress-tests the hidden assumptions underlying a plan, belief, or analysis. | Shipped - Tested & Validated |
| Decision Framework Builder | `decision-framework-builder` | 0.1.1 | Text | Applies structured decision frameworks (criteria, weighting, scenarios, trade-off analysis) to important choices. | Shipped - Tested & Validated |
| Root Cause Analyzer | `root-cause-analyzer` | 0.1.1 | Text | Moves past symptoms to identify underlying systemic causes of problems. | Needs Improvement - Triggering issues |
| Goal to Atomic Action Decomposer | `goal-to-atomic-action-decomposer` | 0.1.1 | Text | Converts vague goals and intentions into concrete, smallest possible next actions with clear ownership and timing. | Shipped - Tested & Validated |
| Skill Update Reminder | `skill-update-reminder` | 0.1.1 | Text | Helps users understand how to update skills from this repo when newer versions are released. | Shipped |
| Skill Architect | `skill-architect` | 0.1.0 | Text | Creates new skills or modifies existing ones while strictly following minocrisy-gemma-skills quality standards. | Shipped |
| Local Decision Journal | `local-decision-journal` | 0.1.0 | Text | Save and retrieve important decisions with tagging, multi-tag search, and date range filtering. | Shipped |

**Status legend**

- Proposed: Prioritized for implementation. Not yet shipped.
- In Review: Implemented and being tested on-device.
- Shipped: Available and passes QUALITY-STANDARDS.
- Shipped - Tested & Validated: Tested on Gemma 4 E2B and performs strongly.
- Needs Improvement - Triggering issues: Failed to trigger reliably during initial device testing.

All skills include a `version` field (semver) in frontmatter. Because Google AI Edge Gallery caches imported skills locally, to get an updated version of a skill you must remove it from the app and re-add it using the raw URL.

Skills are added only after they have been tested on Gemma 4 E2B in Google AI Edge Gallery and meet the bar in QUALITY-STANDARDS.md.

All current skills are text-only (SKILL.md) and follow the Google AI Edge Gallery format for activation via name + description in the frontmatter.