# Rules (extracted)

- Never use `sleep` for synchronization; use condition variables or latches.
- Don't depend on real time or network in unit tests
- Don't use sleeps as synchronization when a condition variable can be used
- Don't over-mock simple value objects
- Don't use brittle string matching for non-critical logs
