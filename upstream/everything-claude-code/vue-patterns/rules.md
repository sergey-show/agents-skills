# Rules (extracted)

- Always provide `type`, and `required`/`default` where appropriate.
- Never mutate props — emit events instead.
- Must start with `use` prefix.
- No module-scope side effects.
- Return reactive values (`ref`, `computed`, `reactive`), never plain primitives.
- Accept reactive inputs via `MaybeRef` / `toRef()` / `toValue()`.
- Clean up side effects in `onUnmounted` or watcher `onCleanup`.
