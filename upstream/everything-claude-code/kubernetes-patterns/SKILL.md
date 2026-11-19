---
id: everything-claude-code__kubernetes-patterns
name: kubernetes-patterns
version: 1.0.0
description: >-
  Kubernetes workload patterns, resource management, RBAC, probes, autoscaling, ConfigMap/Secret handling, and kubectl debugging for production-grade deployments. Use when writing or reviewing Kubernetes manifests, or debugging probes, RBAC, autoscaling, resource limits, or pods that keep getting evicted.
role: kubernetes-patterns
category: ops
triggers:
  - kubernetes patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/kubernetes-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: kubernetes-patterns
---

# kubernetes-patterns

## Role

Portable distillation of upstream skill `kubernetes-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Kubernetes workload patterns, resource management, RBAC, probes, autoscaling, ConfigMap/Secret handling, and kubectl debugging for production-grade deployments. Use when writing or reviewing Kubernetes manifests, or debugging probes, RBAC, autoscaling, resource limits, or pods that keep getting evicted.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
