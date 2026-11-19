---
id: everything-claude-code__uncloud
name: uncloud
version: 1.0.0
description: >-
  Use when managing an Uncloud cluster — deploying services, configuring Caddy ingress, adding static proxy routes for non-cluster devices, publishing ports, scaling, inspecting logs, or managing machines and volumes with the `uc` CLI.
role: uncloud
category: research
triggers:
  - uncloud
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/uncloud/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: uncloud
---

# uncloud

## Role

Portable distillation of upstream skill `uncloud` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when managing an Uncloud cluster — deploying services, configuring Caddy ingress, adding static proxy routes for non-cluster devices, publishing ports, scaling, inspecting logs, or managing machines and volumes with the `uc` CLI.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
