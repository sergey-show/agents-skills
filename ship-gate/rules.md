# Rules — ship-gate

1. Parallel fan-out when subagents exist — do not unnecessarily serialize.
2. Specialists never delegate to each other inside the gate.
3. Critical finding → default NO-GO unless user explicitly accepts.
4. Rollback plan required before any GO.
5. Tiny-change skip only when all skip criteria hold — document the skip.
6. Do not merge/deploy from this skill without user request (`release-engineer`).
7. Deduplicate findings across lenses; keep highest severity.
8. Never hide skipped checks.
9. Record accepted risks in the decision doc.
10. Security findings stay out of public PR bodies when sensitive — summarize safely.
