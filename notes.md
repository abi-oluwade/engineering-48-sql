# SELECT Syntax
- The SELECT keyword is used to select data from the database, and decides what columns are shown in the results-set.

# SELECT DISTINCT Synthax
- The SELECT DISTINCT statement only allows for differing values to be displayed in the columns.

SELECT DISTINCT column1, column2, ...
FROM table_name;

# WHERE Synthax
- A WHERE clause is used to specify a condition in the statement, allowing for the results-table to filter out values that do not meet those conditions.

SELECT column1, column2, ...
FROM table_name
WHERE condition;

# AND, OR, NOT Synthax
- AND, OR AND NOT keywords are used to further specify conditions, where for example the AND keyword means that for the results in the table both of the specified  conditions must be true, while the OR means only one needs to be true, and NOT means none of the conditions can be true.

SELECT column1, column2, ...
FROM table_name
WHERE condition1 AND condition2 AND condition3 ...;

SELECT column1, column2, ...
FROM table_name
WHERE condition1 OR condition2 OR condition3 ...;

SELECT column1, column2, ...
FROM table_name
WHERE NOT condition;

# ORDER BY Syntax
- The ORDER BY keyword is used to sort the result-set in ascending or descending order.

SELECT column1, column2, ...
FROM table_name
ORDER BY column1, column2, ... ASC|DESC;

# INSERT INTO Syntax
- It is possible to write the INSERT INTO statement in two ways.

The first way specifies both the column names and the values to be inserted:

INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);

- If you are adding values for all the columns of the table, you do not need to specify the column names in the SQL query. However, make sure the order of the values is in the same order as the columns in the table. The INSERT INTO syntax would be as follows:

INSERT INTO table_name
VALUES (value1, value2, value3, ...);

# MIN and MAX syntax
- The MIN() function returns the smallest value of the selected column.
- The MAX() function returns the largest value of the selected column.

SELECT MIN(column_name)
FROM table_name
WHERE condition;

SELECT MAX(column_name)
FROM table_name
WHERE condition;

# COUNT, AVG and SUM Syntax
- The COUNT() function returns the number of rows that matches a specified criteria.
- The AVG() function returns the average value of a numeric column.
- The SUM() function returns the total sum of a numeric column.

SELECT COUNT(column_name)
FROM table_name
WHERE condition;

SELECT AVG(column_name)
FROM table_name
WHERE condition;

SELECT SUM(column_name)
FROM table_name
WHERE condition;

# LIKE syntax
- The LIKE operator is used in a WHERE clause to search for a specified pattern in a column.
- There are two wildcards often used in conjunction with the LIKE operator:
  - % The percent sign represents zero, one, or multiple characters
  - The underscore represents a single character

  SELECT column1, column2, ...
  FROM table_name
  WHERE columnN LIKE pattern %,_ ;

# AS syntax
- SQL aliases are used to give a table, or a column in a table, a temporary name.
- Aliases are often used to make column names more readable.
- An alias only exists for the duration of the query.

SELECT column_name AS alias_name
FROM table_name;

SELECT column_name(s)
FROM table_name AS alias_name;

# JOIN syntax
- (INNER) JOIN: Returns records that have matching values in both tables
- LEFT (OUTER) JOIN: Returns all records from the left table, and the matched records from the right table
- RIGHT (OUTER) JOIN: Returns all records from the right table, and the matched records from the left table
- FULL (OUTER) JOIN: Returns all records when there is a match in either left or right table

SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate
FROM Orders
INNER JOIN Customers ON Orders.CustomerID=Customers.CustomerID;

# GROUP BY Syntax
- The GROUP BY statement groups rows that have the same values into summary rows, like "find the number of customers in each country".
- The GROUP BY statement is often used with aggregate functions (COUNT, MAX, MIN, SUM, AVG) to group the result-set by one or more columns.

SELECT column_name(s)
FROM table_name
WHERE condition
GROUP BY column_name(s)
ORDER BY column_name(s);

# Having Syntax
- The HAVING clause was added to SQL because the WHERE keyword could not be used with aggregate functions.

SELECT column_name(s)
FROM table_name
WHERE condition
GROUP BY column_name(s)
HAVING condition
ORDER BY column_name(s);
