---
title: "Week 12 Worklog"
date: 2026-07-07
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Week 12 Objectives:
* Analyze, review, and finalize the Final version of the project's architecture diagram (Minisocial Architect) based on budget constraints.
* Complete 100% of the content on the Hugo Server & Internship Report, conduct cross-checking with the team.

### Tasks to be implemented this week:
| Day | Task | Start Date | End Date | References |
| --- | --- | --- | --- | --- |
| Mon | - Analyze and review the Minisocial Architect diagram <br>&emsp; + Evaluate the current state of network infrastructure (VPC, Subnets, Traffic Optimization). <br>&emsp; + Identify infrastructure limitations (using only 1 NAT Gateway in AZ A and Single-AZ for RDS). Assess risks and decide to maintain this structure to ensure cost optimization for the project's current scale. | 06/07/2026 | 06/07/2026 | Current system diagram |
| Tue | - Finalize the Final diagram and submit the report <br>&emsp; + Refine the diagram: Tidy up the layout, realign connection lines to clarify Logic and Physical communication flows (especially the Outbound Traffic flow via NAT Gateway). <br>&emsp; + Finalize the Hugo Server & Internship Report, proceed with cross-checking, and submit before the deadline (Deadline: 23:59 Tue 07/07). | 07/07/2026 | 07/07/2026 | Draw.io diagram / Internal platform |

### Week 12 Achievements:
* Completed in-depth review and finalized the Minisocial Architecture Diagram Final version (preserved the current infrastructure structure to optimize the budget, perfected the visual presentation).
* Strictly executed cross-checking of documents according to team rules, ensuring no errors.
* Completed all content and successfully submitted the Hugo Server and Internship Report on time (completed before 23:59 Tuesday, July 07, 2026).

### Other Activities / Implementation Evidence:

#### 1. Week 12 Task Assignment Board
Records the task assignments during the Graceful Shutdown & Documentation phase. The tasks "Analyze, review, edit the final version of the Minisocial Architect diagram" and "finalize the report" were handled on time. 

![Week 12 task progress tracking board](/images/Tuan12.png)
*(Extracurricular activity note: The team flexibly organized a direct acceptance meeting at a coffee shop on Wednesday, July 08 to unify the handover and close the project).*
![Week 12 task progress tracking board](/images/Tuan12-1.png)

#### 2. Architecture Diagram (Final Version)
The final drawing was refined to provide the most visual presentation of the project's ecosystem. The diagram focuses on clarifying core network communication flows (VPC Gateway Endpoint for S3, Outbound Traffic via NAT Gateway) and the decision to maintain the Single-AZ design for the Database to align with the team's cost optimization problem.

![Architecture Diagram](/images/SoDoKienTrucDaChinhSua.drawio.png)