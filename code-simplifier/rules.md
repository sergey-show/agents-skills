# Rules — code-simplifier

1. Preserve behavior unless the user explicitly wants a behavior change.
2. Prefer characterization coverage before deleting unclear code.
3. Split by responsibility, never by line-count cosmetics.
4. Do not add new abstraction layers while "simplifying."
5. Grep callers before removing or merging exports.
6. Report residual risk for anything you could not safely touch.
7. No harness-specific tool names.
