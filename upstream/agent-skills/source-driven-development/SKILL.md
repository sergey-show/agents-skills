---
id: agent-skills__source-driven-development
name: source-driven-development
version: 1.0.0
description: >-
  Grounds every implementation decision in official documentation. Use when you want to verify an approach against the official docs before implementing it, or when you want authoritative, source-cited code free from outdated patterns. Use when building with any framework or library where correctness matters.
role: source-driven-development
category: meta
triggers:
  - source driven development
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
sources:
  - research/agent-skills/skills/source-driven-development/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: source-driven-development
---

# source-driven-development

## Role

Portable distillation of upstream skill `source-driven-development` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Grounds every implementation decision in official documentation. Use when you want to verify an approach against the official docs before implementing it, or when you want authoritative, source-cited code free from outdated patterns. Use when building with any framework or library where correctness matters.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
