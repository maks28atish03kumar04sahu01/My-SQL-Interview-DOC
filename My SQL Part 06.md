## MYSQL ORDER CONCEPTS

### Ascending Order Sort

It will display the data in ascending order.

``` sql
select empname from employeedemodb where empid between 1 and 5 order by empname asc;
```

### Descending Order Sort

It will display the data in descending order.

``` sql
select empname from employeedemodb where empid between 1 and 5 order by empname desc;
```

## Distinct Concept

It will display the unique data, and it will not display the duplicate or repeated data.

``` sql
select distinct empcity from employeedemodb;

select distinct empprofile from employeedemodb;

select distinct empage from employeedemodb;

select distinct empcompany from employeedemodb;
```

## Is Null Concept

It will display the data if the data is empty or has a null value. 
IS NULL In SQL, ‘IS NULL’ checks if a column contains ‘NULL’ values, which indicates the absence of any data.  

``` sql
select * from employeedemodb where empcity is null;
```

## Is Not Null Concept

It will display the data if the data is not empty or does not have a null value.
IS NOT NULL In SQL, ‘IS NOT NULL’ checks if a column contains non-‘NULL’ values, meaning the column has data. 

``` sql
select * from employeedemodb where empcity is not null;
```
