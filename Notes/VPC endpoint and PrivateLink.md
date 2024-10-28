#### VPC EndPoints
- VPC endpoint allows you to connect to other AWS services privately.
- There are 3 types of endpoint
  - Interface 
  - Gateway Load Balancer
  - Gateway  (for S3 and DynamoDB)
- Interface endpoints are typically accessed using the public or private DNS name associated with the service, 
- Gateway endpoints and Gateway Load Balancer endpoints serve as a target for a route in your route table for traffic destined for the service.

#### Private Link
- Most scalable and secure way to expose a service to 1000s of VPCs
- Does require VPC peering, NAT, internet gateway, route tables...
- requires a network load balancer (Service VPC) and ENI (customer VPC)
- Below is example architecture of 3rd party vendor who is selling their service to other amazon customer.

![[Pasted image 20241020195443.png]]


Note - ENI (Elastic Network Interface) - It is nothing but a virtual network card in the VPC. You can connect Ec2 instance with ENI when they are in the same AZ. using ENI EC2 instance can connect to internet. You can attach or detach ENI from EC2. 

