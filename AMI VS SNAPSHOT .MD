# AMI VS SNAPSHOT


   |  PARAMETERS  |  AMI  |  SNAPSHOT  |
   |  ---  |  ---  |  ---  |
   |  SERVICE  | Associate With EC2 Instance  | Associate With EBS Instance  |
   |  IT IS  |  Bootable copy of the whole EC2 instance  |  Backup of the data on EBS  |
   |  USE  |  use to store current instance configuation  |  use to store many instance configuration  |
   |  NON-EBS BACKUP  |  Instance are created  |  Instance are not possible  |



Note that when you launch a machine from an AMI you end up with a running instance. To put it another way, you turn AMI's into instances.

A snapshot is an exact copy of a single volume at a single point in time. You can take as many snapshots as you can pay for.
Snapshots are typically used for backup purposes.
Note that you turn snapshots into volumes to attach to an instance. You don't turn snapshots into an instance itself, like an AMI.
You can create a new machine using a snapshot though. Basically create a brand new machine.*

- So the short story:
  - Use AMI's for deploying new machines that are identical.
  - Use snapshot's for doing backups and DR.
