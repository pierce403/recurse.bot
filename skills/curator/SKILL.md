---
name: curator
description: Maintain a compact, useful skill library by recognizing when lessons should become new skills, updating skills when tools or workflows change, consolidating overlapping skills, and pruning stale skills. Use when Codex learns a reusable procedure, changes project guidance, notices duplicated skills, or finishes meaningful work that should improve future agent behavior.
---

# Curator

## Overview

Use this skill to keep procedural knowledge useful over time. Curator follows the Hermes pattern: it treats skills as a small library of class-level procedures, not a growing pile of session-specific notes.

## Workflow

1. Review the task outcome.
   Identify what was learned, what changed, and whether future agents would benefit from procedural guidance.

2. Choose the right destination.
   Put broad facts, project observations, and collaborator preferences in memory or `AGENTS.md`. Put repeatable task procedures in `SKILLS.md` and `skills/<name>/SKILL.md`.

3. Prefer updating before creating.
   Search `SKILLS.md` and `skills/` for an existing class-level skill that can absorb the new lesson. Patch that skill when the new material fits.

4. Create a new skill only for a stable workflow.
   A new skill should have a clear trigger, reusable procedure, and a name that describes a durable class of work. Avoid names tied to a single issue, branch, date, run, or person unless the workflow truly requires it.

5. Consolidate overlapping skills.
   When several narrow skills describe the same kind of work, merge their durable lessons into one umbrella skill with labeled sections, then remove or archive the redundant entries.

6. Prune stale guidance.
   Remove or archive a skill when its workflow is obsolete, unused, or fully absorbed elsewhere. Preserve non-obsolete lessons in the destination skill before pruning.

7. Keep the index current.
   Every skill creation, consolidation, rename, or prune should update `SKILLS.md`. If the public guide or support docs describe the affected pattern, update `index.html`, `README.md`, `FEATURES.md`, and `AGENTS.md` together.

## Skill Shape

- Use lowercase hyphenated names.
- Keep `SKILL.md` focused on procedural instructions.
- Add `references/`, `templates/`, `scripts/`, or `assets/` only when the skill needs them.
- Keep root `SKILLS.md` as a compact catalog, not a second copy of each skill.
- Record both positive and negative learnings when they change how the skill should behave.

## Done Criteria

- The skill library has no obvious duplicate or obsolete guidance for the task just completed.
- New reusable procedure is captured in an existing or new skill.
- `SKILLS.md` points to every live skill and does not point to removed skills.
- Supporting docs stay aligned when the public pattern changes.
