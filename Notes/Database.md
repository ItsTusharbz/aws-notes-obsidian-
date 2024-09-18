Relation Database
Non-Relational Database


AWS provide managed DB 
Benefits - 
- Quick Provisioning, High Availability, Vertical and Horizontal Scaling
- Automated Backup and Restore, Operations, Upgrades
- Operating system patch handled by AWS
- Monitoring, Alerts

Note- You can install DB on EC2 instance. but then you have to manage everything for it.


### Services Provided by AWS 
#### Amazon RDS overview (DB) [[AWS Relational Database Service]]

- RDS - Relational Database Service
- Data is stored in EBS 
 - Below are the available services
   - Postgres
   - MySQL
   - MariaDB
   - Oracle
   - Microsoft SQL Server
   - IBM DB2
   - Aurora 
   - 

#### Amazon Aurora 
- PostgreSQL and MySQL are both supported by Aurora DB
- Proprietary tech of AWS no open source
- 5x performance than MySQL, 3X performance than PostgreSQL
- Automatically grows 10Gb to 128TB
- cost 20% more  than RDS
- Not in free tier

#### Amazon Aurora Serverless
- It is managed by server
- Auto scaling vertical or horizontal depend on load.

#### Caching 
[[AWS ElastiCache]]

### Database Provided by AWS
DynamoDB - [[Dynamo DB]]
Neptune - [[Neptune]]
QLDB - [[QLDB]]
TimeStream - [[TimeStream]]
Neptune - [[Neptune]]

#### Database Analysis Services
[[Redshift]]
[[EMR]]
[[Athena]]
[[QuickSight]]
[[AWS blockchains]]

##### Migration and transform
[[AWS Glue]]
[[DMS (data migration service)]]