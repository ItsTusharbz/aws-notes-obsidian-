- It is a CDN (content delivery network)
- It caches the data on the edge location (216 location globally)
- Improves read performance and reduce lag.
- Prevent DDos attach by having global distribution network.


Origin

S3 bucket
- To distribute file and object
- It enhances the security by providing access origin control
- can at as ingress (mean able to upload file to s3)

HTTP 
- Application load balance
- Ec2 instance
- S3 website (must be static website)
- Any HTTP backend 

![[Pasted image 20240928163858.png]]

S3 as origin

![[Pasted image 20240928163926.png]]


Cloudfront vs S3 Cross Region Replication (CRR)


| CloudFront                                                  | CRR                                                                 |
| ----------------------------------------------------------- | ------------------------------------------------------------------- |
| It caches the data                                          | It does real time data replication                                  |
| Data is available across all edge location (global network) | You have to setup the zone for replication                          |
| Performance oriented                                        | Disaster recovery                                                   |
| Great for static content                                    | Great for dynamic content that needs to be available at low latency |


Protection
- Cloud front uses WAF (AWS firewall by defining the Access control rules to resources)
- Cloud shied which is a distributed and managed DDos protection service.