---
title: "Week 2: VPC Networking & IAM Security Setup"
date: 2026-06-08
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

## 08/06/2026 - 14/06/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS Documentation.

## Objective

Design and implement a custom VPC network topology and configure isolated IAM Execution Roles for AI/ML services.

## Context

Following onboarding, Week 2 focused on isolating network infrastructure and configuring access control before deploying any compute or machine learning services.

## AWS Learning Focus

- **Amazon VPC Subnetting:** Calculated CIDR blocks (`10.0.0.0/16`) across multiple AZs.
- **Routing & Gateways:** Configured Internet Gateways for public subnets and NAT Gateways for private outbound connections.
- **Security Groups vs. NACLs:** Implemented stateful Security Groups for compute resources and stateless NACLs for subnets.
- **Service Roles:** Authored IAM trust policies allowing SageMaker and Lambda to access S3 data securely.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 08/06/2026 | Designed custom VPC IP CIDR blocks and multi-AZ subnet layout. |
| 09/06/2026 | Created custom VPC, 2 Public Subnets, and 2 Private Subnets in `ap-southeast-1`. |
| 10/06/2026 | Attached Internet Gateway, provisioned NAT Gateway, and updated Route Tables. |
| 11/06/2026 | Configured Security Groups for private application tiers and internal endpoints. |
| 12/06/2026 | Created IAM Roles (`SageMaker-Execution-Role`, `Lambda-Inference-Role`). |
| 13/06/2026 - 14/06/2026 | Verified private network isolation and created the VPC diagram. |

## Technical Activities

- Built a custom VPC (`10.0.0.0/16`) with Public and Private Subnets in `ap-southeast-1a` and `ap-southeast-1b`.
- Restricted direct inbound internet access to private subnets while permitting outbound package updates via NAT Gateway.
- Created IAM Execution Roles adhering to the Least Privilege principle.

## Deliverables

- **Isolated Custom VPC Deployed.**
- **Route Tables and NAT Gateway Configured.**
- **IAM Execution Roles for Lambda and SageMaker active.**

## Challenge and Solution

**Challenge:** Managing NAT Gateway hourly running costs on a student AWS account.

**Solution:** Automated NAT Gateway deletion/re-creation using AWS CLI scripts outside active testing hours.

## Project Relevance

Protects downstream ML training and evaluation data by ensuring all processing occurs within isolated private subnets.


## Evidence and References Studied

- [Amazon VPC User Guide](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)
- [AWS IAM Policies](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html)

---

[Back to Worklog](/1-worklog/) | [Next](/1-worklog/1.3-week3/)
