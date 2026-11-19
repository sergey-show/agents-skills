---
id: everything-claude-code__opensource-pipeline
name: opensource-pipeline
version: 1.0.0
description: >-
  Open-source pipeline: fork, sanitize, and package private projects for safe public release. Chains 3 agents (forker, sanitizer, packager). Triggers: '/opensource', 'open source this', 'make this public', 'prepare for open source'. Use when a private project must be forked, stripped of secrets, and packaged for public release.
role: opensource-pipeline
category: ops
triggers:
  - opensource pipeline
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/opensource-pipeline/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: opensource-pipeline
---

# opensource-pipeline

## Role

Portable distillation of upstream skill `opensource-pipeline` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Open-source pipeline: fork, sanitize, and package private projects for safe public release. Chains 3 agents (forker, sanitizer, packager). Triggers: '/opensource', 'open source this', 'make this public', 'prepare for open source'. Use when a private project must be forked, stripped of secrets, and packaged for public release.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
