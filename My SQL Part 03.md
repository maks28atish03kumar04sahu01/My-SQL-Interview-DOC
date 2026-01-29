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
CREATE TABLE employeedemodb(
    empid int(10) not null unique,
    empname varchar(100) not null,
    empprofile varchar(100) not null,
    empcompany varchar(100) not null,
    empcity varchar(100) not null default('Mumbai'),
    empgmail varchar(100) not null,
    empage int(10) not null check(empage >= 20),
    empphone bigint(10) not null,
    empsalary int(10) not null,
    empdob date not null,
    empjoin date not null
);
```

``` sql
INSERT INTO employeedemodb (empid, empname, empprofile, empcompany, empcity, empgmail, empage, empphone, empsalary, empdob, empjoin) VALUES
(1,'Arjun Nair','Frontend Developer','Microsoft','Gurugram','arjun.nair9214@gmail.com',25,7502258532 ,50109,'2001-07-09','2022-02-14'),
(2,'Tanya Kumar','Manager','Netflix','Noida','tanya.kumar1672@gmail.com',58,9122046974 ,80755,'1968-07-03','1988-10-19'),
(3,'Arjun Joshi','Team Lead','Amazon','Bangalore','arjun.joshi8636@gmail.com',41,7068689786 ,74544,'1985-09-26','2016-07-26'),
(4,'Ayesha Verma','Manager','Netflix','Pune','ayesha.verma2788@gmail.com',31,7586176950 ,62390,'1995-12-27','2016-11-29'),
(5,'Rahul Kumar','Team Lead','Microsoft','Gurugram','rahul.kumar8209@gmail.com',60,9473872287 ,74811,'1966-06-01','2002-03-14');
```
