---
id: mattpocock-skills__triage
name: triage
version: 1.0.0
description: >-
  Move issues and external PRs through a state machine of triage roles, categorise, verify, grill if needed, and write agent-ready briefs.
role: triage
category: engineering
triggers:
  - triage
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/skills/skills/engineering/triage/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: triage
---

# triage

## Role

Portable distillation of upstream skill `triage` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Move issues and external PRs through a state machine of triage roles, categorise, verify, grill if needed, and write agent-ready briefs.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
