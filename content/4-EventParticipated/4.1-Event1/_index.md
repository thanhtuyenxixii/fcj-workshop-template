---
title: "Event 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

## Event 1: FiRST CLOUD JOURNEY Community Day

| Attribute | Details |
|---|---|
| Event Name | FiRST CLOUD JOURNEY Community Day |
| Date & Time | 09:00 AM, June 06, 2026 |
| Venue | 26th Floor, Bitexco Financial Tower, 02 Hai Trieu, Saigon Ward, Ho Chi Minh City |
| Attending Role | Participant |
| Objective | Tech Knowledge Exchange & Networking |
| Work Shift | Full-time |
| Participant Name | Bùi Thanh Tuyền |
| Academic Institution | Ho Chi Minh City University of Technology (HCMUT) |
| Student ID | 2353284 |

## Overview

The **FiRST CLOUD JOURNEY Community Day** provided an interactive platform where technical experts and learners gathered to explore multiple technology domains, ranging from DevOps, cloud infrastructure, and cybersecurity to game engineering, soft skills, and Generative AI. What made this gathering stand out was its holistic ecosystem perspective: rather than analyzing technologies in isolation, the sessions illustrated how modern software applications integrate cloud infrastructure, automated pipelines, security mechanisms, and AI models into a cohesive production environment.

By participating in this community event, I gained valuable practical insights directly from industry practitioners. These real-world perspectives expanded my technical mindset beyond the scope of my daily internship assignments, offering clear examples of how enterprise-grade AWS solutions and cloud-native practices are engineered in real-world environments.

## Speaker Lineup & Discussion Topics

The conference featured an array of seasoned speakers addressing various specialized areas:

| Speaker | Primary Focus Area |
|---|---|
| Trần Trung Vinh | Career progression from Helpdesk Operations to Cloud & DevOps Specialist |
| Trương Huy Phước | Modern project execution mindsets and dynamic team collaboration |
| Bảo Huỳnh | Containerization fundamentals and application delivery with Docker |
| Lê Hoàng Gia Đại | Next-gen Network Security combining AWS WAF with ML-driven Intrusion Detection |
| Nguyễn Quốc Bảo | Building real-time multiplayer games using Godot 4 and AWS WebSocket services |
| Việt Phát | Advanced GraphRAG architectures utilizing Amazon Bedrock & Amazon Neptune |

## Key Knowledge Takeaways

### Professional Evolution: From IT Support to Cloud/DevOps Engineering

A key highlight was the session detailing a personal career progression from entry-level Helpdesk support to senior System Administration and DevOps engineering. The core takeaway was that long-term career growth relies on persistent continuous learning, regular hands-on experimentation, and deep operational curiosity.

The speaker highlighted several crucial engineering habits:
- Mastering low-level Linux system concepts and networking fundamentals.
- Maintaining detailed operational documentation and runbooks.
- Implementing proactive monitoring frameworks prior to system deployment.
- Strict avoidance of testing changes directly in production environments.

These principles strongly resonated with my internship workflow, reinforcing the necessity of strict validation, cost-aware resource allocation, and systematic logging during AWS development.

### Team Collaboration & Agile Project Execution

Focused on team dynamics, this topic highlighted the difference between individual coding output and collective team velocity. Successful engineering teams require alignment around unified goals, clear domain delegation, active listening, transparent communication, and individual ownership.

Four key team-building pillars were highlighted:
1. Establishing clear, shared project milestones.
2. Aligning tasks with individual technical strengths.
3. Cultivating transparent and constructive dialogue.
4. Upholding personal responsibility for assigned deliverables.

This topic prompted me to re-evaluate my daily team interactions, emphasizing that engineering success involves effective progress tracking, active coordination, and leveraging collaborative tools like Trello, Slack, and Discord to maintain transparency.

### Containerization with Docker

This session unpacked the technical reasons behind containerization as an industry standard for application deployment. In contrast to resource-heavy Virtual Machines, containers offer lightweight, fast-starting, and highly portable application environments. By encapsulating code along with its runtime, system libraries, and settings, Docker eliminates cross-environment configuration issues.

The presentation covered core container primitives, including Dockerfile configuration, layer caching strategies, image optimization, multi-stage builds, networking setups, and persistent storage volumes. This deepened my technical grasp of how containers power microservices architectures, legacy application migration, and modern CI/CD deployment pipelines.

### AWS Security: Hybrid Protection via WAF and Machine Learning NIDS

Addressing advanced cybersecurity, this session explored how traditional rule-based tools like AWS WAF excel at mitigating common Layer 7 web attacks (e.g., SQLi, XSS, rate-limiting) but struggle against novel, zero-day threat patterns.

To solve this gap, the presenter proposed combining AWS WAF with a Machine Learning-based Network Intrusion Detection System (NIDS). The technical workflow covered feature extraction, class imbalance resolution, and evaluating classifiers including Random Forest, LightGBM, 1D-CNN, and XGBoost. The cloud architecture featured AWS services such as Application Load Balancer, Kinesis Data Firehose, S3, Lambda, SNS, GuardDuty, and Security Hub.

