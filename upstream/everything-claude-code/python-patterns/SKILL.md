---
id: everything-claude-code__python-patterns
name: python-patterns
version: 1.0.0
description: >-
  Pythonic idioms, PEP 8 standards, type hints, and best practices for building robust, efficient, and maintainable Python applications. Use when writing or reviewing Python code and idiomatic structure, typing, or PEP 8 is in question.
role: python-patterns
category: design
triggers:
  - python patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/python-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: python-patterns
---

# python-patterns

## Role

Portable distillation of upstream skill `python-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Pythonic idioms, PEP 8 standards, type hints, and best practices for building robust, efficient, and maintainable Python applications. Use when writing or reviewing Python code and idiomatic structure, typing, or PEP 8 is in question.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
