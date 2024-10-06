
#### ECS (Elastic Container Service)
- Launch docker container on EC2
- Need to maintain the infra (EC2 instance)
- AWS takes care of stopping and starting the docker container
- Has integration with application load balancer

[[Fargate]]
#### ECR
- Elastic Container Registry
- Private docker image registry in aws
- Fargate uses this registry to launch docker