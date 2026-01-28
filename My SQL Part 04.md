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
create table studentdemodb(
  empid int(10) not null unique, empnam varchar(100) not null,
  empprofile varchar(100) not null, empcompany varchar(100) not null,
  empcity varchar(100) not null default("Mumbai"), empgmail varchar(100) not null,
  empage int(10) not null check(empage >= 20), empphone bigint(10) not null,
  empdob date not null,  empjoin date not null
);
```

``` sql
INSERT INTO studentdemodb (empid, empnam, empprofile, empcompany, empcity, empgmail, empage, empphone, empdob, empjoin) VALUES
(101,'Vivek Desai','Backend Developer','Tesla','Noida','vivek.desai7843@gmail.com',28,6691251778 ,'1998-10-29','2019-10-17'),
(102,'Isha Singh','Designer','Microsoft','Gurugram','isha.singh908@gmail.com',55,9824225358 ,'1971-11-19','2000-01-17'),
(103,'Kavya Kumar','Data Analyst','META','Bangalore','kavya.kumar4962@gmail.com',36,9829922995 ,'1990-04-21','2022-08-28'),
(104,'Rahul Verma','Data Analyst','Netflix','Mumbai','rahul.verma9374@gmail.com',21,6907844736 ,'2005-02-02','2025-12-27'),
(105,'Kavya Malhotra','Manager','Microsoft','Noida','kavya.malhotra7610@gmail.com',24,8592555625 ,'2002-12-02','2023-10-21'),
(106,'Ayesha Desai','Backend Developer','Tesla','Noida','ayesha.desai4062@gmail.com',26,8104696325 ,'2000-06-08','2023-01-19'),
(107,'Rahul Bose','Manager','Microsoft','Pune','rahul.bose8149@gmail.com',32,9168733950 ,'1994-03-16','2025-09-30'),
(108,'Arjun Joshi','Manager','Tesla','Gurugram','arjun.joshi134@gmail.com',51,9624565060 ,'1975-10-29','2025-03-04'),
(109,'Rahul Desai','Backend Developer','Microsoft','Gurugram','rahul.desai7379@gmail.com',32,7991216558 ,'1994-06-18','2020-12-07'),
(110,'Isha Singh','Frontend Developer','Google','Delhi','isha.singh2246@gmail.com',32,7787298259 ,'1994-10-17','2019-04-18');
```
