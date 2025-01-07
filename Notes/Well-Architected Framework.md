### General Guiding principle
- Stop guessing your capacity need instead automated the scaling process using autoscaling
- Test system at production scale as resources are easily available.
- Automate to make arch experiment easier using  cloudFormation (infra as code) or beanstack (saas)
- Allow for evolutionary architectures
  - Design based on changing requirements
- Improve through game days
  - Simulate app for flash sale days (stress testing)
### Cloud Best Practices - Design Principles
- Scalability : vertical and horizontal scalable
- Disposable Resources : servers should be disposable & easily configured
- Automation : Serverless, Infrastructure as a Service, Auto Scaling...
- Loos Coupling: 
  - Break coupling between app and create loos coupling using service like [[SNS (Simple notification service)]], [[Amazon SQS (simple queue service)]] etc.
- Service not Server 
  - Don't just use Ec2
  - Use managed services, db, serverless etc to improve the applications.
### 6 Pillars
1. Operational Excellence
2. Security
3. Reliability
4. Performance 
5. Cost
6. Sustainability