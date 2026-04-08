
# State of Good Repair (SOGR) Dashboard

### Executive Analytics for Windows 11 Upgrade Program

## Overview

This project is an **executive-level Power BI dashboard** built to track and analyze the progress of the Windows 11 upgrade program across the organization.

The dashboard consolidates operational data from systems like ServiceNow, SCCM, and asset tracking tools to provide leadership with a **real-time view of upgrade progress, backlog, performance trends, and operational bottlenecks**.

It is designed to answer key questions such as:

* How many RITMs are being completed daily, weekly, and monthly?
* Is upgrade velocity improving or declining?
* Where are the largest backlogs located?
* Which teams or assignment groups are performing best?
* What is preventing assets from being upgraded?

---

## Key Features

### Executive Summary Layer

* Real-time KPI cards:

  * Closed Today / Week / Month / Quarter / Year
  * Open RITMs
  * Upgrade Percentage
* Dynamic narrative insights:

  * Daily performance summaries
  * Week-over-week comparisons
  * Program-wide observations
* Automated “Last Refreshed” timestamp

### Performance Tracking

* Daily completion trend visualization
* Week-over-week and month-over-month comparisons
* Completion pace indicators (increase/decrease vs prior periods)

### eographic & Asset Insights

* Interactive map of asset locations
* Identification of backlog concentration (e.g., high-volume sites like 2 Broadway)
* Location-level breakdowns of upgrade activity

### 🏢 Operational Breakdown

* Assignment group performance analysis
* Replacement scenarios:

  * New asset replacement
  * Already upgraded
  * Not in use / inactive devices
* Model-level and device-level tracking

### Drill-Down Capabilities

* Searchable RITM lookup
* Detailed table view of:

  * RITM
  * Serial Number
  * State (Work in Progress, Closed Complete)
  * IP Address
* Filtering by:

  * State
  * Assigned Technician
  * Location

---

## Dashboard Pages

### 1. Executive Summary

A high-level overview designed for leadership:

* Key KPIs and completion metrics
* Program health summary
* Automated insights and performance commentary

### 2. Operational Dashboard

Deep-dive analytics including:

* Asset distribution map
* Open vs closed RITMs
* Assignment group performance
* Replacement scenario breakdown
* Technician productivity tracking

---

## Tools & Technologies

* **Power BI** – dashboard development and visualization
* **DAX** – KPI calculations and time-based logic
* **Power Query (M)** – data transformation and cleaning
* **ServiceNow + SCCM data integration**
* **Excel / SharePoint pipelines (via Power Automate)**

---

## Data Model & Logic

The dashboard integrates multiple datasets including:

* RITM tracking data (ServiceNow)
* Asset inventory (SCCM)
* Location mapping data

Key logic includes:

* Time-based aggregations (Today, Week, Month, Quarter, Year)
* Distinct RITM counting to avoid duplication
* Status-based filtering (e.g., Closed Complete vs Work in Progress)
* Conditional formatting for performance indicators (↑ ↓ trends)

---

## Screenshots

### Executive Summary

![Executive Summary](images/executive-summary.png)

### Operational Dashboard

![Operational Dashboard](images/operational-dashboard.png)

---

## Business Impact

This dashboard was built to replace manual reporting and provide:

* **Real-time visibility** into upgrade progress across thousands of assets
* **Improved decision-making** through clear KPIs and trends
* **Faster identification of bottlenecks** (locations, teams, devices)
* **Standardized reporting** across multiple stakeholders
* **Operational efficiency gains** by reducing reliance on manual Excel tracking

---

## Why This Project Matters

Instead of just visualizing data, this project focuses on:

* Translating operational data into **actionable insights**
* Designing for **executive consumption**
* Building a **scalable reporting framework**
* Bridging the gap between **technical systems and business decision-making**

---

## Future Improvements

* Forecasting upgrade completion timelines
* SLA tracking and alerting
* Drill-through pages for individual locations
* Integration with real-time APIs
* Automated anomaly detection

---

## Repository Structure

```bash
SOGR-PowerBI-Dashboard/
│
├── SOGR_Dashboard.pbix
├── images/
│   ├── executive-summary.png
│   └── operational-dashboard.png
└── README.md
```
