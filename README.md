<div align="center">

# 🚚 Delivery TAT Analytics

### Enterprise Power BI Dashboard for Supply Chain Operations

<p align="center">

<img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black">
<img src="https://img.shields.io/badge/DAX-Advanced-blue?style=flat-square">
<img src="https://img.shields.io/badge/Power_Query-ETL-217346?style=flat-square">
<img src="https://img.shields.io/badge/Star_Schema-Optimized-6A1B9A?style=flat-square">
<img src="https://img.shields.io/badge/Supply_Chain-Analytics-E53935?style=flat-square">

</p>

Built an end-to-end Power BI solution to monitor delivery performance across **1,600+ monthly shipments**, multiple warehouses, sales channels, and courier partners.

</div>

---

# 📑 Table of Contents

- [Dashboard Preview](#dashboard-preview)
- [Business Problem](#business-problem)
- [Solution](#solution)
- [Key Features](#key-features)
- [Dashboard KPIs](#dashboard-kpis)
- [Data Architecture](#data-architecture)
- [Repository Structure](#repository-structure)
- [Power Query ETL](#power-query-etl)
- [DAX Highlights](#dax-highlights)
- [Business Impact](#business-impact)
- [Tech Stack](#tech-stack)
- [Future Improvements](#future-improvements)
- [Author](#author)

---

# Dashboard Preview

## Customer Performance Dashboard

<p align="center">
<img src="Images/Customer Analysis.webp" width="100%">
</p>

---

## Courier Performance Dashboard

<p align="center">
<img src="Images/Courier Analysis.webp" width="100%">
</p>

---

## Data Model
<p align="center">
<img src="Images/Data Mode.webp" width="95%">
</p>

The semantic model follows a Star Schema with a central fact table connected to supporting dimension tables for efficient filtering and optimized DAX calculations.


# Business Problem

The Supply Chain Operations team relied on manually prepared operational reports, making it difficult to:

- Monitor courier performance
- Compare warehouse efficiency
- Track Delivery TAT
- Identify delayed shipments
- Measure Delivery %
- Monitor Fill Rate

As shipment volumes increased, report preparation became slower while operational visibility decreased.

---

# Solution

Developed an enterprise Power BI dashboard that centralized logistics reporting into a single interactive reporting solution.

The dashboard provides:

- Automated reporting for 1,600+ monthly shipments
- Monitoring across 12 logistics partners
- Courier, warehouse and channel performance analysis
- Interactive drill-through reporting
- Real-time KPI monitoring

---

# Key Features

- Dynamic Date Intelligence
- Courier Performance Analysis
- Customer Performance Analysis
- Warehouse Analytics
- Zone-wise Delivery TAT
- Dispatch TAT Monitoring
- Fill Rate Analysis
- Interactive KPI Cards

---

# Dashboard KPIs

| KPI | Description |
|------|-------------|
| Total Dispatched Shipments | Total shipment volume |
| Delivered Shipments | Successfully delivered shipments |
| Delivery % | Delivery success rate |
| Average Dispatch TAT | PO Share → Dispatch |
| Average Delivery TAT | Dispatch → Delivery |
| Fill Rate % | Invoice Qty / KAM Qty |

---

# Data Architecture

```text
Google Sheets
      │
      ▼
Power Query ETL
      │
      ▼
Data Cleaning
      │
      ▼
Data Modeling
      │
      ▼
DAX Measures
      │
      ▼
Power BI Dashboard
```

---

# Repository Structure

```text
Delivery-TAT-Analytics
│
├── README.md
│
├── Images
│   ├── Customer Analysis.webp
│   └── Courier Analysis.webp
│
├── DAX
│   ├── Date Measures.md
│   ├── Date Table.md
│   ├── Operational KPIs.md
│   ├── Shipment KPIs.md
│   └── TAT Measures.md
│
├── Documentation
│   ├── Business Requirements.md
│   ├── Dataset Description.md
│   └── KPIs.md
│
└── Power Query
    ├── Clean
    └── Data Cleaning.md
```

---

# Power Query ETL

Key transformations include:

- Header Promotion
- Data Type Assignment
- Error Handling
- Removing Unused Columns
- Status Standardization
- Courier Name Cleaning
- Removing Cancelled Orders
- Date Formatting
- Data Validation

---

# DAX Highlights

The report includes optimized DAX measures for:

- Shipment Count
- Delivery %
- Dispatch TAT
- Delivery TAT
- Fill Rate
- Dynamic Date Intelligence

Complete DAX documentation is available inside the **DAX** folder.

---

# Business Impact

The dashboard enables Supply Chain teams to:

- Reduce manual reporting effort
- Monitor logistics KPIs in real time
- Identify high-TAT courier partners
- Compare warehouse performance
- Improve delivery visibility
- Track SLA compliance

---

# Tech Stack

| Layer | Technology |
|---------|------------|
| Reporting | Power BI Desktop |
| ETL | Power Query |
| Semantic Model | DAX |
| Data Source | Google Sheets |
| Data Modeling | Star Schema |

---

# Future Improvements

- Incremental Refresh
- Row-Level Security (RLS)
- Microsoft Fabric Integration
- Deployment Pipelines
- Dataflows
- Automated KPI Alerts

---

# Author

## Paras Kumar

**Business Intelligence Analyst**

**Skills:** Power BI • SQL • DAX • Power Query • Excel
