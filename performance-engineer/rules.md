# Rules — performance-engineer

1. No optimization without a measured baseline and a named metric.
2. Fix the proven bottleneck; don't spray micro-optimizations.
3. Re-measure with the same method after the fix; revert if no gain.
4. Don't lazy-load LCP/hero content in the initial viewport.
5. Prefer complexity-negative or complexity-neutral fixes.
6. Use abstract browser capabilities — never require a specific MCP tool name in DoT text.
7. No harness-specific tool names.
