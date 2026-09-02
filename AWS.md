# AWS

## 1. EBS (Elastic Block Storage)

### Copy EBS from one AZ to another AZ with data

(1). Create a snapshot of a desired EBS volume.  (Tip :  If you can't pause writes to the volume, we recommend that you unmount the volume, from within the instance, before you create the snapshot. You can remount and resume writes once the snapshot enters the pending state.)

(2). Create a new EBS volume from snapshot and while creating choose desired AZ. 

(3). After that attach the volume to the EC2 instace running in that AZ and mount it to use data.

### Automate the backup of data using Lifecycle manager

Use Amazon Data Lifecycle Manager to automate the creation, retention, and deletion of EBS snapshots and EBS-backed AMIs. Creates snapshot of EBS volume at defined intervals and deletes after certain defined period. Useful in case of storing critical data.