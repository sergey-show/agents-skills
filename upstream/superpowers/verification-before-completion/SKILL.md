---
id: superpowers__verification-before-completion
name: verification-before-completion
version: 1.0.0
description: >-
  Use when about to claim work is complete, fixed, or passing, before committing or creating PRs - requires running verification commands and confirming output before making any success claims; evidence before assertions always
role: verification-before-completion
category: engineering
triggers:
  - verification before completion
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/superpowers/skills/verification-before-completion/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: verification-before-completion
---

# verification-before-completion

## Role

Portable distillation of upstream skill `verification-before-completion` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when about to claim work is complete, fixed, or passing, before committing or creating PRs - requires running verification commands and confirming output before making any success claims; evidence before assertions always

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
