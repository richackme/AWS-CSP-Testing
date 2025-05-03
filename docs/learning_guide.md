# 🧭 Cloud Security Learning + Project Build Guide

This guide will help you learn the fundamentals of cloud security while preparing to build a secure AWS environment using Terraform and GitHub.

---

## 🧱 Phase 1: Learn the Foundations

| Topic | What to Learn | Resources |
|------|----------------|-----------|
| **Cloud Fundamentals** | What is a cloud provider (AWS), core services (EC2, VPC, S3), regions, AZs | [AWS Cloud Practitioner Essentials (Free)](https://www.aws.training/Details/Curriculum?id=20685) |
| **Infrastructure as Code (IaC)** | Learn Terraform basics (HCL syntax, resources, state, plans) | [Terraform Learn Guide](https://developer.hashicorp.com/terraform/learn) |
| **VPC & Networking** | VPC, subnets, route tables, NAT gateways, security groups | [AWS VPC Concepts](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) |
| **Security in AWS** | IAM policies, encryption, shared responsibility model | [AWS Security Best Practices](https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/) |
| **CI/CD Basics** | Code deployments, GitHub actions, version control | [GitHub Actions Docs](https://docs.github.com/en/actions) |

---

## 🧪 Phase 2: Practice Small Labs

### 1. Create a VPC with Terraform
- Write a `vpc.tf`
- Add subnets, Internet Gateway, and route tables

### 2. Secure the VPC
- Add security groups with least privilege
- Create IAM roles and policies

### 3. Launch an EC2 Instance
- Use Terraform to provision
- SSH into the instance securely
- Deploy a sample app (even a hello world script)

### 4. Connect GitHub to Terraform
- Push Terraform code to GitHub
- Add `.gitignore` to protect secrets
- Use `.tfvars` for variable management (never commit secrets)

### 5. Add a CI/CD Pipeline
- Use GitHub Actions
- Automatically run `terraform plan` and `terraform apply`
- Make it trigger on pull requests or merges

---

## 🚧 Phase 3: Build Your Final Project

Put it all together into a secure, production-like environment:

- VPC with structured networking
- IAM, secrets, and access control
- Infrastructure organized by folders
- Scripts for provisioning and hardening
- Security assessment tools
- App deployment (basic test app)

---

## 🔐 Bonus: Security Emphasis Topics

| Area | Best Practices |
|------|----------------|
| IAM | Avoid root, enforce MFA, use roles |
| Networking | Public vs private subnets, restrict ports |
| Encryption | Use KMS, encrypt EBS, S3, secrets |
| Auditing | Enable CloudTrail, GuardDuty, AWS Config |
| Secrets Mgmt | Use Secrets Manager or SSM |
| Compliance | Use CIS benchmarks, enable logging and alerts |

---

## ✅ Next Step

1. Go through **Phase 1** and explore the linked resources  
2. Use **Phase 2** to practice and test yourself  
3. Move into **Phase 3** to build your full project

Happy hacking! - richackme
