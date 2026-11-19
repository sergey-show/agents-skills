---
id: everything-claude-code__terraform-patterns
name: terraform-patterns
version: 1.0.0
description: >-
  Terraform and OpenTofu infrastructure-as-code patterns for project layout, remote state, modules, variables, secrets, safe plan/apply workflows, and CI. Use when writing or reviewing .tf files, structuring modules or environments, configuring backends and state locking, or debugging plan drift, state, and provider errors.
role: terraform-patterns
category: engineering
triggers:
  - terraform patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/terraform-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: terraform-patterns
---

# terraform-patterns

## Role

Portable distillation of upstream skill `terraform-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Terraform and OpenTofu infrastructure-as-code patterns for project layout, remote state, modules, variables, secrets, safe plan/apply workflows, and CI. Use when writing or reviewing .tf files, structuring modules or environments, configuring backends and state locking, or debugging plan drift, state, and provider errors.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
