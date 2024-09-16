
- It is AWS database to hold large amount of data.
- It is ==no-SQL== and values stored in key/value pair format.
- It can handle millions of request per seconds, trillions of rows and 100+ TB of storage.
- Fully managed by AWS
- Single digital millisecond latency
- Integrated with IAM for security and authorization and administration.



DynamoDB Accelerator - DAX

- This is caching service for Dynamo db.
- It improves the read speed by 10x and comes down to micro-second retrieval.


Global Tables
- It a feature of DynamoDB where you can create a replica of DB to any other region.
- This replica can read/write and all the replicas will be in sync
- This way you can serve customer with low latency.
- Its called ==Active-Active Replication==