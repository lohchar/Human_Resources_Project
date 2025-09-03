# Human_Resources_Project
Data & Business Analysis, Visualization and PCA
## Overview
 This project explores the Human Resources Data Set from Kaggle. The dataset contains information about employees, such as demographics, job roles, performance, and attrition. The goal is to analyze HR patterns and apply machine learning for basic regression and gain insights into workforce management.
### Part A: Basic EDA (Exploratory Data Analysis)
- Loaded dataset and printed first 5 rows
- Checked shape of dataset which is 311 columns and 36 columns
- Displayed column name and their datatypes. Employee_Name was the only object type
- Employee_Name and EmpID had the most unique values (311) while MarriedID and GenderID had lowest (2).
- Checked missing values where DateofTermination had 207 and ManagerID 8
- Described numerical columns and printed their mean, median and standard deviation.
- Showed the distribution of employee salaries using a Histogram where most salaries were between 50,000 and 80,000
- Claculated the average age of employees at the company which was 33.06
- 207 employees were employed, 88 were voluntarily terminated and terminated for cause
- Production department had the most employees 209 while executive office had the lowest, 1.
### Part B: Business Analysis
- Calculated average salary where Executive Office department had the highest, 250,000 while production department had the lowest, 59953.545455.
- Visualized distribution of employment status using a piechart where Active had the largest propotion of 66.6% and smallest is Terminated  for Cause
- Used boxplot to compare between male and female employees. Male had slightly higher mean and median compared to female. 
- Identified Indeed as the recruitment source that brought in most employees i.e 87 recruits while Online Web application brought 1 recruit.
- 93% of employees attended a Diversity Job Fair.
- Compared engagement survey scores where Executive Office had the highest score 4.830000 and sales the lowest 3.818710
- Identified Hispanic as the race with the highest average salary 8,3667
- Used a scatterplot to show relationship between number of projects and salary.The data points appear to be widely scattered, suggesting that the number of projects an individual works on is not a strong predictor of their salary.(clear strong positive or negative linear relationship).
- Verified that married employees (69827.717742) earn more on average than single employees(68485.540107).
- Michael Albert is the manager that have the largest teams, 22 employees.
### Part C: Data Visualizaton
- Plotted salary distribution using histogram where most salaries were between 48,000 and 100,000
- Visualized count of employees by department using countplot where production had the most employees and executive office lowest
- Software Engineering department had the highest average satisfaction score while Executive Office had the lowest as visualized by the barplot
- Visualized employee terminations over the years using a barplot where 2015 had the most terminations while 2010 had the lowest terminations.
- Used boxplot to visualise average salary by gender where male had slighlty higher average salary compared to female
- Visualized relatinship between perfomance scores and salary using a stripplot which indicates that employees with higher perfomance scores had the highest salaries. 
- Used heatmap to show correlation between numeric variables. It shows strong positive correlation between variables like Termd and EmpStatusID(0.95). Variables like SpecialProjectCount show strong negative correlation of -0.79.
- Visualized the relationship between engagement and satisfaction score using a scatterplot. It shows there is a positive correlation where by the engagement score increases on x-axis as well as satisfaction score which increase on y-axis.
- Visualised the distribution of employee status across departments using a stacked bar plot. Production department has the highest total number of employees, with a large majority being active.
Visualized the distribution of Absentism among employees uisng a histogram. The plot indicates that the most frequent absence totals among the employees are shown by the highest bars at approximately 4 and 16 absences.
### Part D: PCA (Dimensionality Reduction)
- StandardizeD numerical features before applying PCA
- ManagerID was identified as the column with missing values, 8.
- Performed PCA on the dataset and shown the first 2 components i.e PC1 and PC2.
- Visualized the explained variance ratio for the PCA components where by PC1 had large +ve value e.g 2.095023 which is strongly correlated with the first component.
- Visualized the explained variance ratio for the PCA components using a barplot. Principal component 1 has a taller bar compared to PC2 indicating it explains the largest portion of variance in the original data.
- Reduced the dataset to 2 dimensions with PCA and visualised employees colored by department using a scatterplot.The points are employees which are colored by their department.
- Identified PerfScoreID, EngagementSurvey, SpecialProjectsCount, EmpSatisfaction and Salary as top 5 variables contributing the most to the first principal component.
- Applied PCA to engagement, satisfaction, absences and got 0.39958328 as the Variance Ratio for the Principal Component. Indicates the sinngle component can explain around 39.95% of the total variance in the 3 variables. This suggests single dimmension is not sufficient info in the 3 variables hence do not condense to one dimension.
- Visualized employees in PCA-reduced 2D space grouped by PerformanceScore using a scatter plot. It shows the color-coding of the points based on the perfomance score. 
- Compared clustering before and after PCA using k-means on numeric data and visualised them using scatterplos. In the scatterplot of Before PCA, the clusters are somehow mixed and less distinct due to the complex relationships across most features. The second scatterplot is for After PCA, whereby the clusters appear to be more distinct and more spatially separated.
- Visualised loadings of salary, absences, and engagement on the first 2 principal Components.
- 
