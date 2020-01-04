# SQL
- SELECT - extracts data from a database
- UPDATE - updates data in a database
- DELETE - deletes data from a database
- INSERT INTO - inserts new data into a database
- CREATE DATABASE - creates a new database
- ALTER DATABASE - modifies a database
- CREATE TABLE - creates a new table
- ALTER TABLE - modifies a table
- DROP TABLE - deletes a table
- CREATE INDEX - creates an index (search key)
- DROP INDEX - deletes an index
- AND <>(not equal) >(greater than) etc.
- OR
- LIKE (allows us to use wildcards, which allows us to substitute all the characters to one side '%' while  _ allows us to specify the number of characters before or after)
- TOP
- BOTTOM
- UPPER
- LOWER
- IN ()
- BETWEEN (allows us to filter between a range of values
- AS (used to rename columns)
- + concenatetion
- ORDER BY [DESC OR ASC]
- CHARINDEX (Searches for a substring in a string a returns its start position)


# Examples of keyword usage:
- UPDATE <table_name> --> SET <column_name> = <what I want to replace it with> WHERE <table_id> = x;

- DELETE <table_name> WHERE <table_id> = x;

- ALTER TABLE <table_name> ADD <column_name>;

- SELECT productname FROM products WHERE products name LIKE 'Ch%' OR 'Ch__' (where the __ is two characters)

- We can use IDENTITY to cause our PRIMARY KEY column to automatically increment when a row is inserted.

# Questions 26/11/19

There are 3 tables that we must use:

## Users
- user_id (PK)
- name
- phone_numbers
- e_mail

## eBooks
- ebook_id (PK)
- Title
- location
- release_date
- user_id (FK)

## eBook_rental
- ebook_rental_id (PK)
- ebook_id (FK)
- user_id (FK)
- data
- price

The relationship between the tables is as follows:

1. Users --> eBooks is 1:n
2. eBooks --> eBook_rental is 1:n
3. Uses --> eBook_rental is 1:n


# Database Considerations
- Data Security
- Data Recovery
- Data Integrity
- Normal Form (1st, 2nd, 3rd, Bryte-Codd, 4th, 5th)
