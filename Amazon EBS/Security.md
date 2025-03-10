### Encryption
- Data stored at rest on an encrypted volume, disk I/O, and snapshots created from it are all encrypted.
- Also provides encryption for data in-transit from EC2 to EBS since encryption occurs on the servers that hosts EC2 instances.

### The following types of data are encrypted:
- Data stored at rest on the volume.
- All data moving between the volume and the instance.
- All snapshots created from the volume.
- All volumes created from those snapshots.

### Encryption Keys
- EBS encryption uses AWS Key Management Service (KMS) customer master keys (CMKs) when creating encrypted volumes and snapshots.
- You can use either the default CMK that AWS creates for you, or a custom CMK that you create.
- If you use a custom CMK, you retain control of your encryption keys, and full control over who can use your keys.
- You can also use the same CMK to encrypt your EBS volumes, snapshots, and S3 objects.
