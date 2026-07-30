---
title: "Week 5: Containerization with Docker & Amazon ECR"
date: 2026-06-29
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

## 29/06/2026 - 05/07/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS Documentation.

## Objective

Containerize the AI Agent Risk Scoring evaluation microservice using Docker and push image artifacts to Amazon ECR.

## Context

To ensure consistent runtime environments across local development and AWS cloud deployments, Week 5 focused on packaging the Python evaluation code, PyTorch dependencies, and feature extraction scripts into Docker containers.

## AWS Learning Focus

- **Dockerization Best Practices:** Multi-stage builds, minimal base images (Python Slim), and dependency caching.
- **Docker Compose:** Multi-container orchestration for local integration testing.
- **Amazon ECR:** Private registry setup, IAM authentication via AWS CLI, and image tagging strategies.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 29/06/2026 | Structured Python dependencies (`torch`, `boto3`, `scikit-learn`) for containerization. |
| 30/06/2026 | Authored optimized Dockerfile for the Risk Scoring Engine. |
| 01/07/2026 | Built and verified Docker containers locally using Docker Compose. |
| 02/07/2026 | Created private Amazon ECR repository `ai-agent-risk-evaluator`. |
| 03/07/2026 | Authenticated local Docker CLI with ECR and pushed container images. |
| 04/07/2026 - 05/07/2026 | Verified image vulnerability scanning results in ECR. |

## Technical Activities

- Created a multi-stage Dockerfile reducing final image size.
- Pushed container tags (`v1.0.0`, `latest`) to Amazon ECR via AWS CLI.

## Deliverables

- **Optimized Dockerfile for Risk Scoring Engine.**
- **Private Amazon ECR Repository active.**
- **Container image published to ECR.**

## Challenge and Solution

**Challenge:** Large image size caused by heavy PyTorch/CUDA dependencies.

**Solution:** Switched to CPU-only PyTorch base images and multi-stage builds, reducing image footprint significantly.

## Project Relevance

Prepares portable container artifacts required for scalable serverless container execution on ECS Fargate.


## Evidence and References Studied

- [Docker Documentation](https://docs.docker.com/)
- [Amazon ECR User Guide](https://docs.aws.amazon.com/AmazonECR/latest/userguide/what-is-ecr.html)

---

[Back to Worklog](/1-worklog/) | [Next](/1-worklog/1.6-week6/)
