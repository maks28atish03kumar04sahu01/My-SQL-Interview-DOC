## MYSQL Rollback & Commit

Rollback means that what we change in our table through code reverses the process. Commit means whatever we change in sql to a table it stores permanent if we use Commit. Rollback is used for only the insert, update, and delete commands. 

In MySQL, COMMIT and ROLLBACK are used to manage transactions, allowing you to control the finalization or reversal of changes made to the database.

## Rollback

ROLLBACK undoes all changes made during the current transaction, reverting the database to its state before the transaction began. If something goes wrong during the execution of a transaction (e.g., an error occurs), you can use ROLLBACK to cancel the changes and prevent them from being saved. 

## Commit

COMMIT saves all the changes made during the current transaction permanently to the database. After executing multiple SQL statements that modify the database (e.g., INSERT, UPDATE, DELETE), you can use COMMIT to confirm these changes. 
