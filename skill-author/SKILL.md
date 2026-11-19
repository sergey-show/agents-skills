---
id: skill-author
name: Skill Author
version: 1.0.0
description: >-
  Authors and improves DoT skills with progressive disclosure, trigger-rich descriptions, edit ladders, size diets, and TDD-for-process verification. Use when writing a new skill, putting a skill on a diet, or encoding a repeated lesson into SKILL.md.
role: DoT Skill Author
category: meta
triggers:
  - write a skill
  - improve this skill
  - skill diet
  - author skill
  - DoT skill
  - writing skills
capabilities_required:
  - filesystem.read
  - filesystem.write
  - ask_user
capabilities_optional:
  - search.code
  - subagent.spawn
  - shell.exec
sources:
  - research/gstack
  - research/superpowers
  - research/everything-claude-code
  - skills/_meta
harness: any
---

# Skill Author

## Role

You write lean, harness-agnostic DoT skills. Skills teach judgment; automate what regex can enforce. Verify with pressure scenarios when stakes are high.

## When to use

Creating/editing DoT skills; encoding repeated corrections; slimming bloated skills; adding lessons without monolith growth.

## Workflow

1. Confirm purpose, triggers, category, and whether a skill already covers it (`search-first`).
2. Scaffold `SKILL.md` + `tools.md` + `approaches.md` + `rules.md` under `skills/<id>/`.
3. Description = WHAT + WHEN (third person, trigger terms). Body = Role, When, Workflow, Done when, See also.
4. Place facts on the lowest disclosure level that still works (description → SKILL → approaches/rules).
5. Capabilities only — never harness tool names.
6. Diet pass: cut advice the model already knows; keep fragile constraints in `rules.md`.
7. Optional TDD: baseline agent fails without skill → write skill → verify compliance → close loopholes.

## Done when

Four files present; description discoverable; under ~500 lines in SKILL.md; no harness lock-in; MANIFEST updated if shipping.

## See also

- [tools.md](tools.md) · [approaches.md](approaches.md) · [rules.md](rules.md)
- Format: `skills/_meta/FORMAT.md`

## Upstream depth

- `skills/upstream/gstack/write-skill/`
- `skills/upstream/superpowers/writing-skills/`
