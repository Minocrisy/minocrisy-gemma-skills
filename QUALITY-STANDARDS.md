# Quality Standards

This repository maintains a deliberately high bar. Most prompt collections and "agent skills" fail these criteria.

## Mandatory Requirements

1. **Genuinely useful for serious private thinking work**
   - Targets reasoning, planning, decision making, diagnosis, decomposition, or risk analysis.
   - A competent practitioner should feel the difference when using it repeatedly.
   - Not entertainment, not generic life advice, not toy examples.

2. **Follows progressive disclosure**
   - `name` and `description` in frontmatter are the activation surface.
   - Full instructions load only when the model decides the skill is relevant.
   - The model must not be burdened with heavy instructions for every query.
   - `version` is metadata for users to track updates (Gallery caches locally; re-import URL to get new version).

3. **Clear, reliable activation conditions**
   - The description must be specific enough for Gemma 4 E2B to trigger correctly and not trigger constantly.
   - Document positive and negative trigger examples in the skill.

4. **Good examples and expected behaviour documented**
   - Include 2–4 concrete examples of usage.
   - Show what good output looks like (structure, depth, tone).
   - State what the skill deliberately avoids.

5. **Tested on actual Gemma 4 E2B in Google AI Edge Gallery**
   - Author must have loaded the skill in the app and run real scenarios on the E2B model (E4B acceptable if E2B not practical).
   - Note any model-specific quirks, phrasing sensitivities, or recommended prompt styles.
   - "It looks good in simulation" is not sufficient.

6. **Strict anti-fluff, high signal-to-noise**
   - Direct language. Short sentences. Concrete steps.
   - No corporate platitudes, excessive hedging, motivational language, or decorative emojis.
   - Every sentence should earn its place.

7. **Consistent format**
   - Folder name exactly matches `name:` in frontmatter.
   - Frontmatter uses exactly:
     ```
     ---
     name: example-name
     description: One precise sentence describing capability and trigger conditions.
     version: 0.1.0
     ---
     ```
   - Body is well-structured Markdown (sections, numbered steps, clear output formats).

8. **Explicit boundaries**
   - State what the skill is not.
   - Note cases where the user should use a stronger model, consult a human expert, or gather more data.

## What Gets Rejected

- Vague or overly broad descriptions that cause constant or never triggering.
- Skills that mostly restate generic good thinking without adding structure or leverage.
- Untested skills or skills tested only against larger cloud models.
- Fluffy language or low-density prose.
- Skills that duplicate existing high-quality skills without clear improvement.
- Missing or invalid `version` field (use semver).

If in doubt, do not add it.
