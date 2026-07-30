---
title: "Self-Assessment"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

## Self-Assessment

During my internship at **Amazon Web Services Viet Nam Company Limited** within the **Workforce Bootcamp - First Cloud AI Journey** program (from **01/06/2026 to 23/08/2026**), I focused on mastering AWS cloud technologies, actively participating in tech events, and engineering a hands-on project: **An End-to-End MLOps Risk Scoring System for AI Coding Agents on AWS SageMaker**.

This internship bridged the gap between academic theory and real-world cloud MLOps workflows. When encountering initial SageMaker Training quota constraints in the `ap-southeast-1` region (requiring a local baseline model for initial comparison), I proactively requested and secured `ml.m5.large` resource quota in `us-east-1`. This enabled me to complete the entire managed pipeline—including Managed Training, HPO, SageMaker Pipelines, Model Registry, and Model Monitor—while successfully provisioning supporting infrastructure such as SageMaker Processing, Real-time Endpoints, AWS Lambda, API Gateway, Data Capture, IAM policies, and CloudWatch observability.

In terms of professional conduct, I maintained strong autonomy while collaborating effectively with my team, reading official AWS documentation, and learning from community workshops. My focus was on establishing solid governance, gathering verifiable evidence, deleting paid resources promptly to control costs, building a bilingual workshop website, and transparently documenting model limitations.

## Performance Evaluation Criteria

| No. | Criteria | Description | Good | Fair | Average |
|:---:|:---|:---|:---:|:---:|:---:|
| 1 | **Technical Knowledge & Skills** | Understanding AWS ecosystem, MLOps lifecycle, API integration, and applying them effectively | ✅ | ☐ | ☐ |
| 2 | **Self-Learning Ability** | Ability to study new AWS services, read technical docs, test CLI commands, and resolve errors | ✅ | ☐ | ☐ |
| 3 | **Proactiveness** | Taking initiative to select a practical project, define MVP scope, and collect operational evidence | ✅ | ☐ | ☐ |
| 4 | **Sense of Responsibility** | Completing all project deliverables, documenting limitations, and practicing cost awareness | ✅ | ☐ | ☐ |
| 5 | **Discipline** | Adhering to the internship timeline, maintaining weekly worklogs, and organizing deliverables | ☐ | ✅ | ☐ |
| 6 | **Growth Mindset** | Openness to feedback, refining technical content, improving diagrams, and updating reports | ✅ | ☐ | ☐ |
| 7 | **Communication Skills** | Clearly explaining project goals, AWS architecture, limitations, and results in English and Vietnamese | ☐ | ✅ | ☐ |
| 8 | **Teamwork** | Engaging in group discussions and community events while completing individual project scope | ☐ | ✅ | ☐ |
| 9 | **Professional Conduct** | Respecting the learning environment, attending events punctually, and using AWS resources responsibly | ✅ | ☐ | ☐ |
| 10 | **Problem-Solving Skills** | Overcoming technical blockers such as quota limits, API integration issues, and post-cleanup evidence | ✅ | ☐ | ☐ |
| 11 | **Project Contribution** | Building a complete MVP solution and creating a reusable workshop-style report website | ✅ | ☐ | ☐ |
| 12 | **Overall Reflection** | Overall assessment of learning attitude, project quality, technical execution, and documentation | ✅ | ☐ | ☐ |

## Core Strengths

- **Strong Technical Autonomy:** Proven ability to learn AWS services independently via official documentation, execute AWS CLI commands, troubleshoot system blockers, and build production-ready pipelines.
- **End-to-End MLOps Execution:** Successfully implemented a managed ML lifecycle on AWS spanning SageMaker Processing, Managed Training, HPO tuning, model evaluation, automated Pipelines, Model Registry versioning, Endpoint inference, and Model Monitoring.
- **Robust Governance & Security:** Configured strict quality gates (`risky_recall >= 0.85`) for model registration; ensured registered versions require manual approval while maintaining deterministic safety rules for decision-making.
- **Observability & Cost Governance:** Successfully integrated Data Capture, Model Monitor, CloudWatch Metrics/Alarms, and custom Dashboards; strictly performed resource cleanup immediately after testing to avoid unnecessary AWS charges.
- **Integrity in Scientific Evaluation:** Rigorously tested the model on out-of-distribution (OOD) external data and transparently reported the performance gap instead of relying solely on perfect synthetic benchmarks.
- **Evidence-Based Documentation:** Retained comprehensive screenshots, raw logs, S3 artifacts, API payload responses, and cleanup records in a clean, structured report.

## Areas for Improvement

- **Verbal Technical Communication:** Continue practicing how to explain complex architectural trade-offs concisely and confidently during live presentations.
- **Artifact Management:** Better distribute screenshot and log collection throughout weekly progress instead of consolidating documentation near final deadlines.
- **Testing Dataset Expansion:** Expand the external evaluation suite beyond small sample sizes by introducing larger, human-annotated datasets for broader validation.
- **Runtime Environment Alignment:** Ensure strict version alignment between training dependencies and inference container runtimes to eliminate serialization warnings.

## Overall Reflection

This internship taught me that a real-world Cloud AI project is far more than just training a model on a local machine. A production-ready solution requires a holistic approach—combining structured data design, IAM security roles, processing infrastructure, serverless API delivery, continuous observability, cost optimization, and meticulous documentation.

The most valuable lesson was understanding that successful pipeline execution differs from model generalization. Completing the AWS MLOps workflow while maintaining transparency about model limitations has laid a strong foundation for my career as a Cloud and MLOps Engineer.
