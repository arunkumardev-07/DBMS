# EXP NO 2: DATA DEFINITION LANGUGE COMMANDS 
### DATE :13/03/2024
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
### 1) Create a database studentdb
```
create database studentdbb;
```
## OUTPUT:
![Screenshot 2024-03-13 105513](https://github.com/arun1111j/DBMS/assets/128461833/89fa3b98-f16a-47c1-8c5d-d6bea2a5ac4a)

### 2) Create a table student and insert any two rows with the following fieds RegisterNumber,Name,Age,Address,Phone number
# SQL QUERY:

```
 create table student(RegisterNumber int,Name varchar(100),Age int,Address varchar(250),PhoneNumber int) ;
```
## OUTPUT :
![image](https://github.com/arun1111j/DBMS/assets/128461833/395d7e11-abf2-4a2b-9d37-f3fe816f0726)
### 3) Alter the above student table by adding another attribute department
# SQL QUERY:
```
rename table student to mystudent;
```
## OUTPUT :
![Screenshot 2024-03-13 105856](https://github.com/arun1111j/DBMS/assets/128461833/1aabf8f2-2f7b-4705-a471-feec1c925f89)
### 4) Rename the student table to mystudent
# SQL QUERY:
```
rename table student to mystudent;
```
## OUTPUT :
![image](https://github.com/arun1111j/DBMS/assets/128461833/78991881-166a-4506-8360-46fdef70bdf7)
### 5) Delete the mystudent rows using truncate keyword
# SQL QUERY:
```
 truncate table mystudent;
```
## OUTPUT :
![image](https://github.com/arun1111j/DBMS/assets/128461833/a62ed4ad-c385-4dee-891c-baeff4a16a83)
### 4) Drop the mystudent table
# SQL QUERY:
```
 drop table mystudent;
```
## OUTPUT :
![Screenshot 2024-03-13 110223](https://github.com/arun1111j/DBMS/assets/128461833/a851e491-90ab-47e0-91f9-279fc16ef0c2)
## Result:
         Thus the basic D
