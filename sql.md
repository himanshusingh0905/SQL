

# Get started with SQL:

## Pre-requisites:
1. DATABASE and DBMS(Database management System)
   * Database: where data is being stored
   * **Two types:**
       1. Relational ( or SQL-DB) : Data is stored in the form of Tables.  Eg. Postgresql, MariyaDB, Sqlite, etc..
       2. Non-Relational (or No-Sql DB) : Data is not stored in the form of tables. Eg.  **MongoDB** 

   * **DBMS** : It's a software which helps in managing databases.  For example: MySQL, Oracle, Microsoft SQL-Server, etc..

2. SQL (Structured Query Language):

  * **User -->  software(eg. posgresql) -> Database**
  * Softwares like postgresql, mysql, etc understand the SQL.

------------------------------------------------------------------------------------------------------------------------------------------

# BASICS :
## 1. Literals:
  1. **strings**:
    1. 'John'
    2. '1990-01-01'
    3. '50'
    

  2. **Numeric Literals: integer, decimal, or scientific notation :**  
  * **for example:**
    1. 200
    2. -5
    3. 6.0221415E23

## 2. Comments:
 1. ` -- `
 2. `/* */`


## 3. Identifiers
* objects in the database such as **tables**, **columns**, **indexes**, etc. 
* SQL is **case-insensitive** with respect to keywords and identifiers. So the following statements are equivalent.
    1. Select  * From employees;   
    2. SELECT * FROM EMPLOYEES;   
    3. select * from employees;   
    4. SELECT * FROM employees;

--------------------------------------------------------------------------------------------------------------------------------------------

# SQL commands are divided into 5 parts:
## 1. DDL (Data Definition Language)
   1. CREATE
   2. ALTER
   3. DROP
   4. TRUNCATE

## 2. DML (Data Manipulation Language)
   1. INSERT
   2. UPDATE
   3. DELETE

## 3. DQL (Data Query Language)
   1. SELECT

## 4. TCL (Transaction Control Language)
   1. SAVEPOINT
   2. COMMIT 
   3. ROLLBACK

## 5. DCL (Data Control Language)
   1. GRANT
   2. REVOKE


### AGGREGATE FUNCTIONS:  COUNT,  SUM,  AVG,  MAX,  MIN,   GROUP BY,  HAVING,  ORDER BY,    [total = 8 ]

### FILTERING DATA :  WHERE, AND, OR,  BETWEEN,  LIKE,  IN,   'IS NULL',  'IS NOT NULL'     [Total = 8]


### COMBINING DATA : 'INNER JOIN',  'LEFT JOIN', 'RIGHT JOIN',  FULL JOIN,  SELF JOIN,  UNION    [Total = 6]
--------------------------------------------------------------------------------------------------------------------------------------------

## 1. DDL (Data Definition Language):
* **Data definition** means: Defining the data..
    * **For Example:** A simple 2, what is it? 
       * It's Nothing, unless it tells some meaning. Like: is it a salary, age, no. of cars, etc.
       * Simply put it's meaningless
    * **Hence that meaning is provided by 'DDL' by defining schema, attirbutes (in which that data fall).**
    * Under it comes, dealing with structure or schema of data ( or simply put, we don't deal with *actual data* or *rows* ).

    ### Mainly 4 commands: ( CREATE, ALTER, DROP, TRUNCATE )
        1. CREATE : 
             * CREATE TABLE
             * CREATE DATABASE

        2. ALTER :
             * ALTER TABLE  ( operations like: 'delete col', 'rename col', 'change the type of col', 'change constraints of the col', 'add new col' )
             * ALTER DATABASE

        3. DROP :
             * DROP TABLE
             * DROP DATABASE

        4. TRUNCATE : ( Deletes whole data in a table in one go...)
             * TRUNCATE TABLE
             * *This command does not apply on database*

---------------------------------------------------------------------------------------------------------------------------------------------

## 2. DML (Data manipulation Language): 
*  *Dealing with actual Rows* .
*  so we manipulate that ( Like : insert new rows, delete rows, update the rows, delete particular field, etc)

#### Mainly 3 commands ( INSERT, UPDATE, DELETE ):


---------------------------------------------------------------------------------------------------------------------------------------------

## 3. DQL ( Data Query Language ):
* Retrieving data from Table
### Command : SELECT

#### 1. selecting data from all columns
```sql
select * from <tableName>
```

#### 2. selecting data from specific columns
* Specify the *column-list* after the **SELECT** clause.
* **Example:**
```sql
SELECT 
    employee_id, 
    first_name, 
    last_name, 
    hire_date
FROM
    employees;
```

#### 3. Performing a simple calculation
* The following example uses the SELECT statement to get the first name, last name, salary, and new salary:
```sql
SELECT 
    first_name, 
    last_name, 
    salary, 
    salary * 1.5
FROM
    employees;
```
* Here **salary * 1.5** is being calculated while quering the table.

#### 4. Assign an ***expression or a column*** an alias:
* you use the **AS** keyword followed by the ***column alias*** as follows:   
`expression AS column_alias`    

```sql
SELECT 
    first_name, 
    last_name, 
    salary, 
    salary * 1.5 As new_salary
FROM
    employees;
```
* **new_salary** is **Aliase** for **salary * 1.5**.

--------------------------------------------------------------------------------------------------------------------------------------------

## 4. TCL ( Transaction Query Language ):
#### COMMANDS :   SAVEPOINT, COMMIT, ROLLBACK

-------------------------------------------------------------------------------------------------------------------------------------------

## 5. DCL (DATA CONTROL LANGUAGE): 
#### COMMANDS: GRANT, REVOKE

--------------------------------------------------------------------------------------------------------------------------------------------





--------------------------------------------------------------------------------------------------------------------------------------------

