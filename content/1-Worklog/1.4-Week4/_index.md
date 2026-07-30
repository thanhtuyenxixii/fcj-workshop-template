---
title: "Week 4: Serverless API Pipeline with Lambda & API Gateway"
date: 2026-06-22
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

## 22/06/2026 - 28/06/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS Documentation.

## Objective

Develop a serverless API ingestion pipeline using Amazon API Gateway and AWS Lambda to collect AI Agent execution logs.

## Context

Week 4 created the entry point for external AI coding agent execution events. The goal was to build a lightweight HTTP API endpoint that validates JSON payloads and stores raw agent logs into S3.

## AWS Learning Focus

- **AWS Lambda Function Development:** Written in Python 3.11 using `boto3` to handle JSON payloads.
- **Amazon API Gateway:** Configured REST API resources, Lambda Proxy Integration, Request Validation, and CORS.
- **Amazon CloudWatch Logs:** Configured automated execution logs and error tracking.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 22/06/2026 | Defined the JSON schema for AI Agent execution trajectory logs. |
| 23/06/2026 | Developed the Python Lambda function `agent-risk-ingest-fn`. |
| 24/06/2026 | Created the API Gateway REST API with resource `POST /score`. |
| 25/06/2026 | Configured Lambda Proxy Integration and CORS headers. |
| 26/06/2026 | Granted S3 write permissions to the Lambda IAM Execution Role. |
| 27/06/2026 - 28/06/2026 | Executed Postman integration tests and verified CloudWatch logs. |

## Technical Activities

- Built an API Gateway REST API connected to AWS Lambda.
- Implemented payload validation logic in Python to filter malformed execution logs before saving to S3.
- Enabled CloudWatch Log Groups for API Gateway and Lambda execution tracing.

## Deliverables

- **Serverless Ingestion API live (`POST /score`).**
- **Python Ingestion Lambda Function operational.**
- **Postman API test suite verified.**

## Challenge and Solution

**Challenge:** Handling CORS errors when invoking API Gateway from external test environments.

**Solution:** Configured CORS options in API Gateway and explicitly returned `Access-Control-Allow-Origin` headers in the Lambda response object.

## Project Relevance

Serves as the front door for receiving agent behavior data, feeding the downstream ML risk scoring pipeline.

## Evidence and References Studied

- [AWS Lambda Developer Guide](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)
- [Amazon API Gateway Guide](https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html)

---

[Back to Worklog](/1-worklog/) | [Next](/1-worklog/1.5-week5/)
