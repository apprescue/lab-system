## Bug Reproduction

Issue:
Database is publicly writable with no auth.

Steps to reproduce:

1. Open frontend
2. Submit any input
3. Call API directly via curl/Postman
4. Insert data without authentication

Observed behavior:

- Data inserted without user validation
- No rate limiting
- API accessible publicly