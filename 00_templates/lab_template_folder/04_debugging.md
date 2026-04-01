## Debugging

Logs:

- API route logs show successful inserts
- No auth checks present

Analysis:

- Supabase client used directly with anon key
- No validation layer

Root cause:

- Open database policies
- No authentication enforcement
- Backend trusts all requests