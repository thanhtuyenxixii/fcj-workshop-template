---
title: "Sharing and Feedback"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 7. </b> "
---

## Program Reflection & Feedback

This section outlines my personal reflections and constructive feedback following my completion of the **Workforce Bootcamp - First Cloud AI Journey** program at **Amazon Web Services Viet Nam Company Limited**. These insights stem from my hands-on journey studying AWS architecture, engaging in community technical events, and engineering the project: **An End-to-End Risk Scoring and Quality Evaluation System for AI Coding Agents on AWS SageMaker**.

---

## Overall Evaluation

### 1. Learning Environment & Autonomy
The program cultivated an open, highly autonomous learning environment. Participants are empowered to explore AWS services independently, test architectural concepts, read official technical documentation, and turn an initial concept into a functional MVP. This self-directed structure fostered strong personal ownership and problem-solving initiative.

### 2. Program Support & Community Engagement
While the project was self-directed, I benefited greatly from official AWS documentation, technical hands-on workshops, and community events organized by FCAJ. These sessions provided immense value, exposing me to real-world cloud engineering practices across MLOps, Cloud Security, Data Analytics, and Generative AI.

### 3. Alignment with Academic Background
The internship aligned seamlessly with my Computer Science curriculum at university. It enabled me to connect academic concepts—such as software engineering, data structures, machine learning, and API design—into an integrated, enterprise-grade cloud architecture hosted on AWS.

### 4. Skill Enhancement & Growth
- **Technical Competencies:** Gained hands-on proficiency across Amazon S3, SageMaker (Processing, Managed Training, HPO, Pipelines, Model Registry, Real-time Endpoints, Model Monitor), AWS Lambda, API Gateway, IAM Policies, Data Capture, and CloudWatch.
- **Professional Engineering Habits:** Developed strong MLOps governance awareness, cost-control practices, bilingual technical documentation habits, and a rigorous, evidence-based testing methodology.

### 5. Program Culture & Community Spirit
The emphasis on knowledge sharing and community participation was a highlight. Attending technical sessions expanded my perspective beyond a single project, allowing me to learn directly from industry professionals and understand how AWS technologies power real-world production systems and career trajectories.

### 6. Technical Adaptability & Execution
Self-managing a cloud project taught me adaptability when overcoming technical constraints. When facing initial SageMaker Training quota limits in `ap-southeast-1`, I adapted by establishing an interim historical serving pipeline before executing the complete managed workflow upon quota approval in `us-east-1`. This experience taught me to navigate regional resource limitations without sacrificing overall architectural integrity.

---

## Most Satisfying Experience

The most rewarding outcome was delivering a fully operational, governed **End-to-End MLOps Workflow** on AWS. Successfully orchestrating raw agent behavior logs through SageMaker Processing, XGBoost Training, HPO tuning, automated SageMaker Pipelines, quality gating, serverless API Gateway/Lambda integration, and CloudWatch observability was deeply fulfilling.

Equally satisfying was adopting an uncompromised scientific evaluation approach. Rather than over-relying on synthetic training metrics, I rigorously tested the model against external out-of-distribution (OOD) trajectories. Reporting the resulting performance gap reinforced the critical necessity of manual registry approval steps and deterministic safety rules in real-world deployments.

---

## Suggestions for Program Enhancement

1. **Early Quota Onboarding Checklist:** Provide a step-by-step guide during the first week to help students verify and request necessary AWS account quotas (especially for SageMaker Training and Endpoints) early on.
2. **Cost Management Checklist:** Offer a resource cleanup checklist covering paid resources (such as active SageMaker Endpoints or NAT Gateways) to reinforce cost-conscious habits among learners.
3. **Reference Architecture Templates:** Share additional reference architecture diagrams illustrating standard integration patterns between S3, SageMaker, Lambda, and API Gateway for MLOps projects.
4. **Intermediate Review Milestones:** Introduce 1-2 optional milestone check-ins where participants can receive feedback from mentors prior to final report submission.

---

## Program Recommendation

I highly recommend the **First Cloud AI Journey** program to any student aspiring to build a career in Cloud Computing and AI Engineering. It serves as an exceptional bridge for individuals with foundational programming or ML knowledge who wish to understand how production-grade systems are deployed on AWS. While it demands strong self-discipline, that independence is precisely what builds engineering maturity.

---

## Future Roadmap

To further advance the **AI Coding Agent Risk Scorer** project, my future technical roadmap includes:
- Expanding the trajectory collection across diverse real-world agent frameworks with independent human annotations.
- Developing additional data adapters to support emerging AI agent execution formats.
- Fine-tuning decision thresholds, strictly pinning container runtime environments, and establishing canary/rollback deployment pipelines for models that pass manual Registry approval.
