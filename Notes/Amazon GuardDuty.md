
- Intelligent Threat discovery to protect your ==AWS account.
- Uses ML Algo, anomaly detection, 3rd party data to identify the threat.
- Input data include
  - DNS logs.- sending encoded data with DNS queries
  - CloutTrail Event logs - unusual API call, au-auth deployment
    - CloudTrail Management Events - create VPC, subnet etc
    - CloudTrail S3 Data event  - get,list delete object
  - VPC flow logs - unusual traffic and ip adrress
  - Optional Features - EKS audit logs, RDS and Aurora ,EBS, Lambda ,S3 Data event
- We can setup EventBridge to automatic event trigger.
- Good against cryptoCurrency attack.

![[Pasted image 20241028154107.png]]

![[Pasted image 20241028154043.png]]