---
id: agent-reach__agent-reach
name: agent-reach
version: 1.0.0
description: >-
  只读读取各平台内容：搜索、读帖、看评论、取字幕、查行情和职位。 Use when 用户提到或贴出链接：小红书/xiaohongshu、B站/bilibili、Twitter/X、Reddit、 YouTube（字幕、转录）、GitHub、V2EX、雪球/股票行情、LinkedIn/Boss直聘 职位、 Instagram、Facebook、小宇宙播客；或说"帮我搜/看看/读一下这个链接"而自带网页搜索/读取不可用、失败或拿不到正文； 或要安装、加上/去掉某个平台、登录/退出、看状态、更新、卸载 Agent Reach。 不做：发帖、评论、点赞、私信等任何写操作；不替用户登录、不索要密码。 公开内容优先用 Agent 自带工具，Reach 补缺口。
role: agent-reach
category: research
triggers:
  - agent reach
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/Agent-Reach/agent_reach/skill/SKILL.md
harness: any
upstream_repo: Agent-Reach
upstream_skill: agent-reach
---

# agent-reach

## Role

Portable distillation of upstream skill `agent-reach` from `Agent-Reach`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

只读读取各平台内容：搜索、读帖、看评论、取字幕、查行情和职位。 Use when 用户提到或贴出链接：小红书/xiaohongshu、B站/bilibili、Twitter/X、Reddit、 YouTube（字幕、转录）、GitHub、V2EX、雪球/股票行情、LinkedIn/Boss直聘 职位、 Instagram、Facebook、小宇宙播客；或说"帮我搜/看看/读一下这个链接"而自带网页搜索/读取不可用、失败或拿不到正文； 或要安装、加上/去掉某个平台、登录/退出、看状态、更新、卸载 Agent Reach。 不做：发帖、评论、点赞、私信等任何写操作；不替用户登录、不索要密码。 公开内容优先用 Agent 自带工具，Reach 补缺口。

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
