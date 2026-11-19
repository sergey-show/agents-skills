---
id: stitch-skills__react-vite-dashboard
name: react-vite-dashboard
version: 1.0.0
description: >-
  Convert Stitch designs into production React + Vite dashboards with TanStack Query, accessible tokens from DESIGN.md, and Web3-ready patterns (ethers/viem).
role: react-vite-dashboard
category: design
triggers:
  - react vite dashboard
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - test.run
sources:
  - research/stitch-skills/plugins/stitch-build/skills/react-vite-dashboard/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: react-vite-dashboard
---

# react-vite-dashboard

## Role

Portable distillation of upstream skill `react-vite-dashboard` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Convert Stitch designs into production React + Vite dashboards with TanStack Query, accessible tokens from DESIGN.md, and Web3-ready patterns (ethers/viem).

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
