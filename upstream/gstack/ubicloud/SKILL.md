---
id: gstack__ubicloud
name: ubicloud
version: 1.0.0
description: >-
  Run a heavy suite, build or eval on an ephemeral 16-vCPU Ubicloud VM: TTL-named VMs, a reaper, quota preflight and a hang watchdog. Use for: run on ubicloud, ubicloud vm, remote test run. (gstack)
role: ubicloud
category: meta
triggers:
  - ubicloud
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/ubicloud/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: ubicloud
---

# ubicloud

## Role

Portable distillation of upstream skill `ubicloud` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Run a heavy suite, build or eval on an ephemeral 16-vCPU Ubicloud VM: TTL-named VMs, a reaper, quota preflight and a hang watchdog. Use for: run on ubicloud, ubicloud vm, remote test run. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
