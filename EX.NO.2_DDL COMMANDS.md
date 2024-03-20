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
### 1) Create a database studentdb

### SQL QUERY:
```
create database studentdbb;
```

### OUTPUT:
![dbms-21](https://github.com/22008650/DBMS/assets/122548204/9caebeac-584e-4cb5-9b63-697f24024599)


### 2) Create a table student  and insert any two rows with the following fieds RegisterNumber,Name,Age,Address,Phone number

### SQL QUERY: 
```
create table student(RegisterNumber int,Name varchar(100),Age int,Address varchar(250),PhoneNumber int) ;
```


### OUTPUT:
![dbms-22](https://github.com/22008650/DBMS/assets/122548204/9979df90-4c35-42ff-b243-fd32123adbfd)


### 3) Alter the above student table by adding another attribute department

### SQL QUERY:
```
 alter table student add dept varchar(20);
```

### OUTPUT:
![dbms-23](https://github.com/22008650/DBMS/assets/122548204/1cd0b24e-196a-4feb-a5cb-2652689e72d9)


### 4) Rename the student table to mystudent

### SQL QUERY: 
```
rename table student to mystudent;
```



### OUTPUT:
![dbms-24](https://github.com/22008650/DBMS/assets/122548204/89dcbe17-1aa4-433d-b594-c29dc405f320)


### 5) Delete the mystudent rows using truncate keyword

### SQL QUERY: 
```
truncate table mystudent;
```


### OUTPUT:
![dbms-25](https://github.com/22008650/DBMS/assets/122548204/8fe3066a-100c-4052-838f-f8da57f8480a)


### 6) Drop the mystudent table
 
### SQL QUERY: 
```
drop table mystudent;
```


### OUTPUT:
![dbms-26](https://github.com/22008650/DBMS/assets/122548204/feca8c99-49be-4ba7-a31f-aa4b4c0f7bc8)
## Result:
         Thus the basic DDL commands in SQL are executed. 


