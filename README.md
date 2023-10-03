# EX 2 Data Manipulation Language (DML) Commands and built in functions in SQL
## AIM:
To create a manager database and execute DML queries using SQL.


## DML(Data Manipulation Language)
<div align="justify">
The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.
</div>

## List of DML commands: 
<div align="justify">
INSERT: It is used to insert data into a table.<br>
UPDATE: It is used to update existing data within a table.<br>
DELETE: It is used to delete records from a database table.<br>
</div>

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
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/16069cd8-ef4b-443c-944f-2154790ad0af)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/8dfe87a6-a2b6-48e3-b01d-b7779c99bbc1)

### Q2) Delete the records from manager table where the salary less than 2750.
## QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/c44f02ae-5f78-4a03-890a-11fbc53a45e2)


## OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/cc2754d3-2bc0-4364-9b95-0e5c36f964df)


### Q3) Display each name of the employee as “Name” and annual salary as “Annual Salary” (Note: Salary in emp table is the monthly salary)
### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/948964cd-bd99-49f0-8e2a-097c9554cdf8)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/13428a95-d829-4272-afe7-f592858dfb69)


### Q5)	List the names of Clerks from emp table.
## QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/53878f87-a320-48ba-8cd9-508ccd8eb51e)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/d37859a9-d41a-4f74-b3f7-0b87cb15e3fb)


### Q6)	List the names of employee who are not Managers.
### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/f6ca815d-069a-4df5-9d1d-3f69e24e0fa4)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/29bc77ba-d518-40e9-ac5a-b082fe7cd595)


### Q7)	List the names of employees not eligible for commission.
### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/4f84a075-15c4-4dfc-a86c-0db3220d7c5e)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/b0404872-0a3c-4d63-8c5c-7e94bc484283)



### Q8)	List employees whose name either start or end with ‘s’.


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/f8187bd6-fd1c-43c0-abba-b7e2ccdf1865)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/1c9dfd07-78b7-4ba7-8dfe-c31365f99ddd)



### Q9) Sort emp table in ascending order by hire-date and list ename, job, deptno and hire-date.


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/e2165171-e42b-477d-9a45-7156bebf8884)



### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/2b790aa4-fee9-44eb-b7bd-973f9b8102d6)



### Q10) List the Details of Employees who have joined before 30 Sept 81.


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/90748c49-b4a7-41b3-8116-21943dd80f34)



### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/7481799d-85f1-49d9-aa00-21495735fbf3)


### Q11)	List ename, deptno and sal after sorting emp table in ascending order by deptno and then descending order by sal.


### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/b3002db9-7a23-44ba-940c-0ad76df99960)


### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/1303662d-55d5-470c-918e-2f8fd7452e47)



### Q12) List the names of employees not belonging to dept no 30,40 & 10


### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/cc28f676-d410-4447-a818-68390378d0cd)



### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/484cdcd1-586a-4631-9da1-7b6b0d6d2ad7)


### Q13) Find number of rows in the table EMP

### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/a47f67fe-5aee-49b9-9660-4b28848b4605)


### OUTPUT:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/9992588c-32c1-4215-ba06-6505d563a3df)



### Q14) Find maximum, minimum and average salary in EMP table.

### QUERY:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/ebe4a328-b5f3-491c-b2b2-a1de35c4171b)



### OUTPUT:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/03787233-5cde-42c7-8851-08214c1f6b08)



### Q15) List the jobs and number of employees in each job. The result should be in the descending order of the number of employees.

### QUERY:

![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/23591dd0-5f97-44ea-b0f5-09e2c959f824)



### OUTPUT:
![image](https://github.com/dineshgl/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121166004/9da72472-d017-440e-a10a-95ff2e824323)

### RESULT:
Thus the Data Manipulation Language (DML) Commands and built in functions in SQL
