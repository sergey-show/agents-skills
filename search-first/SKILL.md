---
id: search-first
name: Search First
version: 1.0.0
description: >-
  Research-before-coding workflow: search the repo, package registries, skills, MCP capability catalogs, and public code before writing custom utilities. Use when starting a feature, adding a dependency, or about to invent something that may already exist.
role: Reuse Scout
category: engineering
triggers:
  - search first
  - reuse before invent
  - is there a package
  - existing solution
  - don't reinvent
capabilities_required:
  - search.code
  - filesystem.read
capabilities_optional:
  - search.web
  - search.docs
  - shell.exec
  - ask_user
  - subagent.spawn
sources:
  - research/everything-claude-code
harness: any
---

# Search First

## Role

You systematize reuse-before-invent. Report which channels you actually checked.

## When to use

New feature, dependency, integration, or utility that might already exist in-repo or upstream.

## Workflow

1. Preflight: which search channels are available? Skip and label missing ones honestly.
2. Need analysis: functionality + language/framework constraints.
3. Parallel search: repo → package registries → skills/capabilities → public code/docs.
4. Evaluate: functionality, maintenance, community, docs, license, deps.
5. Decide: Adopt / Extend / Compose / Build — then implement the minimum.

## Done when

Decision recorded with candidates checked and why; custom code only if justified.

## See also

- [tools.md](tools.md) · [approaches.md](approaches.md) · [rules.md](rules.md)
- Related: `minimal-coder`, `skill-author`

## Upstream depth

- `skills/upstream/everything-claude-code/documentation-lookup/`
- `skills/upstream/mattpocock-skills/research/`
- `skills/upstream/ponytail/ponytail/`
