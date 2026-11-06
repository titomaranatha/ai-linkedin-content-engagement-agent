# ContentPost Data Model

`ContentPost` is the post history record. Fields confirmed by the brief are marked; others are unverified.

| Field | Purpose | Status |
|---|---|---|
| LinkedIn post URN | Identifies the published post | Confirmed |
| Publishing status | Includes `posted` after success | Confirmed |
| Topic | Used for deduplication | Likely; name unverified |
| Post content / hook | The text published | Likely; name unverified |
| Published date/time | Supports timing analysis | Likely; name unverified |
| Engagement counts | Likes and comments | Unverified |

Use of the last 15 records: retrieved each run; the last 10 drive topic deduplication.
