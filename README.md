# 🚚 Delivery TAT Analytics

<p align="center">

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Advanced-blue?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power_Query-ETL-success?style=for-the-badge)
![Supply Chain](https://img.shields.io/badge/Domain-Supply_Chain-orange?style=for-the-badge)
![Star Schema](https://img.shields.io/badge/Data_Model-Star_Schema-red?style=for-the-badge)

</p>

---

## Dashboard Preview

### Executive Dashboard

![Dashboard](Images/Dashboard.png)

---

## Project Overview

Delivery TAT Analytics is an enterprise Power BI reporting solution developed for Supply Chain Operations to monitor shipment movement, courier performance, warehouse efficiency, and delivery service levels.

The dashboard consolidates operational data into a centralized reporting model, enabling stakeholders to track logistics KPIs, identify high-turnaround-time couriers, and improve delivery performance through data-driven decision making.

---

## Business Problem

The logistics team relied on manual operational reports spread across multiple sources, making it difficult to:

- Monitor courier performance
- Measure delivery turnaround time
- Compare warehouse efficiency
- Track delivery success rates
- Analyze shipment performance across channels

This resulted in delayed operational decisions and limited visibility into logistics performance.

---

## Solution

Developed an end-to-end Power BI solution using:

- Power Query for ETL
- Star Schema data model
- Optimized DAX measures
- Interactive dashboards
- Dynamic filtering
- Operational KPI tracking

---

## Dashboard Features

- Executive KPI Cards
- Courier Performance Analysis
- Channel-wise Delivery Analysis
- Zone-wise Delivery TAT
- Dynamic Date Selection
- Warehouse Performance
- Delivery %
- Dispatch TAT
- Fill Rate
- Interactive Drilldowns

---

## Technology Stack

| Layer | Technology |
|--------|------------|
| Reporting | Power BI |
| ETL | Power Query (M) |
| Semantic Layer | DAX |
| Data Modeling | Star Schema |
| Source | Google Sheets |
| Visualization | Power BI Desktop |

---

## Key Performance Indicators

| KPI | Description |
|------|-------------|
| Total Dispatched Shipments | Number of shipments dispatched |
| Delivered Shipments | Successfully delivered shipments |
| Delivery % | Delivery success rate |
| Average Dispatch TAT | Dispatch efficiency |
| Average Delivery TAT | Delivery performance |
| Fill Rate % | Inventory fulfilment |

---

## Dashboard Pages

### Customer Analysis

![Customer Analysis](Images/Customer%20Analysis.webp)

---

### Courier Analysis

![Courier Analysis](Images/Courier%20Analysis.webp)

---

## Data Model

This solution follows a Star Schema consisting of:

- Fact Table
    - ST - 2026

- Dimension Tables
    - Date
    - Channels
    - Warehouse

Detailed documentation is available under:

```
Data Model/
```

---

## ETL Pipeline

```
Google Sheets
      │
      ▼
Power Query
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

## Repository Structure

```
Delivery-TAT-Analytics
│
├── DAX
├── Data Model
├── Documentation
├── Images
├── Power Query
└── README.md
```

---

## Business Impact

This dashboard enables the operations team to:

- Monitor logistics performance in real time
- Identify high TAT couriers
- Improve delivery visibility
- Measure warehouse efficiency
- Track service level KPIs
- Reduce manual reporting effort

---

## Future Improvements

- Incremental Refresh
- Row-Level Security
- Deployment Pipelines
- Microsoft Fabric Integration
- Dataflows
- Automated Alerts

---

## Author

**Paras Kumar**

Business Intelligence Analyst

Power BI • SQL • Excel • DAX • Power Query
