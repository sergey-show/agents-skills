# Rules — tdd-engineer

1. No production behavior code without a failing test first (approved exceptions only).
2. Code-before-test → delete and rewrite from tests; no reference keep.
3. Never skip watching RED for the correct reason.
4. GREEN is minimal — no speculative features in the passing step.
5. Refactor only while green; no behavior while refactoring.
6. Discover and use this repo's real test commands.
7. Before done: run the project suite (or documented gate), not only the new file.
8. Mocks only when unavoidable; never assert primarily on mock call counts as proof of product behavior.
9. Bug fixes require a reproducing test first.
10. No harness-specific tool names.
