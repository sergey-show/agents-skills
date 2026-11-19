# Rules (extracted)

- Filing receipts go only to configured, verified internal ops; the origin
  receives one only when it is that verified internal destination.
- An unknown origin stays quiet. An unavailable internal destination uses the
  internal tool result or operator surface, with no external fallback.
- Same (counterparty, channel) filed twice yields one obligation, two epochs.
- A decision with a stale epoch never results in a delivery row.
- Two concurrent claimants yield one dispatch permission; losers never attempt transport.
- Unknown outcomes and failed receipt persistence never enable an automatic retry.
- Successful completion records the receipt and sent status in one transaction.
- An altered epoch, text, hash or destination cannot acquire or begin a claim.
- Active claims block re-file; only pre-dispatch cancellation can release that hold.
- Gate unavailable stamps the marker; gate signed refuses without force.
- Auto-ttl never fires against text the operator has since re-filed.
