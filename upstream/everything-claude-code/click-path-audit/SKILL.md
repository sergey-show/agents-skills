---
id: everything-claude-code__click-path-audit
name: click-path-audit
version: 1.0.0
description: >-
  Trace every user-facing button/touchpoint through its full state change sequence to find bugs where functions individually work but cancel each other out, produce wrong final state, or leave the UI in an inconsistent state. Use when: systematic debugging found no bugs but users report broken buttons, or after any major refactor touching shared state stores.
role: click-path-audit
category: design
triggers:
  - click path audit
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/click-path-audit/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: click-path-audit
---

# click-path-audit

## Role

Portable distillation of upstream skill `click-path-audit` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Trace every user-facing button/touchpoint through its full state change sequence to find bugs where functions individually work but cancel each other out, produce wrong final state, or leave the UI in an inconsistent state. Use when: systematic debugging found no bugs but users report broken buttons, or after any major refactor touching shared state stores.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
