# Structure Query Language (SQL)

## Create Database Command

This Command Is Used For Create A Database.

``` sql
create database database_name;
```

``` sql
create database demodatabase;
```

## Use Database Command

The use of the database command is used to access a particular database from MySQL.

## Important Note

``` sql
/*Auto Commit Query: Used For To Access The Value Of Auto Commit Value By Default Value Is 1*/
SELECT @@autocommit;

/*Change The Auto Commit Value From 1 To 0*/
SET autocommit = 0;

/*The given command will permit you to execute the update command*/
SET SQL_SAFE_UPDATES = 0;
```

## Create Table

This command is used to create a table inside a database.

``` sql
create table tablename(column_name1 datatype(size value), column_name2 datatype(size value), .....)
```

``` sql
create table employeedb(
    empid bigint,  empname varchar(100), 
    empgmail varchar(100), empphone bigint, 
    empcity varchar(100),  empprofile varchar(100), 
	  empcompany varchar(100),  empexperience int(10),
    empage int(10),   empjoiningdob date, 
    empsalary bigint
);
```

## Insert Single Table  

This command is used to add a single dataset to a table.

``` sql
insert into employeedb (empid, empname, empgmail, empphone, empcity, empprofile, empcompany, empexperience, empage, empjoiningdob, empsalary) 
values (1, "Atish Kumar Sahu", "kumarsahuatish@gmail.com", 9040627203, "Mumbai", "Full Stack Developer", "Google", 5, 24, "2020-04-28", 100000);
```

## Insert Multiple Table

This command is used to add multiple datasets at a time to a table.

``` sql
insert into employeedb (empid, empname, empgmail, empphone, empcity, empprofile, empcompany, empexperience, empage, empjoiningdob, empsalary) values 
(2, "Lipun Kumar Sahu", "kumarsahulipun@gmail.com", 9937401932, "Pune", "Frontend Developer", "Microsoft", 8, 33, "2018-11-05", 90000),
(3, "Sahil Kumar Sahu", "kumarsahusahil@gmail.com", 8082937146, "Bangalore", "Backend Developer", "Oracle", 10, 30, "2016-10-05", 90000);
```

## Update Table

The update command in MySQL is used to modify existing records in a table. It allows you to change the values of one or more columns for specific rows that meet a certain condition, typically defined by a Where Clause.

``` sql
update employeedb set empname = "Mritunjay Atish Kumar Sahu" where empid = 1;
```

## Delete Table

The delete command in MySQL is used to remove one or more rows from a table based on a specific condition. It permanently deletes data from the table unless used within a transaction that can be rolled back.

``` sql
delete from employeedb where empid = 3;
delete from employeedb where empid = 2;
delete from employeedb where empid = 1;
```

## Alter Table 

### Alter Name Of A Table (rename command)

The rename command is used to rename the particular table's old name to a new table name.

``` sql
rename table employeedb to employeedbms;
```

### Alter New Column On A Table (add command)

The add command is used to add a new column to a particular table. It will add a new column to the given table.

``` sql
alter table employeedbms add empdob date;
```

### Alter Data Type Of A Column From A Table (modify command)

The modify command is used to change/alter the data type of a particular column of a table. This command will change the datatype of a given column of the given table.

``` sql
alter table employeedbms modify empphone varchar(100);
```

### Alter Column Name Of Table (change command)

The change command is used to change/alter the column name of a table. The change command will change the column name of the given table.

``` sql
alter table employeedbms change empname empfullname varchar(100);
```

### Change The Position Of The Column In A Table (modify command)

The modify command is used to change/alter the column position of a table. This command changes the position of a particular column from one position to another position.

``` sql
alter table employeedbms modify empfullname varchar(100) after empphone;
```

### Delete A Particular Column From A Table (drop command)

This drop command is used to delete a particular column from a table using the alter command.

``` sql
alter table employeedbms drop column empdob;
```

## Truncate Command

The truncate command is used to delete the dataset from the given table.

``` sql
truncate table employeedbms;
```

## Drop Table Command

The drop command is used to delete the entire table or schema from the database.

``` sql
drop table employeedbms;
```

## Drop Database Command

The drop database command is used to delete the entire database from the server.

``` sql
drop database testmysql;
```
