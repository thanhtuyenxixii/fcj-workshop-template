---
title: "Week 12: Resource Cleanup, Documentation & Final Review"
date: 2026-08-17
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

## 17/08/2026 - 23/08/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS Documentation and Peer Reviews.

## Objective

Clean up all active AWS cloud resources to prevent ongoing charges, finalize the Hugo internship report, and complete the self-evaluation/feedback sections.

## Context

The final week of the 12-week internship was dedicated to decommissioning active infrastructure safely, compiling final project evidence, and polishing documentation.

## AWS Learning Focus

- **Resource Decommissioning:** Deleting SageMaker Endpoints, ECS Clusters, NAT Gateways, ECR images, and S3 objects safely.
- **Documentation & Retrospective:** Summarizing technical accomplishments, architectural trade-offs, and lessons learned.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 17/08/2026 | Terminated SageMaker Endpoints, Endpoint Configurations, and Models. |
| 18/08/2026 | Deleted ECS Services, Fargate Tasks, ECR Repositories, and NAT Gateways. |
| 19/08/2026 | Emptied and deleted temporary S3 testing buckets and CloudWatch Log Groups. |
| 20/08/2026 | Finalized all Hugo Markdown documentation files across all 8 main report chapters. |
| 21/08/2026 | Completed Section 6 (Self-Evaluation) and Section 7 (Feedback/Mentorship Review). |
| 22/08/2026 - 23/08/2026 | Performed final Hugo static site build check and submitted the internship report. |

## Technical Activities

- Safely decommissioned all billable AWS infrastructure, confirming zero active running resources via AWS Cost Explorer.
- Built and published the final Hugo static documentation site.

## Deliverables

- **Complete 12-Week Internship Worklog published.**
- **All AWS resources cleanly decommissioned.**
- **Final Project Report & Self-Evaluation completed.**

## Challenge and Solution

**Challenge:** Ensuring no orphaned hidden resources (e.g., Elastic IPs, EBS Snapshots) were left running to incur unexpected charges.

**Solution:** Used AWS Resource Groups & Tag Editor alongside AWS Nuke scripts to verify complete account cleanup.

## Project Relevance

Concludes the AWS First Cloud AI Journey internship with a fully documented, production-grade cloud ML architecture and clean resource management.


## Evidence and References Studied

- [AWS Deleting Resources Guide](https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html)
- [Hugo Static Site Generator Docs](https://gohugo.io/documentation/)

---

[Back to Worklog](/1-worklog/)
