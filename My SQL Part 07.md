## MYSQL Limit Concept

LIMIT In SQL, LIMIT is used to specify the maximum number of rows to return in a result set. 

``` sql
select empid, empname, empprofile from employeedemodb limit 5; // show data from 1 to 5

select empid, empname, empprofile from employeedemodb limit 10, 5; // show data from 11 to 15
```

## MYSQL Offset Concept

OFFSET In SQL, OFFSET is used to skip a specified number of rows before starting to return rows from the query. 

``` sql
select empid, empname, empprofile from employeedemodb limit 5 offset 40; // show data from 41 to 45

select empid, empname, empprofile from employeedemodb limit 5 offset 450; // Show Data From 451 to 455
```

## AGGREGATE FUNCTIONS IN MYSQL

### COUNT

count the total number of data from a selected column.

``` sql
select count(distinct empcompany) from employeedemodb;

select count(distinct empcity) from employeedemodb;

select count(distinct empprofile) from employeedemodb;
```

### MAX

It will return the max value from the column.

``` sql
select max(empsalary) from employeedemodb;

select max(empage) from employeedemodb;

```

### MIN

It will return the min value from the column.

``` sql
select min(empsalary) from employeedemodb;

select min(empage) from employeedemodb;
```

### SUM

It will return the sum of the values from the column.

``` sql
select sum(empsalary) from employeedemodb;
```

### AVG

It will return the average value of the column.

``` sql
select avg(empsalary) from employeedemodb;
```
