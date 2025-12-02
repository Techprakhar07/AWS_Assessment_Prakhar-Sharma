# Task 3 — High Availability Architecture using ALB + ASG

## 1. Explanation of HA Architecture
I deployed an **Application Load Balancer (ALB)** across two public subnets to ensure multi-AZ availability.  
The web servers were moved into **private subnets**, and an **Auto Scaling Group (ASG)** was created to automatically launch EC2 instances using a Launch Template.  
Traffic now follows this secure path:  
**Internet → ALB → Target Group → EC2 instances (private subnets)**  
The ASG ensures resilience by replacing unhealthy instances and scaling based on load.

---

## 2. Required Screenshots
- ALB listeners + subnets  
- Target Group  
- Auto Scaling Group configuration  
- EC2 Instances launched by ASG  

---

## 3. GitHub Code
This folder includes the Terraform or CloudFormation code to deploy:
- ALB  
- Target Group  
- Launch Template  
- Auto Scaling Group  

