# Project Title: Production Performance Analytics Dashboard | Data Cleansing & KPI Visualization 

Executed an end-to-end data analysis project to transform raw, inconsistent production data into an interactive Excel dashboard. The goal was to provide management with clear, accurate, and actionable insights into operational efficiency, cost drivers, and resource allocation across product lines and managers.

## The Problem:
The initial dataset suffered from a critical data integrity issue: the Age attribute for production managers was inconsistent and inaccurate. The same manager appeared with multiple different ages, rendering any people-centric analysis (like performance by experience) unreliable and untrustworthy.

## uncleaned dataset i used:-
- <a href = https://github.com/Basavaraj-coder/Production-Performance-Analysis/blob/main/Excel%2BReport%2B2.xlsx> Production dataset </a>
## Cleaned Transformed Dataset:-
- <a href = https://github.com/Basavaraj-coder/Production-Performance-Analysis/blob/main/Excel%2BReport%2B2%20cleaned%20production.xlsx> Cleaned Production Dataset </a>

## My Analytical Process
Define Objective & Understand Data: The goal was to create a single source of truth for production performance. I started by thoroughly examining the dataset, where I immediately identified the inconsistent "Age" data for managers.

Data Cleaning & Validation (The Critical First Step):

I used =XLOOKUP() to create a correct mapping of each manager to a single, accurate age value by fetching the first occurrence of each manager's name.

I then used Paste Special -> Values to hardcode these correct ages, replacing the flawed column and ensuring the base data was reliable for all subsequent analysis.

Feature Engineering: I created new calculated columns:

Age Groups using =IF() logic to categorize managers for demographic analysis.

Production Cost Per Unit (a crucial KPI) by dividing TotalCost by UnitsProduced.

Exploratory Data Analysis (EDA) with PivotTables: I built multiple PivotTables to explore relationships between fields like Manager, ProductType, Date, and my new KPIs.

Dashboard & Visualization: I synthesized the key findings from my EDA into an interactive dashboard using PivotCharts and Slicers, designed for clarity and user-driven exploration.

## Value Delivered:

Data Integrity: Resolved critical data inconsistencies, establishing a reliable dataset for accurate decision-making.

Operational Insight: Provided management with an at-a-glance view of production health, identifying cost inefficiencies and productivity trends.

Data-Driven Culture: Empowered stakeholders with a self-service tool to independently explore data and answer their own questions, reducing the reporting burden on analysts.

## Technical Skills Demonstrated:

Data Cleansing: XLOOKUP(), Data Validation, Paste Special Operations

Data Transformation: Formula-based Column Creation (IF Logic, Arithmetic Operations)

Data Analysis & Visualization: PivotTables, PivotCharts (Column, Bar, Pie, Line Charts)

Dashboarding: Slicers, Interactive Reporting, Dashboard Layout & Design

Attention to Detail: Meticulous data quality assurance and error handling.

## Questions
Based on your dashboard, how would you answer these?

Overall Performance: Which product type has the highest total production cost, and what does that signify?

Efficiency Analysis: Which product type has the highest average cost per unit? Is this a problem, and why?

Manager Performance: Which manager is handling the most production tasks? Does high volume always mean high cost?

Trend Analysis: What is the overall trend in units produced? Was there a significant peak or dip in a particular month?

Data Quality: Walk me through the steps you took to identify and fix the data integrity issue with the managers' ages. Why was this crucial?

## Project Insights Derived
Highest Investment Area: Automobiles has the highest total production cost ($1.15M), indicating it is the most resource-intensive product line and a key area of focus for the business.

Cost Inefficiency Identification: Despite Furniture not having the highest total cost, it has the highest average production cost per unit ($180.44). This signals potential inefficiencies in its manufacturing process or supply chain that require immediate investigation to improve profitability.

Top Performer by Volume: Nancy Grey manages the highest number of production tasks (37). However, further analysis is needed to cross-reference this with cost and quality metrics to determine true performance.

Production Growth: The data shows a strong upward trend in units produced from 2023 into 2024, with significant growth beginning in October 2023. This indicates successful scaling of operations or increased market demand.

