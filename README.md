# Secure Infrastructure Pipeline

> Terraform + GitHub Actions pipeline for automated, security-scanned AWS deployments

## Problem
AWS infrastructure is ofer deployed in a unsecure way, leading to misconfigurations like public S3 buckets, overly permissive security groups, and unencrypted resources. Which is the start of diasaster. 

## Solution
Automated CI/CD pipeline that scans Terraform code for security issues BEFORE deployment, preventing insecure infrastructure from reaching production.

## Tech Stack
- **Infrastructure as Code:** Terraform
- **CI/CD:** GitHub Actions
- **Security Scanning:** tfsec
- **Cloud Provider:** AWS

## Phase 1 Goals
- [ ] Deploy encrypted S3 bucket using Terraform
- [ ] GitHub Actions workflow that runs `terraform plan`
- [ ] Automated tfsec security scanning on pull requests
- [ ] Block merges if security issues are found

## Roadmap
- **Phase 1:** Basic S3 deployment with security scanning *(current)*
- **Phase 2:** Expand to VPC, security groups, and multiple resource types
- **Phase 3:** Add cost estimation and compliance checks
- **Phase 4:** AI-powered security recommendations using AWS Bedrock

## Status
🚧 Phase 1 in progress - Foundation and tooling setup

---
*Building this as part of my journey to become a Cloud + AI Engineer*

