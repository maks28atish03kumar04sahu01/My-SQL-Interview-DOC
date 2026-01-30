## MYSQL Rollback & Commit

Rollback means that what we change in our table through code reverses the process. Commit means whatever we change in sql to a table it stores permanent if we use Commit. Rollback is used for only the insert, update, and delete commands. 

In MySQL, COMMIT and ROLLBACK are used to manage transactions, allowing you to control the finalization or reversal of changes made to the database.

## Rollback

ROLLBACK undoes all changes made during the current transaction, reverting the database to its state before the transaction began. If something goes wrong during the execution of a transaction (e.g., an error occurs), you can use ROLLBACK to cancel the changes and prevent them from being saved. 

``` sql
-- create a table called 'account'
create table account (id int, accname varchar(100), balance int);

-- insert values to the 'account' table
insert into account (id, accname, balance) values
(1, "Ram", 12000), (2, "Hari", 24000), (3, "John", 38000),
(4, "Mohan", 41000), (5, "Michale", 55000), (6, "Max", 67000);

-- display the dataset of 'account' table
select * from account;
```

``` sql
-- rollback command in my sql

-- STEP 1 Start The Transaction
start transaction;

-- STEP 2 Update The 'balance' value where 'id' = 1
update account set balance = balance + 1000 where id = 1;

-- STEP 3 Display the value of 'id' = 1
select * from account where id = 1;

-- STEP 4 Use the rollback command so the 'id' = 1 'balance' value will become 12000 again
rollback;

-- STEP 5 Display the value of 'id' = 1
select * from account where id = 1;
```

## Commit

COMMIT saves all the changes made during the current transaction permanently to the database. After executing multiple SQL statements that modify the database (e.g., INSERT, UPDATE, DELETE), you can use COMMIT to confirm these changes. 

``` sql
-- create a table called 'account'
create table account (id int, accname varchar(100), balance int);

-- insert values to the 'account' table
insert into account (id, accname, balance) values
(1, "Ram", 12000), (2, "Hari", 24000), (3, "John", 38000),
(4, "Mohan", 41000), (5, "Michale", 55000), (6, "Max", 67000);

-- display the dataset of 'account' table
select * from account;
```

``` sql
-- commit command in my sql

-- STEP 1 Start The Transaction
start transaction;

-- STEP 2 Use the select command to see the dataset of 'account' table.
select * from account where id in(3, 4);

/* STEP 3 Use Update Command For 'id' = 3 and 'id' = 4
update balance for 'id' = 3 -> add (+1000)
update balance for 'id' = 4 -> add (+1000) 
*/
update account set balance = balance + 1000 where id = 3;
update account set balance = balance + 1000 where id = 4;

-- STEP 4 Use the select command to see the dataset of 'account' table.
select * from account where id in(3, 4);

-- STEP 5 Use Commit command so the updated balance value is saved permanently
commit; 

-- STEP 6 Use Rollback command to check whether the values will returned to the original value or not.
rollback;

-- STEP 7 Use the select command to see the dataset of 'account' table. you will see the balace will not return to the previous value.
select * from account where id in(3, 4);
```

## Savepoint In MYSQL

SAVEPOINT is a Transaction Control Language (TCL) command in MySQL that creates a named point within a transaction. It allows you to roll back a part of a transaction instead of rolling back the entire transaction. In simple terms, SAVEPOINT lets you undo changes up to a specific point in a transaction. 

### Savepoint Is Used For

* To perform partial rollback. 

* To avoid undoing the entire transaction. 

* To handle complex transactions safely. 

* Useful when multiple operations are executed in one transaction.

**_CREATE SAVEPOINT COMMAND_** = `SAVEPOINT savepoint_name;` 

**_ROLLBACK SAVEPOINT COMMAND_** = `ROLLBACK TO savepoint_name;` 

**_RELEASE SAVEPOINT COMMAND_** = `RELEASE SAVEPOINT savepoint_name;`

## Important Notes On Savepoint Command

* **_SAVEPOINT works only inside a transaction._**

* **_Requires InnoDB storage engine._**

* **_SAVEPOINT is removed automatically after COMMIT._**

* **_ROLLBACK TO SAVEPOINT does not end the transaction._** 

* **_You can create multiple savepoints in one transaction._**

## Savepoint Concept In MYSQL

``` sql
-- create a table called 'account'
create table account (id int, accname varchar(100), balance int);

-- insert values to the 'account' table
insert into account (id, accname, balance) values
(1, "Ram", 12000), (2, "Hari", 24000), (3, "John", 38000),
(4, "Mohan", 41000), (5, "Michale", 55000), (6, "Max", 67000);

-- display the dataset of 'account' table
select * from account;
```

``` sql
-- SAVEPOINT IN MYSQL

-- STEP 1 = START THE TRANSACTION
start transaction;

-- STEP 2 = UPDATE THE BALANCE OF 'ID' = 1
update account set balance = balance + 1000 where id = 1;

-- STEP 3 = DISPLAY THE DATA OF 'ID' = 1 FROM ACCOUNT TABLE
select * from account where id = 1;

-- STEP 4 = CREATE A SAVEPOINT COMMAND CALLED SP1
savepoint sp1;

-- STEP 5 = BY MISTAKE UPDATE OF 'ID1' SET THE BALANCE VALUE = 0
update account set balance = 0 where id = 1;

-- STEP 6 = DISPLAY THE DATA OF 'ID' = 1 FROM ACCOUNT TABLE
select * from account where id = 1;

-- STEP 7 = Undo or rollback the mistaken update value using rollback the savepoint s1
rollback to sp1;

-- STEP 8 = DISPLAY THE DATA OF 'ID' = 1 FROM ACCOUNT TABLE WITH THE UPDATED NEW BALANCE VALUE.
select * from account where id = 1;

-- STEP 9 = SAVE PERMANENTLY SO THE VALUE WILL BE NOT CHANGED TO THE PREVIOUS VALUE
commit;
```

``` sql
-- MULTIPLE SAVE POINT IN MY SQL

START TRANSACTION;

UPDATE ACCOUNT SET BALANCE = BALANCE + 1000 WHERE ID = 5;

SAVEPOINT SP1;

SELECT * FROM ACCOUNT WHERE ID = 5;

UPDATE ACCOUNT SET BALANCE = BALANCE + 1000 WHERE ID = 5;

SAVEPOINT SP2;

SELECT * FROM ACCOUNT WHERE ID = 5;

UPDATE ACCOUNT SET BALANCE = 0 WHERE ID = 5;

SAVEPOINT SP3;

SELECT * FROM ACCOUNT WHERE ID = 5;

ROLLBACK TO SP2;

SELECT * FROM ACCOUNT WHERE ID = 5;

ROLLBACK TO SP1;

SELECT * FROM ACCOUNT WHERE ID = 5;

COMMIT;

ROLLBACK;

SELECT * FROM ACCOUNT WHERE ID = 5;
```
