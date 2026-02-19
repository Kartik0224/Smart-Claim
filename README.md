![](ProjectViz.gif)

# 🚗 Smart Claims Lakehouse

## End-to-End Databricks Data Engineering + Machine Learning Insurance Platform

---

## 🧭 Project Overview

Smart Claims Lakehouse is a production-style enterprise data platform built on Databricks that automates insurance claim processing using a unified Lakehouse architecture and AI-powered damage classification.

The system integrates structured enterprise data, real-time vehicle telemetry streams, and accident images into a single scalable environment to enable automated validation, analytics reporting, and operational decision-making.

The platform transforms a traditionally manual insurance workflow into an intelligent automated claims system.

---

## 🎯 Business Problems Solved

✔ Eliminates fragmented insurance data silos
✔ Enables near real-time accident validation
✔ Automates manual image damage inspection
✔ Detects suspicious claims for investigation
✔ Provides executive dashboards for risk monitoring

---

## 🏗️ System Architecture (Lakehouse Pipeline)

<p align="center">
  <img src="Dashboards&End_result/image.png" width="950">
</p>

The architecture integrates multiple enterprise data sources including relational databases, streaming telemetry feeds, and object storage containing accident images.

Incoming data is processed through automated ingestion pipelines and stored in a Medallion Lakehouse:

**Landing → Bronze → Silver → Gold**

The curated datasets power dashboards, ML models, and operational applications.

---

## 🧠 Automated Claims Decision Engine

<p align="center">
  <img src="images/Screenshot 2026-02-19 191707.png" width="900">
</p>

The decision workflow combines business rule validation and machine learning inference:

* Policy eligibility verification
* Coverage validation
* Telemetry speed analysis
* Accident reconstruction
* AI image severity prediction

Based on these checks, claims are automatically approved or flagged for manual investigation.

---

## 🧾 Customer Claim Submission Portal

<p align="center">
  <img src="images/Screenshot 2026-02-19 191540.png" width="850">
</p>

Customers upload accident images, policy details, and incident information through this operational interface.
The portal connects directly with backend pipelines and deployed ML services for real-time claim analysis.

---

## 🎉 Automated Claim Processing Output

<p align="center">
  <img src="images/Screenshot 2026-02-19 191935.png" width="850">
</p>

After evaluating image severity, policy coverage, telematics data, and financial checks, the system automatically generates claim decisions. Approved claims proceed automatically while suspicious cases are routed for investigation.

---

## 📊 Insurance Analytics Dashboard

<p align="center">
  <img src="images/Screenshot 2026-02-19 191257.png" width="900">
</p>

The dashboard presents operational and financial insights such as:

* Loss ratio metrics
* Liability exposure
* Incident distribution by severity
* Insurance performance tracking

These dashboards support executive-level monitoring and decision-making.

---

## 📈 Incident Trend & Severity Analytics

<p align="center">
  <img src="images/Screenshot 2026-02-19 191320.png" width="900">
</p>

Aggregated visualizations reveal temporal incident patterns, severity distribution, and financial impact trends across accident categories.

This enables proactive risk assessment and operational planning.

---

## 🔧 Technology Stack — Usage & Problem Solved

### Databricks Lakehouse Platform

Unified platform for ingestion pipelines, ETL processing, machine learning lifecycle, dashboards, and applications.
**Solved:** Eliminated fragmented enterprise data systems.

---

### Apache Spark / PySpark

Used for distributed ETL processing, joins, and streaming ingestion.
**Solved:** Enabled scalable processing of large insurance datasets.

---

### Delta Lake

Used as storage layer for Bronze, Silver, Gold tables with ACID guarantees.
**Solved:** Ensured reliable incremental ingestion and prevented corruption.

---

### Lakeflow Pipelines

Used for automated ingestion workflows and incremental ETL orchestration.
**Solved:** Removed complex manual pipeline dependency management.

---

### Change Data Capture

Used to incrementally sync SQL Server insurance tables.
**Solved:** Avoided expensive full database reloads.

---

### Streaming Telemetry Processing

Vehicle sensor data ingested continuously.
**Solved:** Enabled real-time accident validation.

---

### MLflow + Deep Learning (Computer Vision)

Used to train and deploy an image classifier predicting crash severity.
**Solved:** Automated manual image inspection.

---

### SQL Analytics + BI Dashboards

Gold datasets exposed for executive monitoring.
**Solved:** Enabled real-time insurance performance insights.

---

## 🏆 Final Outcome

This project demonstrates how to build a production-ready enterprise data and AI solution capable of:

* Multi-source incremental ingestion
* Real-time analytics processing
* Automated insurance decision workflows
* Production machine learning deployment

---

## 💼 Ideal For

✔ Data Engineering portfolio
✔ Machine Learning production pipelines
✔ Enterprise Lakehouse architecture learning
✔ Real-time analytics system design
