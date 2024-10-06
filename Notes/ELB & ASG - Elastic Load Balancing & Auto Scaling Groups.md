
##### Scalability
Vertical Scaling
- You increase the size of instance to match the load ( eg more ram, memory IOPS, storage space etc)
- Common with Db instances
- limited by hardware.

Horizontal Scaling
- You increase number of instances to match the load.
- Good for distributed system
- Usually used for Web Application.

##### High Availability
- Same application is running on multiple AZ instance to avoid disaster.
- Goes hand in hand with Horizontal scaling
- It means your application is running on atleast 2 AZ

Definitions
##### Scalability 
Ability to accommodate a larger load by making the hardware stronger (scale up) or by adding nodes (scale out) 

Elasticity 
Once a system is scalable. The ability of that system to auto-scale based on load is elasticity.

Agility
It means how fast the resources can be available to developer to start the development or deployment.


#### Auto Scaling Group 

Goal for ASG
- Scale out (increase) or scale in (decrease) EC2 instance to match website load.
- Ensure we have optimal number of server running depend on load.
- Automatically register new instances to a load balancer.
- Replace unhealthy instance.
- Good cost savings


##### ASG strategy
- Manual Scaling - Manually update the size of ASG 
- Dynamic Scaling
  - Simple/Step Scaling
    - When cloud Watch alarm is triggered (eg CPU > 70%) for 5 min increase the size
    - When cloud Watch alarm is triggered (eg CPU < 40%) for 5 min decrease the size
- Target Tracking Scaling 
  - Eg i want to keep the average cpu usage to 40%
- Schedule Scaling
  - If you know when the traffic to your site is high or low, you can schedule the ASG to increase or decrease at that time.
- Predictive Scaling
  - Used machine learning to predict the traffic and increase or decrease ASG size.
  