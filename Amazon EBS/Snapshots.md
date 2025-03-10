### Snapshots
- Back up the data on your EBS volumes to S3 by taking point-in-time snapshots.
- Snapshots are incremental backups, which means that only the blocks on the device that have changed after your most recent snapshot are saved.
- Snapshots are stored in S3.
- EBS snapshots broadly support EBS encryption.
- You can’t delete a snapshot of the root device of an EBS volume used by a registered AMI. You must first deregister the AMI before you can delete the snapshot.
- Snapshots can be shared with other AWS accounts or made public.