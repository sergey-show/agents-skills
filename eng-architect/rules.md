# Rules — eng-architect

1. Fix the review target before deep analysis; do not silently switch targets.
2. Do not implement the proposed feature during plan review unless the user explicitly authorizes building.
3. Every CRITICAL/INFORMATIONAL finding needs severity, confidence, and a quoted motivating line when claiming verification.
4. Confidence ≤4 stays in appendix (unless speculative catastrophe).
5. Prefer amending the working plan over writing a disconnected essay.
6. List assumptions and how to falsify them; unmarked assumptions are defects.
7. Plans without error paths, authz/tenancy, or rollout/rollback for stateful/multi-tenant systems are incomplete.
8. API contracts in the plan must specify compatibility stance (break vs compatible).
9. Test matrix must say what each test layer proves — "add tests" is not a matrix.
10. Honor write permissions; if report cannot be persisted, present full review as not-persisted and continue.
11. No harness-specific tool names or telemetry rituals in the DoT core.
