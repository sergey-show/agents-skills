---
id: agent-skills__documentation-and-adrs
name: documentation-and-adrs
version: 1.0.0
description: >-
  Records decisions and documentation, and detects when documentation has drifted from the code it describes. Use when you need to document an architecture decision (ADR) or the reasoning behind a design choice, when changing public APIs, shipping features, when docs may be stale or out of sync with the code they describe, when working out which module docs are still accurate, or when setting up a check so docs cannot silently go out of date again.
role: documentation-and-adrs
category: engineering
triggers:
  - documentation and adrs
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/documentation-and-adrs/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: documentation-and-adrs
---

# documentation-and-adrs

## Role

Portable distillation of upstream skill `documentation-and-adrs` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Records decisions and documentation, and detects when documentation has drifted from the code it describes. Use when you need to document an architecture decision (ADR) or the reasoning behind a design choice, when changing public APIs, shipping features, when docs may be stale or out of sync with the code they describe, when working out which module docs are still accurate, or when setting up a check so docs cannot silently go out of date again.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
