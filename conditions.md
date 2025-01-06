
# CASE 

## The CASE statement has two forms.
1. **Simple CASE:** 
2. **Searched CASE:** when conditional operators are used with **WHEN**.

### 1. Simple case:
**SYNTAX:**
```SQL
CASE expression
    WHEN value1 THEN result1
    WHEN value2 THEN result2
    ...
    ELSE default_result
END
```
* *'expression'* evaluates to a value.
* Then ***evaluated value*** is compared with value1, value2, etc. 
* If it matches any value, then corresponding result is returned, else *default_result* is returned.

**EXAMPLE:**   
```sql
SELECT
    name,
    grade,
    CASE grade
        WHEN 'A' THEN 'Excellent'
        WHEN 'B' THEN 'Good'
        WHEN 'C' THEN 'Average'

        ELSE 'Needs Improvement'
    END AS performance
FROM students;

```
* **Internal working of above example**:
  * Everytime a new row in the *grade* col is evaluated in **CASE**.
  * If it's value = 'A', then 'Excellent' is returned and so on.
  * If value comes from *grade* doesn't match anything, then *'Needs Improvement'* is returned.

--------------------------------------------------------------------------------------------------------------

### 2. Searched CASE:

**SYNTAX:**
```SQL
CASE
    WHEN condition1 THEN result1
    WHEN condition2 THEN result2
    ...
    ELSE default_result
END
```
* **NOTE**:
  * Here there is no *expression* after *CASE*.
  * After *WHEN* there could be any *expression* which results **boolean**.


**EXAMPLE:**   
```sql
SELECT
    name,
    CASE
        WHEN marks >= 90 THEN 'Excellent'  -- marks is the column name, 
        WHEN marks >= 75 THEN 'Good'
        WHEN marks >= 50 THEN 'Average'
        ELSE 'Needs Improvement'
    END AS performance                    -- performance is ALIASE
FROM students;
```

* **Internal working of above example**:
  * Everytime a new row (in the *grade* col) is evaluated in **CASE**.
  * If it's value = 'A', then 'Excellent' is returned and so on.
  * If value comes from *grade* doesn't match anything, then *'Needs Improvement'* is returned.



## 'CASE' with 'SELECT' : 
