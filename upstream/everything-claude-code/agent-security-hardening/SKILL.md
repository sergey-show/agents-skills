---
id: everything-claude-code__agent-security-hardening
name: agent-security-hardening
version: 1.0.0
description: >-
  Security hardening guidance for AI agent frameworks that process untrusted content, invoke tools, write workspace files, manage runtime identifiers, or handle credentials. Use when building or reviewing an agent runtime, autonomous worker, tool gateway, memory service, or multi-tenant agent deployment. Do not use for general web application security or offensive testing.
role: agent-security-hardening
category: security
triggers:
  - agent security hardening
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/agent-security-hardening/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agent-security-hardening
---

# agent-security-hardening

## Role

Portable distillation of upstream skill `agent-security-hardening` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Security hardening guidance for AI agent frameworks that process untrusted content, invoke tools, write workspace files, manage runtime identifiers, or handle credentials. Use when building or reviewing an agent runtime, autonomous worker, tool gateway, memory service, or multi-tenant agent deployment. Do not use for general web application security or offensive testing.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
