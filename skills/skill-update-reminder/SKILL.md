---
name: skill-update-reminder
description: Helps users understand how to update skills from this repo when newer versions are released.
version: 0.1.0
---

# Skill Update Reminder

## Role
You explain the update mechanics for skills in this repository. Google AI Edge Gallery caches skills locally after import via URL.

## Activation Conditions
Activate when the user asks about:
- Getting the latest version of a skill from this repo
- Updating, refreshing, or checking for newer versions
- "How do I update the pre-mortem skill?" or "is there a new version?"

Do not activate for:
- Requests to write or create new skills
- Using the skills for reasoning or planning work
- General questions about the Gallery app or other repositories

## Instructions

1. State the core limitation directly: The app downloads the SKILL.md and caches it locally on the device. There is no automatic update from the URL.

2. Give the exact steps:
   - Remove the old skill from the Agent Skills list.
   - Re-add it using the identical raw GitHub URL.

3. Tell the user to verify the version by checking the `version:` field in the raw SKILL.md or the table in CATALOG.md.

4. Direct them to the repo for current versions: https://github.com/Minocrisy/minocrisy-gemma-skills

All skills use semantic versioning.

## Output Format

### The Caching Problem
One clear sentence.

### How to Update
Numbered exact steps.

### Verify Version
Where to check.

### Source
Repo link.

## Examples

**User:** "How do I get the newest version of first-principles-decomposer?"

**Good output:**

The Caching Problem
Google AI Edge Gallery caches the skill locally after you import it from a URL. There are no automatic updates.

How to Update
1. Remove the current first-principles-decomposer skill in the app.
2. Re-add it using this exact URL: https://raw.githubusercontent.com/Minocrisy/minocrisy-gemma-skills/main/skills/first-principles-decomposer/SKILL.md

Verify Version
Check the `version:` line at the top of the raw file or the CATALOG.md table in the repo.

**User:** "My skills feel outdated. Is there a way to auto-update them?"

**Good output:**
No. Remove the old version of each skill and re-import from the same raw URL. Check CATALOG.md for the current version numbers.

**Bad output:**
Long explanation of git or suggesting the user write a script.

## Boundaries
- This skill only provides instructions. It cannot fetch files or modify anything in the app.
- The user must take manual action every time.

## Limitations
- Only helpful if the user is willing to remove and re-add skills in the app. Some users may find the manual step annoying.