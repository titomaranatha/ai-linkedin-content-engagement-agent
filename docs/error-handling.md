# Error Handling & Failure Scenarios

Handling is **not verified** in the live project; this table defines the intended behaviour consistent with the operating rules.

| Scenario | Intended behaviour |
|---|---|
| Image generation fails | Do not publish a broken post; notify owner or retry. Text-only fallback requires owner decision. |
| LinkedIn publish fails | Do not mark `posted`; record failure status; notify owner. |
| Token expired or revoked | Stop, notify owner for manual re-authorisation. |
| Missed 10:00 AM window | Do not publish late outside the window, per rules; notify owner. |
| No topic passes deduplication | Do not publish a repeat; notify owner. |
| No verifiable story available | Do not invent one; notify owner. |
| Comment reply fails | Log and retry next run; never post duplicates. |
| Engagement data unavailable | Report with available data and state gaps. |
| Duplicate trigger | Check for an existing `posted` record for that slot before publishing. |
