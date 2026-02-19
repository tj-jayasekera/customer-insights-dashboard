# 🏛️ Customer Insights Dashboard

## 📚 Table of Contents

- [📌 Project Overview](#project-overview)
- [🎯 Business Objective](#business-objective)
- [🛠 Tools](#tools)
- [🏗 Data Architecture](#data-architecture)
- [🤖 AI-Driven NLP Integration](#ai-driven-nlp-integration)
- [📊 Dashboard Implementation](#dashboard-implementation)
- [🔒 Data Governance](#data-governance)
- [🚀 Deployment & Impact](#deployment-and-impact)

## 📌 Project Overview

During my internship at the **City of Melbourne** (Apr 2025 – Jun 2025), I designed and deployed a production-ready [Customer Intelligence Dashboard](https://github.com/tj-jayasekera/customer-insights-dashboard/blob/main/CX%20Dashboard%20CoM.pdf) to replace manual Excel reporting and enable cross-department performance visibility.

The dashboard consolidates:
- Customer survey data
- Genesys call centre voice data
- AI-generated sentiment and topic classifications
- Operational performance metrics

It is now actively used across multiple organisational levels.


## 🎯 Business Objective

The organisation needed a scalable way to:
- Measure customer satisfaction and response rates
- Compare performance across departments and service groups
- Analyse complaint trends
- Extract structured insights from call transcripts
- Enable leadership to track performance over time

Previously, reporting relied heavily on manual spreadsheet processes.
This solution introduced a structured, automated BI framework.

## 🛠 Tools

- **Databricks** – Data transformation, modelling, NLP processing
- **SQL** – Silver/Gold layer table design and KPI logic
- **Power BI** – Interactive dashboard design and automated reporting
- **NLP / AI Models** – Sentiment scoring, topic classification, transcript summarisation
- **Genesys Voice Data** – Call transcript ingestion and analysis

## 🏗 Data Architecture

All raw data (survey + voice transcripts) was hosted in Databricks.

I implemented a layered architecture:

**Silver Layer**
- Cleaned and standardised survey records
- Structured Genesys call transcript data
- Normalised timestamps and service group mappings

**Gold Layer**
- Aggregated department-level performance tables
- Created AI-enriched transcript outputs (topic + sentiment + summary)

All transformations were written in SQL on Databricks and optimised for repeatable execution.

## 🤖 AI-Driven NLP Integration

To enhance voice analytics, I implemented NLP workflows in Databricks to:
- Generate sentiment scores
- Summarise conversations
- Classify transcripts into common topic groups

I manually validated AI outputs to ensure reliability.

**Validation Results:**
- ~93% accuracy in topic classification
- Strong sentiment alignment with transcript context

These AI-derived metrics were integrated directly into Power BI to provide a new lens on departmental performance.


## 📊 Dashboard Implementation

The final dashboard consists of three main pages:

1. **Customer Feedback Analysis**
Survey metrics, performance over time, service-level breakdown
2. 	**Performance Comparison**
Cross-period comparison of departments and service groups
3. **Complaints Analysis**
Focused page for complaint trends and drivers

The dashboard:
- Supports multi-level filtering
- Enables department, service group, and topic analysis
- Displays last refresh timestamp
- Automatically updates from Databricks

[View a PDF of the Dashboard here](https://github.com/tj-jayasekera/customer-insights-dashboard/blob/main/CX%20Dashboard%20CoM.pdf)

## 🔒 Data Governance

The [PDF](https://github.com/tj-jayasekera/customer-insights-dashboard/blob/main/CX%20Dashboard%20CoM.pdf) included in this repository contains redacted screenshots of the dashboard.

Although I used only a small design sample of live data, figures and sensitive metrics have been intentionally blurred to protect privacy and operational confidentiality.

The screenshots demonstrate:
- Layout
- Interactivity
- Filtering structure
- Design logic

## 🚀 Deployment & Impact

- SQL pipelines built for consistent re-execution
- Power BI configured for automated refresh
- Dashboard successfully rolled out organisation-wide
- Actively used across multiple organisational levels

This was my first hands-on experience with both **Power BI** and **Databricks**, and by the end of the internship I was fully confident designing, modelling, and deploying production BI solutions.

