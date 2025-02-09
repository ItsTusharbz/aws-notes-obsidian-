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
 - I
   - Postgress
   - MySQL
   - MariaDB
   - Oracle
   - Microsoft SQL Server
   - IBM DB2
   - Aurora (Postgress and Mysql compatible)
   
#### Amazon Aurora 
- PostgreSQL and MySQL are both supported by Aurora DB.
- It is a db as well act as service doing auto scaling etc
- Proprietary tech of AWS no open source
- 5x performance than MySQL, 3X performance than PostgreSQL
- Automatically grows 10Gb to 128TB
- cost 20% more than RDS
- Not in free tier

#### Amazon Aurora Serverless
- It is managed by server
- Auto scaling vertical or horizontal depend on load.

#### Caching 
[[AWS ElastiCache]]

### Database Provided by AWS
DynamoDB - [[Dynamo DB]] (no-sql db)
Neptune - [[Neptune]]. (graph)
QLDB - [[QLDB]]  (ledger)
TimeStream - [[TimeStream]]
DocumentDb - [[DocumentDB]]
#### Database Analysis Services
[[Redshift]]
[[EMR (Elastic Map Reduce)]]
[[Athena]]
[[QuickSight]]
[[AWS blockchains]]

##### Migration and transform
[[AWS Glue]]
[[DMS (data migration service)]]
[[AWS Snow Family]]