# Rules (extracted)

- Do not sum every row — they are cumulative per session; reduce to the latest
- Do not estimate costs from raw token counts when `estimated_cost_usd` is present.
- Do not assume the log exists without checking.
- Do not hard-code current model pricing in user-facing answers.
- Do not recommend installing unreviewed hooks or plugins that execute arbitrary code.
