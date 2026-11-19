---
id: agent-skills__frontend-ui-engineering
name: frontend-ui-engineering
version: 1.0.0
description: >-
  Builds production-quality, accessible, responsive user-facing UIs. Use when building or modifying interfaces and pages, creating components, implementing layouts, meeting WCAG accessibility requirements, managing state, or when the output needs to look and feel production-quality rather than AI-generated.
role: frontend-ui-engineering
category: design
triggers:
  - frontend ui engineering
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/frontend-ui-engineering/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: frontend-ui-engineering
---

# frontend-ui-engineering

## Role

Portable distillation of upstream skill `frontend-ui-engineering` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Builds production-quality, accessible, responsive user-facing UIs. Use when building or modifying interfaces and pages, creating components, implementing layouts, meeting WCAG accessibility requirements, managing state, or when the output needs to look and feel production-quality rather than AI-generated.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
