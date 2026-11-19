# Rules (extracted)

- Always query `decimals()` at runtime
- Cache by chain plus token address, not symbol
- Use `Decimal`, `BigInt`, or equivalent exact math, not float
- Re-query decimals after bridging or wrapper changes
- Normalize internal accounting consistently before comparison or pricing
