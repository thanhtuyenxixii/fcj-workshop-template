---
title: "Week 1: Onboarding and AWS Foundation"
date: 2026-06-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

## 01/06/2026 - 07/06/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS documentation, tutorials, and peer discussions.

## Objective

Understand internship expectations, select the technical project topic, and establish the core AWS foundational knowledge needed for cloud-native deployment.

## Context

The first week was dedicated to transitioning into the AWS First Cloud AI Journey bootcamp structure. With a self-managed learning style, defining weekly goals, maintaining worklog evidence, and structuring the report were prioritized early.

## AWS Learning Focus

- **AWS Global Infrastructure:** Studied Regions and Availability Zones to ensure consistent single-Region resource allocation (`ap-southeast-1`).
- **AWS IAM & Security:** Reviewed users, groups, roles, policy JSON structure, and the least-privilege principle.
- **Shared Responsibility Model:** Analyzed security boundaries between AWS infrastructure management and customer resource configurations.
- **Amazon S3 & CloudWatch Overview:** Explored bucket architecture, object prefixes, and CloudWatch operational logging.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 01/06/2026 | Reviewed internship requirements and established the 12-week report structure. |
| 02/06/2026 | Studied AWS Global Infrastructure, Regions, AZs, and CLI configurations. |
| 03/06/2026 | Reviewed IAM policies, execution roles, and the AWS Shared Responsibility Model. |
| 04/06/2026 | Selected the AI Coding Agent Risk Scoring project direction. |
| 05/06/2026 | Drafted the initial MVP architecture (S3, SageMaker, Lambda, API Gateway). |
| 06/06/2026 - 07/06/2026 | Organized technical notes, reference links, and initial Worklog evidence. |

## Technical Activities

- Analyzed internship deliverables and set up the Hugo report structure.
- Configured AWS CLI, credentials, and budget alerts on the AWS student account.
- Defined the high-level system service chain: S3 for data, SageMaker for model execution, Lambda and API Gateway for API delivery.

## Deliverables

- **Internship topic selected: AI Coding Agent Risk Scoring.**
- **Initial report outline created.**
- **High-level cloud service map drafted.**

## Challenge and Solution

**Challenge:** Selecting an AI/Cloud project scope that is technically meaningful yet feasible on a student AWS account.

**Solution:** Scoped the MVP strictly to risk-scoring agent execution logs, deferring complex multi-account infrastructure to future phases.

## Project Relevance

Establishes the initial cloud design for processing AI coding agent logs and serving risk evaluations through an AWS ML pipeline.


## Evidence and References Studied

- [AWS Cloud Practitioner Essentials](https://aws.amazon.com/training/digital/aws-cloud-practitioner-essentials/)
- [AWS IAM Best Practices](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)

---

[Back to Worklog](/1-worklog/) | [Next](/1-worklog/1.2-week2/)
