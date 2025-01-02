

# SQL commands are divided into 5 parts:
1. DDL (Data Definition Language)
2. DML (Data Manipulation Language)
3. DQL (Data Query Language)
4. TCL (Transaction Control Language)
5. DCL (Data Control Language) 

--------------------------------------------------------------------------------------------------------------------------------------------
# QUICK SUMMARY : 

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

   ### Mainly 3 commands ( INSERT, UPDATE, DELETE ):
       1. INSERT : 

---------------------------------------------------------------------------------------------------------------------------------------------

## 3. DQL ( Data Query Language ):
* Retrieving data from Table
### Command : SELECT

--------------------------------------------------------------------------------------------------------------------------------------------

## 4. TCL ( Transaction Query Language ):
### COMMANDS :   SAVEPOINT, COMMIT, ROLLBACK

----------------------------------------------------------------------------------

## 5. DCL (DATA CONTROL LANGUAGE): 
### COMMANDS: GRANT, REVOKE

-----------------------------------------------------------------------------------

## AGGREGATE FUNCTIONS:  COUNT,  SUM,  AVG,  MAX,  MIN,   GROUP BY,  HAVING,  ORDER BY,    [total = 8 ]

## FILTERING DATA :  WHERE, AND, OR,  BETWEEN,  LIKE,  IN,   'IS NULL',  'IS NOT NULL'     [Total = 8]


## COMBINING DATA : 'INNER JOIN',  'LEFT JOIN', 'RIGHT JOIN',  FULL JOIN,  SELF JOIN,  UNION    [Total = 6]


======================================================================================================================================


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

  -----------------------------------------------------------------------------------------------------------------------------------

  # BASICS :
  ## 1. Literals:
  1. **strings**:
    `
    'John'
    '1990-01-01'
    '50'
    `

  2. **Numeric Literals: integer, decimal, or scientific notation :**  
  * **for example:**
  `
    200
    -5
    6.0221415E23
    `