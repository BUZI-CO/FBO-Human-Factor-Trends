# Fixed Base Operator Human Factor Trend Analysis (2016–2025)

## Project Overview

An analysis of human factor trends in Fixed Base Operator (FBO)
operations using data from NASA's Aviation Safety Reporting System
(ASRS). This repository documents the technical workflow, from
initial data exploration and transformation in SQL Server to
visualization in Power BI.

**Tools & Technologies:** SQL Server | SSMS | Power BI | Excel

[View Full Project Portfolio](https://claude.ai/artifact/AeUJjvShNzHA22fqVwg3ZH#fbo)

---

## 1. Data Acquisition

The original dataset was obtained from NASA's Aviation Safety
Reporting System (ASRS) and contains aviation incident records
relevant to the analysis of human factors in FBO operations.

[Download Original Dataset (.csv)](https://github.com/user-attachments/files/35474841/ASRS_DBOnline.FBO.Human.Factors.csv)

<!-- Insert ASRS Excel.png here -->

---

## 2. Data Exploration

Used SQL Server to explore the dataset and extract relevant
variables, including event date, reporter organization,
primary problem, and contributing human factors.

[Download Data Exploration Script (.sql)](https://github.com/user-attachments/files/35476672/ASRS.Query.1.sql)

<!-- Insert ASRS SQL.png here -->

---

## 3. Human Factor Extraction and Analysis

Used SQL to examine individual human factor categories,
apply conditional aggregations, and prepare multi-value
human factor records for further analysis.

[Download Human Factor Analysis Script (.sql)](https://github.com/user-attachments/files/35476686/SQLQuery3.sql)

<!-- Insert ASRS SQL 2.png here -->

---

## 4. Data Preparation

Structured the dataset so that each row represented an
individual human factor occurrence, enabling analysis
across human factor categories and reporting periods.

[Download Cleaned Dataset (.csv)](https://github.com/user-attachments/files/35475650/cleaned.ASRS.FBO.Human.Factors.csv)

<!-- Insert ASRS Excel 2.png here -->

---

## 5. Power Query Transformation

Imported the cleaned dataset into Power BI and used
Power Query to transform event dates and prepare
the data for annual and quarterly trend analysis.

<!-- Insert Power BI 1.png here -->

---

## 6. Power BI Dashboard

Developed an interactive dashboard to visualize 3,473
human factor occurrences across 12 categories.

The dashboard enables analysis of:

- Annual human factor trends from 2016 to 2025
- Total occurrences by human factor category
- Quarterly totals and annual averages
- Category-specific trends through interactive filtering

<!-- Insert Screenshot 2026-11-21 231615.png here -->

---

## Data Source

[NASA Aviation Safety Reporting System (ASRS)](https://asrs.arc.nasa.gov/)

ASRS reports are voluntarily submitted. Reported occurrences
should not be interpreted as definitive aviation incident rates.
