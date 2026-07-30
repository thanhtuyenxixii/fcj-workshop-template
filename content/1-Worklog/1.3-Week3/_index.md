---
title: "Week 3: S3 Storage Optimization & VPC Endpoints"
date: 2026-06-15
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

## 15/06/2026 - 21/06/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS Documentation.

## Objective

Set up structured Amazon S3 buckets for AI Agent logs/artifacts and establish private connection paths via S3 VPC Gateway Endpoints.

## Context

Week 3 focused on defining the cloud storage hierarchy for agent trajectory logs and configuring private network access so EC2/SageMaker instances read data without public internet exposure.

## AWS Learning Focus

- **Amazon S3 Architecture:** Organized bucket prefixes (`raw-agent-logs/`, `processed-features/`, `model-artifacts/`).
- **S3 Security:** Enforced Server-Side Encryption (SSE-S3), Bucket Policies, and Block Public Access.
- **S3 VPC Gateway Endpoints:** Routed S3 API calls directly over the internal AWS network backbone.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 15/06/2026 | Provisioned private EC2 Bastion/Host setup for testing isolated subnet operations. |
| 16/06/2026 | Created project S3 bucket with structured prefixes and enabled SSE-S3 encryption. |
| 17/06/2026 | Configured S3 Bucket Policies to restrict access strictly to project IAM roles. |
| 18/06/2026 | Provisioned an S3 VPC Gateway Endpoint and attached it to Private Route Tables. |
| 19/06/2026 | Verified private S3 access from EC2 instances without internet connectivity. |
| 20/06/2026 - 21/06/2026 | Documented S3 storage lifecycle policies and updated network diagrams. |

## Technical Activities

- Created S3 Bucket `ai-agent-risk-data-store-ap-southeast-1` with Versioning and Encryption enabled.
- Attached a Gateway VPC Endpoint to Private Route Tables for zero-internet S3 data transfer.

## Deliverables

- **Encrypted S3 Data Bucket configured.**
- **Private S3 VPC Gateway Endpoint operational.**
- **Verified private S3 file transfer via AWS CLI.**

## Challenge and Solution

**Challenge:** Testing S3 CLI operations from a private instance with no public IP.

**Solution:** Routed traffic through an S3 Gateway Endpoint and verified connectivity via AWS CLI.

## Project Relevance

Establishes a secure data store for AI Coding Agent execution logs that SageMaker and Lambda can access privately.

## Evidence and References Studied

- [Amazon S3 Developer Guide](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)
- [VPC Endpoints for S3](https://docs.aws.amazon.com/vpc/latest/privatelink/vpc-endpoints-s3.html)

---

[Back to Worklog](/1-worklog/) | [Next](/1-worklog/1.4-week4/)
