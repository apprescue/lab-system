## Fixes

Solution:

- Remove direct DB access
- Move logic to secure backend (Lambda)
- Add validation layer

Implementation:

- API Gateway + Lambda introduced
- RDS replaces Supabase
- No direct DB access from frontend

Why it works:

- Backend controls all writes
- Credentials are hidden
- Requests can be validated