 Below are the available services
   - Postgres
   - MySQL
   - MariaDB
   - Oracle
   - Microsoft SQL Server
   - IBM DB2
   - Aurora 

### Deployment

- Read Replicas:
  - Scale the read workload of your DB, By Creating a replica of DB which your application can connect.
  - Can Create up to 15 read Replicas.
  - Data is only written to the main DB.

- Multi-AZ:
- It is a replication of db into 1 other zone. incase of main db is not available. (high availability)
 - Failover in case of AZ outage 
 - Data is only read/written to main db
 - can have only 1 other AZ as failover.

-  Multi-Region:
- Disaster recovery in case of region issue.
- Local performance for global reads
- Replication cost.
 
