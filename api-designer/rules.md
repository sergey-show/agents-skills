# Rules — api-designer

1. Follow in-repo API conventions when they exist; don't invent a second style.
2. Never use HTTP 200 for application failures.
3. State compatibility impact of every contract change.
4. Document error codes and pagination before implementation handoff.
5. Authz/tenancy requirements are part of the contract, not an afterthought.
6. Prefer additive evolution; breaking changes require migration notes.
7. Examples required for happy path and at least one error path.
8. No harness-specific tool names.
