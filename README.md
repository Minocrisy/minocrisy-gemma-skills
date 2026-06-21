# minocrisy-gemma-skills

High-signal Agent Skills for Gemma 4 E2B in Google AI Edge Gallery.

Private, offline cognitive tools for people who already have strong cloud models (Grok, Gemini, Claude, etc.) and want sharp, reliable thinking tools that never leave the device.

## The Point

Cloud models are excellent. They are also not private.

Gemma 4 E2B on-device is fast, capable, and local. It is weaker than frontier cloud models at raw knowledge and breadth. It becomes dramatically more useful when given precise, high-leverage instruction sets that activate only when needed.

This repo exists to provide exactly that: focused, truth-seeking skills for real reasoning, planning, and decision work.

## Philosophy

- Direct, not diplomatic. Minimal hedging.
- High leverage over broad coverage.
- High signal-to-noise. No corporate language, no motivational fluff.
- Progressive disclosure: the model sees only name + description until the skill is relevant.
- Designed to complement cloud tools, not replace them.
- Tested on actual hardware with Gemma 4 E2B before shipping.

If a skill does not meaningfully improve private serious work, it does not belong here.

## Initial Skills

The first batch focuses on core reasoning and decision tools:

- [First Principles Decomposer](skills/first-principles-decomposer/SKILL.md)
- [Pre-Mortem Analyzer](skills/pre-mortem-analyzer/SKILL.md)
- [Devil’s Advocate Simulator](skills/devils-advocate-simulator/SKILL.md)
- [Assumption Challenger](skills/assumption-challenger/SKILL.md)
- [Decision Framework Builder](skills/decision-framework-builder/SKILL.md)
- [Root Cause Analyzer](skills/root-cause-analyzer/SKILL.md)
- [Goal to Atomic Action Decomposer](skills/goal-to-atomic-action-decomposer/SKILL.md)

See [CATALOG.md](CATALOG.md) for the full list and status.

## Installation

1. Open Google AI Edge Gallery on iOS or Android.
2. Select the Agent Skills section.
3. Tap to add a custom skill.
4. Paste the raw URL to a `SKILL.md` file, or download the file and import locally.

Skills live at:

```
https://raw.githubusercontent.com/Minocrisy/minocrisy-gemma-skills/main/skills/<skill-name>/SKILL.md
```

## Repository Layout

- `skills/` — Individual skills. One kebab-case folder per skill. Text skills contain only `SKILL.md`.
- `CATALOG.md` — Scannable index of all skills.
- `QUALITY-STANDARDS.md` — Strict criteria for inclusion.
- `CONTRIBUTING.md` — Process for adding skills.

## License

Apache-2.0

See [LICENSE](LICENSE).
