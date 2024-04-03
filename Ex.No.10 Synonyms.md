# EXP NO 10: SYNONYMS AND ASSERTIONS IN SQL 
### DATE: 18/10/23

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
    employee_id INT ,
    name VARCHAR(255),
    department VARCHAR(255),
    salary DECIMAL(10, 2)
);
```


### OUTPUT:
![image](https://github.com/dharshan004/DBMS/assets/119103799/ec45801b-1834-4162-a56e-d4eee7c5a110)
![image](https://github.com/dharshan004/DBMS/assets/119103799/edf3db7a-f4ee-4e72-8a11-50f48a16b6f9)




### 2) Create a synonym S1 for EMPLOYEE  table.

### SQL QUERY: 
```
CREATE SYNONYM S1 FOR EMPLOYEE;
```

### OUTPUT:
![image](https://github.com/dharshan004/DBMS/assets/119103799/6236d4eb-62a5-48ed-8f9a-2e55f957cbca)





### 3) Display the EMPLOYEE  table using synonym S1.
 
### SQL QUERY: 
```
SELECT * FROM S1;
```


### OUTPUT:
![image](https://github.com/dharshan004/DBMS/assets/119103799/10e07f51-9340-43a2-a538-6ae0db761e54)





### 4) Drop the synonym.

### SQL QUERY: 
```
DROP SYNONYM S1;
```


### OUTPUT:
![image](https://github.com/dharshan004/DBMS/assets/119103799/5fe6bf62-ed6c-4222-ba25-546a62682cb2)



### 5) Create a supplier table and create a sequence S2 for supplier table id.

### SQL QUERY: 
```
CREATE TABLE supplier (
    id INT,
    name VARCHAR(255),
    address VARCHAR(255),
    contact_person VARCHAR(255)
);

CREATE SEQUENCE S2 START 1;

```


### OUTPUT:
![image](https://github.com/dharshan004/DBMS/assets/119103799/6fac4d7b-80b2-45d3-be9c-4daddb7fa3dd)

![image](https://github.com/dharshan004/DBMS/assets/119103799/89c3a912-e3bb-4c92-ae39-fe50ed1be224)



### 6) insert the data into supplier table use sequence.

### SQL QUERY: 
```
INSERT INTO supplier (id, name, address, contact_person)
VALUES (NEXTVAL('S2'), 'ABC Suppliers', '123 Main Street', 'John Doe');

INSERT INTO supplier (id, name, address, contact_person)
VALUES (NEXTVAL('S2'), 'XYZ Distributors', '456 Elm Road', 'Jane Smith');
```


### OUTPUT:
![image](https://github.com/dharshan004/DBMS/assets/119103799/e87b4f75-f185-4818-ba1d-dd101a728c60)



### 7) Drop the sequence

### SQL QUERY: 
```
DROP SEQUENCE S2;
```

### OUTPUT:
![image](https://github.com/dharshan004/DBMS/assets/119103799/f0d7f526-47a6-4949-b60c-440faea24820)



## RESULT :
Thus the sequence and synonym created and used in SQL.
