# azure-terraform-landing-zone
Azure -Infrastructure as Code -Governance mindset
# Azure Terraform Landing Zone

## Overview
This project demonstrates the design and deployment of a secure Azure landing zone using Terraform and Azure DevOps pipelines.

The goal is to showcase Infrastructure as Code, governance, and automation best practices aligned with enterprise environments.

## Architecture
- Azure Resource Group
- Virtual Network with segmented subnets
- Network Security Groups
- Linux Virtual Machine
- Role-Based Access Control (RBAC)

![Architecture](diagrams/architecture.png)

## Technologies Used
- Microsoft Azure
- Terraform (AzureRM Provider)
- Azure DevOps Pipelines (YAML)
- Azure CLI

## Features
- Modular Terraform structure
- Remote Terraform state (Azure Storage)
- CI/CD pipeline with `terraform plan` and `terraform apply`
- Secure access using Azure RBAC
- Environment separation via variables

## How It Works
1. Code is pushed to GitHub
2. Azure DevOps pipeline is triggered
3. Terraform validates and plans infrastructure
4. Manual approval required for apply stage
5. Infrastructure is deployed in Azure

## Lessons Learned
- Managing Terraform state securely
- Designing reusable Terraform modules
- Integrating IaC into CI/CD workflows
- Applying least-privilege RBAC

## Future Improvements
- Add Azure Policy enforcement
- Integrate Azure Key Vault for secrets
- Add monitoring with Azure Monitor
