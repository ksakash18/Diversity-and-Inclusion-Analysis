# Diversity and Inclusion Analysis

## Problem statement
•	Human Resources at phonenow is highly into diversity and inclusion. They’ve been working hard to improve gender balance at the executive management level, but they’re not seeing any progress. 

## Project Goals:
•	Create visualizations to represent HR data, particularly focusing on gender-related KPIs.
•	Identify and discuss potential root causes for the slow progress in achieving gender balance at the executive management level.
• Define relevant KPIs in hiring, promotion, performance and turnover, and create a visualisation
• Find out some root causes of slow progress.

## Data Analysis Summary



![photo_2025-02-10_21-03-43](https://github.com/user-attachments/assets/d90a2035-e805-408e-bf52-674699255e4b)

![photo_2025-02-10_21-03-47](https://github.com/user-attachments/assets/21346e46-fd2f-4fa1-b48d-47c01dd93da7)
•	All job levels are male-dominated in hiring. Only 12.50% of executive positions were occupied by women after FY20 promotions. The junior officer level has a higher proportion of women compared to other levels.
•	Promotions at the executive and director levels are predominantly awarded to men. Junior and senior officer promotions show comparatively less variation.
•	Female senior managers and junior officers who left the company had higher performance ratings than those who stayed.
•	All male employees who left the company had higher performance ratings than those who stayed.
•	No women were hired or promoted to the executive level.
•	There is a significant gender imbalance at the executive level, with men holding the majority of leadership positions.

## Measure and visualisation
four slicers are used for department,job level,region and age group.
Made use of clustered column charts ,line charts ,pie charts and stacked bar charts for visualization.
# of men = CALCULATE(COUNTA('Backing 1'[GENDER]),'Pharma Group AG'[Gender]="Male")
# of women = CALCULATE(COUNT('Pharma Group AG'[Gender]),'Pharma Group AG'[Gender]="Female")
#avg rating of men = CALCULATE(AVERAGE('Pharma Group AG'[FY20 Performance Rating]),'Pharma Group AG'[Gender]="Male")
#avg rating women = CALCULATE(AVERAGE('Pharma Group AG'[FY20 Performance Rating]),'Pharma Group AG'[Gender]="Female")
#employees promoted in 2020 = CALCULATE(COUNT('Pharma Group AG'[Promotion in FY20?]),'Pharma Group AG'[Promotion in FY20?]="Y")
% hires men = DIVIDE('Base measures'[# of men],'Base measures'[Total employees])
% Promotees who were women = Divide(Calculate(distinctcount('Pharma Group AG'[Employee ID]),Filter('Pharma Group AG','Pharma Group AG'[Gender]="Female")),distinctcount('Pharma Group AG'[Employee ID]))
% Promotees who were women = Divide(Calculate(distinctcount('Pharma Group AG'[Employee ID]),Filter('Pharma Group AG','Pharma Group AG'[Gender]="Female")),distinctcount('Pharma Group AG'[Employee ID]))

## Solution
•	All job levels are male-dominated in hiring. Only 12.50% of executive positions were occupied by women after FY20 promotions. The junior officer level has a higher proportion of women compared to other levels.
•	Promotions at the executive and director levels are predominantly awarded to men. Junior and senior officer promotions show comparatively less variation.
•	Female senior managers and junior officers who left the company had higher performance ratings than those who stayed.
•	All male employees who left the company had higher performance ratings than those who stayed.
•	No women were hired or promoted to the executive level.
•	There is a significant gender imbalance at the executive level, with men holding the majority of leadership positions.

## conclusion
•	Hiring at the executive level is highly imbalanced, with men dominating these positions. Women have fewer opportunities.
•	Promotions at the executive level are heavily biased in favor of men.



