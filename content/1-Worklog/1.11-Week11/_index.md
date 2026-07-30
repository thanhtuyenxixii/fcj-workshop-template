---
title: "Week 11: CloudWatch Monitoring, Security & Cost Optimization"
date: 2026-08-10
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

## 10/08/2026 - 16/08/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS Documentation.

## Objective

Set up operational visibility with Amazon CloudWatch Alarms/Dashboards, conduct a security audit, and apply cost optimization measures across all deployed services.

## Context

With the system fully integrated, Week 11 focused on production readiness: monitoring operational health, catching errors automatically, and controlling cloud expenditure.

## AWS Learning Focus

- **Amazon CloudWatch Dashboards & Alarms:** Metrics tracking (API latency, Lambda errors, SageMaker invocation counts, CPU utilization).
- **Cost Optimization Strategies:** AWS Cost Explorer analysis, S3 Lifecycle policies, and Endpoint instance right-sizing.
- **Cloud Security Audit:** Verifying IAM policies and ensuring no public S3 access or exposed API keys exist.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 10/08/2026 | Configured CloudWatch Log Groups for API Gateway, Lambda, and SageMaker. |
| 11/08/2026 | Created CloudWatch Alarms for Lambda error rate (>5%) and API latency (>2s). |
| 12/08/2026 | Built a unified CloudWatch Operational Dashboard for real-time monitoring. |
| 13/08/2026 | Analyzed AWS Cost Explorer metrics and identified cost optimization opportunities. |
| 14/08/2026 | Configured auto-deletion scripts for unused SageMaker Endpoints after testing hours. |
| 15/08/2026 - 16/08/2026 | Completed IAM security audit verifying all credentials and policy boundaries. |

## Technical Activities

- Constructed a custom CloudWatch Dashboard displaying system throughput, error rates, and latency.
- Set up SNS Email Notifications triggered by CloudWatch Alarms.
- Right-sized SageMaker instances to lower student account expenses.

## Deliverables

- **Amazon CloudWatch Dashboard operational.**
- **CloudWatch Alarms & SNS Email Alerts active.**
- **AWS Cost Explorer optimization report completed.**

## Challenge and Solution

**Challenge:** High recurring daily costs driven by idle SageMaker Real-Time Endpoints.

**Solution:** Implemented a Lambda scheduled event (via EventBridge) to delete the endpoint during off-hours and re-create it before testing.

## Project Relevance

Ensures the project adheres to AWS Well-Architected Framework pillars for Operational Excellence, Security, and Cost Optimization.


## Evidence and References Studied

- [Amazon CloudWatch User Guide](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html)
- [AWS Cost Optimization Pillar](https://docs.aws.amazon.com/wellarchitected/latest/cost-optimization-pillar/welcome.html)

---

[Back to Worklog](/1-worklog/) | [Next](/1-worklog/1.12-week12/)
