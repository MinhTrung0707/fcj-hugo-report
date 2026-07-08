---
title: "FCAJ Community Day - June 2026"
date: 2026-06-27
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

![FCAJ Community Day](/images/Evt_3.png)

# Reflection Report “FCAJ Community Day - June 2026”

### Event Objectives (Infrastructure & Operations Perspective)

- Update trends in integrating Artificial Intelligence (AI) into cloud management and operations (Cloud Operations) on the AWS platform.
- Explore how AI tools (like AWS DevOps Agent) automate CI/CD processes and reduce the workload for the SysAdmin/DevOps team.
- Deep dive into the network infrastructure security problem: How to establish safe boundaries (VPC, Private Subnets) to protect data flows when enterprises connect to Large Language Models (LLMs).
- Listen to real-world use cases from solution architecture experts and cloud security engineers.

### List of Speakers

- **Steve Trần** – Representative from Cloud Thinker
- **Hiếu Nghị** – Representative from Renova Cloud
- **Trung** – AWS Study Builder
- **Trung Đ** – CEO of R AI
- **Kiệt** – Expert sharing on infrastructure architecture for voice AI applications
- **Bảo and Nguyên** – Representatives from Cloud Kinetis
- **Trường and Minh Anh** – Representatives from Noventis
- **Toàn Nguyễn** – AWS Security Builder

### Key Highlights: The Intersection of Networking & AI

#### 1. AWS DevOps Agent: A New Era of Operational Automation
- The event outlined the transition roadmap from a passive monitoring system (only sending log alerts via CloudWatch) to an action-driven auto-remediation system using AI.
- Introduced AWS DevOps Agent as a powerful "virtual assistant" capable of analyzing system errors, thereby significantly reducing critical infrastructure metrics such as MTTD (Mean Time To Detect) and MTTR (Mean Time To Recovery).

#### 2. Building Secure Private MCP Connections via VPC Network
- This content closely aligns with my networking expertise. The event introduced the Model Context Protocol (MCP) used for the Amazon Q AI assistant.
- Instead of letting AI data travel through the public Internet, experts demonstrated how to establish a completely closed network traffic flow through Amazon VPC and VPC Endpoints. This helps Enterprise systems absolutely prevent the risk of sensitive data leakage.

#### 3. Infrastructure for Voice AI at Scale
- Analyzed the architecture behind complex Voice AI flows: How to combine streaming data flows with Amazon Bedrock with the lowest latency, requiring an extremely stable network platform.

#### 4. High-level Management Application (HR Planning)
- Further reference on the Application Layer: How Amazon Q is used to analyze the workforce and automate HR tasks, demonstrating the power of AI when provided with a sufficiently large data source.

### Lessons Learned & Practical Applications

#### Next-Generation Infrastructure Mindset
- **Network security is a prerequisite for AI:** No matter how smart an AI model is, it will be a security disaster if the Traffic Flow is not isolated within a secure VPC environment. Designing strict Subnets and Security Groups is the foundation for deploying AI.
- **CI/CD Automation:** Manual operations (like debugging Nginx configuration errors or checking Jenkins logs) in the future can be entirely delegated to AI Agents to handle, allowing engineers to focus on architectural design.

#### Application Plan for Personal Project
- **Integrate Security mindset:** From the knowledge of MCP and VPC, I plan to review the network diagram of the "Mini Social Network" project, ensuring that connections from the application to the Database (RDS) or storage (S3) are configured with secure internal Endpoints.
- **Research DevOps Agent:** Learn how to integrate automated analysis flows into the Jenkins Pipeline to warn about the root causes of build errors (such as insufficient RAM, incorrect environment variables) more intuitively.

### Experience at the Event

Attending the **“FCAJ Community Day”** at the Bitexco building this time gave me an extremely "satisfying" feeling technically. Unlike purely theoretical events, seeing AWS engineers (Builders) demonstrate private VPC configuration for AI or how DevOps Agent catches system errors firsthand helped me answer many questions during my recent network configuration practice.

The atmosphere at the event was very open. Standing in the same space with security experts and cloud architects helped me realize that: The Computer Networking industry is not going to be replaced by AI; rather, those with a solid network infrastructure foundation will be the ones building the safe "highways" for AI to run on. This is a huge motivation for me to continue pursuing the Cloud/DevOps Engineer path.

#### Actual pictures at the event

![FCAJ Community Day](/images/Event3.png)

![FCAJ Community Day](/images/event3-5.png)