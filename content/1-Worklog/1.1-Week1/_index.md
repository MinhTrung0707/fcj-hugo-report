---
title: "Week 1 Worklog"
date: 2026-04-25
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Week 1 Objectives:
* Analyze and estimate system resources (RDS, ECS) for the "Mini Social Network" project.
* Establish a containerized environment (Docker) in preparation for application deployment.

### Tasks to be implemented this week:
| Day | Task | Start Date | End Date | References |
| --- | --- | --- | --- | --- |
| Mon | - Receive Database Schema and calculate resources <br>&emsp; + Analyze DB structure from the Backend team <br>&emsp; + Calculate preliminary RAM/CPU capacity for RDS and ECS to optimize costs | 04/20/2026 | 04/21/2026 | Team Docs |
| Wed | - Build deployment script (Containerization) <br>&emsp; + Write a temporary `docker-compose.yml` file for Frontend, Backend, and Database <br>&emsp; + Optimize Backend Dockerfile (Maven build, JRE) and Frontend Dockerfile (Nginx) | 04/22/2026 | 04/23/2026 | Docker Docs |
| Fri | - Testing and packaging <br>&emsp; + Run system tests using Docker Compose <br>&emsp; + Verify port configurations and connections between containers | 04/24/2026 | 04/25/2026 

### Week 1 Achievements:
* Completed the RAM/CPU configuration estimate board for the AWS infrastructure.
* Successfully configured the `docker-compose.yml` file, allowing the entire system (Frontend, Backend, DB) to launch with a single command.
* Optimized Dockerfiles to ensure compact image sizes (using alpine images).

### Implementation Evidence:

#### 1. Task Tracking Board
Recorded the completion (DONE) of technical tasks in Week 1.
![Week 1 Task Tracking Board](/images/Tuan1.png)

Send the docker-compose.yaml file to the Zalo group.
![Sent to Zalo](/images/Tuan1-1.png)

#### 2. Deployment Script (Infrastructure Code)
The `docker-compose.yml` file configured to manage connections between system components.
![File docker-compose.yml](/images/Tuan1-3.png)

#### 3. Dockerization Results
Terminal displaying the successful build process of the Backend and Frontend images.
![Terminal build Docker](/images/Tuan1-2.png)