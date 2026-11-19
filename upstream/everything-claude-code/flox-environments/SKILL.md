---
id: everything-claude-code__flox-environments
name: flox-environments
version: 1.0.0
description: >-
  Create reproducible, cross-platform (macOS/Linux) development environments with Flox, a declarative Nix-based environment manager. Use when setting up project toolchains, installing system-level dependencies (compilers, databases, native libs), pinning exact package versions for a team, onboarding developers, running local services (PostgreSQL, Redis, Kafka), or solving 'works on my machine' problems — including agent/vibe-coding setups that need project-scoped tools without sudo. Also use when the user mentions .flox/, manifest.toml, flox activate, or FloxHub.
role: flox-environments
category: meta
triggers:
  - flox environments
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/flox-environments/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: flox-environments
---

# flox-environments

## Role

Portable distillation of upstream skill `flox-environments` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Create reproducible, cross-platform (macOS/Linux) development environments with Flox, a declarative Nix-based environment manager. Use when setting up project toolchains, installing system-level dependencies (compilers, databases, native libs), pinning exact package versions for a team, onboarding developers, running local services (PostgreSQL, Redis, Kafka), or solving 'works on my machine' problems — including agent/vibe-coding setups that need project-scoped tools without sudo. Also use when the user mentions .flox/, manifest.toml, flox activate, or FloxHub.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
