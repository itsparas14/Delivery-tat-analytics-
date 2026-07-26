<div align="center">

# 🚚 Delivery TAT Analytics

### Enterprise Power BI Dashboard for Supply Chain Operations

<p align="center">

<img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black" alt="Power BI">
<img src="https://img.shields.io/badge/DAX-Advanced-blue?style=flat-square" alt="DAX">
<img src="https://img.shields.io/badge/Power_Query-ETL-217346?style=flat-square" alt="Power Query">
<img src="https://img.shields.io/badge/Star_Schema-Optimized-6A1B9A?style=flat-square" alt="Star Schema">
<img src="https://img.shields.io/badge/Supply_Chain-Analytics-E53935?style=flat-square" alt="Supply Chain">

</p>
---

Built an end-to-end Power BI solution to monitor delivery performance across
**1,600+ monthly shipments**, multiple warehouses, channels and courier partners.

</div>

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

# Business Problem

The Supply Chain Operations team relied on manually prepared operational reports that made it difficult to:

- Monitor courier performance
- Compare warehouse efficiency
- Track Delivery TAT
- Identify delayed shipments
- Measure Delivery %
- Monitor Fill Rate

As shipment volume increased, generating reports became time-consuming and operational visibility decreased.

---

# Solution

Developed an enterprise Power BI dashboard that centralizes logistics reporting into a single interactive reporting solution.

The report enables operations teams to monitor logistics KPIs in real time while drilling down by:
• Automated reporting for 1,600+ monthly shipments

• Monitored performance across 12 logistics partners

• Centralized courier, warehouse, and channel analytics

• Reduced manual KPI reporting through interactive dashboards


---

# Key Features

✅ Dynamic Date Intelligence

✅ Courier Performance Analysis

✅ Channel Performance Analysis

✅ Zone-wise Delivery TAT

✅ Interactive KPI Cards

✅ Warehouse Analytics

✅ Fill Rate Analysis

✅ Dispatch TAT Monitoring

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

```
Google Sheets
        │
        ▼
 Power Query (ETL)
        │
        ▼
 Data Cleaning
        │
        ▼
 Star Schema
        │
        ▼
 DAX Measures
        │
        ▼
 Power BI Dashboard
```

---

# Repository Structure

```
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
│   ├── DateTable.md
│   ├── Operational KPIs.md
│   ├── Shipment KPIs.md
│   └── TAT Measures.md
│
├── Documentation
│   ├── Business Requirements.md
│   ├── Dataset Description.md
│   └── KPIs.md
│
├── Data Model
│   └── Relationships.md
│
└── Power Query
    ├── Clean
    └── Data Cleaning.md
```

---

# Data Model

The report follows a **Star Schema** consisting of:

### Fact Table

- ST - 2026

### Dimension Tables

- dateTable
- Channels
- Warehouse

Relationship documentation is available inside the **Data Model** folder.

---

# Power Query ETL

The dataset undergoes the following transformations before loading into the semantic model:

- Header Promotion
- Data Type Assignment
- Remove Unused Columns
- Replace Errors
- Status Standardization
- Remove Cancelled Orders
- Courier Name Standardization
- Derived Month Name
- Data Validation

---

# DAX Highlights

The report includes optimized DAX measures for:

- Dynamic Date Selection
- Dispatch TAT
- Delivery %
- Shipment Count
- Fill Rate
- Date Intelligence

Documentation for every measure is available inside the **DAX** folder.

---

# Business Impact

The dashboard enables Supply Chain Operations to:

- Reduce manual reporting effort
- Monitor logistics KPIs in real time
- Identify high TAT courier partners
- Improve delivery visibility
- Compare warehouse performance
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
- Row-Level Security
- Microsoft Fabric
- Deployment Pipelines
- Dataflows
- Automated Alerts

---

# Author

## Paras Kumar

**Business Intelligence Analyst**

Power BI • SQL • DAX • Power Query • Excel
