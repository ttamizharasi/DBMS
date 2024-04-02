# EXP NO 2: DATA DEFINITION LANGUGE COMMANDS 
### DATE
## AIM:
To create a student database and execute DDL queries using SQL.


## THEORY
### DDL (Data Definition Language)

* DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema.
* It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database.
* DDL is a set of SQL commands used to create, modify, and delete database structures but not data.
* These commands are normally not used by a general user, who should be accessing the database via an application.

 
### List of DDL commands: 
1. CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
2. DROP: This command is used to delete objects from the database.
3. ALTER: This is used to alter the structure of the database.
4. TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
5. RENAME: This is used to rename an object existing in the database.

## Query:
### 1) Create a table student  and insert any two rows with the following fieds RegisterNumber,Name,Age,Address,Phone number

### SQL QUERY: 
 create table student(RegisterNumber int,Name varchar(100),Age int,Address varchar(250),PhoneNumber int) ;

### OUTPUT:
![312321602-3b2ea28e-b13f-44f6-aede-bf9c1eda44da](https://github.com/ttamizharasi/DBMS/assets/119657317/5f511db3-f8e7-4966-b072-b19ce06f692d)

### 2) Alter the above student table by adding another attribute department

### SQL QUERY: 
 alter table student add dept varchar(20);
### OUTPUT:
![312322191-64c4a805-220f-4d16-b47e-439959808b5b](https://github.com/ttamizharasi/DBMS/assets/119657317/d2b92123-ff7b-4b4c-83a7-0ecdd4e49c05)

### 3) Rename the student table to mystudent

### SQL QUERY: 
alter table student rename to student1;

### OUTPUT:
![312323419-84cd3e30-6347-4a6e-97b8-20d2ea033dd6](https://github.com/ttamizharasi/DBMS/assets/119657317/8d57f90b-aa14-4643-a5eb-1e2dbdda490a)

### 4) Drop the mystudent table
 
### SQL QUERY: 
drop table student1;

### OUTPUT:
![312323647-5f948625-f601-407a-b9c0-7833e51a999c](https://github.com/ttamizharasi/DBMS/assets/119657317/9bf81ecc-a89f-4bbc-914b-43c4784a7168)





## Result:
         Thus the basic DDL commands in SQL are executed. 


