# Rules (extracted)

```go
// Bad: Ignoring error with blank identifier
result, _ := doSomething()
// Good: Handle or explicitly document why it's safe to ignore
result, err := doSomething()
if err != nil {
    return err
}
// Acceptable: When error truly doesn't matter (rare)
_ = writer.Close() // Best-effort cleanup, error logged elsewhere
```
