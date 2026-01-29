## SQL Constraints 

### Not Null

Not null is used to prevent null or empty values in the table.

### Unique

Unique value is used to allow unique values, like roll and phone, in the table.

### Default

Default is used if the user does not give any value for the particular column.

### Check

The check () is used to check a condition, and if the condition is true, then only the data will be allowed into the table.

``` sql
CREATE TABLE studentdemodb(
    empid int(10) not null unique,
    empname varchar(100) not null,
    empprofile varchar(100) not null,
    empcompany varchar(100) not null,
    empcity varchar(100) not null default('Mumbai'),
    empgmail varchar(100) not null,
    empage int(10) not null check(empage >= 20),
    empphone bigint(10) not null,
    empdob date not null,
    empjoin date not null
);
```

``` sql
INSERT INTO studentdemodb (empid, empname, empprofile, empcompany, empcity, empgmail, empage, empphone, empdob, empjoin) VALUES
(1,'Akash Patel','Team Lead','META','Bangalore','akash.patel1680@gmail.com',21,9960013389 ,'2005-12-09','2025-12-16'),
(2,'Aman Desai','Full Stack Developer','META','Noida','aman.desai9655@gmail.com',32,7026542351 ,'1994-12-21','2022-11-01'),
(3,'Riya Bhat','Data Analyst','Google','Bangalore','riya.bhat7528@gmail.com',26,9618495931 ,'2000-06-28','2022-06-02'),
(4,'Arjun Gupta','Backend Developer','Microsoft','Pune','arjun.gupta7429@gmail.com',38,7255341928 ,'1988-02-28','2013-05-19'),
(5,'Mohan Gupta','Team Lead','Netflix','Pune','mohan.gupta917@gmail.com',30,8056413953 ,'1996-08-13','2019-08-23');
```
