# Hi there, I'm Shubham Raghawant 👋

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shubham--raghawant-0077B5?logo=linkedin)](https://linkedin.com/in/shubham-raghawant)
[![Email](https://img.shields.io/badge/Email-shubhamraghawant%40gmail.com-D14836?logo=gmail)](mailto:shubhamraghawant@gmail.com)
[![Location](https://img.shields.io/badge/Location-Pune%2C%20India-blue)](https://github.com/shubhamraghawant)

**Software Engineer** with 4+ years of experience architecting and operating mission-critical, high-availability distributed systems at **Amdocs** (Tier-1 telecom platforms for AT&T and European carriers). Passionate about **event-driven microservices, transaction idempotency, real-time streaming, distributed scheduling, and resilient cloud architectures**.

---

## 🚀 Featured Engineering Projects

### ⚡ [TaskPulse — Distributed Task Scheduling & Worker Coordination Engine](https://github.com/shubhamraghawant/taskpulse)
> **Stack:** Java 21 • Spring Boot 3.2 • PostgreSQL 16 • Docker Compose • OpenAPI 3 • JUnit 5
* **Distributed Leader Leasing:** Enforces an atomic database heartbeat lease (`TASK_PULSE_LEADER`) ensuring active-active multi-node clusters execute scheduled jobs without duplicate runs or split-brain.
* **Priority Worker Pool:** Features an internal priority queue executing `CRITICAL` > `HIGH` > `NORMAL` > `LOW` tasks with non-blocking graceful thread termination.
* **Resilient Retry State Machine & DLQ:** Implements exponential backoff retries with automatic dead-letter queue isolation, dynamic cron calculations, and full audit telemetry.

---

### 💳 [PayFlow — Real-Time Payment Processing Microservices System](https://github.com/shubhamraghawant/payflow)
> **Stack:** Java 21 • Spring Boot 3.2 • Apache Kafka 7.5 • PostgreSQL 16 • Docker Compose • OpenAPI 3
* **Event-Driven Architecture:** Decoupled three microservices (`payment-service`, `fraud-detection-service`, `notification-service`) communicating asynchronously over Kafka event streams.
* **Fraud Velocity Engine:** In-memory concurrent sliding-window rate limiters detecting transaction velocity breaches and high-value anomalies in real time without DB table scans.
* **Financial Reliability:** Enforced strict idempotency keys, ACID state transitions, and single-command local orchestration via Docker Compose.

---

### 🔭 [LogLens — Distributed Log Aggregation & Real-Time Alerting Engine](https://github.com/shubhamraghawant/loglens)
> **Stack:** Java 21 • Spring Boot 3.2 • Apache Kafka 7.5 • PostgreSQL 16 • Docker Compose • JUnit 5
* **Centralized Observability:** Simulated 5 distributed microservices streaming structured logs to Kafka (`logs.raw`), persisted to PostgreSQL via batch JDBC inserts.
* **Anomaly Alerting Engine:** Real-time sliding-window detector triggering automated alerts (`>10 errors/min` or `>3 FATALs/min`) published to `logs.alerts`.
* **SRE Incident Workflows:** Paginated REST search API with multi-criteria filtering, 24-hour service metrics, and alert acknowledgement workflows.

---

### 🎯 [SmartHire — AI-Powered Job Application Tracker](https://github.com/shubhamraghawant/smarthire)
> **Stack:** Java 21 • Spring Boot 3 • React 18 • TypeScript 5 • Tailwind CSS • Spring Security (JWT) • Docker
* **Full-Stack SPA:** Drag-and-drop Kanban board pipeline backed by a Spring Boot 3 REST API.
* **Match Scoring Engine:** Pure-Java keyword extraction and tokenization algorithm that scores candidate-to-job match percentage (0–100%) and identifies skill gaps without external API latency.
* **Production Packaging:** Multi-stage Docker builds orchestrating Spring Boot, PostgreSQL, and Vite/Nginx frontend.

---

## 🛠️ Technical Stack & Skills

- **Languages:** Java 17/21, SQL, Python, TypeScript, JavaScript
- **Frameworks & Libraries:** Spring Boot 3, Spring Data JPA, Spring MVC, Spring Security (JWT), Hibernate, React 18
- **Messaging & Streaming:** Apache Kafka (mTLS, consumer groups, partition scaling, event-driven design)
- **Cloud & Infrastructure:** AWS, Kubernetes, OpenShift, Docker, Podman, Nginx
- **Databases:** PostgreSQL (ACID transactions, indexing, partitioning, advisory locking)
- **CI/CD & Testing:** Jenkins pipelines, GitHub Actions, Maven, JUnit 5, Mockito, SonarQube, Veracode

---

## 📈 Engineering Principles
* **Resilience First:** Assume networks drop and services fail — design with idempotency, circuit breakers, and dead-letter queues.
* **Zero Fluff:** Clean architecture, observable systems, and tested code over hand-waving.
* **Continuous Ownership:** From requirement discovery to production incident triage (RCA) and post-mortems.
