# Rules (extracted)

- Repeatability requires the same verified document geometry and a valid transform.
- Incomplete or degenerate calibration stops before target placement.
- Untrusted origins/frames or mismatched composer/document identity stop reads
  and mutations; navigation invalidates earlier checks.
- Every counterparty field is owned by recipient 2, every one of ours by
  recipient 1.
- With no `--draft` or explicit send instruction, the envelope is not sent.
- A logged-out session exits non-zero before touching the composer.
