# Approaches — api-designer

Distilled from agent-skills api-and-interface-design, ECC api-design / backend-patterns.

## Resource design
- Nouns, plural, lowercase, kebab-case: `/api/v1/team-members`
- Sub-resources for ownership: `/users/:id/orders`
- Verbs sparingly for non-CRUD actions: `/orders/:id/cancel`
- BAD: `/getUsers`, singular `/user`, snake_case paths, verbs in nested resources

## Method semantics
| Method | Idempotent | Safe | Use |
|--------|------------|------|-----|
| GET | Yes | Yes | Retrieve |
| POST | No | No | Create / trigger |
| PUT | Yes | No | Full replace |
| PATCH | No* | No | Partial update |
| DELETE | Yes | No | Remove |

## Status codes
Success: 200, 201(+Location), 204. Client: 400, 401, 403, 404, 409, 422, 429. Server: 500 (no internal leak), 502, 503(+Retry-After).
**Never** wrap failures as HTTP 200 with `success:false`.

## Error envelope
Stable machine-readable code + human message + optional field errors; correlate with request id.

## Pagination / filtering
Cursor preferred for large sets; document sort stability; query params for filters not path verbs.

## Versioning
Explicit strategy (URL `/v1`, header, or none for truly internal-only with process). Breaking changes need migration plan (`migration-engineer`).

## Idempotency
Risky POSTs (payments, submits): idempotency keys; document replay behavior.

## Authz / tenancy
Every mutating and sensitive read path states authn + authz + tenant scope. Backend patterns: validate at boundary; never trust client tenancy ids without server check.

## Compatibility checklist
- Additive fields OK; renames/removals/type changes = break
- New required request fields = break unless defaulted
- Enum extensions: document unknown-value client behavior
