# AWS Project 1b: Secure and Scalable Web Application Infrastructure

## 🚀 Objective

To create a secure and scalable web application infrastructure on AWS by leveraging services like VPC, Subnets, Route Tables, Network ACLs, Internet Gateway, EC2 Instances, VPN, Transit Gateway, NAT Gateway, Route 53, Elastic Load Balancer (ELB), and Auto Scaling Group. This project demonstrates a well-architected environment for hosting a web application.

---

## 🧰 Services Used

- **Networking**: VPC, Subnets, Route Tables, Network ACLs, Internet Gateway, VPN, Transit Gateway, NAT Gateway  
- **Compute**: EC2 Instances  
- **Scalability**: Elastic Load Balancer (ELB), Auto Scaling Group  
- **Domain Management**: Route 53  

---

## ✅ Prerequisites

- An active AWS account  
- Basic knowledge of AWS services  
- Familiarity with AWS Management Console and CLI  
- AWS CLI installed on your local machine  
- Basic understanding of networking concepts (CIDR, Subnets, NAT, etc.)

---

## 🛠️ Project Steps

1. **Create a Custom VPC**
   - VPC CIDR block: `10.0.0.0/16`

2. **Create Subnets**
   - Public Subnets: `10.0.1.0/24`, `10.0.2.0/24`
   - Private Subnets: `10.0.3.0/24`, `10.0.4.0/24`

3. **Configure Route Tables**
   - Public route table with IGW
   - Private route table with NAT Gateway

4. **Configure Network ACLs (NACL)**
   - Inbound/Outbound rules for public and private subnets

5. **Attach Internet Gateway (IGW)**

6. **Launch EC2 Instances**
   - 1 public instance (web app)
   - 1 private instance (backend/database)

7. **Set Up NAT Gateway**
   - For outbound internet access from private subnets

8. **Configure VPN and Transit Gateway**
   - Simulate hybrid cloud setup
   - Enable routing across multiple VPCs (if required)

9. **Configure Route 53**
   - Create hosted zone
   - Point domain to ALB DNS

10. **Set Up Elastic Load Balancer (ALB)**
    - Associate with public subnets
    - Forward traffic to public EC2 instance

11. **Enable Auto Scaling**
    - Configure Auto Scaling Group for EC2 in public subnet
    - Define scaling policies based on traffic

12. **Test the Setup**
    - Deploy basic HTML app on public EC2 instance
    - Access app via custom domain

---

## 🎯 Outcome

- A secure, scalable, and modular AWS infrastructure
- Public-facing web app with domain name via Route 53
- Load-balanced and auto-scaled EC2 instances
- Backend services secured in private subnets with controlled internet access
- Simulated hybrid cloud using VPN and Transit Gateway

---


