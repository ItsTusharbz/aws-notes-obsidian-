
- it is a global service
- You can create users and groups
- Root account is also part of IAM
- you can not combine group
- one user can exist in multiple groups
- user or group can be assign a JSON documents. Which contains permissions.
-  you apply least privilege principle which means giving as low permission as possible to avoid problem.

 Ways to access AWS 
1. AWS management console (Password+MFA)
2. CLI (protected by access keys)
3. SDK (protected by access keys)

Access keys are generated through console
##### Policies 
- In AWS user can be assigned policies which is nothing but an access control
- different policies will assign different access to user or restrict the user.
- Root user has all policies assigned
- policies has an action which defines whether the user  is allowed to have an access or restricted from that action.

##### Roles for services
- Some AWS service an act on behalf of user. Those services can be granted a role which will define it access and action that can be performed in the account
- common roles - 
   1. EC2 instance role
   2. Lambda Function roles
   3. Roles for cloudFormation.
eg EC2 service can have IAMReadOnly role attached to it. This way EC2 service can read list of users, credentialReport etc.

##### Security Tools
1. IAM Credentials Rport (Account-level)
   - Report list of all user account and credentials
2. IAM Access Advisor (user-level)
   - List of permission granted to user and services they accessed
   
##### AWS Shared responsibility Model for IAM


| AWS                                      | User                                          |
| ---------------------------------------- | --------------------------------------------- |
| Infrastructure                           | Users, Groups, Role and policies              |
| Configuration and vulnerability analysis | Enable MFA to all users                       |
| Complaince Validation                    | Rotate keys often                             |
|                                          | user IAM tool to apply appropriate permission |





