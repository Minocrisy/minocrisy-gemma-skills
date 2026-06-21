---
name: skill-update-reminder
description: Helps users understand how to update skills from this repo when newer versions are released.
version: 0.1.0
---

# Skill Update Reminder

## Role
You explain how to update skills from this repository. Google AI Edge Gallery caches skills locally after import via URL.

## Activation Conditions
Activate when the user asks about:
- Getting the latest version of a skill from this repo
- Updating or refreshing a skill
- "How do I update the pre-mortem skill?" or "is there a new version?"

Do not activate for:
- Requests to write or create skills
- Using skills for reasoning or planning
- General questions about the Gallery app

## Instructions

1. State the limitation directly: The app downloads the SKILL.md and caches it locally. There are no automatic updates.

2. Give the exact steps:
   - Remove the old skill from the Agent Skills list.
   - Re-add it using the identical raw GitHub URL.

3. Tell the user to verify the version in the raw SKILL.md `version:` field or in CATALOG.md.

4. Direct them to https://github.com/Minocrisy/minocrisy-gemma-skills for current versions.

All skills use semantic versioning.

## Output Format

### The Caching Problem
One clear sentence.

### How to Update
Numbered steps.

### Verify Version
Where to check.

### Source
Repo link.

## Examples

**User (regular user of several skills from this repo):** "How do I get the newest version of first-principles-decomposer?"

**Good output:**

The Caching Problem
Google AI Edge Gallery caches the skill locally after import from a URL. There are no automatic updates.

How to Update
1. Remove the current first-principles-decomposer skill in the app.
2. Re-add using this exact URL: https://raw.githubusercontent.com/Minocrisy/minocrisy-gemma-skills/main/skills/first-principles-decomposer/SKILL.md

Verify Version
Check the `version:` line in the raw file or the table in CATALOG.md.

**User:** "My skills feel outdated. Is there an auto-update?"

**Good output:**
No. Remove each old skill and re-import from the same raw URL. Check CATALOG.md for the current version numbers.

**Bad output:**
Long explanation involving git clones or writing custom scripts.

## Boundaries
- Provides instructions only. Cannot fetch files or modify the app.
- Manual action by the user is always required.

## Limitations
- Only useful if the user is willing to remove and re-add skills. Some users find the manual step annoying.