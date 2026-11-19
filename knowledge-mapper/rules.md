# Rules — knowledge-mapper

1. Do not claim a relationship without an evidence pointer (file/line or doc anchor).
2. Keep artifacts deterministic enough to regenerate.
3. Prefer incremental updates over full rebuilds when possible.
4. Never dump the entire graph into chat — summarize and link.
5. Query-first: if a graph artifact already exists, answer from it before rebuilding or grepping the whole tree.
6. Tag edges honestly: EXTRACTED / INFERRED / AMBIGUOUS — never invent confident links.
7. Code structure prefers deterministic AST extraction; reserve LLM semantics for docs/ambiguity.
8. Never ask for API keys to unblock a code-only graph; structural extraction needs none.
9. On oversized corpora, ask which subfolder before expensive semantic work.
10. No harness-specific tool names — declare capabilities only.
## Upstream distillations

### From `graphify/graphify`

# Rules (extracted)

- Never invent an edge. If unsure, use AMBIGUOUS.
- Never skip the corpus check warning.
- Always show token cost in the report.
- Never hide cohesion scores behind symbols - show the raw number.
- Never run HTML viz on a graph with more than 5,000 nodes without warning the user.
