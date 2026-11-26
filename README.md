# Fixed Base Operator Human Factor Trend Analysis (2016–2025)

## Project Overview

An analysis of human factor trends in Fixed Base Operator (FBO)
operations using data from NASA's Aviation Safety Reporting System
(ASRS). This repository documents the technical workflow, from
initial data exploration and transformation in SQL Server to
visualization in Power BI.

**Tools & Technologies:** SQL Server | SSMS | Power BI | Excel

[View Full Project](https://claude.ai/artifact/AeUJjvShNzHA22fqVwg3ZH#fbo)

---

## 1. Data Acquisition

The original dataset was obtained from NASA's Aviation Safety
Reporting System (ASRS) and contains aviation incident records
relevant to the analysis of human factors in FBO operations.

[Download Original Dataset (.csv)](https://github.com/user-attachments/files/35474841/ASRS_DBOnline.FBO.Human.Factors.csv)

<img width="959" height="530" alt="ASRS Excel" src="https://github.com/user-attachments/assets/9d9d4557-acd4-432f-b188-b316de349b3f" />


---

## 2. Data Exploration

Used SQL Server to explore the dataset and extract relevant
variables, including event date, reporter organization,
primary problem, and contributing human factors.

[Download Data Exploration Script (.sql)](https://github.com/user-attachments/files/35476672/ASRS.Query.1.sql)

<img width="959" height="565" alt="ASRS SQL 2" src="https://github.com/user-attachments/assets/d8e1c38b-ab11-4a06-bfcd-12cbb0fa9961" />


---

## 3. Human Factor Extraction and Analysis

Used SQL to examine individual human factor categories,
apply conditional aggregations, and prepare multi-value
human factor records for further analysis.

[Download Human Factor Analysis Script (.sql)](https://github.com/user-attachments/files/35476686/SQLQuery3.sql)

<img width="955" height="367" alt="ASRS SQL 3" src="https://github.com/user-attachments/assets/2bc358f8-17f8-4bb3-a215-2d6964967a2e" />


---

## 4. Data Preparation

Structured the dataset so that each row represented an
individual human factor occurrence, enabling analysis
across human factor categories and reporting periods.

[Download Cleaned Dataset (.csv)](https://github.com/user-attachments/files/35475650/cleaned.ASRS.FBO.Human.Factors.csv)

<img width="959" height="528" alt="ASRS Excel 2" src="https://github.com/user-attachments/assets/0b031554-17d6-4193-a9d0-90074ade430c" />


---

## 5. Power Query Transformation

Imported the cleaned dataset into Power BI and used
Power Query to transform event dates and prepare
the data for annual and quarterly trend analysis.

<img width="959" height="563" alt="Power BI 1" src="https://github.com/user-attachments/assets/ed8f8e13-1bf5-4080-8114-f20914ff4544" />


---

## 6. Power BI Dashboard

Developed an interactive dashboard to visualize 3,473
human factor occurrences across 12 categories.

The dashboard enables analysis of:

- Annual human factor trends from 2016 to 2025
- Total occurrences by human factor category
- Quarterly totals and annual averages
- Category-specific trends through interactive filtering

[Power BI Dashboard](https://app.powerbi.com/groups/me/reports/7750c434-5674-43c0-908c-d42795d14c85/d1c2b9764db1c78fbbcd?experience=power-bi)

<img width="713" height="401" alt="Screenshot 2026-11-21 232857" src="https://github.com/user-attachments/assets/cae82e54-ec03-4569-9c7a-dc48c3ca8af7" />


---

## Data Source

[NASA Aviation Safety Reporting System (ASRS)](https://asrs.arc.nasa.gov/search/database.html)

ASRS reports are voluntarily submitted. Reported occurrences
should not be interpreted as definitive aviation incident rates.
