# Task 2 — EC2 Static Website Hosting with Nginx

## 1. Explanation of Setup
I launched a **t2.micro EC2 instance** in the **public subnet** created earlier.  
After configuring a Security Group allowing HTTP (80) and SSH (22), I installed **Nginx** and uploaded my static resume website to `/var/www/html`.  
For basic security hardening, I disabled password-based SSH login, restricted inbound rules, enabled automatic updates, and used least-privilege access.  
The resume is now accessible publicly from the instance’s public IPv4 address on port 80.

---

## 2. Required Screenshots
- EC2 instance running  
- Security Group inbound rules  
- Website opened in browser  

---

## 3. GitHub Code
This folder contains:
- Terraform file provisioning EC2 + Security Groups  
- User data script to install Nginx and deploy resume  

