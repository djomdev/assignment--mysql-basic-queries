# MySQL Basic Queries

## The Assignment

You are the only DBA in the [JP Morgan](#) company right know, and your manager have asked you to bring the correct data from a confidential paper for a client. This is your opportunity to show your skills. Please, pay attention to the business questions.

## Deliverables

+ a github repository named `assignment--mysql-basic-queries` with a `.sql` file containing all answers.
  
###### Example
  
```sql
#1 Write a query to display all names from Products.

SELECT Id, Name FROM Products;
```

## Setup Instructions

  1. Connect to MySQL Server on [45.55.135.14/phpmyadmin](45.55.135.14/phpmyadmin)
  2. Copy the `HR` database and add your initial letters as suffix.

  ###### Example
  
  ```sql
  CREATE DATABASE HR_BG; # Bill Gates
  ```

## Exercise

  ```sql
  #1 Write a query to display the name (FIRST_NAME, LAST_NAME) and SALARY for all employees whose salary is not in the range $10,000 through $15,000.

  #2 Write a query to display the name (FIRST_NAME, LAST_NAME) and DEPARTMENT_ID of all employees in departments 30 or 100 in ascending order.

  #3 Write a query to display the name (FIRST_NAME, LAST_NAME) and SALARY for all employees whose salary is not in the range $10,000 through $15,000 and are in department 30 or 100.

  #4 Write a query to display the name (FIRST_NAME, LAST_NAME) and HIRE_DATE for all employees who were hired in 1987.

  #5 Write a query to display the first_name of all employees who have both "b" and "c" in their first name.

  #6 Write a query to display the last name, job, and salary for all employees whose job is that of a Programmer (IT_PROG) or a Shipping Clerk (SH_CLERK), and whose salary is not equal to $4,500, $10,000 or $15,000.

  #7 Write a query to display the last name of employees whose names have exactly 6 characters.

  #8 Write a query to display the last name of employees having 'e' as the third character.

  #9 Write a query to display the JOBS available in the employees table.

  #10 Write a query to display the name (FIRST_NAME, LAST_NAME), SALARY and PF (15% of salary) of all employees.

  #11 Write a query to select all record from employees where last name in 'BLAKE', 'SCOTT', 'KING' and 'FORD'.
  ```