This session closely mirrored my internship project, as both leverage ML algorithms to evaluate risk metrics. While my project focuses on scoring AI coding-agent execution paths, this session analyzed raw network traffic packets. The vital lesson learned is that ML model predictions should complement hard safety rules rather than operate in complete isolation.

### Real-Time Serverless Multiplayer Infrastructure (Godot 4 & AWS WebSockets)

In game engineering, this session showcased building real-time multiplayer interactions using Godot 4 integrated with AWS serverless services. The speaker evaluated communication protocols—comparing UDP/ENet, HTTP polling, and WebSockets—highlighting why WebSockets are ideal for turn-based mechanics, player lobbies, and live chat features.

The serverless implementation relied on API Gateway WebSocket routes, stateless AWS Lambda functions for game state handling, and Amazon DynamoDB for active connection tracking. Practical operational hurdles were also discussed, such as managing dead client sockets (`GoneException`), optimizing DynamoDB query costs, and keeping Lambda handlers stateless.

The main takeaway was architectural trade-off analysis: while serverless WebSocket setups significantly reduce server maintenance and baseline costs, high-frequency physics-heavy games still benefit more from dedicated server hosting platforms like AWS GameLift.

### Contextual GraphRAG with Amazon Bedrock & Neptune

The AI track covered GraphRAG—an advanced evolution of Retrieval-Augmented Generation that merges LLMs with Knowledge Graphs. Standard RAG relies on retrieving unstructured, isolated document chunks, which often falls short when answering queries requiring multi-hop logical connections across entities.

GraphRAG structures knowledge into nodes (entities) and edges (relationships), enabling LLMs to traverse interconnected context paths for higher reasoning precision. Two implementation paths on AWS were presented: a fully managed pipeline using Bedrock Knowledge Bases paired with Neptune Analytics, and a custom orchestration using LlamaIndex connected to Amazon Neptune.

This provided a clear technical perspective on how Generative AI precision can be significantly enhanced through structured data retrieval design rather than solely relying on larger LLM context windows.

## Personal Event Experience

Participating in this event was an enriching experience that blended deep technical insights with practical industry context. Listening to real-world engineering experiences provided clarity on production challenges that standard online tutorials often overlook, such as handling orphan WebSocket sockets, minimizing database scan costs, optimizing Docker layer builds, and evaluating security ML models.

The in-person format also allowed me to practice technical professionalism: adhering to the event schedule, actively taking structured notes, engaging with session topics, and contextualizing the presented solutions back to my own cloud engineering tasks.

## Key Professional Lessons

- **Portfolio over Theory:** Hands-on lab execution, thorough documentation, and tangible project proofs are essential for professional credibility.
- **Architecture as Trade-Offs:** Every technical option—whether VMs vs. Containers, Serverless vs. Dedicated Servers, or Rule-Based vs. ML-Based Security—involves clear trade-offs depending on the context.
- **Layered Defense Strategy:** Modern security strategies require combining deterministic rule filters with statistical anomaly detection for comprehensive threat coverage.
- **Serverless & AI Convergence:** Fully managed cloud services (Lambda, API Gateway, DynamoDB, Bedrock) allow small teams to rapidly build complex AI-driven platforms.
- **Structured Collaboration:** Technical skill alone is insufficient; successful projects depend on explicit goals, open communication, and individual accountability.

## Practical Relevance to My Internship Project

The knowledge gained from this event directly benefited my internship project, **AI Coding Agent Risk Scoring on AWS SageMaker**. The ML-based threat detection session reinforced my approach to combining machine learning output scores with strict system policy checks. Furthermore, the discussions on Docker packaging and serverless integration provided actionable ideas for refining my deployment procedures and pipeline automation.

Ultimately, the event reinforced a fundamental engineering principle: complex automated systems require continuous observability. Whether detecting network intrusions, executing GraphRAG lookups, or assessing AI agent behavior, reliable production deployments depend on accurate logging, metrics collection, and defined guardrails.

## Registration Verification

| Verification Attribute | Recorded Information |
|---|---|
| Student Name | Bùi Thanh Tuyền |
| Primary Email | tuyen.bui2005@hcmut.edu.vn |
| Contact Phone | 0387697447 |
| Educational Institution | Ho Chi Minh City University of Technology (HCMUT) |
| Student Identification | 2353284 |
| Date of Registration | June 06, 2026 |
| Assigned Shift | Fulltime |
| Facility Level | 26th Floor |
| Engagement Objective | Attend Events |

## Attendance Proof

Because I did not capture a personal photograph during the conference, official attendance is verified via the FCAJ Portal check-in record below. The log confirms my registration and check-in for the 09:00 AM shift on June 06, 2026, at the 26th Floor venue.

![FCAJ Portal attendance-history evidence for Event 1 on 06 June 2026](/images/events/event1-portal-checkin.png)

---

[Back to Events Participated](/4-eventparticipated/) | [Next](/4-eventparticipated/4.2-event2/)
