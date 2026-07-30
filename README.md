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

I build back-end systems in Python, with a focus on distributed architecture and the infrastructure that keeps it running. At Wayfair I built automation pipelines that pulled competitor pricing data from 13 sources and turned it into something leadership could actually act on. Right now I work as a Tier I Network Engineer at Nextlink Internet, where I spend my days tracing faults through a distributed fixed-wireless network, which has taught me more about systems failing in the real world than any course could. I also completed a cybersecurity internship at UNT through GenCyber, running attack simulations and hardening systems against them.

I'm currently finishing a B.S. in Computer Science at Western Governors University, but the engineering work isn't waiting for the degree to catch up.

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
Four independently deployable microservices (Order, Inventory, Notification, Auth), each owning its own PostgreSQL database with no shared schema. Services communicate over Kafka with idempotent consumers, so replayed or duplicate events never trigger duplicate side effects. Stock reservations are protected with Redis-backed distributed locks to prevent overselling under concurrent load, synchronous calls are wrapped in circuit breakers and retries via tenacity, and JWTs are validated locally against a JWKS endpoint rather than hitting Auth on every request. Contract-tested with Pact and pytest, all four services orchestrated through Docker Compose.

**Receipt and Document Processing Pipeline**
<br>
Event-driven OCR pipeline: a FastAPI endpoint accepts an upload to S3, EventBridge triggers a Lambda that runs the document through AWS Textract's AnalyzeExpense API, and the extracted data lands in PostgreSQL. The entire stack, S3, Lambda, EventBridge, IAM, RDS, and ECS/Fargate, is provisioned as infrastructure-as-code in Terraform, with pytest and moto tests running in GitHub Actions on every push.

**Speed Test Diagnostics Platform**
<br>
A full-stack network diagnostics engine (Flask, SQLite) I built to solve a real problem at work: raw throughput numbers were getting skewed by TCP ramp-up. I validated a trimmed-mean sampling approach across 300+ closed-environment test runs to correct for it before trusting the numbers.

**Level 2 Rocket, Flight Control**
<br>
Wrote the C++ flight-control and altimeter logic for a Level 2 high-power rocket built to 2025 American Rocketry Challenge standards. The team placed in the top 100 nationally.

---

### Current Focus

- B.S. Computer Science, Western Governors University (expected May 2028)
- Tier I Network Engineer, Nextlink Internet
- Certified: Microsoft Specialist, Python Programming Fundamentals, Automation and Scripting with Python, Introduction to Software Engineering
