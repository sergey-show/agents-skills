# Rules (extracted)

- **Dynamic discovery only.** Never hardcode agent lists. New files in the directory auto-appear in the menu.
- **Max 5 agents per team.** More than 5 produces diminishing returns and excessive token usage. Enforce at selection time.
- **Parallel dispatch.** All agents run simultaneously — use the Agent tool's parallel invocation pattern.
- **Parallel Agent calls, not TeamCreate.** This skill uses parallel Agent tool calls for independent work. TeamCreate (a the coding agent tool for multi-agent dialogue) is only needed when agents must debate or respond to each other.
