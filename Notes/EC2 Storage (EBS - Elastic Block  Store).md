
### EBS volume 

- This is a storage block connected to EC2 instance using network
- EBS  can be detached from one EC2 and attached to another EC2 in same AZ
- EBS is bound to one AZ and can not be shared between any AZ
- EBS can we preserved even after attached EC2 instance is deleted.
- You have to provisioned before using the EBS
- You have can EBS created which is not attached to any instance.
- By Default the root EBS volume is marked for deletion once instance is deleted (can be changed)
- By default any other EBS volume is not mark for deletion on instance delete (can be changed)

### Snapshot (backup)

recommendation - detached EBS from instance first.

- Can copy snapshot across AZ or Region
- if Snapshot is attached to AMI then you need to delete the AMI before deleting the snapshot.


##### EBS snapshot feature
 ##### Archive
 - You can move snapshot to 'archive tier' which is 75% cheaper.
 - it take 24 to 72 hr to restore snapshot from archive
Recycle bin
You can setup rules to move snapshot into recycle bin for (1 day to 1 year).
And restore snapshot from it in case of accidental deletion.
