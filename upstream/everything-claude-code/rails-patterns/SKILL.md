---
id: everything-claude-code__rails-patterns
name: rails-patterns
version: 1.0.0
description: >-
  Ruby on Rails framework patterns for Rails 7.1+ and 8.x apps. Covers the directory contract, skinny controllers with service objects, form objects, query objects, idiomatic ActiveRecord, background jobs, ViewComponent, Hotwire, and the Rails 8 Solid stack. Use when building or reviewing Rails apps, controllers, models, services, jobs, or views.
role: rails-patterns
category: design
triggers:
  - rails patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/rails-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: rails-patterns
---

# rails-patterns

## Role

Portable distillation of upstream skill `rails-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Ruby on Rails framework patterns for Rails 7.1+ and 8.x apps. Covers the directory contract, skinny controllers with service objects, form objects, query objects, idiomatic ActiveRecord, background jobs, ViewComponent, Hotwire, and the Rails 8 Solid stack. Use when building or reviewing Rails apps, controllers, models, services, jobs, or views.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
