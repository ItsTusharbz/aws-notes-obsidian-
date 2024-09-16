
- Expose single point of access (DNS) to you applications
- Distribute load across multiple instance.
- Handle failure
- Provide SSL termination (HTTPS) for you website 
- High Availability

Type of load balancer provided by AWS

- Application - layer 7 for http and https
- Network - Ultra high performance TCP layer 4
- Gateway  Layer 3
- Classic (retired) - layer 4 & 7

![[Pasted image 20240907193749.png]]


#### Auto Scaling Group 

goal for ASB
- Scale out (increase ) or scale in (decrease) EC2 instance to match website load.
- Ensure we have optimal number of server running depend on load.
- Automatically register new instances to a load balancer.
- Replace unhealthy instance.
- Good cost savings
