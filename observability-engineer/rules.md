# Rules — observability-engineer

1. No instrumentation without named on-call questions.
2. Prefer structured events over prose logs.
3. Propagate correlation/request IDs across boundaries.
4. Never log secrets or sensitive PII.
5. Avoid high-cardinality metric labels.
6. Follow existing observability stack in-repo; don't add a second vendor casually.
7. Alerts require owner + runbook or they are noise.
8. No harness-specific tool names.
