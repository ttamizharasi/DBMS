# EXP NO 10: SYNONYMS AND ASSERTIONS IN SQL 
### DATE: 
## AIM:
To create a student database and create a synonym and assertions.

## THEORY
## SYNONYM
<div align="justify">
A SYNONYM provides another name for database object, referred to as original object, that may exist on a local or another server.
</div>
## ASSERTIONS
<div align="justify">
* An assertion is a piece of SQL which makes sure a condition is satisfied, else or it stops the action being taken on a database.
* An assertion is a constraint that might be dependent upon multiple rows of multiple tables.
</div>

## Query:
### 1) Create a table EMPLOYEE and perform insertion of two rows.

### SQL QUERY: 
```
CREATE TABLE EMPLOYEE (
    employee_id INT PRIMARY KEY,
    employee_name VARCHAR(255),
    employee_salary DECIMAL(10, 2)
);

INSERT INTO EMPLOYEE (employee_id, employee_name, employee_salary)
VALUES (1, 'Kayal', 50000.00);

INSERT INTO EMPLOYEE (employee_id, employee_name, employee_salary)
VALUES (2, 'Dolly', 60000.00);
```
### OUTPUT:
![image](https://github.com/ttamizharasi/DBMS/assets/119657317/628cd1ff-413b-40b7-bd36-d174bbefe653)

### 2) Create a synonym S1 for EMPLOYEE  table.

### SQL QUERY: 
CREATE SYNONYM S1 FOR EMPLOYEE;
### OUTPUT:
![318716718-4da68d32-b801-448b-821a-6d33faea53f8](https://github.com/ttamizharasi/DBMS/assets/119657317/da733c60-26a1-466f-83cf-fa9bc3b1966c)


### 3) Display the EMPLOYEE  table using synonym S1.
 
### SQL QUERY: 
SELECT * FROM S1;

### OUTPUT:
![image](https://github.com/ttamizharasi/DBMS/assets/119657317/fe68c714-cca8-471a-ac86-eb029d42abf8)


### 4) Drop the synonym.

### SQL QUERY: 
DROP SYNONYM S1;

### OUTPUT:
![318716660-4a0abc5f-bcd9-4f06-895f-a4e86c47cb91](https://github.com/ttamizharasi/DBMS/assets/119657317/72a9a4e3-57ae-4160-bebc-9e4f04c3ccbc)


### 5) Create a supplier table and create a sequence S2 for supplier table id.

### SQL QUERY: 
```
CREATE TABLE SUPPLIER (
    supplier_id INT PRIMARY KEY,
    supplier_name VARCHAR(255)
);

CREATE SEQUENCE S2;
```
### OUTPUT:
![318716606-e7b66211-5bf4-4293-8d00-53f01a69d27c](https://github.com/ttamizharasi/DBMS/assets/119657317/6912b813-6b81-4245-b721-b58d888dad90)


### 6) insert the data into supplier table use sequence.

### SQL QUERY: 
INSERT INTO SUPPLIER (supplier_id, supplier_name)
VALUES (S2.NEXTVAL, 'AB Suppliers');

INSERT INTO SUPPLIER (supplier_id, supplier_name)
VALUES (S2.NEXTVAL, 'CD Suppliers');

### OUTPUT:
![318716563-a592143c-d033-4385-ba95-90edc540ad76](https://github.com/ttamizharasi/DBMS/assets/119657317/dd9a7d0e-c4ab-4e2a-a61d-6b9f013751fd)

### 7) Drop the sequence

### SQL QUERY: 
DROP SEQUENCE S2;

### OUTPUT:
![318716500-d9df85ea-cf61-4cfe-adb3-90a65529a68e](https://github.com/ttamizharasi/DBMS/assets/119657317/b1384769-3e03-4907-98b1-f789a6d9c389)

## RESULT :
### Thus the sequence and synonym created and used in SQL.
