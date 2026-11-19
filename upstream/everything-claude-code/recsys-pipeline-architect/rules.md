# Rules (extracted)

1. **Do not invent benchmark numbers.** "How much faster?" → "depends on workload, run it yourself."
2. **Attribution discipline.** When the pattern is referenced, attribute as "popularized by xAI's open-sourced For You algorithm" / `github.com/xai-org/x-algorithm` (Apache 2.0).
3. **No trademark use.** Do not name the user's artifact "X-like" or use "For You" branding. Pattern is free; brand is not. Suggested naming: "candidate pipeline", "feed pipeline", "ranking pipeline", "recsys pipeline".
4. **Surface trade-offs.** Multi-action vs single, isolation vs joint, online vs offline — never default silently.
5. **The generated scaffold must run.** No pseudocode passing as code.
6. **Filter order matters.** Cheap before expensive. Universal before user-specific.
7. **Side effects never block.** Wrap in fire-and-forget patterns (goroutines / promises without await / asyncio tasks).
