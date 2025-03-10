### Features
- Provides **durable, block-level storage volumes** that you can attach to a running instance.
- You can use Amazon EBS volumes as **primary storage** for data that requires frequent updates, such as the system drive for an instance or storage for a database application.
- You can also use them for **throughput-intensive** applications that perform continuous disk scans.
- Amazon EBS volumes are particularly well-suited for use as the primary storage for file systems, databases, or for any applications that require fine granular updates and access to raw, unformatted, block-level storage.
- Amazon EBS volumes **persist independently** from the running life of an instance.
- You can create a file system on top of these volumes, or use them in any other way you would use a block device (like a hard drive).
- You can copy **snapshots** to other regions and then **restore them** to new volumes there, making it easier to leverage multiple AWS regions for geographical expansion, data center migration, and disaster recovery.
- EBS fast snapshot restore allows you to create a volume from a snapshot that is fully initialized.
- Elastic Volumes allow you to increase the volume size, adjust performance, or change the volume type while the volume is in use.
- With AWS Backup, you can configure backups for EBS volumes, automate backup scheduling, set retention policies, and monitor backup and restore activity.

### Types of EBS Volumes
- **General Purpose SSD (gp2)**: General purpose, balances price and performance for a wide variety of workloads.**max throughput 250 MB/s**.
- **General Purpose SSD (gp3)**: General purpose, balances price and performance for a wide variety of workloads. **max throughput 1000 MiB/s**.
- **Provisioned IOPS SSD (io1)**: High performance SSD volume designed for latency-sensitive transactional workloads. **max throughput 1,000 MB/s**.
- **Provisioned IOPS SSD (io2)**:  High performance SSD volume designed for business-critical latency-sensitive applications. **max throughput 4,750 MB/s/ 7,500 MB/s for io2 block express**.
=