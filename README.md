Project Title : BootsGalore-Cloud-Migration

The BootsGalore Migration Project is a real-world cloud engineering initiative that demonstrates the migration of a online football store's traditional web application into modern AWS three-tier cloud architecture.

While the live WordPress demo site (bootsgalore.shop) was hosted externally for the presentation, the entire production-grade AWS infrastructure was fully provisioned and configured to validate the complete migration path. This showcases my ability to design, implement and optimize cloud solutions that balance real-world trade-offs in availability, cost and complexity in practical business scenairos. 

What This Project Demonstrates:

1.) VPC Networking: Custom VPC with both public and private subnets, internet gateway, and route tables.

2.) Compute Layer (EC2): Auto Scaling Group across private subnets for elasticity. 

3.) Database Layer (RDS): Amazon RDS (MySQL) deployed in private subnets with Multi-AZ for high availability.

4.) Storage: Amazon S3 for static content, media, and backups.

5.) Load Balancing: Application Load Balancer (ALB) distributing traffic across EC2 instances.

6.) Security: IAM roles with least-privilege, security groups for EC2, RDS, and ALB.

7.) Monitoring: CloudWatch alarms for CPU utilization, Auto Scaling health checks, and RDS monitoring.

8.) Domain Management: Route 53 configured for bootsgalore.shop. Domain remained mapped to the demo site for presentation, but AWS DNS integration was provisioned.

Why This Project Matters : 

This project demonstrates a cloud migration scenario, one of the most common enterprise use cases. It showcases not only cloud resource setup but also:

Availability → Multi-AZ RDS and ALB ensure redundancy.Designed a custom VPC with public and private subnets across multiple Availability Zones and configuring route tables for secure,segmented traffic.

Scalability → Auto Scaling group tied to CloudWatch alarms.

Security → Public/private subnet isolation, IAM least privilege, and fine-grained SG rules.

Cost Awareness → Transparent decision-making when balancing between full AWS hosting vs. demo hosting.

Architecture Diagram : This Diagram shows the overall flow of the Cloud Migration Site Project: 
<img width="3100" height="2060" alt="image" src="https://github.com/user-attachments/assets/766cb03c-fe1d-481a-ba2b-c81ad29e9f96" />

The design follows a 3-Tier Architecture pattern:

1.   Presentation Tier (Web Layer)  
   - Application Load Balancer (ALB)  
   - Route 53 for DNS (bootsgalore.shop)  
   - Auto Scaling Group for web tier availability  

2.   Application Tier (Private EC2)  
   - EC2 instances placed in private subnets  
   - Security groups to restrict direct internet access  
   - Bastion host in public subnet for administrative access  

3.   Database Tier  
   - Amazon RDS (MySQL) in private subnets  
   - Multi-AZ for high availability  
   - Encrypted at rest and in transit  

Supporting services:  
- Amazon S3 → object storage for static assets  
- CloudWatch → monitoring and alarms for EC2, ALB, RDS, and scaling policies  
- VPC + Subnets + Routing → custom networking with public/private isolation  

Tech Stack Used : 
Cloud Services
1.) Amazon VPC, Subnets, Routes Tables, IGW → Custom network design.

2.) Amazon EC2 (Public + Private instances)  + Auto Scaling → Application compute layer.

3.) Amazon RDS (MySQL) → Managed database tier.

4.) Amazon S3 → Static storage for assets and backups.

5.) Amazon Route 53 → Domain management.

6.) AWS IAM/Security Groups → Secure role-based access control.

7.) Amazon CloudWatch → Monitoring and alarms.

Lessons Learned:  
- Importane of networking fundamentals in VPC design
- Trade-offs between demo vs production-ready setups
- Hands-on understanding of AWS Well-Architected Framework principles

Future Improvements:
- Add CI/CD pipeline with CodePipeline + CodeDeploy
- Enable WAF (Web Application Firewall) in front of ALB
- Use CloudFront for global caching and HTTPS termination
- Automate provisioning with CloudFormation

Author : Luyanda Hele ( Cloud Engineer ) 
Email : luyandalui576@gmail.com
Github : luyandahele.github.io
LinkedIn : https://www.linkedin.com/in/luyanda-hele-8999761b4








