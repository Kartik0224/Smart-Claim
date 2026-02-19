#  Smart Claims Lakehouse

### End-to-End Enterprise Data Engineering + AI Insurance Platform (Databricks)

---

<p align="center">

<img src="https://img.shields.io/badge/Platform-Databricks-red">
<img src="https://img.shields.io/badge/Processing-Apache%20Spark-orange">
<img src="https://img.shields.io/badge/Storage-Delta%20Lake-blue">
<img src="https://img.shields.io/badge/ML-MLflow-green">
<img src="https://img.shields.io/badge/Architecture-Lakehouse-purple">
<img src="https://img.shields.io/badge/Status-Production%20Style-success">

</p>

---

## 📑 Table of Contents

* [Overview](#-overview)
* [Business Problems Solved](#-business-problems-solved)
* [System Architecture](#-system-architecture)
* [Decision Engine Workflow](#-automated-claims-decision-engine)
* [Operational Application](#-customer-claim-submission-portal)
* [Analytics Dashboards](#-insurance-analytics-dashboard)
* [Technology Stack](#-technology-stack--usage--problem-solved)
* [Repository Structure](#-repository-structure-faang-style)
* [How To Run](#-how-to-run-the-project)
* [Final Outcome](#-final-outcome)

---

##  Overview

Smart Claims Lakehouse is a production-style enterprise insurance analytics platform that automates claim validation using a unified Databricks Lakehouse and AI-powered damage classification.

The platform ingests structured enterprise data, real-time telemetry streams, and accident images into a scalable Medallion architecture to support analytics dashboards, operational apps, and automated decision workflows.

---

##  Business Problems Solved

✔ Eliminates fragmented insurance data silos
✔ Enables near real-time accident validation
✔ Automates manual image inspection
✔ Detects suspicious claims automatically
✔ Provides executive analytics dashboards

---

## System Architecture

<p align="center">
<img src="Dashboards&End_result/Smart_claim architecture.png" width="950">
</p>

Enterprise data flows through:

Landing → Bronze → Silver → Gold

before powering analytics, machine learning models, and operational applications.

---

##  Automated Claims Decision Engine

<p align="center">
<img src="Dashboards&End_result/Screenshot 2026-02-19 191707.png" width="900">
</p>

Validation includes:

* Policy eligibility checks
* Coverage validation
* Telemetry speed verification
* Accident reconstruction
* AI-based image classification

Claims are automatically approved or flagged for manual review.

---

##  Customer Claim Submission Portal

<p align="center">
<img src="Dashboards&End_result/Screenshot 2026-02-19 191540.png" width="850">
</p>

Customers upload accident images and claim details.
The portal connects directly to backend pipelines and ML services.

---

##  Automated Claim Result

<p align="center">
<img src="Dashboards&End_result/Screenshot 2026-02-19 191935.png" width="850">
</p>

After evaluating policy data, telemetry, financial checks, and ML severity prediction, the system generates automated claim decisions.

---

##  Insurance Analytics Dashboard

<p align="center">
<img src="Dashboards&End_result/Screenshot 2026-02-19 191257.png" width="900">
</p>

Provides:

* Loss ratio tracking
* Incident distribution
* Severity analysis
* Operational monitoring

---

## 📈 Incident Trend Analysis

<p align="center">
<img src="Dashboards&End_result/Screenshot 2026-02-19 191320.png" width="900">
</p>

Shows temporal incident patterns and financial impact trends for proactive risk management.

---

##  Technology Stack — Usage & Problem Solved

| Technology          | Used For                    | Problem Solved                            |
| ------------------- | --------------------------- | ----------------------------------------- |
| Databricks          | Unified data + ML platform  | Eliminated siloed enterprise systems      |
| Apache Spark        | Distributed ETL + streaming | Enabled large-scale processing            |
| Delta Lake          | Storage layer               | Guaranteed reliable incremental ingestion |
| Lakeflow Pipelines  | Workflow orchestration      | Automated incremental processing          |
| CDC ingestion       | SQL Server sync             | Avoided full reloads                      |
| Streaming ingestion | Telemetry validation        | Enabled real-time accident checks         |
| MLflow + ResNet     | Damage classification model | Automated image inspection                |
| SQL dashboards      | Business analytics          | Enabled executive insights                |

---

##  Repository Structure (FAANG Style)

```
smart-claims-lakehouse/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── notebooks/
│   ├── ingestion/
│   ├── transformations/
│   ├── ml_training/
│
├── pipelines/
│   ├── bronze_to_silver/
│   ├── silver_to_gold/
│
├── app/
│   ├── claim_portal/
│
├── images/
│   ├── all screenshots here
│
└── README.md
```

---

##  How To Run The Project

1. Create a Databricks workspace
2. Import notebooks from `/notebooks`
3. Configure Lakeflow ingestion pipelines
4. Load sample datasets into object storage / SQL source
5. Run ingestion → transformation → ML pipeline
6. Launch dashboards or claim portal

---

## Final Outcome

This project demonstrates a production-style enterprise data + AI system capable of:

* Multi-source incremental ingestion
* Real-time analytics workflows
* Automated insurance claim approval
* Production machine learning deployment
