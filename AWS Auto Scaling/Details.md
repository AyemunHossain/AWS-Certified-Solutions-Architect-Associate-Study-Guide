

### EC2 Auto Scaling
- Ensuring you have the correct number of EC2 instances available to handle your application load using Auto Scaling Groups.
- **Auto Scaling group**: Contains a collection of EC2 instances that share similar characteristics and are treated as a logical grouping for the purposes of instance scaling and management.
- You specify the minimum, maximum and desired number of instances in each Auto Scaling group.
- **Launch Configuration**: A template that an Auto Scaling group uses to launch EC2 instances.

### Scaling Policy Types
- **Target Tracking Scaling**: A scaling policy for an Auto Scaling group that automatically adjusts the number of instances in the group as the value of a specified CloudWatch metric changes.
- **Step Scaling**: A scaling policy for an Auto Scaling group that adjusts the number of instances in the group based on a set of scaling adjustments, known as step adjustments.
- **Simple Scaling**: A scaling policy for an Auto Scaling group that increases or decreases the current capacity of the group based on a single scaling adjustment.


### Termination of Instances
- When you configure automatic scale in, you must decide which instances should terminate first and set up a termination policy. You can also use instance protection to prevent specific instances from being terminated during automatic scale in.

### Launch templates
- You can create launch templates that specifies instance configuration information when you launch EC2 instances, and allows you to have multiple versions of a template.

### A Launch configuration
- A launch configuration is an instance configuration template that an Auto Scaling group uses to launch EC2 instances, and you specify information for the instances.
- You can only specify one launch configuration for an Auto Scaling group at a time, and you can’t modify a launch configuration after you’ve created it. If you need to change the launch configuration for your Auto Scaling group, create a new launch configuration.
- If you set the tenancy attribute of a VPC to **dedicated**, all instances launched in the VPC run as **single-tenancy** instances.
- When you create a launch configuration, the default value for the instance placement tenancy is null and the instance tenancy is controlled by the **tenancy attribute of the VPC**.
