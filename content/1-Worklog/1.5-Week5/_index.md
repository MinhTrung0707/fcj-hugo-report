---
title: "Week 5 Worklog"
date: 2026-05-24
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:
* Visually draft the entire infrastructure system of the "Mini Social Network" project onto an architecture diagram (AWS Architecture Diagram).
* Clearly depict the network security boundary layers (Network Layer, Subnetting Layer) and the routing of data flows (Traffic Flow).

### Tasks to be implemented this week:
| Day | Task | Start Date | End Date | References |
| --- | --- | --- | --- | --- |
| Mon | - Design System Architecture Diagram <br>&emsp; + Use the Draw.io tool with standard AWS Architecture Icons. <br>&emsp; + Clearly partition into 4 layers: Network (VPC), Subnetting (Public/Private Subnet), and External Storage Layer. | 05/18/2026 | 05/19/2026 | https://aws.amazon.com/vi/architecture/icons/ |
| Wed | - Plan Traffic Flow <br>&emsp; + Use colored arrows to simulate the access flow: User -> Internet -> WAF -> ALB -> Fargate -> RDS/S3. <br>&emsp; + Design a detailed Legend for each type of arrow. | 05/20/2026 | 05/21/2026 |  https://aws.amazon.com/vi/architecture/icons/ |
| Fri | - Publish and Analyze Architecture <br>&emsp; + Export the source file (.drawio) and high-resolution image file (PNG/PDF) with a transparent background. <br>&emsp; + Assist the team in writing documentation to decode the 3-Tier architecture. | 05/22/2026 | 05/24/2026 | https://aws.amazon.com/vi/architecture/icons/ |

### Week 5 Achievements:
* 100% completed the architectural diagram accurately simulating the current infrastructure status of the "Mini Social Network" project.
* Provided the full original design files and high-resolution images along with the network traffic flow legend.
* Successfully systematized the multi-layer security theory (Defense-in-Depth) into the practical diagram.

### Implementation Evidence:

#### 1. Mini Social Network System Architecture Diagram
The diagram sketches in detail the 3-Tier model on AWS, clearly separating the Frontend, Backend, Media, and CI/CD flows.
![System Architecture Diagram drawn on Draw.io](/images/Tuan5.png)

#### 2. Sent the Architecture Decoding to the Zalo group for peer review
![Week 5 Worklog Image](/images/Tuan5-1.png)