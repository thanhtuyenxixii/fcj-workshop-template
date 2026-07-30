---
title: "Week 10: End-to-End AI Service Integration"
date: 2026-08-03
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

## 03/08/2026 - 09/08/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS Documentation.

## Objective

Connect API Gateway and AWS Lambda with the deployed SageMaker Endpoint to form a complete, end-to-end AI scoring web pipeline.

## Context

Week 10 focused on joining all individual components built over previous weeks into a unified cloud system: `Client -> API Gateway -> Lambda -> SageMaker Endpoint -> S3/CloudWatch`.

## AWS Learning Focus

- **Lambda Boto3 SageMaker Runtime:** Invoking `sagemaker-runtime` `invoke_endpoint()` inside Python Lambda.
- **Request/Response Transformation:** Parsing incoming client JSON, extracting features, formatting endpoint payloads, and returning structured risk levels (`LOW`, `MEDIUM`, `HIGH`).
- **IAM Policy Integration:** Granting Lambda explicit `sagemaker:InvokeEndpoint` permissions.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 03/08/2026 | Updated Lambda function code to import `boto3` SageMaker Runtime client. |
| 04/08/2026 | Added `sagemaker:InvokeEndpoint` permissions to Lambda's IAM Execution Role. |
| 05/08/2026 | Implemented payload formatting and risk threshold classification (`LOW`/`MED`/`HIGH`) in Lambda. |
| 06/08/2026 | Connected API Gateway `POST /eval-risk` directly to the updated Lambda function. |
| 07/08/2026 | Executed End-to-End integration tests using Postman with sample AI agent logs. |
| 08/08/2026 - 09/08/2026 | Verified raw log archiving in S3 and execution logging in CloudWatch. |

## Technical Activities

- Integrated API Gateway, Lambda, and SageMaker Real-Time Endpoint.
- Processed AI Agent trajectory payloads in real time and generated structured risk evaluation responses.

## Deliverables

- **End-to-End AI Risk Scoring Pipeline fully functional.**
- **Lambda-to-SageMaker Boto3 bridge implemented.**
- **Integrated Postman test suite passing 100%.**

## Challenge and Solution

**Challenge:** High latency when Lambda invoked the SageMaker Endpoint on cold starts.

**Solution:** Optimized Lambda memory allocation (increased to 1024MB) and reused the Boto3 client connection outside the main handler.

## Project Relevance

Delivers the final working MVP, allowing external applications to query risk evaluations of AI Coding Agent actions via a single API call.


## Evidence and References Studied

- [Invoke SageMaker Endpoints using AWS Lambda](https://aws.amazon.com/blogs/machine-learning/call-an-amazon-sagemaker-model-endpoint-from-an-aws-lambda-function/)
- [AWS SDK for Python (Boto3) SageMaker Runtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html)

---

[Back to Worklog](/1-worklog/) | [Next](/1-worklog/1.11-week11/)
