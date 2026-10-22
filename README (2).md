# AWS Three-Tier Architecture

## Overview

This project implements a Three-Tier Architecture on AWS to demonstrate cloud infrastructure deployment, networking, load balancing, auto scaling, and database connectivity.

The architecture separates the infrastructure into three layers: Web Tier, Application Tier, and Database Tier.

## AWS Services Used

- **Amazon VPC:** Creates an isolated virtual network.
- **Public and Private Subnets:** Organize resources based on network accessibility.
- **Amazon EC2:** Hosts the web and application workloads.
- **Application Load Balancer (ALB):** Distributes incoming traffic across registered targets.
- **Auto Scaling:** Adjusts the number of EC2 instances according to configured policies.
- **Amazon RDS:** Provides managed relational database functionality.
- **MySQL:** Database management system.
- **Security Groups:** Control inbound and outbound traffic.

## Architecture

1. **Web Tier:** Receives incoming application traffic through the Application Load Balancer.
2. **Application Tier:** Processes requests using EC2 instances, with Auto Scaling configured for capacity management.
3. **Database Tier:** Stores application data using the configured MySQL database service.

The tiers are separated using VPC networking, subnets, and Security Groups.

## Implementation Steps

1. Created an Amazon VPC and configured public and private subnets.
2. Configured network routing and connectivity.
3. Launched and configured EC2 instances.
4. Created an Application Load Balancer and configured its target group.
5. Configured an Auto Scaling Group for EC2 instances.
6. Configured MySQL database connectivity using the database service deployed for the project.
7. Configured Security Groups to control communication between the tiers.
8. Verified application access and connectivity between infrastructure components.

## Security

- Restricted access using Security Groups.
- Limited database access to authorized resources.
- Used subnet separation to isolate internal resources.
- Avoided exposing database services directly to the public internet.

## Key Concepts Learned

- AWS VPC and subnet configuration
- EC2 instance management
- Application Load Balancer configuration
- Auto Scaling Groups
- Amazon RDS and MySQL connectivity
- Security Groups and network access control
- Three-Tier Architecture design

## Author

**Payal Ahire**

GitHub: [payalahire04](https://github.com/payalahire04)
