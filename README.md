# POWER BI REAL LIFE DATA DOCUMENTATION

## LITA-HR-DATA

### Data Source
This data was provided by our facilitator

### Data Description
   The dataset contains 1,470 employee records across 41 columns, providing a comprehensive overview of various HR-related details.
**Employee Attributes**: The dataset includes information on employee ID, gender, age, marital status, education level, and department, with fields like Employee Number, Gender, Age, Department, and Education Field.

**Work and Role Details**: Data on job-related factors such as Job Role, Job Level, Years at the Company, Years in the Current Role, Years Since the Last Promotion, and Years With the Current Manager are provided. The average tenure within the company is around 7 years, and employees have been in their current roles for an average of 4 years.

**Compensation & Financials**: Employee compensation details include Monthly Income, Hourly Rate, Daily Rate, and Monthly Rate. In addition, Stock Option Level and Percent Salary Hike indicate bonus and salary increase metrics, contributing to insights on compensation growth over time.

**Performance and Job Satisfaction**: Ratings like Performance Rating, Environment Satisfaction, Job Satisfaction, Relationship Satisfaction, and Work-Life Balance are available, allowing for analysis of employee satisfaction and engagement. Performance Rating has an average score of about 3.15, with most ratings in the 3–4 range.

**Attrition and Over Time**: This includes labels for employees who have left the company (Attrition), travel requirements (Business Travel), and whether they work overtime (Over Time). Around 16% of employees have left (marked as Yes in Attrition).

**Training and Development**: Fields like Training Times Last Year capture professional development frequency, averaging 2–3 training sessions per year.

**Age and Experience Bands**: Grouped fields, such as CF_age band and CF_attrition label, categorize employees by age range and attrition status (current or former employees), facilitating analysis across age groups and tenure.

### Exploratory Data Analysis
* What is the total number of employees in each education field?
* How many employees are in the Organization?
* What is the total number of attrition and attrition count?
* Classify the job satisfaction range by the job roles.
* What is the total number of employees according to their marital status?
* What is the percentage of employees according to their age band?
* What is the total number of female employees according to their age band?
* What is the total number of male employees according to their age band?
* What is the total number of employees in each department?
* What is the highest and lowest level of education in each department? And many more......


### Data Cleaning and Preparation
The data was loaded into the tool and transformed before visualization was done. The first row was made the header as the columns were without a header. Then the data was ready for visualization. In the process of visualizing, conditional columns were created to attain:
* Age sort which represents- Under 25 = 1, 25-34 = 2, 35-44 = 3, 45-54 = 4, while Above 55 = 5
* Job Satisfaction which represents- Very Dissatisfied = 1, Dissatisfied = 2, Satisfied = 3, Very Satisfied = 4
* Attrition Count which represents- Yes = 1, No = 0
Also. measures were calculated to attain:
* Average Age- Average(Age)
* Attrition Rate- Sum(Attrition Count) / Sum(Employee Count), the column will then be changed under measure tools from whole numbers to percentage.







 A calculated column was created to attain the Total Sales/Revenue while a measure was calculated to attain the Average Revenue. The column quality, profile and distribution were checked before visualization was performed.

![HR Data Quality](https://github.com/user-attachments/assets/8410f406-4259-43a8-a0d6-048e14eddae1)


![HR Data Dashboard](https://github.com/user-attachments/assets/e99b5be7-39a3-465c-b39e-9d1c30046f82)
![HR Data Dashboard 1](https://github.com/user-attachments/assets/270a4379-573c-4e81-a36f-10b3528c0ce1)
![HR Data Dashboard 2](https://github.com/user-attachments/assets/0e6ab1ad-1212-494a-9844-2248c2c1ea3c)






