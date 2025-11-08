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

### [Fiction Collection Size](https://www.codechef.com/practice/course/sql-case-studies-topic-wise/SQLBP01/problems/SQLPBP02)

```sql
SELECT COUNT(*) AS fiction_count 
FROM Books
WHERE genre = 'Fiction';
```
## Thought Process
- Step 1: Use the `COUNT(*)` function to count the total number of records in the `Books` table.  
- Step 2: Apply the `WHERE` clause to include only those rows where the `genre` is `'Fiction'`.  
📌 This query returns the total number of books that belong to the Fiction genre.

### [List of Movies with Ratings](https://www.codechef.com/practice/course/sql-case-studies-topic-wise/SQLBP01/problems/SQLPBP01)

```sql
SELECT Movie_name 
FROM Cinema
WHERE Rating > 7 AND Rating < 9;
```
## Thought Process
- Step 1: Use the `SELECT` statement to retrieve the `Movie_name` column from the `Cinema` table.  
- Step 2: Apply the `WHERE` clause to filter movies with ratings greater than 7 and less than 9.  
📌 This query displays the names of movies whose ratings fall between 7 and 9.

### [Handling NULL Values](https://www.codechef.com/practice/course/sql-case-studies-topic-wise/SQLBP01/problems/SQLPBP07)

```sql
SELECT book_id, title, author, published_year 
FROM Library
WHERE rating IS NULL;
```
## Thought Process
- Step 1: Use the `SELECT` statement to retrieve `book_id`, `title`, `author`, and `published_year` columns from the `Library` table.  
- Step 2: Apply the `WHERE` clause with the condition `rating IS NULL` to filter books that have no rating.  
📌 This query returns the details of all books in the library that do not have a rating value.
