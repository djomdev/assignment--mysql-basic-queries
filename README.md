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

1. Create assignment folder in terminal

  ```sh
  cd ~/muktek/assignments
  mkdir assignment--mysql-basic-queries

  curl  https://raw.githubusercontent.com/muktek/assignment--mysql-basic-queries/master/assignment-files/mysql-basic-queries.sql > mysql-basic-queries.sql
  ```

2. Connect to MySQL Server on [45.55.135.14/phpmyadmin](45.55.135.14/phpmyadmin) and create your a copy of the database under your name. NOTE: Format name of should be `HR_«your-github-name»`.

  ```sh
  ssh root@45.55.135.14
    # enter password when asked to

  # create the DATABASE with your GITHUB name
  echo "CREATE DATABASE HR_yourGithubUsername;" | mysql -u root -p
    ## Example: echo "CREATE DATABASE HR_tphdev" | mysql -u root -p

  # clone .sql copy of database to your MySQL database
  mysql HR_yourGithubUsername -u root -p < dbcopy/HRCopy.sql
    ## Example: mysql HR_tphdev -u root -p < dbcopy/HRCopy.sql

  ```


3. Inside mysql shell, connect to your HR_ database to complete the exercises
  ```sh
  mysql> mysql -u root -p
    # enter password when asked to

  # enter your database
  mysql> USE HR_yourGithubUsername
  ```

4. Check to see the tables are there

  ```sh
  mysql> SHOW TABLES;
  # =>
  +------------------------+
  | Tables_in_HR_scoobydoo |
  +------------------------+
  | Countries              |
  | Departments            |
  | Employees              |
  | JobHistory             |
  | Jobs                   |
  | Locations              |
  | Regions                |
  +------------------------+
  ```

4. You will need to write/record your queries in the `mysql-basic-queries.sql` file


## Exercise

```sql
# [Example]
# 0 Write a query to display the full name (FIRST_NAME + LAST_NAME) for all employees whose first name is 'John'.

SELECT FIRST_NAME, LAST_NAME
FROM Employees
WHERE
  FIRST_NAME = 'John';


# 1  Write a query to select all record from employees
#    where last name in 'BLAKE', 'SCOTT', 'KING' or 'FORD'.
#     [HINT: look up the OR operator]


# 2 Write a query to display the full name (FIRST_NAME + LAST_NAME) and DEPARTMENT_ID
#   of all employees in departments 30 and 100 in ascending order.
#     [HINT: checkout the ORDER BY opeartor ]



# 3 Write a query to display the full name (FIRST_NAME + LAST_NAME) and SALARY
#   for all employees whose salary that is greater than $15,000.



# 4 Write a query to display the full name (FIRST_NAME + LAST_NAME) and SALARY
#   for all employees with salaries that are outside the range $10,000 through $15,000
#   and are in departments with an id of 30 or 100.
#     [HINT: research 'combining multiple conditions in mysql']



# 5 Write a query to display the last name, job, and salary for all employees
#   whose job is that of a Programmer (IT_PROG) or a Shipping Clerk (SH_CLERK),
#   and whose salary is not equal to $4,500, $10,000 or $15,000.
#     [HINT: research 'combining multiple conditions in mysql']



# 6 Write a query to display the full name (FIRST_NAME + LAST_NAME)
#    and HIRE_DATE for all employees who were hired in after July, 1 1987.
#     [HINT: research 'comparing date in mysql']



# 7 Write a query to display the unique values of
#   JOBS_ID available in the employees table.
#     [HINT: look up the DISTINCT operator]



# 8 Write a query to display the first name of all employees who have the letters
#   "b" or "c" in their first name.
#     [HINT: research LIKE operator]



# 9 Write a query to display the last name of employees whose names
#   have exactly 6 characters.
#     [HINT: look up CHARLENGTH operator  ]



# 10 Write a query to display the last name of employees having 'e'
#    as the third character.
#     [HINT: look up SUBSTRING operator ]

```
