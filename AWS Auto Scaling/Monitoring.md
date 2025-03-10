### Monitoring

- **Health checks** – identifies any instances that are unhealthy
  - Amazon EC2 status checks (default)
  - Elastic Load Balancing health checks
  - Custom health checks.
- Auto scaling does not perform health checks on instances in the standby state. Standby state can be used for performing updates/changes/troubleshooting without health checks being performed or replacement instances being launched.
- **CloudWatch metrics** – enables you to retrieve statistics about Auto Scaling-published data points as an ordered set of time-series data, known as metrics. You can use these metrics to verify that your system is performing as expected.
- **CloudWatch Events** – Auto Scaling can submit events to CloudWatch Events when your Auto Scaling groups launch or terminate instances, or when a lifecycle action occurs.
- **SNS notifications** – Auto Scaling can send Amazon SNS notifications when your Auto Scaling groups launch or terminate instances.
- **CloudTrail logs** – enables you to keep track of the calls made to the Auto Scaling API by or on behalf of your AWS account, and stores the information in log files in an S3 bucket that you specify.