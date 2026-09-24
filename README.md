# 🛡️ Enterprise Intelligence & Customer Retention Platform

> An end-to-end analytics platform that transforms raw transactional data into data quality reports, cohort analytics, leakage-safe RFM churn predictions, executive summaries, and downloadable PowerPoint presentations.

---

## 📐 Platform Architecture

```text
RAW DATA INGESTION (CSV/XLSX)
   │
   ├──> Raw Data Preserved (Read-Only)
   │
   ▼
DATA VALIDATION & CLEANING ──> DATA QUALITY REPORT & DICTIONARY
   │
   ▼
BUSINESS ANALYTICS & COHORTS ──> KPI ENGINE & INTERACTIVE EDA
   │
   ▼
HISTORICAL SNAPSHOT ENGINE ──> Zero Target/Feature Leakage
   │
   ▼
RFM FEATURE ENGINEERING
   │
   ▼
MACHINE LEARNING PIPELINE ──> Logistic Regression & Calibration
   │
   ▼
CUSTOMER RISK SCORING ──> HIGH / MEDIUM / LOW Tiering
   │
   ├──> Interactive Streamlit Dashboards
   ├──> Automated Executive Summaries
   └──> Downloadable PPTX & CSV Exports
