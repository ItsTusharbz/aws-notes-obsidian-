### Discovery Service -
- Plan projects migration  by gathering information about on-premises data centers.
- Things like server utilization and dependacy mapping is important.
This can be done 2 ways
- Agentless- Discovery (Agentless Collector)
  - Application Discovery Service Agentless Collector (Agentless Collector) is an on-premises application that collects information through agentless methods about your on-premises environment, including server profile information (for example, OS, number of CPUs, amount of RAM), database metadata, utilization metrics, and data about network traffic among on-premises servers
- Discovery Agent -
  - The AWS Application Discovery Agent (Discovery Agent) is software that you install on on-premises servers and VMs targeted for discovery and migration. Agents capture system configuration, system performance, running processes, and details of the network connections between systems.

Resulting data can be viewed within AWS Migration Hub.


### AWS Migration Service 
- Lift and shift (rehost) solution which simplify migrating application to AWS.
- Converts your physical, virtual and cloud-based servers to run natively on AWS.
- Supports wide range of platforms, OS and db
- Minimal downtime, reduced costs

Below is simple architecture.
![[Pasted image 20250102161312.png]]