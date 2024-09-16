
User-based
- IAM policies  - you can define which api can are allowed for specific IAM user

Resource-Based
- Bucket Policies - bucket wide rules from the s3 console. - allows across account
- Bucket Access Control List - Bucket specific rules.
- Object Access Control List (ACL) - This is object level rules (very fine grain)

Encryption
- you can encrypt the s3 object using keys

Note - an IAM principal (account) can access s3 object if IAM policy or resource policy Allows it, and there is no explicit deny.

#### S3 Bucket policies

JSON object
- Resource : Specify the bucket to attach policy to 
- Effect : effects are applied on actions (eg Allow/ Deny)
- Action: Set of api to be allowed or denied
- Principal : The account or user to apply the policy to


S3 Encryption
- Server-side Encryption - server encrypts the file after receiving it
- Client-side encryption - Client encrypts data before upload.



