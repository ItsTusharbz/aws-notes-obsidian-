
- Global service
- allows to manage multiple aws account, main account is master account
- cost benefit:
  - Consolidated billing across all accounts - single payment methods
  - Pricing benefits from aggregated usage
  - Pooling of Reserved EC2 instances for optimal savings
- API is available to automate AWS account creation.
- Restrict account privilege using Service Control Policies (SCP)

#### Multi Account Strategies
- Create account per department, per cost center, per dev / test / prod based on regulatory restrictions to better resource isolation (ex. VPC). To have separate per-account service limits, isolated account for logging.

- Multi Account vs One Account Multi VPC
- Use tagging standards for billing purposes.
- Enable CloudTrail on all accounts, send logs to central S3 account.
- Send CouldWatch Logs to central logging account.

#### Service Control Policies 
- Whitelist or blacklist IAM actions
- Applies at the OU (Organisation Unit) or Account level.
- Does not apply to the Master Account
- SCP is applies to all the Users and Roles of the account, including Root
- The SCP does not affect service-linked roles
  - Service-link roles enable other AWS services to integrate with AWS Organisations  and cant be restricted by SCPs.
- SCP must have an explicit Allow (does not allow anything by default)
- Use cases :
  - Restrict access to certain services (for example: cant use EMR)
  - Enforce PCI compliance by explicitly disabling services

There are 6 different policies 
![[Pasted image 20241122120056.png]]