---
id: everything-claude-code__cpp-coding-standards
name: cpp-coding-standards
version: 1.0.0
description: >-
  C++ coding standards based on the C++ Core Guidelines (isocpp.github.io). Use when writing, reviewing, or refactoring C++ code to enforce modern, safe, and idiomatic practices.
role: cpp-coding-standards
category: engineering
triggers:
  - cpp coding standards
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/cpp-coding-standards/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: cpp-coding-standards
---

# cpp-coding-standards

## Role

Portable distillation of upstream skill `cpp-coding-standards` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

C++ coding standards based on the C++ Core Guidelines (isocpp.github.io). Use when writing, reviewing, or refactoring C++ code to enforce modern, safe, and idiomatic practices.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
