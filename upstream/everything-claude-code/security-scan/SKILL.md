---
id: everything-claude-code__security-scan
name: security-scan
version: 1.0.0
description: >-
  Scan your the coding agent configuration (.claude/ directory) for security vulnerabilities, misconfigurations, and injection risks using AgentShield. Checks CLAUDE.md, settings.json, MCP servers, hooks, and agent definitions. Use when auditing a .claude/ directory — CLAUDE.md, settings.json, MCP servers, hooks, or agent definitions.
role: security-scan
category: security
triggers:
  - security scan
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/security-scan/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: security-scan
---

# security-scan

## Role

Portable distillation of upstream skill `security-scan` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Scan your the coding agent configuration (.claude/ directory) for security vulnerabilities, misconfigurations, and injection risks using AgentShield. Checks CLAUDE.md, settings.json, MCP servers, hooks, and agent definitions. Use when auditing a .claude/ directory — CLAUDE.md, settings.json, MCP servers, hooks, or agent definitions.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
