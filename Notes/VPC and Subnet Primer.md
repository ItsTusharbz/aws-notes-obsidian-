- VPC - Virtual private cloud - private network to deploy your resources
- Subnet - Allow you to partition your network inside vpc
- Public subnet - subnet which is connect to internet through Internet gateway 
- private subnet - subnet which has only outgoing traffic to internet.

- Internet gateway -  helps your vpc instance connect to internet
- NAT (Network address Translation)  gateway - Using this private subnet can access internet using NAt gateway.
- subnet is connected to internet gateway using route table. which keep track of origin and target location.

![[Pasted image 20241018155716.png]]