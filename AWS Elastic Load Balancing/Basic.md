### Introduction
- Elastic Load Balancing automatically distributes incoming application traffic across multiple targets, such as:
     * Amazon EC2 instances, 
     * containers, 
     * IP addresses, and 
     * Lambda functions. 
It can handle the varying load of your application traffic in a single Availability Zone or across **multiple Availability Zones**. Elastic Load Balancing offers three types of load balancers that all feature the high availability, automatic scaling, and robust security necessary to make your applications fault tolerant.


### General Features
- **High Availability**, **Fault Tolerance**, **Automatic Scaling**, **Security**

### Types of Load Balancers
- **Application Load Balancer**: Best suited for load balancing of HTTP and HTTPS traffic. They operate at Layer 7 and are application-aware. They are intelligent and can create advanced request routing, sending specified requests to specific web servers.
- **Network Load Balancer**: Best suited for load balancing of TCP traffic where extreme performance is required. Operating at the connection level (Layer 4), Network Load Balancer is capable of handling millions of requests per second while maintaining ultra-low latencies.
- **Gateway Load Balancer ( GWLB )**: Best suited for load balancing of third-party appliances such as firewalls, intrusion detection systems, and deep packet inspection systems. GWLB operates at the connection level (Layer 4) and supports the load balancing of TCP and UDP traffic.
- **Classic Load Balancer ( CLB )**: This is the previous generation Elastic Load Balancer. It provides basic load balancing across multiple Amazon EC2 instances and operates at both the request level and connection level. CLB is being deprecated and should not be used for new deployments.

### Application Load Balancer
* Support for routing requests to multiple applications on a single EC2 instance.
* Support for routing requests to multiple ports on a single EC2 instance.
* Support for containerized applications.
* Support for returning a custom HTTP response.
* Supports load balancer-generated cookies for sticky sessions.
* Supports Application-based cookie stickiness.

### Network Load Balancer ( NLB )
* Support for static IP addresses for the load balancer.
* Ability to handle volatile workloads and scale to millions of requests per second.
* Support for routing requests to multiple applications on a single EC2 instance (register each instance or IP address with the same target group using multiple ports).
* Support for containerized applications.

### Gateway Load Balancer ( GWLB )
* Support for third-party appliances.
* The virtual appliances can be your custom firewalls, deep packet inspection systems, or intrusion detection and prevention systems in AWS 
* Uses the Internet Protocol (IP) to pass the OSI Layer 3 traffic to its registered targets.
* Runs within one Availability Zone (AZ)
* You cannot specify publicly routable IP addresses as your target

### Classic Load Balancer ( CLB )
* Basic load balancing across multiple Amazon EC2 instances.
* Operates at both the request level and connection level.
* Support for sticky sessions using load balancer-generated cookies.


### Security, Authentication and Access Control
* Use IAM Policies to grant permissions
* Resource-level permissions
* Security groups that control the traffic allowed to and from your load balancer.