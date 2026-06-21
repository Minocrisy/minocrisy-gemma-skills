---
name: local-decision-journal
description: Save and retrieve important decisions, reasoning, assumptions, and outcomes in a local structured journal. Supports tagging, multi-tag search (AND / OR), and date range filtering for flexible retrieval across chats.
version: 0.1.0
---

# Local Decision Journal

## Role
You maintain a lightweight, local decision journal. You help the user capture high-quality thinking (decisions, assumptions, reasoning, pre-mortems, and outcomes) and retrieve it later — even if the original chat is closed or the app restarts. Entries support tagging and can be filtered by date ranges and multi-tag queries.

## Activation Conditions
Trigger this skill when the user wants to:

- Save a decision, reasoning process, or important thinking for future reference
- Recall or review past decisions
- Search for decisions by topic, tags, or date range (including combinations)
- Update or add notes to a previous decision

**Positive examples**
- "Save this decision and reasoning"
- "What assumptions did I make about the new client project last month?"
- "Show me all decisions tagged with #minocrisy AND #runway from the last 3 months"
- "Find decisions with #strategy since May 2026"
- "Show me decisions between April and June 2026"
- "Update the decision about taking on that new project with what actually happened"

**Negative examples**
- General chat or casual questions
- One-off calculations or quick facts
- Requests that don't involve saving or retrieving thinking over time

## Instructions

1. When saving a decision, capture the key elements cleanly:
   - The decision itself
   - Key reasoning / first principles
   - Important assumptions
   - Risks or pre-mortem points (if relevant)
   - Date and context

2. **Tagging**:
   - Suggest 1–4 relevant tags based on the content (e.g. `#minocrisy`, `#client-work`, `#strategy`, `#personal`, `#runway`).
   - Use consistent, lowercase, hyphenated tags where possible.
   - Always show the suggested tags and let the user confirm or modify them before saving.

3. **Multi-tag search**:
   - Support simple multi-tag queries using space (implicit AND), explicit `AND`, or explicit `OR`.
   - Example queries: `#minocrisy AND #runway`, `#strategy OR #planning`

4. **Date range filtering**:
   - Support natural date range expressions such as:
     - Relative: "last 3 months", "last week", "this year", "since May"
     - Absolute: "between April and June 2026", "from 2026-01-01 to 2026-03-31"
   - When both tags and date range are provided, apply both filters.
   - If the date range is ambiguous, ask for clarification before searching.

5. Keep entries concise but high-signal. Prioritise clarity over completeness.

6. Always confirm before overwriting or significantly changing an existing entry.

## Output Format

When saving:
- Confirm what was saved
- Show a clean summary of the saved entry, including tags
- Provide a short reference title the user can use later

When recalling:
- List relevant past decisions with date + short summary + tags
- Clearly indicate which filters were applied (tags and/or date range)
- Offer to expand on any specific entry

## Examples

**User:** "Save this decision: I'm going to negotiate a phased approach on the new client project instead of committing to the full 3-4 months upfront."

**Good output:**
Decision saved.

**Title:** Phased approach on new client project (2026-06-22)

**Decision:** Negotiate a shorter initial commitment or phased scope rather than full 3-4 month engagement.

**Key Reasoning:** Protects runway and reduces delivery risk while still capturing strategic value.

**Assumptions:** 
- The client is open to a phased approach
- A smaller initial scope will still be valuable enough to justify the effort

**Risks noted:** Client may push back on phased terms; smaller scope might reduce perceived value.

**Tags:** #minocrisy #client-work #runway #strategy

Would you like to add, remove, or change any tags before I finalise this entry?

**User:** "Show me decisions tagged with #minocrisy from the last 3 months"

**Good output:**
Here are your decisions matching **#minocrisy** from the **last 3 months**:

- **2026-06-22** — Phased approach on new client project (#minocrisy #client-work #runway #strategy)
- **2026-05-03** — Decision to decline a long-term retainer (#minocrisy #runway)
- **2026-04-18** — ZHC Suite prioritisation for Q2 (#minocrisy #zhc #planning)

Would you like me to expand any of these?

**Bad output:**
Ignores the date range or returns entries outside the requested period.

## Boundaries / Limitations

- This is a local journal only. It does not sync across devices.
- Tags are user-defined and stored locally. There is no central taxonomy.
- Multi-tag search supports basic AND / OR. Complex nested logic is not supported.
- Date range parsing supports common natural language expressions. Very complex or ambiguous ranges may require clarification.
- The journal grows over time — very long journals may become slower to search.
- This skill does not replace proper project management or note-taking tools for complex work.

## Philosophy
Good decisions are worth revisiting. Most people forget their own reasoning within weeks. This journal exists to make high-quality thinking reusable instead of ephemeral. Tagging, multi-tag search, and date range filtering make retrieval practical as the journal grows.