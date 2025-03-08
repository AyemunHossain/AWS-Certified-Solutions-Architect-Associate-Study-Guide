# AWS Security Best Practices

## 1. Use IAM to Control Access to Your Instances
AWS Identity and Access Management (IAM) helps you securely control access to AWS resources.

- **IAM Policies**
- **IAM Roles**

## 2. Restrict Access to Trusted Hosts or Networks
Only allow trusted hosts or networks to access ports on your instance to enhance security.

## 3. Security Groups as Virtual Firewalls
A security group acts as a virtual firewall that controls traffic for one or more instances.

- Create different security groups to handle instances with varying security requirements.
- Add rules to each security group to allow traffic to or from its associated instances.
- Modify security group rules at any time.
- New rules apply automatically to all instances associated with the security group.
- AWS evaluates all rules from all security groups associated with an instance to determine access.
- By default, security groups allow **all outbound traffic**.
- Security group rules are **always permissive**—you cannot create rules that deny access.
- Security groups are **stateful**.

---

✅ Follow these best practices to ensure better security for your AWS instances.