
### Usage
- Media hosting
- static website
- Archived files 
- Backup and storage 
- Disaster Recovery 
- Application hosting
- Data lakes and big data analytics
- Software delivery

Buckets
- Store objects (files) in buckets (directories)
- Must have globally unique name 
- bucket is region specific
- Naming convention 
  - No uppercase, No underscore
  - 3-63 characters long
  - Not an IP
  - Must start with lowercase letter or number
  - No prefix xn-- and suffix -s3alias
- Objects (files) have key
- Keys is composed of prefix (path) + object name (file name)
- eg path = s3://my-bucket/my_folders/my_files.txt

#### Security 
[[S3 security]]

Replication
[[S3 Replication]]


IAM Access Analyzer for S3
- Its an S3 monitoring feature provided by aws
- Ensures that only intended people have access to your s3 bucket.
- Evaluates S3 Bucket Policies, S3 ACLs, S3 Access Points Policies
