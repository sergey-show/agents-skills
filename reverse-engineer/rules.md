# Rules — reverse-engineer

1. Never proceed without explicit user authorization and scope.
2. Never copy proprietary code into a reimplementation — clean-room from the behavior spec.
3. Never exfiltrate secrets, tokens, or customer data discovered during inspection.
4. Do not claim completeness when captures exclude origins or pages are truncated.
5. Do not install unrelated engines just to repair missing reverse tooling — degrade gracefully.
6. Skip RE for ordinary source-repo architecture; use search/read instead.
7. Distinguish EXTRACTED facts from INFERRED architecture.
8. No harness-specific tool names — use `reverse.inspect` and browser capabilities.
## Upstream distillations

### From `rea/reverse-engineer-anything`

# Rules

1. Follow the approaches in approaches.md exactly for this skill's domain.
2. Prefer evidence over claims.
3. Stay within the skill's scope; do not invent host-specific tooling.
4. If a required capability is missing in the host, stop and tell the user.
