- It is a developer centric service where you dont manage infra, but only worry about the cod.
- Beanstalk uses component like EC2,ASG,ELB,RDS etc.
- We still have full control of the resources.
- It is platform as a service.
- Beanstalk is free but the underline resources cost money.
- It uses cloudFormation to deploy the resources

Managed service
- instance configuration
- Capacity provisioning
- Load balancing and auto-scaling
- Application health-monitoring and responsiveness.

Three architecture models
- Single instance deployment : good for dev
- LB  + ASG great for production or pre-prod web app
- ASG only : great for non web prod app. (workers etc).

Health Monitoring
- Health agent pushes metrics to cloudWatch
- App health monitoring
