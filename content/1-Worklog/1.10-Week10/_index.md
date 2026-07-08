---
title: "Week 10 Worklog"
date: 2026-06-28
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:
* Implement Code Freeze and conduct a comprehensive review of the network infrastructure before deploying to the production environment.
* Evaluate security and recalibrate all infrastructure configuration files (YAML).
* Finalize the Architecture Diagram to its ultimate version.

### Tasks to be implemented this week:
| Day | Task | Start Date | End Date | References |
| --- | --- | --- | --- | --- |
| Mon | - Review Infrastructure as Code (IaC) <br>&emsp; + Analyze and inspect all YAML files configuring the network (VPC, Subnet, Route Table) provided by the team. <br>&emsp; + Synthesize inconsistencies, cross-check structures, and create an evaluation report proposing edits to the YAML files. | 22/06/2026 | 23/06/2026 |  |
| Wed | - Finalize Architecture Diagram <br>&emsp; + Update and refine the finalized architecture diagram (Minisocial Architect) based on the actual infrastructure post-Rebuild. <br>&emsp; + Fully incorporate new connection flows and services (NAT Gateway, S3 VPC Endpoint) into the diagram. | 24/06/2026 | 25/06/2026 | [AWS Architecture Icons](https://aws.amazon.com/vi/architecture/icons/) |
| Fri | - Cloud Network Security Review <br>&emsp; + Review all Inbound/Outbound rules of Security Groups and Network ACLs on the VPC to ensure no unnecessary ports are exposed at the Public Subnet layer. <br>&emsp; + Verify the internal network connection flow between the Compute cluster (Amazon ECS Fargate) and the Database (Amazon RDS) to ensure data security. | 26/06/2026 | 26/06/2026 |  |

### Week 10 Achievements:
* Completed the evaluation report and successfully fixed configuration errors in the YAML files.
* Successfully published the most complete version of the Architecture Diagram, accurately reflecting 100% of the current network infrastructure.
* Completed the network infrastructure security review, updating the task status to completed (DONE) on time (Deadline 23:59 on June 23).

### Other Activities / Implementation Evidence:

#### 1. Completion of Week 10 Assigned Tasks
Finished the items "Analyze and inspect all YAML files" and "Finalize Architecture diagram". The task status on the team's tracking system has turned green (DONE). 

*(Note: The team proactively organized an offline meeting (Cafe Sync-up) on June 26 to finalize the errors in the YAML files and agree on the final architecture diagram before deploying to the production environment. The DONE status update board below serves as evidence of the meeting's outcome).*
![Week 10 task progress tracking board](/images/Tuan10-1.png)

![Sent to zalo group](/images/Tuan10.png)

#### 2. System Architecture Diagram (Final Update)
The overall network architecture diagram has been refined, adding new components after the Rebuild and Security Audit process. This is the direct result of the infrastructure review, ready to serve as official documentation for the project defense session.
![Detailed modified architecture diagram](/images/SoDoKienTrucDaChinhSua.drawio.png)