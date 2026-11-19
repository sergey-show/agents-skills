---
id: everything-claude-code__ai-regression-testing
name: ai-regression-testing
version: 1.0.0
description: >-
  Regression testing strategies for AI-assisted development. Sandbox-mode API testing without database dependencies, automated bug-check workflows, and patterns to catch AI blind spots where the same model writes and reviews code. Use when adding regression coverage to AI-assisted code, or when the same model both wrote and reviewed a change.
role: ai-regression-testing
category: design
triggers:
  - ai regression testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/ai-regression-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ai-regression-testing
---

# ai-regression-testing

## Role

Portable distillation of upstream skill `ai-regression-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Regression testing strategies for AI-assisted development. Sandbox-mode API testing without database dependencies, automated bug-check workflows, and patterns to catch AI blind spots where the same model writes and reviews code. Use when adding regression coverage to AI-assisted code, or when the same model both wrote and reviewed a change.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
