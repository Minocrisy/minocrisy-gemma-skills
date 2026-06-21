# minocrisy-gemma-skills

> **High-signal Agent Skills for Gemma 4 E2B** — Private, offline tools for serious thinking.

[![Gemma 4 E2B](https://img.shields.io/badge/Gemma_4-E2B-4285F4?style=flat&logo=google)](https://ai.google.dev/gemma)
[![Text Skills](https://img.shields.io/badge/Type-Text_Only-34A853?style=flat)](https://github.com/Minocrisy/minocrisy-gemma-skills)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue?style=flat)](LICENSE)
[![Tested](https://img.shields.io/badge/Tested-Gemma_4_E2B-brightgreen?style=flat)](CATALOG.md)

Private, offline cognitive tools for people who already have strong cloud models (Grok, Gemini, Claude, etc.) and want sharp, reliable thinking tools that never leave the device.

<p align="center">
  <strong>Built for truth-seeking. Designed for real work.</strong>
</p>

## The Point

Cloud models are excellent. They are also not private.

Gemma 4 E2B on-device is fast, capable, and local. It is weaker than frontier cloud models at raw knowledge and breadth. It becomes dramatically more useful when given precise, high-leverage instruction sets that activate only when needed.

This repo exists to provide exactly that: focused, truth-seeking skills for real reasoning, planning, and decision work.

## Philosophy

- **Direct, not diplomatic.** Minimal hedging.
- **High leverage** over broad coverage.
- **High signal-to-noise.** No corporate language, no motivational fluff.
- **Progressive disclosure:** the model sees only name + description until the skill is relevant.
- Designed to **complement** cloud tools, not replace them.
- Tested on actual hardware with Gemma 4 E2B before shipping.

If a skill does not meaningfully improve private serious work, it does not belong here.

## Current Status

- **Strong / tested on device:** decision-framework-builder, first-principles-decomposer, pre-mortem-analyzer, assumption-challenger, goal-to-atomic-action-decomposer
- **Needs improvement (triggering):** root-cause-analyzer, devils-advocate-simulator
- **Meta skills:** skill-architect (new), skill-update-reminder
- **New:** Local Decision Journal — local memory + tagging, multi-tag search, and date range filtering

See [CATALOG.md](CATALOG.md) for per-skill details and status.

## Featured Skills

| Skill | Use Case | Key Feature |\n|-------|----------|-------------|\n| [First Principles Decomposer](skills/first-principles-decomposer/SKILL.md) | Break down complex problems to fundamentals | Strong for high-stakes analysis |
| [Pre-Mortem Analyzer](skills/pre-mortem-analyzer/SKILL.md) | Identify risks before committing | Prospective failure simulation |
| [Decision Framework Builder](skills/decision-framework-builder/SKILL.md) | Structure important choices | Weighted criteria + sensitivity |
| [Local Decision Journal](skills/local-decision-journal/SKILL.md) | Capture & retrieve decisions over time | Tagging + date range + AND/OR search |
| [Skill Architect](skills/skill-architect/SKILL.md) | Create or improve skills | Enforces repo quality standards |

## Installation

1. Open **Google AI Edge Gallery** on iOS or Android.
2. Go to **Agent Skills**.
3. Tap **+** to add a custom skill.
4. Paste the raw URL:

```
https://raw.githubusercontent.com/Minocrisy/minocrisy-gemma-skills/main/skills/<skill-name>/SKILL.md
```

**Example for Local Decision Journal:**
```
https://raw.githubusercontent.com/Minocrisy/minocrisy-gemma-skills/main/skills/local-decision-journal/SKILL.md
```

## Keeping Skills Updated

Google AI Edge Gallery caches skills locally. To get updates:

1. Remove the old skill in the app.
2. Re-add using the same raw URL.

Check the `version:` in the raw file or [CATALOG.md](CATALOG.md).

See the [Skill Update Reminder](skills/skill-update-reminder/SKILL.md) for in-app help.

## Repository Layout

- `skills/` — One kebab-case folder per skill (Text-only `SKILL.md`)
- `CATALOG.md` — Full index with status & versions
- `QUALITY-STANDARDS.md` — Strict rules for what ships
- `CONTRIBUTING.md` — How to add high-quality skills

## License

Apache-2.0 — See [LICENSE](LICENSE).

---

<p align="center">
  <sub>Truth-seeking tools. Zero fluff. Built for the edge.</sub>
</p>
