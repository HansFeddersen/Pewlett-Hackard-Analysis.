# Pewlett-Hackard-Analysis.

Data Bootcamp Module 7: Employee Database with SQL
## Overview of Project

### The purpose of this project is to retrieve information by using SQL queries. We start with 4 databases that have information about the employees of a company (Pewlett-Hackard) and the deparments of the same company. Using those databases, we need to join them to retrieve and filter specific information, in this case how many people (per department) are soon to be retired according to their birth date and how many people are elegible to participate in a mentorship program offered by the company (also according to their birthdate).

## Resources
**For this analysis, the following resuorces were used**:
- Data Sources: dept_emp.csv, departments.csv, dept_manager.csv, employees.csv, salaries.csv, titles.csv.
- Software: pgAdmin 4, Visual Studio Code


## Results

**Deliverable 1: The Number of Retiring Employees by Title**

- Of all the employees of the company, we select all of them who were born between the 01-01-1951 and the 12-31-1955 and group them by the position that they have in the company (title), obtaining the following result:

![This is an image](https://github.com/HansFeddersen/World_Weather_Analysis/blob/main/more/setp1/Random_coordinates_generator.png)

- The code to obtain the information above is as follows:

![This is an image](https://github.com/HansFeddersen/World_Weather_Analysis/blob/main/more/setp1/Nearest_city_coordinates.png)

**Deliverable 2: The Employees Eligible for the Mentorship Program**

- For this deliverable, we have to select all of the employess that are elegible for a mentorship program. For that, we have to find all of the active employees that were born between January 1, 1965 and December 31, 1965. In this summary, we'll be displaying the employee number (emp_no), first name (first_name), last name (last_name), birth date (birth_date), first date on the job (from_date), if they are still active (to_date equals to 9999-01-01) and their position on the company (title). We obtain the following result (in total there are 1,941 employees elegible, but we only display the first 10 of the list as an example):

![This is an image](https://github.com/HansFeddersen/World_Weather_Analysis/blob/main/more/setp1/Nearest_city_coordinates.png)

- The code to obtain the information above is as follows:

![This is an image](https://github.com/HansFeddersen/World_Weather_Analysis/blob/main/more/setp1/Nearest_city_coordinates.png)

**Mayor points about the results**

**1)** 

**2)** 

**3)** 

**4)** 

