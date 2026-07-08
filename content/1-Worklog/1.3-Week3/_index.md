---
title: "Week 3 Worklog"
date: 2026-05-10
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:
* Build an automated CI/CD pipeline using Jenkins (Jenkinsfile) following DevOps standards.
* Fix outstanding bugs in the Unit Test phase and optimize the pipeline flow for the Frontend.
* Successfully containerize (Dockerize) the source code and push it to the Amazon ECR repository.

### Tasks to be implemented this week:
| Day | Task | Start Date | End Date | References |
| --- | --- | --- | --- | --- |
| Mon | - Bug fixing and ECR setup <br>&emsp; + Fix the `NullPointerException` in `NotificationServiceTest.java` by reconfiguring the Database connection and mock data. <br>&emsp; + Initialize 2 Private Repositories on ECR (`minisocial-backend` and `minisocial-frontend`). | 04/05/2026 | 05/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Wed | - Frontend and Jenkinsfile configuration <br>&emsp; + Apply Multi-stage build and write an `nginx.conf` file for the Frontend to handle React Router SPA and Reverse Proxy to avoid CORS errors. <br>&emsp; + Initialize the Jenkinsfile to declare AWS environment variables, configure Checkout, Build Docker, Login ECR, and Push Image steps. | 06/05/2026 | 07/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Fri | - Pipeline optimization, Automated Deploy, and Team meeting <br>&emsp; + Resolve the Pipeline hanging issue by removing the `npm ci` command on the Host, moving it to Docker Stage 1 (Alpine Linux) to avoid I/O bottlenecks. <br>&emsp; + Create a new Pipeline Job on Jenkins, point it to the GitHub repository, and execute it automatically. <br>&emsp; + Attend an offline team meeting to summarize and present results. | 08/05/2026 | 10/05/2026 | Internal report |

### Week 3 Achievements:
* The Backend source code successfully loaded the Application Context and passed all 186/186 Unit Tests.
* The CI system ran automatically with 100% success, the build speed increased significantly, and it no longer hangs.
* Images were successfully containerized and automatically pushed to AWS ECR with optimized sizes (Backend: 144.02 MB, Ultra-lightweight Frontend: 26.33 MB).

### Implementation Evidence:

#### 1. Week 3 Task Progress Tracking Board
Recorded the completion (DONE) of the source code containerization and Image push tasks to the Amazon ECR repository, along with the Offline team meeting schedule on May 10.
![Week 3 progress board](/images/Tuan3-5.png)

![Visiting AWS office](/images/Tuan3-7.png)

#### 2. Deployment Scripts (Infrastructure as Code)
The source code configurations for Dockerfile, Nginx, and Jenkinsfile have been set up and optimally fine-tuned to serve the CI/CD pipeline.
![Dockerfile configuration](/images/Tuan3.png)

![Nginx configuration part 1](/images/Tuan3-1.png)

![Nginx configuration part 2](/images/Tuan3-2.png)

![Jenkinsfile configuration part 1](/images/Tuan3-3.png)

![Jenkinsfile configuration part 2](/images/Tuan3-4.png)