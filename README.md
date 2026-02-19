![](ProjectViz.gif)
# Smart Claims Lakehouse — End-to-End Databricks Data Engineering & ML Project

## Overview

This project demonstrates a complete end-to-end modern data platform built on Databricks to support an intelligent insurance claims processing system. The solution integrates batch, streaming, and file-based data sources into a unified Lakehouse architecture and applies machine learning to automatically assess vehicle damage severity from uploaded images.

The primary goal of the system is to create a single source of truth for customer, policy, telematics, and claims data while automating claim validation and improving decision-making through analytics and AI.

---

## Business Problem

Insurance claim processing is traditionally manual, slow, and error-prone.
This project solves two key challenges:

* Consolidating enterprise data from multiple systems into one analytical platform
* Automating claim verification using telematics data and computer vision

The system validates whether:

* The driver's recorded speed matches the accident report
* The customer is eligible based on policy rules
* The uploaded accident image matches the declared damage severity

---

## Architecture Highlights

The platform follows a modern Lakehouse design using the Medallion Architecture:

**Landing → Bronze → Silver → Gold**

* Landing: Raw data ingestion
* Bronze: Source-aligned structured Delta tables
* Silver: Cleaned and validated datasets with data quality checks
* Gold: Aggregated business-ready datasets for analytics and applications

---

## Data Sources Integrated

* SQL Server database (customers, claims, policies) using change data capture
* Streaming telematics sensor data
* Object storage containing accident images and metadata

All ingestion pipelines are incremental and support real-time processing.

---

## Key Features Implemented

### Data Engineering

* Incremental database ingestion using CDC pipelines
* Real-time stream processing for telematics data
* Automated file ingestion from object storage
* Schema evolution handling
* Automated archiving of processed files

### Data Transformation

* Declarative ETL pipelines using Apache Spark
* Built-in data quality validation rules
* Automated type normalization and cleaning
* Materialized business views for analytics

### Machine Learning

* Computer vision model trained to classify car damage severity
* Experiment tracking and lifecycle management
* Model registry and versioning
* Batch and real-time inference support

### Analytics & Applications

* SQL warehouse reporting layer
* Natural language data querying interface
* Customer portal for claim submission
* Admin dashboard for claim investigation

---

## Technology Stack

Databricks Lakehouse Platform • Apache Spark • Delta Lake • Python / PySpark • MLflow • Computer Vision (ResNet-based model) • Streaming pipelines • SQL analytics

---

## System Architecture

### End-to-End Lakehouse Architecture

The architecture integrates multiple enterprise data sources including relational databases, streaming telematics feeds, and object storage containing accident images. Incoming data is processed through automated ingestion pipelines and stored in a Medallion Lakehouse consisting of Landing, Bronze, Silver, and Gold layers.

Data validation, transformation, and incremental processing ensure reliability and scalability. The curated datasets power analytics dashboards, real-time applications, and a deployed machine learning model for automated claim verification.

---

## Automated Decision Engine

The claims validation pipeline combines structured business rules and machine learning inference. Policy eligibility, coverage limits, accident speed, and telematics data are validated alongside an AI-based image severity classifier.

Based on these checks, the system automatically determines whether a claim qualifies for immediate approval or requires manual investigation.

---

## Customer Claim Submission Portal

The platform includes a customer-facing submission interface allowing users to upload accident images, enter policy details, and submit claims for automated analysis. This portal connects directly with backend pipelines and deployed ML services to enable near real-time processing.

---

## Analytics Dashboard

Operational dashboards provide insights into insurance performance metrics such as loss ratios, incident distribution, severity classification, and financial impact. Interactive filtering enables stakeholders to monitor risk trends and business performance.

---

## Incident Trend Analysis

Aggregated visualizations highlight incident frequency, severity distribution, and temporal patterns throughout the day. These analytics support proactive risk management and operational planning.

---

## Automated Claim Processing Output

The system produces automated decision results after evaluating image severity, policy coverage, telematics validation, and financial checks. Approved claims are processed automatically, while suspicious cases are routed for manual review. This demonstrates the operational impact of integrating data engineering, analytics, and AI into one platform.

---

## Outcomes

This project showcases how to build a production-ready enterprise data and AI solution capable of:

* Handling multi-source data ingestion
* Supporting real-time analytics
* Automating operational decision workflows
* Deploying machine learning models into business applications

---

## Ideal For

* Data Engineering portfolio projects
* Machine Learning production pipeline demonstrations
* Lakehouse architecture learning
* End-to-end enterprise analytics solutions

