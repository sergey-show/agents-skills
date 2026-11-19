---
id: loopforge__devflow
name: devflow
version: 1.0.0
description: >-
  在用户明确要求结构化、可恢复、多阶段的软件交付流程，或要求按 devflow 继续已有任务时使用。覆盖任务分级、需求、设计、计划、实现、设计稿还原、代码审查、测试、固定产物归档、知识沉淀和预览部署；适用于不同 Agent、语言、框架和仓库。普通的一次性小改、单独问答或无需流程编排的代码操作不应仅因属于软件开发而自动触发。
role: devflow
category: meta
triggers:
  - devflow
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/LoopForge/local/skills/devflow/SKILL.md
harness: any
upstream_repo: LoopForge
upstream_skill: devflow
---

# devflow

## Role

Portable distillation of upstream skill `devflow` from `LoopForge`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

在用户明确要求结构化、可恢复、多阶段的软件交付流程，或要求按 devflow 继续已有任务时使用。覆盖任务分级、需求、设计、计划、实现、设计稿还原、代码审查、测试、固定产物归档、知识沉淀和预览部署；适用于不同 Agent、语言、框架和仓库。普通的一次性小改、单独问答或无需流程编排的代码操作不应仅因属于软件开发而自动触发。

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
