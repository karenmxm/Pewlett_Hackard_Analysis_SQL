# Pewlett-Hackard-Analysis
## Project Objectives

Pewlett-Hackard is a big company with a large size of employees. As baby boomers begin to retire at a rapid rate, Pewlett-Hackard is looking toward the future in two ways:
  - Offering retiring pacakge for those who meets certain criteria.
  - Getting information about which positions needed to be filled in near future.
  
Based on these needs, we analized Pewlett-Hackard's employee data to provide information on:
  - Who will be retiring in the next few years.
  - Which positions and how may positions will Pewlett-Hackard needs to fill.
  - Mentorship eligible employees to train new employees.

## Analysis Procedure

### Tools
  - Postgres for creating a database
  - pgAdmin4 for working with the data imported
  - QuickDBD for Entity Relationship Diagrams(ERD)

### Procedure
  - Identify data relationships and create Entity Relationship Diagrams. 
  - Lauch pgAdmin4 and create database.
  - Create tables in SQL.
  - Import six data sets into tables created in SQL in last step.
  - Query current retiring employees born between Jan. 1, 1952 and Dec. 31, 1955.
    - Use INNER JOIN and LEFT JOIN to merge data sets: employee, dept_emp, titles and salaries.
    - Use WHERE and AND to query current retiring employees.
    - Use PARTITION BY to query only the most recent title of each employee.  
  - Query how many empoyees are retiring for each title.
    - Use COUNT() function, PARTITION BY and GROUP BY to query the number of employees per title.
  - Query how many titles have retiring employees.
    - Use COUNT() function to count the number of titles that have retiring employees. 
  - Query how many employees are eligible for mentiorship for new employees.
    - Use INNER JOIN to merge data sets: employee, dept_emp, titles and salaries.
    - Use WHERE and AND to query current employees who have a date of birth that falls between January 1, 1965 and December 31, 1965 to be eligible to participate in the mentorship program.
    - Use PARTITION BY to query only the most recent title of each employee.  
    
 ### Results and Analysis
   - Results
     - EDA image shows data relationships.
     - There are 72,458 employees are retiring in near future.
     - There are 1,549 employees are available for mentor roles.
     - There are 7 titles have retiring employees. 
       - [Retiring Employees per Title](https://github.com/karenmxm/Pewlett-Hackard-Analysis/blob/master/Data/current_retirement_per_title.csv)

   </p>
   <p align="center">
   <img src="EmployeeDB.png">
   </p>



