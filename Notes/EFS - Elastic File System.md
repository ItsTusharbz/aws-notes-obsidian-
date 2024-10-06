- It is a managed file system that can be mounted on multiple EC2 instance across different zone
- it works with Linux EC2 only
- pay per use
- Highly scalable, expensive (3 x gp2)

##### EFS IA (Infrequent Access)
- This storage is used when a file is not used frequently.
- 90 % less cost than standard EFS
- If EFS IA is enabled and you define lifecycle policy to move any file which is not used since some defined duration, once that duration is passed EFS will move file to IA storage. This file will be moved back to standard again when accessed by EC2 instance. 