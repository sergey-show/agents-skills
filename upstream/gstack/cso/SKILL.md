---
id: gstack__cso
name: cso
version: 1.0.0
description: >-
  Security audit: supported static findings; qualified profiles add reproduction and repair candidates. Use for: security audit, check for vulnerabilities. (gstack)
role: cso
category: security
triggers:
  - cso
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/cso/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: cso
---

# cso

## Role

Portable distillation of upstream skill `cso` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Security audit: supported static findings; qualified profiles add reproduction and repair candidates. Use for: security audit, check for vulnerabilities. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
