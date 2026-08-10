<h1 align="center">Tyree Franklin Jr.</h1>
<h3 align="center">Python Back-End Engineer</h3> 

<p align="center">
  <a href="https://www.linkedin.com/in/tyree-franklin-jr/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:tyree.franklinjr@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://github.com/tyreefranklinjr"> 
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</p> 

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tyreefranklinjr/tyreefranklinjr/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/tyreefranklinjr/tyreefranklinjr/output/github-contribution-grid-snake.svg">
  <img alt="contribution snake" src="https://raw.githubusercontent.com/tyreefranklinjr/tyreefranklinjr/output/github-contribution-grid-snake.svg">
</picture>

---

### Background

Python back-end engineer focused on distributed systems. Built automation pipelines at Wayfair that pulled competitor pricing from 13 sources for leadership. Tier I Network Engineer at Nextlink Internet, tracing faults across a distributed fixed-wireless network. Completed a cybersecurity internship at UNT (GenCyber) running attack simulations and hardening systems.

Based in Fort Worth, Texas.

---

### Core Skills

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
</p>

---

### Selected Projects

**Distributed Order Management System**
<br>
- Four independently deployable microservices (Order, Inventory, Notification, Auth), each with its own PostgreSQL database. 
- Kafka messaging with idempotent consumers, Redis-backed distributed locks on stock reservations, circuit breakers and retries via tenacity, JWTs validated locally against JWKS.
- Contract-tested with Pact and pytest, orchestrated with Docker Compose.

**Receipt and Document Processing Pipeline**
<br>
- Event-driven OCR pipeline: FastAPI upload to S3, EventBridge triggers a Lambda running AWS Textract's AnalyzeExpense API, results land in PostgreSQL.
- Full stack (S3, Lambda, EventBridge, IAM, RDS, ECS/Fargate) provisioned in Terraform, tested with pytest and moto in GitHub Actions CI.

**Speed Test Diagnostics Platform**
<br>
- Full-stack network diagnostics engine (Flask, SQLite) using a trimmed-mean sampling algorithm to correct for TCP ramp-up bias, validated across 300+ closed-environment test runs.

---

### Current Focus

- B.S. Computer Science, Western Governors University (expected May 2028)
- Tier I Network Engineer, Nextlink Internet
- Certified: Microsoft Specialist, Python Programming Fundamentals, Automation and Scripting with Python, Introduction to Software Engineering
