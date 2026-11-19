---
id: mattpocock-skills__implement-spec
name: implement-spec
version: 1.0.0
description: >-
  Implement the result of /to-spec and /to-tickets in code.
role: implement-spec
category: ops
triggers:
  - implement spec
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - subagent.spawn
  - test.run
sources:
  - research/skills/skills/engineering/implement-spec/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: implement-spec
---

# implement-spec

## Role

Portable distillation of upstream skill `implement-spec` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Implement the result of /to-spec and /to-tickets in code.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
