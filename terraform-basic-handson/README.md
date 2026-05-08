# Terraform EC2 Provisioning on AWS

This project demonstrates how to provision an EC2 instance on AWS using Terraform.

The hands-on covers:
- Terraform installation
- AWS CLI configuration
- Terraform provider setup
- EC2 resource creation using HCL
- Terraform workflow commands

---

# Technologies Used

- Terraform
- AWS CLI
- Amazon EC2
- Git & GitHub
- Amazon Linux 2023

---

# Project Structure

```text
terraform-basic-handson/
│
├── provider.tf
├── ec2.tf
├── .gitignore
└── README.md
```
---
# Terraform Files
## provider.tf

Defines:
AWS provider
Terraform provider configuration
AWS region

## ec2.tf
Defines:
EC2 instance resource
Instance type
AMI
Tags

## Prerequisites
Before running this project:
AWS Account
IAM User with required permissions
AWS CLI installed
Terraform installed
Git installed

## AWS CLI Configuration
Configure AWS credentials:
aws configure

Provide:
AWS Access Key
AWS Secret Key
Region → ap-south-1
Output format → json

Verify configuration:

aws sts get-caller-identity
Terraform Workflow
Initialize Terraform
terraform init

Downloads required provider plugins.

Format Terraform Code
terraform fmt

Formats Terraform files.

Validate Terraform Code
terraform validate

Validates Terraform syntax.

Review Execution Plan
terraform plan

Displays infrastructure changes before deployment.

Provision Infrastructure
terraform apply

Creates AWS infrastructure.

Destroy Infrastructure
terraform destroy

Deletes created resources.

Outcome
Using Terraform, this project provisions:
One AWS EC2 instance in ap-south-1 region
