# AWS Enterprise Networking Lab

## Project Overview

This project demonstrates the design and implementation of a secure AWS networking environment using enterprise cloud architecture principles.

The infrastructure is deployed inside a custom Amazon VPC with public and private subnets distributed across multiple Availability Zones. It includes an Application Load Balancer, Bastion Host, private EC2 application servers, dedicated route tables, security groups, and an S3 Gateway Endpoint.

The project focuses on secure networking, high availability, scalability, and cloud best practices commonly used in production environments.

---

# Architecture

![Architecture](Architecture/aws-2-tier-architecture.png)

---

# Services Used

- Amazon VPC
- EC2
- Application Load Balancer
- Target Groups
- Internet Gateway
- Route Tables
- Security Groups
- Bastion Host
- S3 Gateway Endpoint
- Amazon Linux
- Apache HTTP Server

---

# Architecture Components

| Component | Purpose |
|-----------|----------|
| VPC | Private Virtual Network |
| Public Subnets | Host internet-facing resources |
| Private Subnets | Host application servers |
| Internet Gateway | Internet connectivity |
| Route Tables | Traffic routing |
| Bastion Host | Secure SSH access |
| ALB | Distribute traffic |
| Target Group | Health monitoring |
| Security Groups | Firewall rules |
| S3 Gateway Endpoint | Private access to S3 |

---

# Security Implementation

- Bastion Host for SSH
- Private Application Servers
- Security Group referencing
- Least Privilege Principle
- Separate Public and Private Subnets

---

# Skills Demonstrated

- AWS Networking
- Amazon VPC
- CIDR Planning
- Route Tables
- Security Groups
- Internet Gateway
- Load Balancing
- Bastion Architecture
- Linux Administration
- Apache Configuration
- High Availability
- Network Troubleshooting

---

# Lessons Learned

- Designing secure AWS networks
- Building production-style VPCs
- Configuring ALB with healthy targets
- Managing private EC2 instances
- Troubleshooting networking issues
- Implementing least-privilege security

---

# Future Improvements

- Amazon RDS
- Auto Scaling Group
- NAT Gateway
- Route 53
- CloudFront
- WAF
- CloudWatch
- Terraform
- CI/CD Pipeline

---

# Author

Rushikesh Chorge

MSc Computer Science

Aspiring AWS Cloud & DevOps Engineer
