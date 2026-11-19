---
id: mattpocock-skills__diagnosing-bugs
name: diagnosing-bugs
version: 1.0.0
description: >-
  Diagnosis loop for hard bugs and performance regressions. Use when the user says "diagnose"/"debug this", or reports something broken/throwing/failing/slow.
role: diagnosing-bugs
category: meta
triggers:
  - diagnosing bugs
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/skills/skills/engineering/diagnosing-bugs/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: diagnosing-bugs
---

# diagnosing-bugs

## Role

Portable distillation of upstream skill `diagnosing-bugs` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Diagnosis loop for hard bugs and performance regressions. Use when the user says "diagnose"/"debug this", or reports something broken/throwing/failing/slow.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
