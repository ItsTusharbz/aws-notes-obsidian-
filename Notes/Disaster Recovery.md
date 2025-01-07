- There are 4  cloud disaster recovery strategies available
  - Backup and Restore - 
    - This is a simple backup and restore service. 
    - This may lead to downtime as data will be downloaded from the cloud.
    - Cheapest of all
- Pilot Light - 
  - Deploy minimum app with core functionality only, which is ready to scale.
  - Data live but services are idle.
  - Cost more than B&R 
- Warm Standby  - 
  - Service is always running but at smaller scale. when event happen resources are provided to scale.
  - Mostly for bussiness critical app
- Multi-site active/active 
  - Zero downtime.
  - Deploy full version of app at full size.
  - You can run your workload simultaneously in multiple Regions as part of this.
  - most expensive.