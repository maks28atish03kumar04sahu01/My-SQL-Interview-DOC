# Select Queries In My SQL

## Select The Entire Table In MySQL

```sql
select * from employeedemodb;
```

## Select Multiple Columns From a Table in MySQL

``` sql
select empname, empprofile from employeedemodb;
```

## Select Single Column From Table In MYSQL

``` sql
select empname from employeedemodb;
```

## Where Clause In MYSQL

``` sql
select * from employeedemodb where empname = "Arjun Nair";
```

``` sql
select empname, empprofile, empcompany from studentdemodb where empname = "Tanya Chaudhary";
```

## Comparison Operator (=, !=, <, >, <=, >=)

### Equal Operator

``` sql
select empname from employeedemodb where empage = 50;
```

### Not Equal Operator

``` sql
select empname, empprofile from employeedemodb where empcompany != "Google";
```

### Greater Than Operator

``` sql
select empname, empcompany from employeedemodb where empage > 50;
```

### Greater Than Equal Operator

``` sql
select empname, empcompany from employeedemodb where empsalary >= 90000;
```

### Smaller Than Operator

``` sql
select empname, empcompany from employeedemodb where empsalary < 60000;
```

### Smaller Than Equal Operator

``` sql
select empname, empcompany from employeedemodb where empage <= 23;
```

## AND Operator

``` sql
select empname, empcompany, empprofile from employeedemodb where empage <= 30 and empsalary >= 90000;
```

## OR Operator

``` sql
select empname, empcompany, empprofile from employeedemodb where empage <= 30 or empsalary >= 90000;
```

## Between Operator

``` sql
select empname, empcompany, empprofile from employeedemodb where empid between 1 and 5;
```

## In Operator

``` sql
select empname, empcompany, empprofile from employeedemodb where empid in(1, 5);
```
