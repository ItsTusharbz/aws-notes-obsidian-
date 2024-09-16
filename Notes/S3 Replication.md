
- Must enable versioning in source and destination buckets
- Cross-Region Replication (CRR)
- Same-Region Replication (SRR)
- Bucket can be in different AWS account
- Copying is asynchronous
- Must give proper IAM permission to S3
Use cases:
- CRR - compliance, lower latency access, replication across accounts
- SRR - log aggregation, live replication between production and test accounts