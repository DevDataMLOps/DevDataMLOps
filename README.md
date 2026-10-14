# Cloud & Data Engineering | Python · SQL · AWS

I build data pipelines that turn fragmented source data into validated, auditable datasets, analytics, and APIs.

My work focuses on **data quality, query efficiency, access controls, and recovery from failure**. This portfolio includes an AWS financial analytics platform, a governed healthcare data pipeline, and a climate-health intelligence project.

**Open to full-time cloud/data engineering roles and technical contract projects.**

## Selected engineering results

- **AWS data engineering:** ZIPCO validates **2.34 million synthetic relational records** across six datasets before publishing curated Parquet.
- **Measured query optimization:** ZIPCO recorded an **88.21% reduction in Athena data scanned** for its CSV-to-Parquet full-scan benchmark.
- **Governed data delivery:** PATIENTRA documents **13/13 independent release checks**, with lineage, reconciliation, and disclosure controls.
- **Resilient processing:** Project RISING demonstrates validation, retry, dead-letter isolation, deduplication, and checkpointing for simulated climate events.

## Featured projects

### [ZIPCO — Financial Risk Intelligence Platform](https://github.com/DevDataMLOps/Zipco-Financial-Risk-Intelligence-platform)

**AWS Glue · PySpark · S3 · Athena · SQL · Lambda · CloudWatch · IAM · Lake Formation**

An AWS-deployed portfolio platform covering ingestion, quality gates, partitioned Parquet, financial analytics, access controls, and event recovery.

- Measured an **88.21% CSV-to-Parquet scan reduction** and a separate **95.55% reduction** from full Parquet to a partition-pruned 2023 workload.
- Verified authorized and denied Athena access through an isolated Lake Formation demonstration.
- Demonstrated event processing with **25/25 valid events curated** and **3/3 expected-invalid events quarantined**.

[Architecture](https://github.com/DevDataMLOps/Zipco-Financial-Risk-Intelligence-platform/blob/main/docs/ARCHITECTURE.md) · [7-minute walkthrough](https://github.com/DevDataMLOps/Zipco-Financial-Risk-Intelligence-platform/blob/main/docs/PORTFOLIO_DEMO.md) · [Verification and scope](https://github.com/DevDataMLOps/Zipco-Financial-Risk-Intelligence-platform/blob/main/PROJECT_STATUS.md)

### [PATIENTRA — Governed Healthcare Data Pipeline](https://github.com/DevDataMLOps/Patientra)

**Python · pandas · SQL · SQLite · FastAPI · pytest · GitHub Actions**

A Bronze → Silver → Gold pipeline for a fictional merged hospital network, connecting patient identities and producing disclosure-controlled readmission analytics.

- Preserves source lineage, quarantines ambiguous records, and routes uncertain identity matches to human review.
- Documents **13/13 release checks** and **eight suppressed rows out of 51 aggregate breakdown rows**.
- Extends validated aggregate delivery into an authenticated API and dashboard.

[Architecture](https://github.com/DevDataMLOps/Patientra/blob/main/docs/architecture.md) · [Evidence](https://github.com/DevDataMLOps/Patientra/blob/main/docs/evidence/README.md) · [Demo guide](https://github.com/DevDataMLOps/Patientra/blob/main/docs/demo.md)

*Synthetic-data demonstration. The reconstructed release retains eight unresolved identity reviews; technical validation does not establish clinical validity.*

### [Project RISING — Resilient Climate-Health Intelligence](https://github.com/DevDataMLOps/Project-Rising)

**Python · FastAPI · PostgreSQL · Docker Compose · Streamlit · pytest**

A three-person hackathon project combining ASEAN health indicators, simulated climate events, an explainable risk-scoring model, and an operations dashboard. My role: **Lead Data Pipeline Engineer**.

- Demonstrates batch ingestion and resilient event processing with buffering, retries, dead-letter routing, and checkpoints.
- Provides API endpoints, warehouse integration, and a dashboard for inspecting data and pipeline behavior.

[Architecture](https://github.com/DevDataMLOps/Project-Rising/blob/main/docs/architecture/01_system_architecture.md) · [API documentation](https://project-rising-api.onrender.com/docs) · [Dashboard](https://project-rising.streamlit.app/)

*Hackathon decision-support demonstration; simulated events and deterministic risk scores do not establish a validated outbreak forecast.*

## Additional focused projects

| Project | Engineering focus | Review scope |
|---|---|---|
| [Telecom Data Revolution](https://github.com/DevDataMLOps/Telecom-Data-Revolution) | Mage orchestration, BigQuery loading, contracts, quarantine, and audit records | README documents 243,553 input records, 223,966 curated records, and 19,587 quarantined records |
| [AeroMart semantic vector pipeline](https://github.com/DevDataMLOps/Building-A-Semantic-Vector-Database-) | PySpark joins, Parquet tables, text chunking, and embeddings | Learning prototype; vector indexing and retrieval are future work |
| [CoffeeClub PostgreSQL analytics](https://github.com/DevDataMLOps/CoffeeClub-Capstone) | Relational integrity, indexing, transformations, and analytical views | Focused SQL capstone; performance gains require benchmarking |

## Engineering toolkit

| Area | Technologies demonstrated in these projects |
|---|---|
| Languages and processing | Python, SQL, pandas, PySpark |
| AWS data platform | S3, Glue, Athena, Lambda |
| Governance and operations | IAM, KMS, Lake Formation, CloudWatch, EventBridge |
| Serving and storage | FastAPI, PostgreSQL, SQLite, Streamlit |
| Delivery and verification | Git, Docker Compose, pytest, GitHub Actions |

## How I approach engineering

I document data contracts and architecture, validate before publishing, isolate invalid records, and retain evidence of what ran. I distinguish measured results from planned capabilities and make each project's setup, limitations, and verification available for review.

**Explore the project walkthroughs above to see the implementation, design decisions, and evidence.**
