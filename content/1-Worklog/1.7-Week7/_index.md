---
title: "Week 7: Application Load Balancer & High Availability"
date: 2026-07-13
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

## 13/07/2026 - 19/07/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS Documentation.

## Objective

Configure an Application Load Balancer (ALB) and Auto Scaling policies to ensure high availability and fault tolerance for the scoring service.

## Context

To handle unpredictable evaluation traffic spikes, Week 7 focused on distributing incoming requests across healthy container tasks and scaling capacity automatically.

## AWS Learning Focus

- **Application Load Balancer (ALB):** Listener rules, Target Groups, Health Checks, and SSL/TLS termination concepts.
- **Target Tracking Scaling:** Scaling container tasks dynamically based on average CPU utilization or request count per target.
- **Fault Tolerance:** Testing AZ failure resilience.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 13/07/2026 | Provisioned an Application Load Balancer across Public Subnets. |
| 14/07/2026 | Configured Target Groups pointing to ECS Fargate tasks with HTTP health checks. |
| 15/07/2026 | Configured Target Tracking Auto Scaling policies (CPU target 70%). |
| 16/07/2026 | Simulated high traffic loads to verify automatic task scale-out. |
| 17/07/2026 | Verified scale-in behavior when traffic normalized. |
| 18/07/2026 - 19/07/2026 | Collected metrics and updated network/scaling diagrams. |

## Technical Activities

- Set up ALB routing HTTP traffic to ECS Fargate Target Groups.
- Tested Auto Scaling by stressing the API endpoint, observing task count expansion from 1 to 4.

## Deliverables

- **Application Load Balancer active with Health Checks.**
- **Target Tracking Auto Scaling policy configured.**
- **High availability and load test evidence documented.**

## Challenge and Solution

**Challenge:** Unhealthy Target Group status during initial ALB setup.

**Solution:** Adjusted health check paths (`/health`) and matched container port mappings in the ECS Task Definition.

## Project Relevance

Guarantees the API layer remains responsive even when receiving multiple concurrent evaluation requests.


## Evidence and References Studied

- [Elastic Load Balancing Guide](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html)
- [Target Tracking Scaling Policies](https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-scaling-target-tracking.html)

---

[Back to Worklog](/1-worklog/) | [Next](/1-worklog/1.8-week8/)
