# AWS Enterprise Networking Lab

> **Secure Multi-AZ 2-Tier Web Application Architecture using Amazon VPC, Application Load Balancer, Bastion Host, and Private EC2 Instances**

---

## 📖 Project Overview

This project demonstrates the design and deployment of a secure, scalable, and highly available **AWS 2-Tier Enterprise Networking Architecture** using Amazon Web Services (AWS).

The infrastructure is built inside a custom Amazon Virtual Private Cloud (VPC) with public and private subnets distributed across multiple Availability Zones. The architecture follows AWS networking best practices by isolating application servers in private subnets while providing secure administrative access through a Bastion Host and distributing application traffic using an Application Load Balancer.

This project was built as part of my hands-on preparation for the **AWS Certified Solutions Architect – Associate (SAA-C03)** certification.

---

# 🚀 AWS Services Used

- Amazon VPC
- Amazon EC2
- Application Load Balancer (ALB)
- Target Groups
- Internet Gateway
- Public Subnets
- Private Subnets
- Route Tables
- Security Groups
- Bastion Host
- S3 Gateway Endpoint
- Amazon Linux 2023
- Apache HTTP Server

---

# 🏛 Architecture Components

| Component | Purpose |
|------------|---------|
| Amazon VPC | Creates an isolated virtual network for AWS resources. |
| Public Subnets | Host internet-facing resources like the Bastion Host and ALB. |
| Private Subnets | Securely host application servers without public IP addresses. |
| Internet Gateway | Enables internet connectivity for public resources. |
| Route Tables | Control traffic routing inside the VPC. |
| Bastion Host | Provides secure SSH access to private EC2 instances. |
| Application Load Balancer | Distributes incoming HTTP requests across multiple application servers. |
| Target Group | Performs health checks and routes traffic only to healthy instances. |
| Security Groups | Provide stateful firewall protection. |
| S3 Gateway Endpoint | Enables private access to Amazon S3 without internet access. |

---

# 🔒 Security Features

- Custom Amazon VPC
- Multi-AZ Deployment
- Public & Private Network Segmentation
- Bastion Host Architecture
- Least Privilege Security Groups
- Private EC2 Instances
- Secure SSH Access
- Application Load Balancer
- Health Checks
- S3 Private Connectivity using Gateway Endpoint

---

# 🌐 Traffic Flow

```text
Internet
      │
Internet Gateway
      │
Application Load Balancer
      │
 ┌───────────────┐
 │               │
 ▼               ▼
App Server 1   App Server 2
```

---

# 🔐 Secure SSH Flow

```text
Developer Laptop
        │
 SSH (22)
        │
 Bastion Host
        │
 SSH (22)
        │
 Private EC2 Instances
```
---

# 🎯 Skills Demonstrated

- Amazon VPC
- AWS Networking
- Public & Private Subnets
- CIDR Planning
- Route Tables
- Internet Gateway
- Security Groups
- Bastion Host
- Amazon EC2
- Apache Web Server
- Application Load Balancer
- Target Groups
- High Availability
- Linux Administration
- AWS Network Troubleshooting

---

# 📚 Key Learnings

- Designed a custom AWS Virtual Private Cloud (VPC).
- Implemented secure public and private subnet architecture.
- Configured route tables and internet connectivity.
- Secured application servers using security groups.
- Used a Bastion Host for secure SSH access.
- Configured an Application Load Balancer with healthy target groups.
- Applied AWS networking best practices for scalability and security.

---

# 🚀 Future Improvements

- Deploy Amazon RDS (3-Tier Architecture)
- Configure Auto Scaling Groups
- Add NAT Gateway
- Integrate Amazon Route 53
- Configure Amazon CloudFront
- Protect the application with AWS WAF
- Monitor infrastructure using Amazon CloudWatch
- Provision infrastructure using Terraform
- Build a CI/CD pipeline with GitHub Actions

---

# 👨‍💻 Author

**Rushikesh Chorge**

Aspiring AWS Cloud & DevOps Engineer

---

⭐ **If you found this project useful, feel free to star this repository.**
