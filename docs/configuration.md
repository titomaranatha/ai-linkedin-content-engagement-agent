# Configuration

See [`../.env.example`](../.env.example). All values are placeholders.

- `POST_SCHEDULE=MON,WED,FRI@10:00` and `REPORT_SCHEDULE=MON@09:00` match the documented rules. Do not change them without owner authorization.
- Store LinkedIn tokens in a secure secret store. Tokens expire; renewal is manual unless automated (unverified).
- Verify time zone before enabling schedules.
- Test with publishing disabled first.
