---
title: "Week 6 Worklog"
date: 2026-05-31
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:
* Convert network infrastructure design into Infrastructure as Code (IaC) using AWS CloudFormation.
* Automate the provisioning and synchronization of core network resources to prepare for the cloud deployment phase (Pre-flight Check).

### Tasks to be implemented this week:
| Day | Task | Start Date | End Date | References |
| --- | --- | --- | --- | --- |
| Mon | - Write foundational IaC script <br>&emsp; + Draft the `infrastructure.yaml` script defining the VPC (10.0.0.0/16) and Internet Gateway resources. <br>&emsp; + Declare configurations for 2 Public Subnets and 2 Private Subnets distributed across different Availability Zones (AZs). | 05/25/2026 | 05/26/2026 | [AWS CloudFormationn](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks?filteringText=&filteringStatus=active&viewNested=true) |
| Wed | - Configure routing and security <br>&emsp; + Provision a Route Table to route Public Subnet traffic to the Internet. <br>&emsp; + Define initialization parameters for separate Security Groups: ALB (opening Port 80) and Backend (opening Port 8080). | 05/27/2026 | 05/28/2026 | [AWS CloudFormationn](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks?filteringText=&filteringStatus=active&viewNested=true) |
| Fri | - Automate resource deployment <br>&emsp; + Append the Application Load Balancer (ALB) resource block into the YAML file. <br>&emsp; + Upload the `infrastructure.yaml` template to AWS CloudFormation, name the stack `MiniSocial-Tuan6-Infra`, and execute the creation command. | 05/29/2026 | 05/31/2026 | Team Docs |

### Week 6 Achievements:
* Completed an accurate IaC script, successfully linking the Load Balancer, Subnet layers, and Security Groups.
* The CloudFormation stack deployment process was 100% successful, returning a `CREATE_COMPLETE` status.
* Decoded and mastered the resource synchronization mechanism (Consistency check) of the global AWS system during the provisioning phase.

### Implementation Evidence:

#### 1. Automated Infrastructure Deployment via CloudFormation
Successfully uploaded the `infrastructure.yaml` template and configured the Stack named `MiniSocial-Tuan6-Infra` on the AWS Console.
The system deployment was fully completed, returning the **CREATE_COMPLETE** status.
*(Technical note: The brown segments on the chart indicate the "Consistency check" status - a process where AWS pauses for a few seconds to review and synchronize data across its global system. The endpoint turning green proves that the resource passed the inspection and was 100% successfully created.)*

The result will be: CREATE_COMPLETE:
![Hình ảnh Worklog Tuần 6 ](/images/Tuan6.png) 

![Hình ảnh Worklog Tuần 6 ](/images/Tuan6-1.png)

2. Send Tai_Lieu_CloudFormation_MiniSocial to the Zalo group.
![Hình ảnh Worklog Tuần 6 ](/images/Tuan6-2.png) 