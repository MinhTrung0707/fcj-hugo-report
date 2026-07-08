---
title: "Week 2 Worklog"
date: 2026-04-27
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:
* Research the secure storage service Amazon ECR and the Serverless Compute engine AWS Fargate.
* Perform packaging, push the Docker Image to ECR, and independently launch the application on the AWS Console to overcome server downtime issues.

### Tasks to be implemented this week:
| Day | Task | Start Date | End Date | References |
| --- | --- | --- | --- | --- |
| Mon | - Local Packaging Operations <br>&emsp; + Use AWS CLI to retrieve the Token and authenticate access to AWS ECR. <br>&emsp; + Use the `docker build` command with the `--platform linux/amd64` flag to create the Image, helping prevent CPU architecture errors. | 04/27/2026 | 04/28/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Wed | - Push Image to ECR repository <br>&emsp; + Tag the Image to match the ECR repository URI. <br>&emsp; + Use the `docker push` command to securely push the Backend Image to the AWS internal system. | 04/29/2026 | 04/30/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Fri | - Launch on Amazon ECS <br>&emsp; + Access Amazon ECS to create a Cluster (logical network environment). <br>&emsp; + Create a Task Definition with 1 vCPU and 2 GiB RAM parameters, while granting the `ecsTaskExecutionRole`. <br>&emsp; + Create a Service to run the application and implement cost optimization by setting Desired tasks to 0 after testing. | 05/01/2026 | 05/03/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Week 2 Achievements:
* Grasped the Serverless AWS Fargate model, thereby providing an independent environment to handle complex logic workloads (API communication, JWT security, Sockets) without relying on Firebase or a local SQLite database.
* Successfully pushed the Docker Image to the Amazon ECR repository (replacing Docker Hub).
* Completed the ECS Service configuration in `awsvpc` network mode, properly established IAM permissions, and implemented cost control procedures since AWS Fargate is not included in the Free Tier.

### Implementation Evidence:

#### 1. Week 2 Task Tracking Board
Recorded the completion (DONE) of the task to research ECR & Fargate services.
*(Note: During this holiday week, the team had an OFF meeting schedule, but members still proactively completed their individual tasks on time)*.
![Week 2 Task Tracking Board](/images/worklogtuan2.png)

#### 2. Research Document Submission
The detailed analysis document on the deployment process, expected configuration, and practical application of the ECR/Fargate architecture was drafted into a Word file (`tuan2.docx`) and sent directly to the shared Zalo group for the team to stay informed.
![Evidence of Week 2 report submission](/images/worklogtuan2-1.png)