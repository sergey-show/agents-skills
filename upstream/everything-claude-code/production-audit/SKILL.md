---
id: everything-claude-code__production-audit
name: production-audit
version: 1.0.0
description: >-
  Local-evidence production readiness audit for shipped apps, pre-launch reviews, post-merge checks, and "what breaks in prod?" questions without sending repo data to an external audit service. Use when auditing production readiness before launch, after a merge, or when asked what breaks in prod.
role: production-audit
category: ops
triggers:
  - production audit
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/production-audit/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: production-audit
---

# production-audit

## Role

Portable distillation of upstream skill `production-audit` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Local-evidence production readiness audit for shipped apps, pre-launch reviews, post-merge checks, and "what breaks in prod?" questions without sending repo data to an external audit service. Use when auditing production readiness before launch, after a merge, or when asked what breaks in prod.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
