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

![This is an image](https://github.com/HansFeddersen/Pewlett-Hackard-Analysis./blob/main/Data/more/Elegible%20for%20retirement.png)

- The code to obtain the information above is as follows:

![This is an image](https://github.com/HansFeddersen/Pewlett-Hackard-Analysis./blob/main/Data/more/Code_deliverable_1.png)

**Deliverable 2: The Employees Eligible for the Mentorship Program**

- For this deliverable, we have to select all of the employess that are elegible for a mentorship program. For that, we have to find all of the active employees that were born between January 1, 1965 and December 31, 1965. In this summary, we'll be displaying the employee number (emp_no), first name (first_name), last name (last_name), birth date (birth_date), first date on the job (from_date), if they are still active (to_date equals to 9999-01-01) and their position on the company (title). We obtain the following result (in total there are 1,549 employees elegible, but we only display the first 10 of the list as an example):

![This is an image](https://github.com/HansFeddersen/Pewlett-Hackard-Analysis./blob/main/Data/more/elegible_for_mentorship.png)

- The code to obtain the information above is as follows:

![This is an image](https://github.com/HansFeddersen/Pewlett-Hackard-Analysis./blob/main/Data/more/Code_deliverable_2.png)

**Mayor points about the results**

**1)** The company should run a survey among theier employees that are elegible for retirement to know exactly how many of them are planning to retire soon and how many ar planning to keep working (that would help them to plan ahead and prepare for the future), but according to the results there are 72,458 employees that are elegible for retirement according to their birth date.

**2)** Of the 1,549 employees elegibles for mentorship, 569 are senior staff, 529 are senior engineers, 190 are engineers, 155 are staff, 77 are technique leaders and 29 are assistant engineers. There are no managers.

**3)** The titles witht the most percent of employees elegible for retirement are the senior positions (senior staff and senior engineer) with almost 27% of the total employess for each of the titles.

**4)** To count the employees elegible for retirement, it is necesary to use the distinct function on the employee number, because there are many employees that held many positions during their time in the company.

**Mayor points about the results**

Answer the following questions:

**How many roles will need to be filled as the "silver tsunami" begins to make an impact?**

- In total there are 72,458 employees that are elegible for retirement, so thats the amount of roles that will need to be filled. If we consider that this year only people born in 1952 will retire (the oldest elegible) the company would have to worry only about filling 16,981 roles this year.

**Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?**

- Yes there are. The number of employees that are elegible for retirement is much larger for every postion that the number of employees that are elegible or mentorship. The comparison is as follows:

![This is an image](https://github.com/HansFeddersen/Pewlett-Hackard-Analysis./blob/main/Data/more/Last_question.png)
