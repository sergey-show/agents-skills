---
id: agent-skills__code-simplification
name: code-simplification
version: 1.0.0
description: >-
  Simplifies code for clarity. Use when refactoring code for clarity without changing behavior. Use when code works but is harder to read, maintain, or extend than it should be. Use when reviewing code that has accumulated unnecessary complexity. Use when asked to simplify, clean up, or reduce the nesting of a function or module that already works, even when the code is pasted inline and nothing else needs to change.
role: code-simplification
category: meta
triggers:
  - code simplification
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - test.run
sources:
  - research/agent-skills/skills/code-simplification/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: code-simplification
---

# code-simplification

## Role

Portable distillation of upstream skill `code-simplification` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Simplifies code for clarity. Use when refactoring code for clarity without changing behavior. Use when code works but is harder to read, maintain, or extend than it should be. Use when reviewing code that has accumulated unnecessary complexity. Use when asked to simplify, clean up, or reduce the nesting of a function or module that already works, even when the code is pasted inline and nothing else needs to change.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
