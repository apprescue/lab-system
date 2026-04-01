## AWS Migration

Original setup:

- Next.js frontend
- Supabase DB
- Direct client DB writes

New architecture:

- S3 (frontend hosting)
- CloudFront (CDN)
- API Gateway
- Lambda (backend)
- RDS (Postgres)

Migration steps:

1. Created RDS database
2. Built Lambda handler
3. Connected API Gateway
4. Updated frontend API calls
5. Deployed frontend to S3