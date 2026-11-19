---
id: everything-claude-code__ecc-contribution-review
name: ecc-contribution-review
version: 1.0.0
description: >-
  Prepare an ECC skill contribution for review by organizing repository, install-surface, cross-harness, validation, security, and commit observations into a local proposal. Use when preparing a skill contribution for review.
role: ecc-contribution-review
category: meta
triggers:
  - ecc contribution review
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/ecc-contribution-review/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ecc-contribution-review
---

# ecc-contribution-review

## Role

Portable distillation of upstream skill `ecc-contribution-review` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Prepare an ECC skill contribution for review by organizing repository, install-surface, cross-harness, validation, security, and commit observations into a local proposal. Use when preparing a skill contribution for review.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
