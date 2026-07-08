---
title: "Week 7 Worklog"
date: 2026-06-07
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:
* Finalize and comprehensively map out the 3-Tier Architecture system diagram on the AWS platform.
* Visualize network traffic flows (Data Plane & Control Plane) to support "The Big Move" deployment phase.
* Draft a detailed presentation script for defending the project's architecture.

### Tasks to be implemented this week:
| Day| Task | Start Date | End Date | References |
| --- | --- | --- | --- | --- |
| Mon | - Finalize Architecture Diagram <br>&emsp; + Design a diagram encompassing VPC boundaries, Public/Private Subnets, ALB, ECS Fargate, RDS, and NAT Gateway. | 06/01/2026 | 06/03/2026 | [AWS Architecture Icons](https://aws.amazon.com/vi/architecture/icons/) |
| Thur | - Analyze Traffic Flows <br>&emsp; + Breakdown the User Access flow (1-7) and the CI/CD & Monitoring pipeline (8-10, A-B). | 06/04/2026 | 06/05/2026 | [AWS Architecture Icons](https://aws.amazon.com/vi/architecture/icons/) |
| Sat | - Write Presentation Script <br>&emsp; + Compile all documentation into an in-depth architectural discussion regarding the small-scale Social Network. | 06/06/2026 | 06/07/2026 |  |

### Week 7 Achievements:
* 100% completion of the isolated internal network architecture diagram adhering to AWS standards.
* Clearly established the routing for static web interface distribution via S3 and internal API processing mechanisms.
* Completed the detailed presentation script to serve as a reference document for the team while deploying the actual infrastructure using CloudFormation.

### Implementation Evidence:

#### 1. Finalized Architecture Diagram
Successfully designed the overarching architecture diagram, clearly illustrating the 3-Tier Architecture model integrated within the AWS VPC environment.
![Small-scale Social Network Architecture Diagram - AWS 3-Tier Architecture](/images/Tuan7.png)

![Hình ảnh Worklog Tuần 7 ](/images/Tuan7-1.png)