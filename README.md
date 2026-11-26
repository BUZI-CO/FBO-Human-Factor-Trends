# FBO-Human-Factor-Trends
My First Data Analytics Project
<img width="959" height="530" alt="ASRS Excel" src="https://github.com/user-attachments/assets/3a3c7343-1f7e-4243-bc9d-1de9731a76bc" />
<img width="959" height="528" alt="ASRS Excel 2" src="https://github.com/user-attachments/assets/c4b61e54-6081-4a89-95d1-eaba317c88cd" />
<img width="958" height="562" alt="ASRS SQL" src="https://github.com/user-attachments/assets/3871ca1f-4e33-44c7-bf3b-439bb9f5535d" />
<img width="959" height="565" alt="ASRS SQL 2" src="https://github.com/user-attachments/assets/0d4203ae-471f-431a-a8e6-f3db320b9d18" />
[ASRS Query 1.sql](https://github.com/user-attachments/files/35470351/ASRS.Query.1.sql)
USE [ASRS]
GO

SELECT [Event_Date],
[Primary_Cause],
COUNT(CASE WHEN [Human_Factor] = 'Communication Breakdown' THEN 1 END) AS communication_breakdown,
COUNT(CASE WHEN [Human_Factor] = 'Confusion' THEN 1 END) AS confusion,
COUNT(CASE WHEN [Human_Factor] = 'Distraction' THEN 1 END) AS distraction,
COUNT(CASE WHEN [Human_Factor] = 'Fatigue' THEN 1 END) AS fatigue,
COUNT(CASE WHEN [Human_Factor] = 'Human-Machine Interface' THEN 1 END) AS humanmachine_i,
COUNT(CASE WHEN [Human_Factor] = 'Other / Unknown' THEN 1 END) AS other_unknown,
COUNT(CASE WHEN [Human_Factor] = 'Physiological - Other' THEN 1 END) AS physiological_other,
COUNT(CASE WHEN [Human_Factor] = 'Situational Awareness' THEN 1 END) AS situational_awareness,
COUNT(CASE WHEN [Human_Factor] = 'Time Pressure' THEN 1 END) AS time_pressure,
COUNT(CASE WHEN [Human_Factor] = 'Training / Qualification' THEN 1 END) AS training_qual,
COUNT(CASE WHEN [Human_Factor] = 'Troubleshooting' THEN 1 END) AS troubleshooting,
COUNT(CASE WHEN [Human_Factor] = 'Workload' THEN 1 END) AS workload
  FROM [dbo].[cleaned ASRS FBO Human Factors]
  GROUP BY [Event_Date],
[Primary_Cause]
ORDER BY [Event_Date] ASC;

GO
<img width="955" height="367" alt="ASRS SQL 3" src="https://github.com/user-attachments/assets/8c414dbd-c289-4a95-9621-253777128f0b" />
[SQLQuery3.sql](https://github.com/user-attachments/files/35470395/SQLQuery3.sql)
USE [ASRS]
GO

SELECT [Date]
		,[Primary_Problem]
		, TRIM(value) AS human_factor
FROM damage_reports
CROSS APPLY STRING_SPLIT(Human_Factors, ';');

GO
<img width="959" height="563" alt="Power BI 1" src="https://github.com/user-attachments/assets/1129e52b-4841-492e-be8c-cd8457d2eeac" />
<img width="715" height="400" alt="Screenshot 2026-11-21 222854" src="https://github.com/user-attachments/assets/5591f7c3-a609-4d08-828c-ed8f9165b4f9" />

