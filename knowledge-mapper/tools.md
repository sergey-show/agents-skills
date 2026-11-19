# Tools — knowledge-mapper

## Required
- `filesystem.read` / `search.code` / `filesystem.list` — detect corpus and extract structure
- `filesystem.write` — graph JSON, GRAPH_REPORT, wiki/index artifacts

## Optional
- `graph.build` — Graphify or equivalent graph pipeline when installed
- `shell.exec` — run graph CLI / detectors
- `subagent.spawn` — parallel semantic extraction on docs/papers
- `ask_user` — narrow oversized corpora

## Artifact layout (portable)
- `graphify-out/graph.json` (or project `knowledge-graph.json`)
- `GRAPH_REPORT.md` — hubs, orphans, communities, risks
- Optional: HTML viz, GraphML, Cypher export, agent wiki (`index.md` + community articles)

## Levels
- **lite** — structure-only code graph + short report
- **full** (default) — + communities + query helpers
- **ultra** — + deep semantic edges + cross-repo merge
