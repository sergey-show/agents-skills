---
id: superpowers__diagnosing-superpowers
name: diagnosing-superpowers
version: 1.0.0
description: >-
  Use when a superpowers session went wrong and your human partner wants to know why — repeated work, ignored plans, stumbles, poor results, a skill that didn't fire, "it took too long", "why is it so expensive", "what is it doing" — or wants to build a bug report for the superpowers maintainers, for the current session or a past one identified by id or path, on any harness.
role: diagnosing-superpowers
category: meta
triggers:
  - diagnosing superpowers
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - subagent.spawn
sources:
  - research/superpowers/skills/diagnosing-superpowers/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: diagnosing-superpowers
---

# diagnosing-superpowers

## Role

Portable distillation of upstream skill `diagnosing-superpowers` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when a superpowers session went wrong and your human partner wants to know why — repeated work, ignored plans, stumbles, poor results, a skill that didn't fire, "it took too long", "why is it so expensive", "what is it doing" — or wants to build a bug report for the superpowers maintainers, for the current session or a past one identified by id or path, on any harness.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
