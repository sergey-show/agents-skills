---
id: loopforge__devflow-clarify-requirements
name: devflow-clarify-requirements
version: 1.0.0
description: >-
  在技术设计前澄清软件交付需求，解决重要产品决策、隐含假设、范围边界、成功标准和未决分支。用于 DevFlow medium/large 的 REQUIREMENT 阶段，或功能请求过于模糊、无法安全设计时。只询问无法从项目证据中回答的问题；不实现、不提交、不写技术方案，也不调用计划类 skill。
role: devflow-clarify-requirements
category: engineering
triggers:
  - devflow clarify requirements
capabilities_required:
  - filesystem.read
capabilities_optional:
  - ask_user
sources:
  - research/LoopForge/local/skills/devflow-clarify-requirements/SKILL.md
harness: any
upstream_repo: LoopForge
upstream_skill: devflow-clarify-requirements
---

# devflow-clarify-requirements

## Role

Portable distillation of upstream skill `devflow-clarify-requirements` from `LoopForge`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

在技术设计前澄清软件交付需求，解决重要产品决策、隐含假设、范围边界、成功标准和未决分支。用于 DevFlow medium/large 的 REQUIREMENT 阶段，或功能请求过于模糊、无法安全设计时。只询问无法从项目证据中回答的问题；不实现、不提交、不写技术方案，也不调用计划类 skill。

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
