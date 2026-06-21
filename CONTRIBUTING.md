# Contributing

We want fewer, better skills.

## Before You Start

1. Read [QUALITY-STANDARDS.md](QUALITY-STANDARDS.md) in full. This is non-negotiable.
2. Ask: does this tool create meaningful leverage for private, serious thinking work on a small on-device model?

## Process

1. Open an issue describing the proposed skill and why it meets the standards.
2. Or fork and implement directly if you are confident.
3. Create a folder under `skills/` using kebab-case. The folder name must match the `name` in frontmatter.
4. Add only `SKILL.md` for text skills (current focus).
5. Write clear frontmatter, activation conditions, examples, and boundaries.
6. Test the skill thoroughly in Google AI Edge Gallery with Gemma 4 E2B.
7. Update `CATALOG.md`.
8. Submit a PR.

## PR Requirements

- Link to the raw SKILL.md (for easy import testing).
- Include notes from on-device testing with E2B (specific prompts tried, observed behaviour, any tweaks needed).
- Confirm it passes every item in QUALITY-STANDARDS.md.

Low-quality or untested contributions will be closed without merge.

## Style

Match the tone of existing skills: direct, structured, zero fluff.
