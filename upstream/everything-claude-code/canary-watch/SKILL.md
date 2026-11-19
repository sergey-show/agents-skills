---
id: everything-claude-code__canary-watch
name: canary-watch
version: 1.0.0
description: >-
  Monitors and verifies deployed URLs after releases by checking HTTP endpoints, SSE streams, static assets, console errors, and performance regressions after deploys, merges, or dependency upgrades. Smoke, canary, and post-deploy verification.
role: canary-watch
category: ops
triggers:
  - canary watch
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
sources:
  - research/everything-claude-code/skills/canary-watch/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: canary-watch
---

# canary-watch

## Role

Portable distillation of upstream skill `canary-watch` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Monitors and verifies deployed URLs after releases by checking HTTP endpoints, SSE streams, static assets, console errors, and performance regressions after deploys, merges, or dependency upgrades. Smoke, canary, and post-deploy verification.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
