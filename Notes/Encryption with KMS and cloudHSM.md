
- There are 2 types of state of data.
  1. Data at rest
  2. Data at transit
- There are different encryption for both state.

#### KMS (Key Management Service)
- AWS uses KMS to manage the keys in aws.
- Below service can opt in for encryption
  - EBS volumes
  - S3 buckets
  - Redshift db 
  - RDS db
  - EFS drive
- Automatically enabled
  - CloudTrail Logs
  - S3 Glacier


#### Types of KMS keys
##### Customer Managed Keys
- Create, manage and used by customer can enable or disable.
- Possibility of rotation
- Possibility to bring-your-won-key
##### AWS managed keys:
- Created, managed and used on customer's behalf by AWS
- used by aws service (pattern aws/s3, aws/ebs, aws/redshift)
##### Owned key:
- Collection of CMKs that an AWS service owns and manages to use in multiple accounts
- AWS can use those to protect resources in your account
##### CloudHSM keys (custom keystore)
- Keys generated from your own CloudHSM hardware device
- Cryptographic operations are performed within cloudHSM cluster.