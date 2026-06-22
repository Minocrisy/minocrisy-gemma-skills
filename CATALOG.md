# Catalog

> All skills in this repository — built for **Gemma 4 E2B** in Google AI Edge Gallery

All skills use semantic versioning. Users should check the repository for newer versions before re-importing.

## Core Reasoning

| Skill | Folder | Version | Description | Status |
|-------|--------|---------|-------------|--------|
| First Principles Decomposer | `first-principles-decomposer` | 0.1.1 | Breaks complex problems down to fundamental truths and axioms before building back up. | Tested & Validated |
| Assumption Challenger | `assumption-challenger` | 0.1.1 | Identifies and stress-tests the hidden assumptions underlying a plan, belief, or analysis. | Tested & Validated |
| Root Cause Analyzer | `root-cause-analyzer` | 0.1.1 | Moves past symptoms to identify underlying systemic causes of problems. | Needs Improvement |

## Planning & Risk

| Skill | Folder | Version | Description | Status |
|-------|--------|---------|-------------|--------|
| Pre-Mortem Analyzer | `pre-mortem-analyzer` | 0.1.1 | Forces identification of failure modes and risks before committing to a plan or decision. | Tested & Validated |
| Devil’s Advocate Simulator | `devils-advocate-simulator` | 0.1.1 | Systematically attacks your current line of thinking to surface weaknesses, counterarguments, and blind spots. | Needs Improvement |

## Decision & Execution

| Skill | Folder | Version | Description | Status |
|-------|--------|---------|-------------|--------|
| Decision Framework Builder | `decision-framework-builder` | 0.1.1 | Applies structured decision frameworks (criteria, weighting, scenarios, trade-off analysis) to important choices. | Tested & Validated |
| Goal to Atomic Action Decomposer | `goal-to-atomic-action-decomposer` | 0.1.1 | Converts vague goals and intentions into concrete, smallest possible next actions with clear ownership and timing. | Tested & Validated |
| Local Decision Journal | `local-decision-journal` | 0.1.0 | Save and retrieve important decisions with tagging, multi-tag search, and date range filtering. | Shipped |

## Meta Tools

| Skill | Folder | Version | Description | Status |
|-------|--------|---------|-------------|--------|
| Skill Architect | `skill-architect` | 0.1.0 | Creates new skills or modifies existing ones while strictly following minocrisy-gemma-skills quality standards. | Shipped |
| Skill Update Reminder | `skill-update-reminder` | 0.1.1 | Helps users understand how to update skills from this repo when newer versions are released. | Shipped |

## Status Legend

- **Tested & Validated**: Loaded and evaluated on Gemma 4 E2B in Google AI Edge Gallery. Performs reliably and delivers clear leverage.
- **Shipped**: Meets QUALITY-STANDARDS.md. Available for use.
- **Needs Improvement**: Triggering or output quality issues observed during device testing. Retained for visibility while work continues.
- **Proposed / In Review**: Not yet present in this catalog.

---

All skills include a `version` field (semver) in frontmatter. Because Google AI Edge Gallery caches imported skills locally, to get an updated version of a skill you must remove it from the app and re-add it using the raw URL.

Skills are added only after they have been tested on Gemma 4 E2B in Google AI Edge Gallery and meet the bar in [QUALITY-STANDARDS.md](QUALITY-STANDARDS.md).

All current skills are **text-only** (`SKILL.md`) and follow the Google AI Edge Gallery format for activation via name + description in the frontmatter.
