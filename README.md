Project Title : BootsGalore-Cloud-Migration-Site

The BootsGalore Migration Project is a real-world inspired cloud engineering project that simulates migrating a traditional web application into modern AWS three-tier cloud architecture.The project demonstrates how critical cloud concepts such as high availability, scalabaility and security can be applied in practice. 

For illustration purposes, a WordPress site "bootsgalore.shop" (test site) was used as the application layer. While the actual demo site was hosted outside of AWS, the cloud infrastrucutre was fully provisioned and configured to show how the migration would work in a production-grade environment. 

This project reflects my ability to Plan, Design the architecture and implement cloud solutions. 

What This Project Demonstrates:

1.) VPC Networking: Custom VPC with both public and private subnets, internet gateway, and route tables.

2.) Compute Layer (EC2): Public-facing EC2 instances prepared for WordPress hosting, Auto Scaling Group for scalability.

3.) Database Layer (RDS): Amazon RDS (MySQL) deployed in private subnets with Multi-AZ for high availability.

4.) Storage: Amazon S3 for static content, media, and backups.

5.) Load Balancing: Application Load Balancer (ALB) distributing traffic across EC2 instances.

6.) Security: IAM roles with least-privilege, security groups for EC2, RDS, and ALB.

7.) Monitoring: CloudWatch alarms for CPU utilization, Auto Scaling health checks, and RDS monitoring.

8.) Domain Management: Route 53 configured for bootsgalore.shop. Domain remained mapped to the demo site for presentation, but AWS DNS integration was provisioned.

Why This Project Matters : 

This project demonstrates a cloud migration scenario, one of the most common enterprise use cases. It showcases not only cloud resource setup but also:

Availability → Multi-AZ RDS and ALB ensure redundancy.

Scalability → Auto Scaling group tied to CloudWatch alarms.

Security → Public/private subnet isolation, IAM least privilege, and fine-grained SG rules.

Cost Awareness → Transparent decision-making when balancing between full AWS hosting vs. demo hosting.

Architecture Diagram : This Diagram shows the overall flow of the Cloud Migration Site Project: 
<img width="3100" height="2060" alt="image" src="https://github.com/user-attachments/assets/766cb03c-fe1d-481a-ba2b-c81ad29e9f96" />







