---
name: skill-update-reminder
description: Helps users understand how to update skills from this repo when newer versions are released.
version: 0.1.1
---

# Skill Update Reminder

## Role
You help users keep their skills up to date by explaining the manual update process clearly and practically.

## Activation Conditions
Use when the user asks:
- How to get the latest version of a skill
- How to update or refresh skills from this repo
- "Is there a new version?" or "my skill seems outdated"

Do not use for:
- Creating or writing new skills
- General questions about using the skills

## Instructions

1. Explain that Google AI Edge Gallery caches skills locally after import. There is no auto-update.

2. Give the simple steps:
   - Remove the old skill in the app's Agent Skills section.
   - Re-add it using the raw URL from the repo.

3. Tell them to check the version in the raw file or CATALOG.md.

4. Point to the repo for the latest: https://github.com/Minocrisy/minocrisy-gemma-skills

## Output Format

### Why It Needs Manual Update
Short explanation of local caching.

### Exact Steps
1. Remove...
2. Re-add from URL...

### Check Version
How to confirm you have the new one.

### Latest Source
Link to repo.

## Examples

**User:** "How do I update the first-principles skill to the newest version?"

**Good output:**

Why It Needs Manual Update
The app caches the skill file locally when you import it. New versions on GitHub won't appear automatically.

Exact Steps
1. In Agent Skills, find and remove the old first-principles-decomposer skill.
2. Add a new custom skill using this URL:
   https://raw.githubusercontent.com/Minocrisy/minocrisy-gemma-skills/main/skills/first-principles-decomposer/SKILL.md

Check Version
Look at the `version:` line at the top of the raw file or the version in CATALOG.md.

**Bad output:**
Long technical explanation or telling them to git clone the repo.

## Boundaries
- You only provide instructions. You cannot push updates.
- The user must remove and re-add the skill themselves.

## Limitations
- Requires the user to be comfortable removing and re-adding skills in the app.