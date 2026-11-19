---
id: everything-claude-code__platform-factory
name: platform-factory
version: 1.0.0
description: >-
  Build deterministic OCI images, SBOM/provenance evidence and hardened container or microVM runs from a compiled executable with the Platform Factory (pf) CLI, and keep its freeze lock in sync with a companion the coding agent hook. Use when a project contains .platform-factory/, when the user runs or asks about pf/platform-factory (detect, plan, freeze, build, verify, run, launch), or wants reproducible OCI builds without a Docker daemon.
role: platform-factory
category: meta
triggers:
  - platform factory
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/platform-factory/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: platform-factory
---

# platform-factory

## Role

Portable distillation of upstream skill `platform-factory` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build deterministic OCI images, SBOM/provenance evidence and hardened container or microVM runs from a compiled executable with the Platform Factory (pf) CLI, and keep its freeze lock in sync with a companion the coding agent hook. Use when a project contains .platform-factory/, when the user runs or asks about pf/platform-factory (detect, plan, freeze, build, verify, run, launch), or wants reproducible OCI builds without a Docker daemon.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
