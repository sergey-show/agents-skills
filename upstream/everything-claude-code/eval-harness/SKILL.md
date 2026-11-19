---
id: everything-claude-code__eval-harness
name: eval-harness
version: 1.0.0
description: >-
  Formal evaluation framework for the coding agent sessions implementing eval-driven development (EDD) principles. Use when a the coding agent workflow needs a formal eval before it is trusted or changed.
role: eval-harness
category: meta
triggers:
  - eval harness
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/eval-harness/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: eval-harness
---

# eval-harness

## Role

Portable distillation of upstream skill `eval-harness` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Formal evaluation framework for the coding agent sessions implementing eval-driven development (EDD) principles. Use when a the coding agent workflow needs a formal eval before it is trusted or changed.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
