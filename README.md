# Exp-6 SET OPERATIONS.
## AIM:
To write a sql query to perform set operations on two tables.
## PROCEDURE:
### STEP 1:
create database SET_OPERATION.
### STEP 2:
create table A,B.
### STEP 3:
Insert Value to the tables.
### STEP 4:
Perform Set operations like Union,Union all,Intersect,Except.
## PROGRAM:
```sql
CREATE DATABASE SET_OPERATION;
SHOW DATABASES;
USE SET_OPERATION;
CREATE TABLE A (
  ID INT PRIMARY KEY,
  name VARCHAR(50)
);
CREATE TABLE B (
  ID INT PRIMARY KEY,
  name VARCHAR(50)
);
INSERT INTO A (ID, name) VALUES (1, 'John');
INSERT INTO A (ID, name) VALUES (2, 'Mary');
INSERT INTO A (ID, name) VALUES (3, 'David');
INSERT INTO B (ID, name) VALUES (2, 'Mary');
INSERT INTO B (ID, name) VALUES (3, 'David');
INSERT INTO B (ID, name) VALUES (4, 'Lisa');
SELECT * FROM A;

SELECT * FROM B;

SELECT * FROM A
UNION
SELECT * FROM B;

SELECT * FROM A
UNION ALL
SELECT * FROM B;

SELECT * FROM A
INTERSECT
SELECT * FROM B;

SELECT * FROM A
EXCEPT
SELECT * FROM B;
```
## OUTPUT:
![image](https://github.com/Bharath745/DBMS-Ex-06/assets/94508354/786df994-7073-4705-bc23-a3148953fd8c)

![image](https://github.com/Bharath745/DBMS-Ex-06/assets/94508354/b2e0a6be-9a2d-49a9-a130-c8fb134c0fd1)

![image](https://github.com/Bharath745/DBMS-Ex-06/assets/94508354/6de7c601-7ed5-4b47-a4a9-c0bcef327402)

![image](https://github.com/Bharath745/DBMS-Ex-06/assets/94508354/cfc55ed8-2546-4854-a81a-a7a0733010a3)

![image](https://github.com/Bharath745/DBMS-Ex-06/assets/94508354/62cc41af-39fa-4157-8ed0-6e659a6ef752)

![image](https://github.com/Bharath745/DBMS-Ex-06/assets/94508354/d097fcf5-58c6-44da-8205-c509280d94bb)


## RESULT:
A sql query to perform set operations on two tables has been executed.
