---
id: impeccable__audit
name: audit
version: 1.0.0
description: >-
  a user-authored audit skill
role: audit
category: design
triggers:
  - audit
capabilities_required:
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/impeccable/tests/oracle/workspaces/ctx-pin/.claude/skills/audit/SKILL.md
harness: any
upstream_repo: impeccable
upstream_skill: audit
---

# audit

## Role

Portable distillation of upstream skill `audit` from `impeccable`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

a user-authored audit skill

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
