
- It is a DNS (domain name service)  to manage the mapping of ip address to hostname.
- In AWS most common records are
  - domain name => IPv4 == A record
  - domain name => IPv6 === AAAA IPV6
  - domain name => domain name  == CNAM: hostname to hostname
  - domain name => AWS resource == Alias (eg ELB, CloudFront, S3, RDS etc)
![[Pasted image 20240928154410.png]]


Routing Policies

- Simple routing policies (No health check)
- Weighted routing policies (traffic is distributed between weighted servers) (health check)
- Latency Routing policy (route depend on the latency, provide low latency to user) (health check)
- Failover Routing policy (When primary fails redirect to failover server)(health check)