# AWS EC2 Networking

* An elastic network interface is a logical networking component in a VPC that represents a virtual network card, which directs traffic to your instance
* Every instance in a VPC has a default network interface, called the primary network interface (eth0). You cannot detach a primary network interface from an instance.
* Default interfaces are terminated with instance termination.
* Scale with EC2 Scaling Groups and distribute traffic among instances using Elastic Load Balancer.