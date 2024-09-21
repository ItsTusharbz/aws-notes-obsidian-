
#### ECS (Elastic Container Service)
- Launch docker container on EC2
- Need to maintain the infra (EC2 instance)
- AWS takes care of stopping and starting the docker container
- Has integration with application load balancer

#### Fargate
- Its a serverless service where user doesnt have to manage the infra
- Fargate will create the docker image based on the provisioned ram/rom and CPU base on need.

#### ECR
- Elastic Container Registry
- Private docker image registry in aws
- Fargate uses this registry to launch docker