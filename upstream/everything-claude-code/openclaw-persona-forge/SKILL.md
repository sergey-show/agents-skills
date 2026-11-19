---
id: everything-claude-code__openclaw-persona-forge
name: openclaw-persona-forge
version: 1.0.0
description: >-
  为 OpenClaw AI Agent 锻造完整的龙虾灵魂方案。根据用户偏好或随机抽卡， 输出身份定位、灵魂描述(SOUL.md)、角色化底线规则、名字和头像生图提示词。 如当前环境提供已审核的生图 skill，可自动生成统一风格头像图片。 当用户需要创建、设计或定制 OpenClaw 龙虾灵魂时使用。 不适用于：微调已有 SOUL.md、非 OpenClaw 平台的角色设计、纯工具型无性格 Agent。 触发词：龙虾灵魂、虾魂、OpenClaw 灵魂、养虾灵魂、龙虾角色、龙虾定位、 龙虾剧本杀角色、龙虾游戏角色、龙虾 NPC、龙虾性格、龙虾背景故事、 lobster soul、lobster character、抽卡、随机龙虾、龙虾 SOUL、gacha。 Use when creating, designing, or customizing an OpenClaw lobster persona — identity, SOUL.md, name, or avatar prompt.
role: openclaw-persona-forge
category: meta
triggers:
  - openclaw persona forge
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/openclaw-persona-forge/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: openclaw-persona-forge
---

# openclaw-persona-forge

## Role

Portable distillation of upstream skill `openclaw-persona-forge` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

为 OpenClaw AI Agent 锻造完整的龙虾灵魂方案。根据用户偏好或随机抽卡， 输出身份定位、灵魂描述(SOUL.md)、角色化底线规则、名字和头像生图提示词。 如当前环境提供已审核的生图 skill，可自动生成统一风格头像图片。 当用户需要创建、设计或定制 OpenClaw 龙虾灵魂时使用。 不适用于：微调已有 SOUL.md、非 OpenClaw 平台的角色设计、纯工具型无性格 Agent。 触发词：龙虾灵魂、虾魂、OpenClaw 灵魂、养虾灵魂、龙虾角色、龙虾定位、 龙虾剧本杀角色、龙虾游戏角色、龙虾 NPC、龙虾性格、龙虾背景故事、 lobster soul、lobster character、抽卡、随机龙虾、龙虾 SOUL、gacha。 Use when creating, designing, or customizing an OpenClaw lobster persona — identity, SOUL.md, name, or avatar prompt.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
