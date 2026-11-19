# Approaches — eng-architect

Distilled from gstack plan-eng-review, agent-skills api-and-interface-design, ECC api-design / backend-patterns. Host preambles, telemetry, and path helpers stripped.

## Scope gate (first)
Fix one target before discovery:
- A) Branch diff (work in progress)
- B) Plan / design doc (paste or path) — prefer when already in plan mode with an active plan
- C) Specific file/directory

Clarify ambiguous targets. Announce auto-selected plan in one line.

## Evidence policy
| Target | Evidence |
|--------|----------|
| Plan/design | Proposed paths checked against existing interfaces and tests |
| Branch diff | Changed behavior + surrounding code from entry points |
| Path | Existing behavior + callers/tests |

Implementation steps in a plan are proposals — calibrate findings by quoting the motivating requirement. Bounded probes of **current** behavior OK; do not build the proposed feature during review unless user authorizes.

Retrospective: git log / revert greps on relevant paths for recurring issues.

## Review sections (walk in order)
1. **Boundaries and modules** — ownership, coupling, circular deps, seam quality
2. **Data flow (happy path)** — ingress → processing → storage → egress
3. **State machines / lifecycles** — legal transitions; idempotency
4. **Error paths and retries** — timeouts, partial failure, poison messages
5. **Consistency / migrations** — transactions, dual-write, backfill, expand/contract
6. **Security & tenancy** — authn/z, trust boundaries, PII, isolation
7. **Performance budgets** — expected load, N+1, hot paths, caching
8. **API / interface contracts** — compatibility, versioning, error shapes (see `api-designer`)
9. **Test matrix** — unit/integration/e2e; what each layer proves; gaps in Review Focus
10. **Rollout / rollback** — flags, shadow, migration reverse, monitoring signals
11. **Open assumptions** — listed with owners / how to falsify

## Confidence calibration
Every finding: severity CRITICAL (blocks ship) or INFORMATIONAL; confidence 1–10.
- 9–10: verified by reading specific code / demonstrated bug
- 7–8: high-confidence pattern
- 5–6: medium — caveat "verify"
- 3–4: appendix only
- 1–2: speculation — only if potential catastrophe, marked speculative

**Format:** `[CRITICAL|INFORMATIONAL] (confidence: N/10) path:line — description`

### Pre-emit gate
Quote the specific line that motivates the finding. If you cannot quote it, do not emit as verified.

## API / backend patterns to enforce in plans
- Resources as nouns; correct method semantics and status codes
- Explicit pagination/filtering contracts
- Stable error envelope; never HTTP 200 for application failures
- Idempotency keys for risky POSTs where needed
- Authz checks at the right layer; tenancy on every query
- Migrations: expand/contract; no unreviewed destructive DDL with app cutover in one step

## Output
Prefer **amending the existing plan** with a decision ledger and accepted remedies. Keep diagrams ASCII/mermaid in-repo. Separate working plan / findings / final structured report sections.

## Outside / adversarial lens
Before closing, steelman the top risk: what would a skeptical staff engineer say is most likely to page someone? Address or accept explicitly.
