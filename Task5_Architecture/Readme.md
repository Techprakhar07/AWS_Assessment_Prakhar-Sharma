# Task 5 — AWS Scalable Architecture Diagram (10,000 Concurrent Users)

## 1. Architecture Explanation (5–8 lines)
This design uses an **Application Load Balancer (ALB)** in public subnets to distribute traffic across an **Auto Scaling Group** deployed in private subnets.  
A **multi-tier VPC architecture** separates public, application, and database layers for enhanced security.  
**Amazon RDS/Aurora** provides a scalable and fault-tolerant database backend, while **ElastiCache Redis** improves application performance through caching.  
Security Groups, NACLs, and AWS WAF protect the system against external attacks.  
CloudWatch handles monitoring, logging, metrics, and alerts.  
The architecture is fully elastic and supports 10,000+ concurrent users.

---

## 2. Included Files
- `architecture.png` 
