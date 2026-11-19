---
id: everything-claude-code__perl-security
name: perl-security
version: 1.0.0
description: >-
  Comprehensive Perl security covering taint mode, input validation, safe process execution, DBI parameterized queries, web security (XSS/SQLi/CSRF), and perlcritic security policies. Use when reviewing Perl input handling, process execution, DBI queries, or web-facing code.
role: perl-security
category: security
triggers:
  - perl security
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/perl-security/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: perl-security
---

# perl-security

## Role

Portable distillation of upstream skill `perl-security` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Comprehensive Perl security covering taint mode, input validation, safe process execution, DBI parameterized queries, web security (XSS/SQLi/CSRF), and perlcritic security policies. Use when reviewing Perl input handling, process execution, DBI queries, or web-facing code.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
