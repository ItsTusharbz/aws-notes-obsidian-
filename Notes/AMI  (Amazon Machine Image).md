
- AMI are nothing but customized EC2 instance
  - you add ur own software, configuration and operating systems
  - Faster boot and configuration time as all software are pre-packaged
- AMI are built for specific region
- There are public AMI, your own AMI, or Marketplace AMI


#### Process

1. Start an EC2 instance and customize it.
2. Stop the instance
3. Build an AMI - this will create EBS snapshot
4. You can copy AMI from one region to another
5. During the creation EC2 makes snapshot of each EBS attached to instance.


EC2 image builder overview
- Automate the creation, maintain, validate and test EC2 AMIs.
- It cam be run on schedule
- Free service.
- Flow is automated flow
  1. Build will create EC2 instance
  2. New AMI is created out of it
  3. New Test EC2 instance is created
  4. AMI is distributed (to multiple region)