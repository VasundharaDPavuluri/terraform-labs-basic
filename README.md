# Terraform Labs Basic

This repository contains beginner-to-intermediate Terraform hands-on projects focused on AWS Infrastructure as Code (IaC).

The labs cover:
- Terraform basics
- AWS provider configuration
- EC2 provisioning
- VPC networking
- Public and Private Subnets
- Security Groups
- Route Tables
- Internet Gateway
- Terraform Variables
- Infrastructure automation concepts

---

# Repository Purpose

This repository is created for learning and practicing:
- Terraform fundamentals
- AWS infrastructure provisioning
- Networking concepts
- Real-time infrastructure flow
- Infrastructure modular thinking

---

# Technologies Used

- Terraform
- AWS CLI
- Amazon EC2
- AWS VPC
- Git & GitHub
- VS Code

---

# Repository Structure

```text
terraform-labs-basic/
│
├── terraform-basic-handson/
├── terraform-vpc-handson/
├── terraform-vpc-ec2-project/
└── README.md
```

---

# Projects Overview

## Project-1 — Terraform Basic Hands-On

### Topics Covered
- Terraform installation
- AWS CLI configuration
- IAM User setup
- EC2 provisioning
- Key Pair integration
- Security Group basics
- Terraform lifecycle commands

### Key Learnings
- Infrastructure as Code (IaC)
- Terraform workflow
- AWS authentication
- EC2 provisioning

---

## Project-2 — Terraform VPC Hands-On

### Topics Covered
- VPC creation
- Public and Private Subnets
- Internet Gateway
- Route Tables
- Route Table Associations

### Key Learnings
- AWS networking basics
- Public vs Private Subnets
- Internet routing
- VPC communication flow

---

## Project-3 — Terraform VPC EC2 Project

### Topics Covered
- Custom VPC
- Public Subnet
- Security Groups
- EC2 inside custom VPC
- Terraform Variables
- Infrastructure dependency mapping

### Project Structure

```text
terraform_project/
├── provider.tf
├── variables.tf
├── vpc.tf
├── subnet.tf
├── security-group.tf
├── ec2-instance.tf
├── outputs.tf
```

---

# Terraform Files Explained

| File | Purpose |
|---|---|
| provider.tf | AWS provider configuration |
| variables.tf | Define reusable input variables |
| vpc.tf | Create VPC and networking |
| subnet.tf | Create public/private subnets |
| security-group.tf | Configure firewall rules |
| ec2-instance.tf | Provision EC2 instance |
| outputs.tf | Display resource outputs |

---

# Variables in Terraform

Variables are used to make Terraform code:
- reusable
- dynamic
- configurable

Instead of hardcoding values directly:

```hcl
instance_type = "t2.micro"
```

Terraform variables allow:

```hcl
instance_type = var.instance_type
```

This helps reuse the same code across:
- Dev
- QA
- Production

environments.

---

# Terraform Workflow

## Initialize Terraform

```bash
terraform init
```

Downloads required provider plugins.

---

## Format Terraform Code

```bash
terraform fmt
```

Formats Terraform files.

---

## Validate Terraform Configuration

```bash
terraform validate
```

Validates Terraform syntax.

---

## Review Infrastructure Changes

```bash
terraform plan
```

Displays infrastructure changes before deployment.

---

## Provision Infrastructure

```bash
terraform apply
```

Creates AWS infrastructure.

---

## Destroy Infrastructure

```bash
terraform destroy
```

Deletes Terraform-managed resources.

---

# Real-Time Architecture Flow

```text
Users
  ↓
Internet
  ↓
Internet Gateway
  ↓
Public Route Table
  ↓
Public Subnet
  ↓
Frontend / EC2
  ↓
Private VPC Communication
  ↓
Private Subnet
  ↓
Backend / Database
```

---

# Key AWS Networking Concepts

| Component | Purpose |
|---|---|
| VPC | Application network |
| Public Subnet | User-facing resources |
| Private Subnet | Internal secure resources |
| Internet Gateway | Internet access |
| Route Table | Traffic routing |
| Security Group | Instance firewall |
| NAT Gateway | Outbound internet for private subnet |

---

# Learning Outcomes

This repository helps understand:
- Infrastructure as Code (IaC)
- Terraform fundamentals
- AWS networking
- EC2 provisioning
- Resource dependencies
- Security Groups
- Route Tables
- Terraform Variables
- Infrastructure automation

---

# Future Enhancements

Planned advanced topics:
- Terraform Modules
- Remote Backend (S3 + DynamoDB)
- ALB (Application Load Balancer)
- Auto Scaling
- NAT Gateway
- RDS Integration
- Jenkins CI/CD
- EKS Terraform deployment

---
