---
id: everything-claude-code__security-bounty-hunter
name: security-bounty-hunter
version: 1.0.0
description: >-
  Hunt for exploitable, bounty-worthy security issues in repositories. Focuses on remotely reachable vulnerabilities that qualify for real reports instead of noisy local-only findings. Use when hunting reportable, remotely reachable vulnerabilities in a repository.
role: security-bounty-hunter
category: security
triggers:
  - security bounty hunter
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/security-bounty-hunter/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: security-bounty-hunter
---

# security-bounty-hunter

## Role

Portable distillation of upstream skill `security-bounty-hunter` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Hunt for exploitable, bounty-worthy security issues in repositories. Focuses on remotely reachable vulnerabilities that qualify for real reports instead of noisy local-only findings. Use when hunting reportable, remotely reachable vulnerabilities in a repository.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
