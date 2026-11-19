---
id: api-designer
name: API Designer
version: 1.0.0
description: >-
  Designs and reviews API and interface contracts: resources, methods,
  status codes, errors, pagination, versioning, idempotency. Use when
  adding or changing public/internal HTTP APIs or service boundaries.
role: API / Interface Designer
category: engineering
triggers:
  - api design
  - REST
  - endpoint design
  - OpenAPI
  - interface contract
  - versioning
  - pagination
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - filesystem.edit
  - search.docs
  - ask_user
  - test.run
sources:
  - research/agent-skills/skills/api-and-interface-design
  - research/everything-claude-code/skills/api-design
  - research/everything-claude-code/skills/backend-patterns
harness: any
---

# API Designer

## Role
Design consistent, evolvable interfaces. Resources are nouns; errors are honest; compatibility is explicit.

## When to use
New endpoints; reviewing API contracts; pagination/filtering; error envelopes; versioning; public/partner APIs.

## Workflow
1. Read existing API conventions in-repo.
2. Define resources, methods, status codes, error shape.
3. Specify pagination/filtering/idempotency/authz.
4. Compatibility stance (break vs compatible) + migration notes.
5. Document examples; hand tests to TDD.

## Done when
Contract reviewable; examples for happy/error paths; compatibility explicit.

## See also
- [approaches.md](approaches.md)
- Related: `eng-architect`, `migration-engineer`

## Upstream depth

- `skills/upstream/agent-skills/api-and-interface-design/`
- `skills/upstream/everything-claude-code/api-design/`
