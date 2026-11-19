---
id: mattpocock-skills__ask-matt
name: ask-matt
version: 1.0.0
description: >-
  Ask which skill or flow fits your situation. A router over the skills in this repo.
role: ask-matt
category: ops
triggers:
  - ask matt
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/skills/skills/engineering/ask-matt/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: ask-matt
---

# ask-matt

## Role

Portable distillation of upstream skill `ask-matt` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Ask which skill or flow fits your situation. A router over the skills in this repo.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
