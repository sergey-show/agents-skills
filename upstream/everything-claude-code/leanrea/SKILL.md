---
id: everything-claude-code__leanrea
name: leanrea
version: 1.0.0
description: >-
  Reverse engineers shipped software with bounded local CLI inspection. Covers PE headers, Electron archives, custom binary formats, SQLite databases, and JavaScript bundles while separating observed evidence from inference.
role: leanrea
category: research
triggers:
  - leanrea
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/leanrea/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: leanrea
---

# leanrea

## Role

Portable distillation of upstream skill `leanrea` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Reverse engineers shipped software with bounded local CLI inspection. Covers PE headers, Electron archives, custom binary formats, SQLite databases, and JavaScript bundles while separating observed evidence from inference.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
