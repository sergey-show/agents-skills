---
id: everything-claude-code__mle-workflow
name: mle-workflow
version: 1.0.0
description: >-
  Production machine-learning engineering workflow for data contracts, reproducible training, model evaluation, deployment, monitoring, and rollback. Use when building, reviewing, or hardening ML systems beyond one-off notebooks.
role: mle-workflow
category: ops
triggers:
  - mle workflow
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/mle-workflow/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: mle-workflow
---

# mle-workflow

## Role

Portable distillation of upstream skill `mle-workflow` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Production machine-learning engineering workflow for data contracts, reproducible training, model evaluation, deployment, monitoring, and rollback. Use when building, reviewing, or hardening ML systems beyond one-off notebooks.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
