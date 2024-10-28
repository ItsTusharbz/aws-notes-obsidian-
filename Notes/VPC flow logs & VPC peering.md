Flow Logs
- Capture information about IP traffic going into tour interfaces 
  - VPC flow logs
  - Subnet Flow logs
  - Elastic Network interface flow logs
- Helps to monitor and troubleshoot connectivity issues
  - Subnet to internet
  - Subnet to subnet
  - Internet to subnet
- Captures networks information from AWS managed interface : Elastic load balancer, ElastiCache, RDS, Aurora etc
- VPC flow logs data can go to S3, CloudWatc Logs and Kinesis Dara Firehose.


VPC peering
  - Connected to VPC privately using AWS network
  - Make them behave as if they were in the same network
  - Must not have overlapping CIDR (IP range)
  - It is not transitive mean every VPC must be connected to each other 