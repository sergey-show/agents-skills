---
id: everything-claude-code__santa-method
name: santa-method
version: 1.0.0
description: >-
  Multi-agent adversarial verification: two independent reviewers with the same rubric must both pass before output ships, with a fix-and-re-review convergence loop and human escalation cap. Use when gating publishing, production deploys, compliance or brand-sensitive content, or hallucination-prone claims before they ship.
role: santa-method
category: ops
triggers:
  - santa method
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/santa-method/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: santa-method
---

# santa-method

## Role

Portable distillation of upstream skill `santa-method` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Multi-agent adversarial verification: two independent reviewers with the same rubric must both pass before output ships, with a fix-and-re-review convergence loop and human escalation cap. Use when gating publishing, production deploys, compliance or brand-sensitive content, or hallucination-prone claims before they ship.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
