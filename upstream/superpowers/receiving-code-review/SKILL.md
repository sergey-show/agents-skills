---
id: superpowers__receiving-code-review
name: receiving-code-review
version: 1.0.0
description: >-
  Use when receiving code review feedback, before implementing suggestions, especially if feedback seems unclear or technically questionable - requires technical rigor and verification, not performative agreement or blind implementation
role: receiving-code-review
category: meta
triggers:
  - receiving code review
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/superpowers/skills/receiving-code-review/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: receiving-code-review
---

# receiving-code-review

## Role

Portable distillation of upstream skill `receiving-code-review` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when receiving code review feedback, before implementing suggestions, especially if feedback seems unclear or technically questionable - requires technical rigor and verification, not performative agreement or blind implementation

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
