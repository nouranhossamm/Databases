# SQL Commands and Concepts

## 1. Create Database
Creates a new database in SQL.
```sql
CREATE DATABASE database_name;

2. Show Databases
Lists all databases available in the SQL server.

SHOW DATABASES;

3. Show Schemas
Displays the schemas (or databases) in the current database.

SHOW SCHEMAS;

4. Drop Database
Deletes an existing database. Use caution, as this will remove all data within the database.

DROP DATABASE database_name;

5. Single-line Comments
SQL comments are useful for leaving notes in your code. A single-line comment begins with --.

-- This is a single-line comment

6. Multi-line Comments
Multi-line comments begin with /* and end with */.

/* 
This is a 
multi-line comment 
*/

7. Data Types in SQL
Data types define the kind of data a column can hold in a table.

INT: Integer (whole number).
VARCHAR(n): String with a maximum length of n.
DATE: Date in YYYY-MM-DD format.
DECIMAL(m,n): Decimal number with m digits in total and n digits after the decimal point.
BOOLEAN: Stores TRUE or FALSE.

8. Primary Key Concept
A primary key uniquely identifies each record in a table. It must be unique and cannot contain NULL values.

CREATE TABLE table_name (
    column_name INT PRIMARY KEY
);

9. Create Table
Creates a new table with defined columns and their data types.

CREATE TABLE table_name (
    column1_name column1_data_type,
    column2_name column2_data_type,
    ...
);

10. Select
Retrieves data from one or more tables.

SELECT column_name(s) FROM table_name;

Select all columns:

SELECT * FROM table_name;

11. Use Database
Switches the current database to the specified one.

USE database_name;

12. Show Columns From
Displays the column structure of a specific table.

SHOW COLUMNS FROM table_name;

13. Add New Column in the Table
Adds a new column to an existing table.

ALTER TABLE table_name
ADD column_name data_type;

