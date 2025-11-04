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

