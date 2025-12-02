# Task 1 — AWS VPC, Subnets, IGW, NAT Gateway Setup

## 1. Explanation of VPC & Subnet Design
I designed a custom VPC named **FirstName_Lastname_VPC** using a /16 CIDR block (10.0.0.0/16) to ensure enough IP space for scaling. Inside the VPC, I created **two public** and **two private subnets** across 2 Availability Zones for high availability.  
An **Internet Gateway (IGW)** provides external connectivity for public subnets, while private subnets use a **NAT Gateway** to access the internet securely without exposing backend servers.  
Separate route tables ensure correct network segmentation following AWS best practices.

---

## 2. CIDR Ranges Used

| Component | CIDR Block | Reason |
|----------|------------|--------|
| VPC | 10.0.0.0/16 | Large address space for future scaling |
| Public Subnet A | 10.0.1.0/24 | Public AZ1 resources |
| Public Subnet B | 10.0.2.0/24 | Public AZ2 resources |
| Private Subnet A | 10.0.3.0/24 | Private AZ1 backend |
| Private Subnet B | 10.0.4.0/24 | Private AZ2 backend |

---

## 3. Required Screenshots
- VPC list  
- Subnets list  
- Route tables  
- Internet Gateway + NAT Gateway  

---

## 4. Terraform / CloudFormation Code
My IaC file (`main.tf` or `template.yaml`) is included inside this folder.

