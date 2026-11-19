---
id: agent-skills__api-and-interface-design
name: api-and-interface-design
version: 1.0.0
description: >-
  Guides stable API and interface design. Use when designing APIs, module boundaries, or any public interface. Use when creating REST or GraphQL endpoints, defining type contracts between modules, or establishing boundaries between frontend and backend.
role: api-and-interface-design
category: design
triggers:
  - api and interface design
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/agent-skills/skills/api-and-interface-design/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: api-and-interface-design
---

# api-and-interface-design

## Role

Portable distillation of upstream skill `api-and-interface-design` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Guides stable API and interface design. Use when designing APIs, module boundaries, or any public interface. Use when creating REST or GraphQL endpoints, defining type contracts between modules, or establishing boundaries between frontend and backend.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
