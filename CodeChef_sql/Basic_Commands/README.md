# Basic Commands

This file has all the problems from the Basic Commands section of SQL Practice Queries.

### [All Products](https://www.codechef.com/practice/course/sql-case-studies-topic-wise/SQLBP01/problems/SQLPBP11)

```sql
SELECT * 
FROM Products;
```
## Thought Process  
- Step 1: Use the `SELECT *` command to fetch every column from the table.  
- Step 2: Specify the table name `Products` using the `FROM` clause.  
📌 This query returns the complete dataset from the `Products` table, displaying every product and its associated information.

### [High Price of Products](https://www.codechef.com/practice/course/sql-case-studies-topic-wise/SQLBP01/problems/SQLPBP12)

```sql
SELECT product_name, category 
FROM Products
WHERE price > 100.00;
```
## Thought Process
- Step 1: Use the `SELECT` statement to retrieve the `product_name` and `category` columns from the `Products` table.  
- Step 2: Apply the `WHERE` clause to filter only those products whose `price` is greater than 100.00.  
📌 This query displays the names and categories of all products priced above 100.

### [Average Salary](https://www.codechef.com/practice/course/sql-case-studies-topic-wise/SQLBP01/problems/SQLPBP14)

```sql
SELECT AVG(salary) AS avg_salary 
FROM Works;
```
## Thought Process
- Step 1: Use the `AVG()` function to calculate the average of the `salary` column from the `Works` table.  
- Step 2: Assign the result an alias `avg_salary` for better readability.  
📌 This query returns the average salary of all employees in the `Works` table.

### [Locate People](https://www.codechef.com/practice/course/sql-case-studies-topic-wise/SQLBP01/problems/SQLPBP15)

```sql
SELECT department_name, location 
FROM departments
WHERE location LIKE 'S%';
```
## Thought Process
- Step 1: Use the `SELECT` statement to fetch `department_name` and `location` columns from the `departments` table.  
- Step 2: Apply the `WHERE` clause with the `LIKE 'S%'` condition to filter locations starting with the letter 'S'.  
📌 This query displays all departments whose locations begin with the letter 'S'.

### [Distinct Companies](https://www.codechef.com/practice/course/sql-case-studies-topic-wise/SQLBP01/problems/SQLPBP13)

```sql
SELECT DISTINCT(company_name) 
FROM Works;
```
## Thought Process
- Step 1: Use the `DISTINCT` keyword to eliminate duplicate values from the `company_name` column.  
- Step 2: Retrieve unique company names from the `Works` table.  
📌 This query returns a list of all distinct company names where employees work.
