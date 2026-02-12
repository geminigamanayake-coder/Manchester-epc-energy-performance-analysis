# Energy Performance Analysis of Manchester Local Authorities: SQL & Power BI Implementation

This project investigates energy efficiency patterns across Greater Manchester using Energy Performance Certificate (EPC) data from 2014–2024. By combining SQL Server for backend data processing with an interactive Power BI dashboard, the project delivers insights into energy performance, cost burdens, emissions levels, and improvement opportunities across property types and local authorities.

---

## Project Overview

* Analyze large-scale EPC certificate data to evaluate regional energy efficiency trends
* Measure the gap between current and potential energy performance ratings
* Quantify heating and lighting cost burdens across property types
* Identify the most frequently recommended and highest-impact energy improvement measures
* Provide actionable insights for policymakers, sustainability planners, and property stakeholders

---

## Dataset

Source: UK Energy Performance Certificate (EPC) Register
Format: CSV datasets processed in SQL Server
Coverage: Greater Manchester, 2014–2024

Dataset includes:

* Energy efficiency scores (current and potential)
* Heating and lighting cost estimates
* CO₂ emissions
* Property type classifications
* Recommended energy improvement measures

Total Records:

* 326,000+ EPC Certificates
* 1,000,000+ Recommendations
* 85% of properties identified with improvement potential

---

## Project Components

### 1. SQL Analysis

SQL Server was used to clean, integrate, and structure the data for analysis.

Key processes:

* Data cleaning and validation
* Cost standardization and outlier handling
* Safe type conversion using TRY_CAST()
* Dataset integration using LMK_KEY
* Creation of structured analysis tables:

  * clean_certificates
  * clean_recommendations
* KPI calculations and aggregations

Key analytical outputs:

* Average energy efficiency (current vs potential)
* Annual heating and lighting cost comparisons
* Emissions analysis
* Property-type distribution and performance comparison
* Recommendation frequency analysis

SQL scripts are located in the `sql/` directory.

---

### 2. Power BI Dashboard

An interactive Power BI dashboard was developed to visualize key findings.

Dashboard features:

* KPI cards showing current vs potential averages
* Donut charts for property-type distribution
* Scatter plots analyzing heating vs lighting cost correlation
* Geospatial mapping by local authority
* Recommendation frequency breakdown
* Comparative analysis of energy efficiency across property types

The dashboard uses Import Mode for optimized performance and DAX measures for KPI calculations.

Power BI Dashboard:
[https://drive.google.com/file/d/1RP0WksukF4vYe3EdqYhzEuAJuwGa7s3Z/view?usp=drive_link](https://drive.google.com/file/d/1RP0WksukF4vYe3EdqYhzEuAJuwGa7s3Z/view?usp=drive_link)

---

### 3. Project Report and Video

The repository includes:

* Full analytical report (PDF) detailing methodology, SQL implementation, and insights
* Project demonstration video explaining findings and dashboard functionality

Project Overview Video:
[https://drive.google.com/file/d/1Ggp5H36fQi2XzsiCqUkUN44QngCWZ-Nj/view?usp=drive_link](https://drive.google.com/file/d/1Ggp5H36fQi2XzsiCqUkUN44QngCWZ-Nj/view?usp=drive_link)

---

## Key Findings

* Average current energy efficiency score: 67.26
* Average potential energy efficiency score: 79.12
* 85% of properties have measurable improvement potential
* Heating costs (£570.45 annually) significantly exceed lighting costs (£73.52 annually)
* Houses incur the highest combined energy costs
* Flats are the most energy-efficient property type (average score ~73)
* Park Homes are the least energy-efficient (average score ~42)
* Most common recommendations:

  * Low-energy lighting
  * Cavity wall insulation
* High-impact carbon reduction measures include solar PV panels and advanced heating systems

---

## Limitations

* EPC Register covers approximately 60% of buildings (primarily properties built, sold, or rented since 2008)
* No socio-economic variables included (e.g., income, fuel poverty levels)
* Geographic granularity limited to local authority boundaries
* Recommendations reflect potential improvements, not confirmed installations

---

## Recommendations

* Integrate socio-economic datasets to analyze fuel poverty risks
* Incorporate postcode-level data for more granular geographic insights
* Develop predictive models to forecast cost savings and emissions reductions
* Expand analysis to include retrofit implementation tracking

---

## Impact

* Provides data-driven insight into regional energy efficiency performance
* Supports sustainability planning and carbon reduction strategies
* Demonstrates scalable SQL data engineering and BI reporting capabilities
* Highlights measurable cost-saving opportunities for households

---

## Tools & Technologies

* SQL Server
* T-SQL
* Power BI
* DAX
* Data Cleaning & Transformation
* Geospatial Analysis

---

## Author

Gemini Gamanayake
BSc in Applied Data Science Communication (Undergraduate)

