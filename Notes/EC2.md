EC2 = Elastic Compute Cloud = Infrastructure as a Service (IAAS)

##### Capability 
- Renting virtual machines(EC2)
- Storing data on virtual drives (EBS)
- Distributing load across machine(ELB)
- Scaling the services using an auto scaling group (ASG)
##### Configuration options

- OS
- CPU
- RAM
- Storage 
  - Network attached (EBS or EFS)
  - Hardware (EC2 instance store)
- Network card : speed of the card, public IP address
- Firewall rules
- Bootstrap script (configure at first launch ) : EC2 user data

##### EC2 instance type

![[Pasted image 20240902205847.png]]

==Free Tier -==
==User gets total 750hr/month/year of EC2 instance usage. This means one instance can run for 750hr or 2 instance can run 375hr it is a total hour run by all the instance in the account. If they exceed 750hr they you will be charge.==
==Same follow for any free tier service in AWS==


Ec2 instance - T2.micro

T family is burstable instance.
Burstable instance - This instance had baseline CPU capacity. These instance earns CPU credit.
those credit can be used while in burst mode.
burst mode is nothing but sudden rise of work load to the CPU
T2 instance earn CPU credit by below formula

CPU Credit = % baseline utilization * number of vCPU * 60min;



Note - site to see all available EC2 instance in aws https://instances.vantage.sh/ 

EC2 instance Types

- General purpose
- Compute Optimized
- Memory Optimized
- Accelerated Computing
- Storage Optimized
- HPC (high performance computing) 


Security Groups

- Fundamental of network security n AWS
- They control how trafffice s allowed into or out of EC2
- They only contain allow rules
- They are firewall of EC2
- Regulate
  - Access to port
  - Authorized IP ranges  - IP4V and IP6V
  - Control of inbound network 
  - Control of outbound network

Note - If you are trying to connect to EC2 and getting timeout error while trying connect using any mode (SSH,HTTP etc) it is due to security group rule.

Ports

- 22 = SSH (secure shell ) - log into a Llinux instance
- 21 == FTP (File Transfer Protocol ) - Upload files into a file share
- 22 = SFTP (Secure File Transfer Protocol) - Upload files using SSH
- 80 = HTTP - access unsecured website
- 443 = HTTPS - access secured website
- 3389 = RDP (Remote Desktop Protocol) - Log into a windows instance


Window 10 ssh connect

1. check if ssh is installed
2. go to directory which contains key pair file of EC2
3. and type  ssh -i <key_pair_file.pem> ec2-user@<Public_IP> eg 65.2.73.159, public ip changes whenever EC2 instance starts


## EC2 purchase options

##### On-demand - Pay as you use
  - Linux or widows - billing per second
  - other operating system - blling per hr
- highest cost no upfront payment
- Recommended for short term and un interrupted workloads 
##### Reserved instance
- 72% discount compared to on-demand
-  You reserve specific instance attribute (Type,Region,Tenancy, OS)
- Reservation Period - 1 year or 3 year
- payment options - no upfront , partial ,all upfront
- Scope - Regional or zonal 
- Good for steady state usage app (eg db)
- you can buy or sell RI on marketplace
##### Convertible instance
- Can change above reserve attribute
- less discount 66%

##### Savings instance
- Get discount 72 %
- commit to certain type of usage (10/hr for 1 to 3 year)
- locked to specific instance family & AWS region 
- Flexible across
  - Instance size
  - os 
  - tenancy

##### Spot instance
- Highest discount 90%
- can  you lose the instance if the max price is less than current spot price
- most cost-effective instance
- Useful for workload that are resilient to failure
  - Batch jobs
  - Data Analysis
  - Image processing
  - Any distributed workloads
  - Workloads with flexible start and end time

##### Dedicated host
- Physical server with EC2 instance capacity fully 
- Allows you to address compliance requirements and use your existing server bound software licenses (per socket, per core , per - VM software licenses)
- Purchasing options
  - on-demand 
  - reserved

##### Dedicated instance
- instance run on hardware that's dedicated to you
- When stop/start the instance it may or may not start on the same machine. Instance is getting moved but you get dedicated hardware which has no other instance running.
- instance for same account (dedicate or not ) may run on the same host, but other AWS account instance will never run on the same hard which has dedicated instance running

##### Capacity Reservations
- On-demand instance capacity in any specific AZ for duration
- No time commitment (create/cancel anytime) no billing discount.
- Combine with regional reserved instance and savings plans to benefit billing discount.
- You are charged at on demand rate whether you run instance or not
- Used for short term, uninterrupted workloads in AZ



Storage 

[[EC2 Storage (EBS - Elastic Block  Store)]]
[[EC2 instance storage]]
[[EFS - Elastic File System]]


EC2 responsibility model
 

| AWS                                               | USER                                         |
| ------------------------------------------------- | -------------------------------------------- |
| Infrastructure                                    | Seeting up backup / snapshot procedures      |
| Replication for data for EBS volumes & EFS drives | setting up data encryption                   |
| Replacing faulty hardware                         | responsibility of any data on the dries      |
| Ensuring their employees cannot access your data  | Understanding the rick of EC2 instance store |
|                                                   |                                              |
