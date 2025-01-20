
# Host a Static Website on AWS
## **Project Overview**
### **AWS Resources and Configurations**

1. **Virtual Private Cloud (VPC):** Configured with both public and private subnets across two different Availability Zones for fault tolerance.
2. **Internet Gateway:** Facilitated connectivity between the VPC and the wider Internet.
3. **Security Groups:** Acted as a network firewall to control inbound and outbound traffic.
4. **High Availability:** Leveraged two Availability Zones to enhance system reliability.
5. **Public Subnets:** Hosted infrastructure components like the NAT Gateway and Application Load Balancer.
6. **EC2 Instance Connect Endpoint:** Secured connections to resources in both public and private subnets.
7. **Private Subnets:** Deployed web servers (EC2 instances) for enhanced security.
8. **NAT Gateway:** Allowed private subnets to access the Internet securely.
9. **EC2 Instances:** Hosted the static website files.
10. **Application Load Balancer:** Distributed web traffic evenly to an Auto Scaling Group of EC2 instances across multiple Availability Zones.
11. **Auto Scaling Group:** Managed EC2 instances automatically for scalability, availability, and fault tolerance.
12. **GitHub:** Stored web files for version control and collaboration.
13. **Certificate Manager:** Secured application communications.
14. **Simple Notification Service (SNS):** Configured to alert about activities within the Auto Scaling Group.
15. **Route 53:** Registered the domain name and set up DNS records.

### **Deployment Steps**

1. Clone the repository:
   ```bash
   git clone https://github.com/Godwin-svg/static-website-on-aws
   ```
2. Launch an EC2 instance and install the necessary software using the provided scripts.
3. Deploy the static website files to the EC2 instance.
4. Configure load balancing, scaling, and secure connections as outlined in the repository.
5. Verify the deployment using the domain name registered with Route 53.

### **Features**
- High availability through the use of multiple Availability Zones.
- Scalability and elasticity managed via Auto Scaling Groups.
- Enhanced security with private subnets and SSL/TLS encryption.
- Reliable notifications using AWS SNS.
- Organized version control via GitHub.

### **Getting Started**
Refer to the reference diagram and deployment scripts in the repository to replicate the setup or adapt it for your own use.
---
For more details, visit the [GitHub repository](https://github.com/Godwin-svg/static-website-on-aws).

