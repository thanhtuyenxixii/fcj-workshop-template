---
title: "Week 6: ECS Fargate Deployment & CI/CD Automation"
date: 2026-07-06
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

## 06/07/2026 - 12/07/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS Documentation.

## Objective

Deploy the containerized evaluator onto Amazon ECS Fargate and automate build/deployment pipelines via Azure DevOps / GitHub Actions.

## Context

Week 6 focused on executing serverless containers. Instead of managing EC2 clusters, Amazon ECS with AWS Fargate was used to run evaluation tasks on demand.

## AWS Learning Focus

- **Amazon ECS Architecture:** Task Definitions, IAM Task Execution Roles, Services, and Clusters.
- **AWS Fargate:** Serverless compute engine for container orchestration.
- **CI/CD Integration:** Automated pipelines pushing builds to ECR and triggering ECS task updates.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 06/07/2026 | Created ECS Task Definition referencing the ECR image with resource limits (0.5 vCPU, 1GB RAM). |
| 07/07/2026 | Provisioned an ECS Cluster and deployed the service on AWS Fargate in private subnets. |
| 08/07/2026 | Configured Azure DevOps / GitHub Actions pipeline for automated testing. |
| 09/07/2026 | Automated ECR image pushing and ECS service redeployment upon Git commits. |
| 10/07/2026 | Verified automated rolling updates and container health checks. |
| 11/07/2026 - 12/07/2026 | Collected CI/CD pipeline run logs and updated documentation. |

## Technical Activities

- Created ECS Task Definition with environment variables pointing to S3 buckets.
- Configured a CI/CD pipeline triggered by Git pushes that builds Docker images and updates ECS.

## Deliverables

- **Amazon ECS Cluster running on Serverless Fargate.**
- **Automated CI/CD Pipeline fully operational.**
- **Zero-downtime rolling update deployment verified.**

## Challenge and Solution

**Challenge:** Container tasks failing to launch in private subnets due to missing image pull access.

**Solution:** Ensured NAT Gateway routing was active and attached ECR VPC Endpoints to private subnets.

## Project Relevance

Enables automated, serverless container execution whenever new model updates or code changes are committed.


## Evidence and References Studied

- [Amazon ECS Developer Guide](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/Welcome.html)
- [AWS Fargate Overview](https://aws.amazon.com/fargate/)

---

[Back to Worklog](/1-worklog/) | [Next](/1-worklog/1.7-week7/)
