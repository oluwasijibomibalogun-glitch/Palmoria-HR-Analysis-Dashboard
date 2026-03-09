# Palmoria-HR-Analysis-Dashboard
## Description  This project analyzes HR data from Palmora Group using Power BI. The goal is to identify gender distribution, salary structure, and potential pay gaps across different regions and departments.  The dashboard provides insights that can help improve decision-making regarding employee compensation and workforce balance.

## Project Overview
This project focuses on:
•	Gender distribution
•	Salary distribution
•	Minimum salary compliance
•	Bonus calculations
•	Regional analysis

## Tools Used
•	Power BI
•	Power Query
•	DAX
•	Data Visualization

## Dataset Features
The dataset includes:
•	Employee Gender
•	Department
•	Region
•	Salary
•	Rating

## Data Cleaning Actions
The following steps were performed:
•	Replaced blank gender values
•	Removed null departments
•	Removed blank salary rows
•	Cleaned dataset for analysis

## Measures Used
Employees Below Minimum Salary
Employees Below Minimum Salary =
COUNTX(
FILTER(Employee, Employee[Salary] < 90000),
Employee[Salary]
)
Bonus Amount
Bonus Amount =
IF(Employee[Rating] > 3,
Employee[Salary] * 0.1,
0)
Total Amount Paid
Total Amount Paid =
Employee[Salary] + [Bonus Amount]

## Dashboard Features
The dashboard includes:
•	Gender distribution charts
•	Salary distribution charts
•	Bonus payout charts
•	Regional comparison
•	Department comparison

## Key Insights
•	Male employees are more than female employees
•	Generic gender is the smallest group
•	Total departments after cleaning: 12
•	Minimum salary is consistent across regions
•	Average salary differs by region
The required minimum salary is about 90K
Palmoria’s average salary is about 73.7K
Many employees earn below the required minimum
Even after bonuses, many salaries are still below the requirement

<img width="874" height="486" alt="Overview" src="https://github.com/user-attachments/assets/acdd61b3-968d-4a5c-8fbc-c24284493fac" />

<img width="869" height="490" alt="Performance Analysis" src="https://github.com/user-attachments/assets/58e4ee64-6091-4108-bd95-91a25f5adc87" />

<img width="868" height="486" alt="image" src="https://github.com/user-attachments/assets/09ea7c3f-3156-4044-aad8-f62a6e19aedb" />

<img width="870" height="490" alt="image" src="https://github.com/user-attachments/assets/d0afa45c-2cc8-487e-8a07-5912e3c0ce51" />

<img width="871" height="489" alt="image" src="https://github.com/user-attachments/assets/bbab9a0c-c3dd-48c8-93d3-babe28a0c86d" />

<img width="873" height="550" alt="image" src="https://github.com/user-attachments/assets/2b642d3f-58c2-4414-ab4f-51d5e556196e" />
