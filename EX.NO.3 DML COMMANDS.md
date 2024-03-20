# EX 3 Data Manipulation Language (DML) Commands and built in functions in SQL
## AIM:
To create a manager database and execute DML queries using SQL.

# THEORY
## DML(Data Manipulation Language)
*  The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements.
*  It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.

## List of DML commands: 
1. INSERT: It is used to insert data into a table.
2. UPDATE: It is used to update existing data within a table.
3. DELETE: It is used to delete records from a database table.
4. SELECT: The SELECT command shows the records of the specified table.

## Create the table as given below:
```sql
create table manager(enumber number(6),ename char(15),salary number(5),commission number(4),annualsalary number(7),Hiredate date,designation char(10),deptno number(2),reporting char(10));
```
## insert the following values into the table
```sql
insert into manager values(7369,'Dharsan',2500,500,30000,'30-June-81','clerk',10,'John');
insert into manager values(7839,'Subu',3000,400,36000,'1-Jul-82','manager',null,'James');
insert into manager values(7934,'Aadhi',3500,300,42000,'1-May-82','manager',30,NULL);
insert into manager values(7788,'Vikash',4000,0,48000,'12-Aug-82','clerk',50,'Bond');
```

### Q1) Update all the records of manager table by increasing 10% of their salary as bonus.

### QUERY:
![dbms-31](https://github.com/22008650/DBMS/assets/122548204/b62b75f2-fb25-42e4-ad50-e2d613345939)



### OUTPUT:
![dbms-32](https://github.com/22008650/DBMS/assets/122548204/f110ab40-3c5e-4e08-91b8-d042ceca413c)


### Q2) Delete the records from manager table where the salary less than 2750.


### QUERY:
![dbms-33](https://github.com/22008650/DBMS/assets/122548204/d2b0ad11-89f9-4393-b9e1-8b81f801227b)


### OUTPUT:
![dbms-34](https://github.com/22008650/DBMS/assets/122548204/ef063c09-55fa-4037-9312-11c9cef3790a)


### Q3) Display each name of the employee as “Name” and annual salary as “Annual Salary” (Note: Salary in emp table is the monthly salary)


### QUERY:
![dbms-35](https://github.com/22008650/DBMS/assets/122548204/8fddeeb9-0397-4141-9014-81c1400b7ec1)



### OUTPUT:
![dbms-36](https://github.com/22008650/DBMS/assets/122548204/44e5b8e8-d96d-4f57-8bad-512aab0642cc)


### Q5)	List the names of Clerks from emp table.


### QUERY:
![dbms-37](https://github.com/22008650/DBMS/assets/122548204/bc45d2be-c13b-4d79-b028-dd0506b7fa5a)



### OUTPUT:
![dbms-38](https://github.com/22008650/DBMS/assets/122548204/13963839-07e3-4d9b-900e-183fa7f743fe)



### Q6)	List the names of employee who are not Managers.


### QUERY:
![dbms-39](https://github.com/22008650/DBMS/assets/122548204/fa9288fe-7881-4416-9ded-d71bd08a7630)



### OUTPUT:
![dbms-311](https://github.com/22008650/DBMS/assets/122548204/ea6cb99d-0daa-41d2-90f4-5105753931b4)




### Q7)	List the names of employees not eligible for commission.


### QUERY:
![dbms-312](https://github.com/22008650/DBMS/assets/122548204/004621b7-d6c0-40e0-9dc4-8427b044cb9a)



### OUTPUT:
![dbms-313](https://github.com/22008650/DBMS/assets/122548204/2ca19561-f259-49f7-a7b7-4a338195f99d)



### Q8)	List employees whose name either start or end with ‘s’.


### QUERY:
![dbms-314](https://github.com/22008650/DBMS/assets/122548204/440a06c9-60bb-474c-b5af-edc00ee7376a)




### OUTPUT:
![dbms-315](https://github.com/22008650/DBMS/assets/122548204/f1c2b13b-0702-4e39-8f5c-fdf2f13b68d7)



### Q9) Sort emp table in ascending order by hire-date and list ename, job, deptno and hire-date.


### QUERY:
![dbms-316](https://github.com/22008650/DBMS/assets/122548204/e73a50d0-a9f2-4328-86b4-ff89a1b37078)


### OUTPUT:
![dbms-317](https://github.com/22008650/DBMS/assets/122548204/377c703d-2a2a-422c-91ef-a63599313970)


### Q10) List the Details of Employees who have joined before 30 Sept 81.


### QUERY:
![dbms-318](https://github.com/22008650/DBMS/assets/122548204/379fb1cc-b559-4ddb-b94b-291b68c74331)



### OUTPUT:
![dbms-319](https://github.com/22008650/DBMS/assets/122548204/0caa72ab-3a5f-4be4-8107-721f31cba7a9)



### Q11)	List ename, deptno and sal after sorting emp table in ascending order by deptno and then descending order by sal.


### QUERY:
![dbms-321](https://github.com/22008650/DBMS/assets/122548204/6e47af4b-7eed-4ca2-bd95-9dbe0edb9db6)



### OUTPUT:
![dbms-322](https://github.com/22008650/DBMS/assets/122548204/1f6109a0-3e14-467f-89d3-34959bdb51d1)


### Q12) List the names of employees not belonging to dept no 30,40 & 10


### QUERY:
![dbms-323](https://github.com/22008650/DBMS/assets/122548204/2ae0edca-21f2-4eba-96e0-1d44ec999039)



### OUTPUT:
![dbms-324](https://github.com/22008650/DBMS/assets/122548204/e0a7f8f2-96b8-42d7-a4b4-7bb09664e7f4)


### Q13) Find number of rows in the table EMP

### QUERY:
![dbms-325](https://github.com/22008650/DBMS/assets/122548204/48394cce-f184-44b3-815e-ba82480871f8)



### OUTPUT:
![dbms-326](https://github.com/22008650/DBMS/assets/122548204/0cd490d5-85ae-43e2-a235-9094e8efea83)



### Q14) Find maximum, minimum and average salary in EMP table.

### QUERY:
![dbms-327](https://github.com/22008650/DBMS/assets/122548204/8e7b863d-2c27-4261-a955-4469ca2990e7)




### OUTPUT:
![dbms-328](https://github.com/22008650/DBMS/assets/122548204/e89b0402-9692-464c-a53c-a8a79b8bb5e4)



### Q15) List the jobs and number of employees in each job. The result should be in the descending order of the number of employees.

### QUERY:
![dbms-329](https://github.com/22008650/DBMS/assets/122548204/103e59ae-5e32-422f-86fe-8bdd446cf126)


### OUTPUT:
![dbms-331](https://github.com/22008650/DBMS/assets/122548204/198ea737-6503-482f-98e7-fef4c1af81cd)




## RESULT :
Thus the basic DML commands are executed.
