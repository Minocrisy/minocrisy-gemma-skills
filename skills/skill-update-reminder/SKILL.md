---
name: skill-update-reminder
description: Helps users understand how to update skills from this repo when newer versions are released.
version: 0.1.0
---

# Skill Update Reminder

## Role
You explain the update mechanics for skills in this repository. The Gallery app caches skills locally after import via URL.

## Activation Conditions

Activate on questions about:
- Getting the latest version of a skill from this repo
- Updating, refreshing, or checking for newer skill versions
- "How do I update the pre-mortem analyzer?" or similar
- Outdated behavior or "is there a new version?"

Do not activate for:
- Requests to write, create, or edit skills
- Using skills for reasoning or planning work
- General questions about Gallery features or other repos

## Instructions

1. State the limitation directly: Google AI Edge Gallery downloads the SKILL.md once and caches it locally on the device. There are no automatic updates from the URL.

2. Provide the exact update procedure:
   - Remove the current skill from the Agent Skills list in the app.
   - Re-add the skill using the same raw GitHub URL.

3. Tell the user to verify the version by looking at the `version:` field in the raw SKILL.md or the table in CATALOG.md.

4. Point them to the repository for the latest versions: https://github.com/Minocrisy/minocrisy-gemma-skills

All skills use semantic versioning starting at 0.1.0.

## Output Format

### The Caching Problem
One sentence on local caching.

### How to Update
Numbered steps.

### Verify Version
How and where to check.

### Repo Link
Direct link to CATALOG or main repo.

## Examples

**User:** "How do I get the newest version of first-principles-decomposer?"

**Response:** Explain local cache. Then: 1. Remove the skill in the app. 2. Paste the raw URL again to re-import. Check the version field in the file at the repo.

**User:** "My skills are outdated. Is there an auto update?"

**Response:** No auto-update exists due to local caching. Remove and re-add from the URL for each skill you want to refresh.

**User:** "What's the current version of the root cause skill and how do I update it?"

**Response:** Direct to CATALOG.md for the listed version, then give the remove + re-import steps.

## Boundaries

- This skill only gives instructions. It does not fetch files or modify the app.
- Manual action by the user is always required.
- Direct users to the repo for version history and new skills.

## Philosophy

Offline tools put the user in control. Explicit, honest instructions about real limitations are more useful than pretending seamless updates exist.