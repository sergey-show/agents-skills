# Approaches — security-hunter

## Core hunting method (Cloudflare portable)

Work from a concrete invariant:
1. Name the lower-trust principal and starting capability.
2. Name the accepted value, action, state transition, or resource selector.
3. Locate the control that should reject, bind, isolate, limit, or revoke it.
4. Trace the exact source path after that decision.
5. Stop at the smallest affected dummy record, wrong return value, or locally observable shared-resource effect.
6. State a source-level change and regression case that enforce the invariant.

Read sibling/legacy/batch/retry/cancellation/migration/error paths that produce the same effect. Compare sibling controls for equivalence, not only presence.

## Sad paths & disagreements

Absent, empty, zero, negative, maximum, over-limit, duplicate, mixed encoding, stale, revoked, reordered, concurrent, partially migrated, failed dependency, rollback — only where the interface accepts them. Canonicalization mismatches at handoffs are high-yield.

## Depth bound

Trace only paths that can reach the assigned boundary or whose guarantees that boundary relies on. When settled, record disposition and stop.

## Variants

If a high/critical root cause appears, search lexical/structural/logical variants inside owned coverage IDs. Establish each variant's conditions independently. Peer units → `uncovered`, don't poach.

## Candidate gate

1. Complete repository-relative source trace including strongest source-visible control.
2. Proposed confirmed needs bounded local observed result (when execution allowed), meaningful impact across a stated boundary, complete conditions, no visible preventing layer.
3. Do not upgrade crashes→RCE, self-impact→shared avail, same-principal→priv-gain.
4. Missing decisive deploy/provider facts → `needs_validation` with exact blocker — no severity.

## Local execution

Only inside parent-approved sandbox: no external network, empty allowlisted env, read-only target, scratch writes only, resource limits. Else return needs_validation with the missing control. Prefer existing unit tests / minimal harnesses / dummy tenants. Stop at minimum boundary result.

## Priority order for units (when capped)

Unauthenticated/lowest trust → high-value resources → prior gaps/changed source → historical yield. Ties by stable coverage id.
