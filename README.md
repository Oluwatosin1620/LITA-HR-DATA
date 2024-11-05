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
The data was loaded into the tool and transformed before visualization was done. The first row was made the header as the columns were without a header.  The column quality, profile and distribution were checked before visualization was performed, and the data was ready for visualization. In the process of visualizing, conditional columns were created to attain:
* Age sort which represents- Under 25 = 1, 25-34 = 2, 35-44 = 3, 45-54 = 4, while Above 55 = 5
* Job Satisfaction which represents- Very Dissatisfied = 1, Dissatisfied = 2, Satisfied = 3, Very Satisfied = 4
* Attrition Count which represents- Yes = 1, No = 0

Also, measures were calculated to attain:
* Average Age- Average(Age)
* Attrition Rate- Sum(Attrition Count) / Sum(Employee Count), the column will then be changed under measure tools from whole numbers to percentage.


![HR Data Quality](https://github.com/user-attachments/assets/8410f406-4259-43a8-a0d6-048e14eddae1)

### Data Visuaization


![HR Data Dashboard](https://github.com/user-attachments/assets/e99b5be7-39a3-465c-b39e-9d1c30046f82)
![HR Data Dashboard 1](https://github.com/user-attachments/assets/5565a1bc-edd1-43cb-bf3b-5a1ab74b8e2f)
![HR Data Dashboard 2](https://github.com/user-attachments/assets/c1149b52-5b3f-4d6e-858b-0f155fa7d6ad)




### Employee Attrition Analysis for Strategic Insights
This analysis presents a comprehensive overview of employee attrition within an organization of 1,470 employees, focusing on patterns and trends across key demographic and job-related variables. The dataset includes 44 attributes, and our primary interest is in variables such as Attrition, Age Band, Department, Education Field, Gender, Job Role, Marital Status, Overtime, and Education Level. The findings reveal both strengths and challenges in employee retention across departments and educational backgrounds, offering insights into potential strategies to enhance organizational growth.

#### Key Findings
* Total Workforce and Attrition: Out of the total 1,470 employees, 237 individuals have left the organization, signalling a considerable attrition level that may merit further investigation. This base attrition rate, together with details on education fields and departments, highlights which groups may need tailored retention strategies.
**Summary**: This level of attrition indicates potential underlying issues, especially in specific fields and departments, and suggests an opportunity for focused engagement programs.
  
* Attrition by Education Field: Breaking down attrition by education reveals valuable insights:
1. Human Resources: With 20 current employees and an attrition count of 7 (4 males, 3 females), Human Resources has a total of 27 employees.
2. Life Sciences: The largest contributor to attrition, Life Sciences has 517 current employees and an attrition count of 89 (38 females, 51 males), totalling 606 employees.
3. Marketing: 124 current employees with 35 attritions (15 females, 20 males), totalling 159 employees.
4. Medical: 401 current employees and an attrition count of 63 (19 females, 44 males), making a total of 464 employees.
5. Technical Degree: 100 current employees with 32 attritions (10 females, 22 males), totalling 132 employees.
6. Others: 71 current employees with 11 attritions (2 females, 9 males), totalling 82 employees.
**Summary**: Life Sciences has the largest number of both employees and attritions, suggesting it may require further analysis to determine why this field sees such high turnover. Human Resources has the smallest attrition count, indicating relative stability.

* Attrition by Department: Attrition varies significantly across departments:
1. Sales: Highest attrition rate at 21% with 92 attritions (38 females, 54 males).
2. Research & Development (R&D): 14% attrition rate with 133 attritions (43 females, 90 males).
3. Human Resources (HR): Moderate attrition rate at 19% with 12 attritions (6 females, 6 males).
**Summary**: The Sales department’s 21% attrition rate is the highest, signalling possible job dissatisfaction or workload challenges. R&D, while being the largest department, shows a relatively lower attrition rate, suggesting its workforce may have greater stability or satisfaction compared to Sales and HR.

* Age Band and Gender Distribution by Department: Age demographics reveal that employees are predominantly in the 25-34 and 35-44 age groups.
1. HR Department: The majority are aged 25-34 (22 employees: 9 females, 13 males), while the smallest group is those under 25.
2. R&D Department: The most significant age groups are 25-34 (348 employees: 137 females, 211 males) and 35-44 (342 employees: 136 females, 206 males).
3. Sales Department: The age groups with the most employees are 25-34 (184 employees: 71 females, 113 males) and 35-44 (138 employees: 54 females, 84 males).
**Summary**: Across all departments, the 25-34 age range is the most represented, while employees over 55 represent the smallest group. The age distribution suggests that retention strategies should prioritize the young workforce, who may be in the early stages of their careers and are more open to opportunities for development and progression.

* Attrition by Education Level: Attrition patterns by education reveal that Bachelor’s degree holders have the highest attrition, followed by Master’s degree holders, Associate degree holders, and then those with High School and Doctoral degrees.
**Summary**: This trend indicates that mid-level educated employees (primarily Bachelor’s degree holders) may be more mobile and open to external opportunities, warranting a focus on creating compelling advancement paths and development programs to retain this group.
  
* Marital Status: Most employees are married, with divorced and single employees evenly distributed across departments. There is no significant correlation between marital status and attrition rate.
**Summary**: Marital status does not appear to be a defining factor in attrition, suggesting that other factors, such as job role and satisfaction level, play a more pivotal role in influencing employee decisions to leave.
Job Role and Satisfaction Levels:

* Employee satisfaction varies across job roles:
1. Healthcare Representatives: Out of 9 employees, satisfaction is mixed, with both high and low levels.
2. HR Roles: Of the 12 employees, a high dissatisfaction level is notable (5 are very dissatisfied).
3. Laboratory Technicians: 62 employees show a balanced spread, although some experience dissatisfaction.
4. Managers: 5 employees show varied satisfaction, with some indicating dissatisfaction.
5. Sales Executive and Research Scientist roles indicate higher dissatisfaction, with 16 and 13 very dissatisfied employees, respectively.
**Summary**: Job roles like Sales Executive and Research Scientist report high dissatisfaction, which may contribute to the organization’s attrition levels in these roles. Targeted engagement and job redesign strategies could improve job satisfaction and, ultimately, retention in these roles.

* Age Distribution by Job Role: Analysis of age distribution within job roles reveals that:
1. Healthcare Representatives: Predominantly aged 25-34, with the fewest employees under 25.
2. HR Roles: Most employees are aged 35-44, while under 25 and over 55 have minimal representation.
3. Manager Roles: Highest representation is within the 45-54 age band.
4. Sales Representatives and Executives: Predominantly in the 25-34 age range.
**Summary**: The 25-34 age group dominates many job roles, particularly in Sales and Research, where dissatisfaction is also high. This suggests that younger employees in these roles may need enhanced development and recognition programs to maintain their engagement.


### General Summary and Recommendations
This analysis shows that the Sales and R&D departments have the highest attrition, with employees aged 25-34 forming the majority in nearly all departments. Life Sciences and Medical education fields contribute significantly to employee numbers but also face high attrition rates. Sales Executive and Research Scientist roles exhibit high levels of dissatisfaction, indicating potential for improvement in job design, workload management, and employee support structures.

#### Recommendations
* Enhanced Career Development for Young Professionals: Offering targeted career development programs for employees aged 25-34 could help retain this demographic, which is the largest and most likely to seek external opportunities.
  
* Job Redesign in High-Attrition Roles: Roles with high dissatisfaction, particularly Sales Executive and Research Scientist, may benefit from job redesigns, increased support, and clearer career paths.

* Departmental Engagement Initiatives: The Sales department’s high attrition suggests a need for engagement initiatives that could include team-building activities, clear progression plans, and improved working conditions.

* Targeted Retention in Education Fields: Focus on Life Sciences and Medical fields, where attrition is notably high, to understand and address the specific causes of turnover, possibly through tailored retention and rewards programs.

* Continued Support for Senior Employees: For employees over 55, the organization can introduce programs that support longer-term retention, such as flexible working hours or transition planning.

  Implementing these strategies could strengthen retention across departments, foster growth, and enhance job satisfaction, promoting a balanced, motivated, and committed workforce.



