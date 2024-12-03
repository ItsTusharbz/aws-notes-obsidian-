- When enabled, provides you with :
  - Combined Usage - combine the usage across all AWS accounts in the AWS Organization to ==share the Volume pricing, Reserved Instances and Savings Plans discounts.
  - One Bill - get one bill for all AWS Accounts in the AWS Organization.
- The management account can turn off Reserved Instances discount sharing for any account in the AWS Organization, including itself.

Example:
Account Bob has no reserved instances, but account Susan has 5 reserved instance. Now susan launches 3 EC2 instance consuming 3/5 reserved instance. If the resource sharing is enabled bob can use 2 remaining reserved instance space and save cost. 

![[Pasted image 20241122122823.png]]