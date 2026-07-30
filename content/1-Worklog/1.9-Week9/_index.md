---
title: "Week 9: PyTorch Training & SageMaker Endpoint Deployment"
date: 2026-07-27
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

## 27/07/2026 - 02/08/2026

**Work mode:** Individual implementation combined with group-based learning and discussion.
**Program:** Workforce Bootcamp - First Cloud AI Journey.
**Mentor:** Self-managed supported by AWS Documentation.

## Objective

Train the PyTorch Risk Scoring Model using SageMaker Training Jobs and deploy the trained artifact to a SageMaker Real-Time Endpoint.

## Context

Week 9 focused on core MLOps execution: training the PyTorch evaluation model on cloud compute and hosting it as a persistent, low-latency inference endpoint.

## AWS Learning Focus

- **SageMaker PyTorch Estimator:** Configuring training entry points, hyperparameters, and instance types.
- **Model Artifacts:** Saving model weights to S3 (`model.tar.gz`).
- **SageMaker Endpoints:** Configuring Model objects, Endpoint Configurations, and Real-Time Endpoints.
- **SageMaker Boto3 Runtime:** Invoking endpoints programmatically using `invoke_endpoint()`.

## Daily Breakdown

| Date | Work performed |
|---|---|
| 27/07/2026 | Authored PyTorch model training script (`train.py`) and model architecture. |
| 28/07/2026 | Launched a SageMaker Training Job using the PyTorch Estimator (`ml.m5.xlarge`). |
| 29/07/2026 | Verified training convergence and checked output artifacts stored on S3. |
| 30/07/2026 | Created SageMaker Model and Endpoint Configuration (`ml.t2.medium`). |
| 31/07/2026 | Deployed the SageMaker Real-Time Endpoint and verified status `InService`. |
| 01/08/2026 - 02/08/2026 | Tested real-time model inference using Python `boto3` scripts. |

## Technical Activities

- Trained a Neural Network model in PyTorch via SageMaker Estimators.
- Hosted a Real-Time Endpoint (`ai-agent-risk-score-endpoint`) for inference.
- Executed inference test scripts verifying risk score outputs between 0.0 and 1.0.

## Deliverables

- **SageMaker Training Job completed successfully.**
- **Model Artifacts stored in S3.**
- **SageMaker Real-Time Endpoint deployed (`InService`).**
- **Python `boto3` inference test script verified.**

## Challenge and Solution

**Challenge:** Endpoint deployment timeouts caused by missing dependency packages in the inference container.

**Solution:** Added a `requirements.txt` inside the `code/` directory packaged with the model artifact.

## Project Relevance

Provides the core Machine Learning intelligence layer capable of serving real-time risk evaluations for AI Agent actions.


## Evidence and References Studied

- [Deploy Models with SageMaker](https://docs.aws.amazon.com/sagemaker/latest/dg/deploy-model.html)
- [SageMaker PyTorch Container SDK](https://sagemaker.readthedocs.io/en/stable/frameworks/pytorch/using_pytorch.html)

---

[Back to Worklog](/1-worklog/) | [Next](/1-worklog/1.10-week10/)
