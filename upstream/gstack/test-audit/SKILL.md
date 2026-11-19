---
id: gstack__test-audit
name: test-audit
version: 1.0.0
description: >-
  Find low-value or duplicate tests and the test-only code they keep alive. Use for: audit the test suite, find low-value tests. (gstack)
role: test-audit
category: meta
triggers:
  - test audit
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/test-audit/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: test-audit
---

# test-audit

## Role

Portable distillation of upstream skill `test-audit` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Find low-value or duplicate tests and the test-only code they keep alive. Use for: audit the test suite, find low-value tests. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
