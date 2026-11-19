---
id: mattpocock-skills__chief-of-staff
name: chief-of-staff
version: 1.0.0
description: >-
  Pursue a long-running goal in a single session by co-ordinating subagents.
role: chief-of-staff
category: engineering
triggers:
  - chief of staff
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - subagent.spawn
  - test.run
sources:
  - research/skills/skills/in-progress/chief-of-staff/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: chief-of-staff
---

# chief-of-staff

## Role

Portable distillation of upstream skill `chief-of-staff` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Pursue a long-running goal in a single session by co-ordinating subagents.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
