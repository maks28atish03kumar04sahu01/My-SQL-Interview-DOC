# MySQL Programming Language

## Data

Data is the raw, unprocessed facts or figures collected from various sources. It can come in many forms, such as numbers, text, images, audio, or video, and it doesn’t carry much meaning on its own. For example, “25”, “Blue”, or “John” are pieces of data, but without context, they don’t provide much insight. Data represents the basic building blocks of information and is usually collected for further processing or analysis. 

## Information

Information, on the other hand, is processed, organized, and structured data that has meaning and can be used for decision-making. When data is interpreted and put into context, it transforms into information. For instance, “John is 25 years old and drives a blue car” is information because it combines data elements in a way that tells us something useful. Information is the outcome of analyzing, organizing, and presenting data in a comprehensible format. 

## Database

A Database is a structured collection of data that is stored electronically and can be accessed, managed, and updated efficiently. Databases are used to store data in a way that allows for easy retrieval, manipulation, and management.  

They are managed through database management systems (DBMS), which provide tools to insert, query, update, and delete data while ensuring security, integrity, and consistency. A database is an organized collection of data, stored and retrieved electronically. Databases can be used to store various types of data, such as text, numbers, dates, images, or even multimedia files. 

## Structured Query Language (SQL) 

Structured Query Language (SQL) is a standard programming language used to manage and manipulate relational databases. It allows users to perform tasks such as inserting data, querying data, updating records, and creating or modifying the structure of database tables.  

SQL is powerful for handling structured data with clearly defined relationships and follows a fixed schema, making it suitable for systems that demand consistency and transactional accuracy.  

SQL stands for Structured Query Language. It is a standard programming language specifically designed for managing and manipulating databases. SQL is used primarily for creating querying and updating databases as well as to create and modify database structure.

Not Only Structured Query Language (NoSQL) 

Not Only Structured Query Language (NoSQL) refers to a category of database systems that provide a mechanism for storage and retrieval of data that is not modeled in tabular form. NoSQL databases are designed for handling large volumes of varied data types, including unstructured and semi-structured data. They offer high performance, horizontal scalability, and are schema-less, allowing dynamic and flexible data models. These databases are often used in applications involving big data, real-time analytics, or content management

## Difference Between No SQL VS MySQL

### MySQL

1. SQL databases use a relational data model, where data is stored in structured tables consisting of rows and columns. Each table has a fixed schema, and the relationships between tables are strictly defined using foreign keys. This model is excellent for maintaining data consistency and integrity. 

2. SQL databases typically scale vertically, meaning to handle more load, you need to upgrade the existing server's hardware—adding more CPU, RAM, or storage. This approach can become costly and eventually reach physical limitations. 

3. SQL uses a standardized query language (Structured Query Language) that is powerful for complex queries involving multiple joins, filters, aggregations, and transactions. However, it requires precise knowledge of the schema and is rigid in nature. 

4. SQL databases follow the ACID properties—Atomicity, Consistency, Isolation, and Durability. These ensure reliable transactions and strong consistency, making SQL suitable for applications like banking or e-commerce where data integrity is crucial. 

5. SQL databases are ideal for applications requiring structured data, complex relationships, and strict data integrity, such as enterprise systems, accounting software, and inventory management. They perform well when the data schema is stable and doesn’t change frequently. 

### No SQL

1. NoSQL databases use a non-relational or schema-less model. They can store data as key-value pairs, documents, wide-column stores, or graphs, allowing greater flexibility to accommodate diverse and changing data structures without needing to define a fixed schema beforehand. 

2. NoSQL databases are designed to scale horizontally by adding more servers to distribute the load. This makes NoSQL more suitable for handling large-scale data and high-traffic applications like social media platforms or big data analytics systems. 

3. NoSQL does not have a single query language; each database (e.g., MongoDB, Cassandra) has its own API or query method. This allows for more flexible and intuitive querying, especially for applications dealing with unstructured or semi-structured data like JSON or XML. 

4. NoSQL databases often follow the BASE model—Basically Available, Soft state, eventually consistent. This model prioritizes high availability and partition tolerance over immediate consistency, making NoSQL better for real-time applications where eventual accuracy is acceptable. 

5. NoSQL databases, in contrast, are suited for modern applications that handle massive volumes of unstructured or dynamic data, such as content management systems, IoT platforms, recommendation engines, and real-time analytics. Their flexible data models and scalability features make them a natural choice for fast-evolving, large-scale projects. 

## Database Management System

A Database Management System (DBMS) is a software system that enables users to define, create, maintain, and control access to databases. It acts as an interface between the user and the database, allowing data to be stored, retrieved, and manipulated efficiently. A DBMS ensures data integrity, security, and consistency while providing features such as backup, recovery, concurrency control, and access control. It eliminates data redundancy and enhances data sharing among multiple users or applications. 


## Relational Database Management System (RDBMS) 

A Relational Database Management System (RDBMS) is a type of DBMS that stores data in the form of related tables composed of rows and columns. Each table has a defined schema, and the relationships between different tables are established using foreign keys. RDBMSs use Structured Query Language (SQL) for querying and manipulating data. They strictly adhere to the principles of data integrity and the ACID properties (Atomicity, Consistency, Isolation, Durability), making them highly reliable for transactional applications such as banking, inventory, and payroll systems. 


## Non Relational Database Management System (NO-RDBMS)

A Non-Relational Database Management System refers to databases that do not use the traditional table-based structure of relational databases. Instead, they use alternative data models such as key-value pairs, documents, columns, or graphs. These systems are designed to handle large volumes of diverse, unstructured, or semi-structured data and are highly scalable, often supporting horizontal scaling. Non-relational DBMSs are flexible in terms of schema design and are better suited for modern applications such as real-time analytics, big data, and distributed systems. 

## Key-Value Management System

A Key-Value Type Database Management System stores data as a collection of key-value pairs, where each key is unique and maps directly to a value. This type of database is simple, fast, and highly scalable, making it ideal for use cases that require quick lookups, such as caching systems, session storage, and real-time recommendation engines. The key acts like an identifier, and the value can be any type of data, from simple strings to complex objects. Redis and Amazon DynamoDB are examples of key-value databases.

## Column Based Database Management System

A Column-Based Database Management System, also known as a columnar database, stores data by columns instead of rows. This structure allows for efficient storage, retrieval, and aggregation of large datasets, especially for read-heavy workloads such as data warehousing and business intelligence. By reading only the necessary columns rather than entire rows, columnar databases improve performance in analytical queries. Examples of column-based databases include Apache Cassandra and Google Bigtable.

## Graph Type Database Management System

A Graph Type Database Management System is designed to store and represent data in the form of nodes (entities) and edges (relationships). This model is highly efficient for applications that require complex relationship mapping, such as social networks, recommendation systems, and fraud detection. Graph databases make traversing relationships fast and intuitive, which is often challenging in traditional relational databases. Neo4j and Amazon Neptune are well-known examples of graph database systems. 

## Document Based Database Management System

A Document-Based Database Management System stores data in document formats, typically using JSON, BSON, or XML. Each document contains all the data for a given record, which allows for flexibility in the structure and schema. This type of DBMS is ideal for content management systems, e-commerce platforms, and applications that require a dynamic schema. Document databases allow nested data, indexing, and powerful query capabilities without strict schema enforcement. MongoDB and CouchDB are prominent examples of document-oriented databases. 

## Types Of Databases

* **Relational Database** it organizes data into tables with rows and columns and use Structured Query Language (SQL) for managing data. They are ideal for applications requiring complex queries and data integrity, such as banking or inventory systems. 

* **NoSQL Databases** these are designed for scalability and flexibility; they can store unstructured or semi-structured data in formats like key-value pairs, documents, wide-columns, or graphs. These are commonly used in big data and real-time web applications. 

* **Hierarchical Databases** this is use a tree-like structure where data is organized in a parent-child relationship, often found in legacy systems. 

* **Network Databases** these are similar but allow more complex many-to-many relationships. 

* **Object-Oriented Databases** It store data in the form of objects, as used in object-oriented programming, making them suitable for applications requiring tight integration with code. 

* **Distributed Databases** these are spread across multiple physical locations and synchronize data across different servers, improving availability and performance. 

* **Cloud Databases** these are hosted on cloud platforms, allowing scalability, flexibility, and reduced infrastructure costs. 

## Components Of Database

A typically contains tables, columns, rows, indexes and constraints. Table store data in rows and columns, with each row representing a specific record and each column representing a specific attribute of that record. Indexes are used to speedup queries and constraints enforce data integrity rules. 

## Difference Between RDBMS VS NO-DBMS

A relational database management system (RDBMS) uses a structured schema and tables to store data in relations, where data items are related to each other through keys. It enforces ACID (Atomicity, Consistency, Isolation, Durability) properties for transactions and supports SQL for querying data. 

A non-relational database management system also known as a NoSQL database, does not rely on a fixed schema or relations between data items. Non-relational databases store data in other formats such as key-values, documents or graphs and may have different ways of querying and updating data. These databases typically provide more flexibility and scalability but may sacrifice strict consistency for performance. 

## Backend

Backend refers to the server-side part of a software application or website that users do not directly see or interact with. It is responsible for managing the logic, database interactions, authentication, data processing, and server configuration that power the application's functionality. The backend ensures that user requests from the frontend (user interface) are processed correctly and securely. Technologies commonly used in backend development include programming languages like Java, Python, Node.js, and PHP, along with databases and server frameworks. 

## Server

Server is a system—either software, hardware, or a combination of both—that provides services or resources to other devices, known as clients, over a network. In web development, a server hosts the backend of an application, listens to client requests (like opening a webpage), processes those requests (such as fetching data), and sends back appropriate responses. Servers can be physical machines, virtual machines, or cloud-based instances, and they play a critical role in ensuring availability, scalability, and performance of applications. 

## Schma

Schema in the context of databases is the structural blueprint that defines how data is organized within the database. It specifies the tables, fields, data types, relationships, indexes, and constraints that determine how the data is stored and accessed. A schema acts as a framework that ensures consistency and integrity in the database. In relational databases, the schema is essential for enforcing rules on what kind of data can be stored and how different pieces of data relate to each other. 

## Table

Table is a fundamental component of a relational database where data is stored in a structured format using rows and columns. Each column in a table represents a specific attribute or field (such as name, age, or email), while each row represents a single record or entry. Tables are used to organize related data so that it can be easily queried, updated, and managed. Multiple tables can exist within a database, and they can be connected through keys to form relationships between different sets of data. 

## More On SQL

SQL is a short-form of the structured query language, and it is pronounced as S-Q-L or sometimes as See-Quell. This database language is mainly designed for maintaining the data in relational database management systems. It is a special tool used by data professionals for handling structured data (data which is stored in the form of tables). It is also designed for stream processing in RDSMS. You can easily create and manipulate the database, access and modify the table rows and columns, etc. Big enterprises like Facebook, Instagram, and LinkedIn, use SQL for storing the data in the back-end. 

## History Of SQL

"A Relational Model of Data for Large Shared Data Banks" was a paper which was published by the great computer scientist "E.F. Codd" in 1970. The IBM researchers Raymond Boyce and Donald Chamberlin originally developed the SEQUEL (Structured English Query Language) after learning from the paper given by E.F. Codd. They both developed the SQL at the San Jose Research laboratory of IBM Corporation in 1970. At the end of the 1970s, relational software Inc. developed their own first SQL using the concepts of E.F. Codd, Raymond Boyce, and Donald Chamberlin. This SQL was totally based on RDBMS. 

## Characteristics Of SQL

1. SQL may be utilized by quite a number of users, which include people with very little programming experience. It uses functions to perform some formatting.   

2. SQL is a non-procedural language. We can without difficulty create and replace databases in SQL. It isn’t a time-consuming process. 

3. SQL is primarily based totally on ANSI standards. SQL does now no longer have a continuation individual.  

4. SQL is entered into the SQL buffer on one or more lines. SQL makes use of a termination individual to execute instructions immediately. It makes use of features to carry out a few formatting. 

## Uses Of SQL

1. Data Definition It is used to define the structure and organization of the stored data and the relationships among the stored data items. 

2. Data Retrieval SQL can also be used for data retrieval. 

3. Data Manipulation If the user wants to add new data, remove data, or modifying in existing data then SQL provides this facility also. 

4. Access Control SQL can be used to restrict a user’s ability to retrieve, add, and modify data, protecting stored data against unauthorized access. 

5. Data Sharing SQL is used to coordinate data sharing by concurrent users, ensuring that changes made by one user do not inadvertently wipe out changes made at nearly the same time by another user. 

## SQL Rules & Regulation

* A ‘;’ is used to end SQL statements. Statements may be split across lines, but keywords may not. Identifiers, operator names, and literals are separated by one or more spaces or other delimiters. Numeric literals can be represented by simple values. 

* A comma (,) separates parameters without a clause. A space separates a clause. Reserved words cannot be used as identifiers unless enclosed with double quotes. 

* Identifiers can contain up to 30 characters. Identifiers must start with an alphabetic character. Characters and date literals must be enclosed within single quotes. 

## SQL Commands

Developers use structured query language (SQL) commands, which are specific keywords or SQL statements, to work with data stored in relational databases. The following are categories for SQL commands. 

## Data Definition Language (DDL)

Data Definition Language (DDL) is a category of SQL commands used to define and modify the structure of database objects such as tables, schemas, indexes, and views. It deals with the creation, alteration, and deletion of the database framework itself. Commands like CREATE, ALTER, DROP, and TRUNCATE fall under DDL, and they directly affect how the database is organized and structured. 

## Data Manipulation Language (DML)

Data Manipulation Language (DML) includes SQL commands that are used to manipulate the data stored within database tables. It allows users to insert new rows, update existing records, delete unwanted data, and merge or replace rows. Common commands such as INSERT, UPDATE, DELETE, and MERGE fall under DML, enabling everyday operations that change the contents of the database. 

## Data Query Language (DQL)

Data Query Language (DQL) is used to retrieve data from a database based on specific conditions. The primary command in DQL is SELECT, which allows users to query one or more tables to extract useful information while optionally filtering, sorting, or grouping results. DQL focuses only on fetching data without altering either the data or the structural design of the database. 

## Data Control Language (DCL)

Data Control Language (DCL) manages permissions and access control for users within a database system. It allows database administrators to grant or revoke privileges such as the ability to read data, modify data, or execute certain commands. The main DCL commands are GRANT and REVOKE, which ensure that only authorized users can access or manipulate database resources. 

## Transaction Control Language (TCL)

Transaction Control Language (TCL) is used to manage transactions in a database, ensuring data integrity and consistency. It allows users to group a series of operations into a single logical unit of work that must be either completely executed or fully cancelled. Commands like COMMIT, ROLLBACK, and SAVEPOINT fall under TCL and help control whether changes made during a transaction are permanently saved or undone based on whether the transaction completes successfully or encounters an error. 

## Session Control Languge (SCL)

Session Control Language (SCL) in DBMS refers to a set of commands used to manage user sessions and their interaction environment with the database system. These commands control session-level properties such as user login, logout, and settings that affect only the current connection or session.  

They are used to establish or modify characteristics like language, date format, schema, and roles for the duration of a user's session. For example, commands like ALTER SESSION or SET ROLE in SQL are used to customize how the database behaves specifically for the current user session without permanently affecting the database structure or data. 

## Advantages Of SQL

1. No programming needed. 

2. High-Speed Query Processing 

3. Standardized Language 

4. Portability 

5. Interactive Language 

6. More Than One Data View

## ER Diagram (Entity-Relationship)

An Entity-Relationship (ER) diagram is a visual representation of the data model that depicts the entities (such as people, objects, concepts), their attributes (properties or characteristics), and the relationships between them. ER Diagrams are commonly used in database design to provide a clear and concise overview of the database structure. 

## Entity

An entity represents a real-world object or concept that can be uniquely identified. It is typically represented by a rectangle in an ER diagram. 

## Attribute 

An attribute describes a characteristics or property of an entity. It is represented within the entity rectangle. 

## Relationship 

A relationship illustrates the connection between two or more entities. It describes how entitles are related to each other. 

## Cardinality 

Cardinality defines the numerical relationship between entitles in a relationship. It specifies how many instances of one entity are associated with one instance of another entity. 

## Key Attribute 

A key attribute uniquely identifies each instance of an entity. It is often designated as the primary key in a database. 

## Clarity 

ER Diagram provide a clear visualization of the database structure, making it easier to understand and communicate database designs. 

## Complteness

By identifying entities, attributes, and relationships, ER diagrams ensure that all relevant components of the database are considered. 

## Normalization 

ER diagrams help in normalizing the database design by identifying redundant data and ensuring data integrity. 

## Documentation

ER diagrams serve as documentation for database designs, aiding in maintenance, troubleshooting, and future development. 

## Dependency In RDBMS 

In DBMS, a dependency refers to the relationship between two or more attributes in a database such that the value of one attribute is determined by, or depends on, the value of another attribute. It shows how data items are related to each other within a table or across tables. Dependencies are used to ensure data consistency and are a fundamental concept in normalization — the process of organizing a database to reduce redundancy and avoid anomalies. For example, in a functional dependency, if attribute A determines attribute B (written as A → B), it means that the value of B is dependent on the value of A; whenever A changes, B must be updated accordingly to preserve accuracy. 

## Functional Dependency 

Functional dependency occurs when the value of one attribute (or a group of attributes) uniquely determines another attribute in a relation. If attribute A functionally determines attribute B, it means that for every unique value of A, there is exactly one corresponding value of B. It is denoted as A → B. Functional dependency forms the foundation of normalization rules and helps maintain consistency in data. 

## Partial Dependency

Partial dependency exists when a non-prime attribute (an attribute that does not belong to any candidate key) is functionally dependent on part of a candidate key rather than the whole key. This usually happens in tables with composite primary keys. Partial dependency is removed when converting a relation from First Normal Form (1NF) to Second Normal Form (2NF). 

## Transitive Dependency

A transitive dependency occurs when one non-key attribute depends on another non-key attribute (not directly on the primary key). In other words, if A → B and B → C, then A → C is a transitive dependency. These are undesirable because they can lead to redundancy and anomalies. Transitive dependencies are removed when moving from Second Normal Form (2NF) to Third Normal Form (3NF). 

## Multivalued Dependency

Multivalued dependency happens when one attribute in a table uniquely determines another attribute, independent of other attributes. It is denoted by A ↠ B. This means that for a single value of A, there are multiple independent values of B. These types of dependency are handled while converting a relation into Fourth Normal Form (4NF) to remove repeated groups. 

## Join Dependency

Join dependency is a constraint where a relation can be reconstructed by joining multiple projections (subsets of attributes) without losing any information. It is a generalization of multivalued dependency. If a relation R can be decomposed into R1, R2, ..., Rn and can be losslessly joined back, then R has a join dependency. Elimination of join dependency leads to Fifth Normal Form (5NF), also known as Project-Join Normal Form (PJNF). 

## One-To-One Relationship

One-to-One Relationship is a type of database relationship where a single record in one table is directly linked to only one record in another table, and vice-versa. This means both tables have a unique connection between their records. For example, in a system where each employee is assigned one unique company laptop, the relationship between the Employees table and the laptops table would be one-to-one. 

## One-To-Many Relationship

One-to-Many Relationship refers to a scenario where a single record in one table can be associated with multiple records in another table, but each of those multiple records relates back to only that one record. For instance, in a database where one customer can place many orders, the Customers table relates to the Orders table through a one-to-many relationship. 

## Many-To-One Relationship 

Many-to-One Relationship is essentially the reverse of one-to-many: multiple records in one table can be associated with a single record in another table, but that single record connects back to many. An example would be many employees working in one specific department — where the Employees table has many entries pointing to a single entry in the Departments table. 

## Many-To-Many Relationship

Many-to-Many Relationship exists when multiple records in one table can be linked to multiple records in another table. This kind of relationship usually requires a junction or linking table to handle the associations. A classic example is students and courses, where one student can enroll in many courses, and each course can have many students; the association between them is managed through a separate enrollment table. 

## ACID (Atomicity Consistency Isolation Durability) PROPERTIES 

Atomicity ensures that a transaction is treated as a single unit; it either completes fully or does not happen at all. Consistency ensures that a transaction takes the database from one valid state to another valid state, maintaining all rules and constraints. Isolation ensures that concurrent transactions do not interfere with each other and appear to run independently. Durability guarantees that once a transaction is committed, its changes are permanent even in the case of system failure. 

## CAP (Consistency Availability Partition Tolerance) PROPERTIES 

Consistency means that every node in the distributed system sees the same data at the same time. After a write operation, all future reads should return the updated value no matter which node is accessed. Availability ensures that the system is always accessible and responsive. Every request made to the system receives a response, whether it returns the requested data or an error — the system should not go down or refuse to respond. Partition Tolerance refers to the system’s ability to continue functioning even when there is a network failure or communication break between nodes. Despite these partitions in the network, the system should still operate without total failure. 

## BASE (Basically Available Soft State Eventually Consistent) PROPERTIES 

Basically, Available indicates that the system guarantees availability most of the time, responding quickly even if some parts of the system are experiencing issues. It favors access over perfection. Soft State means that the state of the system may change over time, even without input. This is because data from different nodes might be inconsistent temporarily due to replication delays, and synchronization happens gradually. Eventually Consistent ensures that although data might not be immediately consistent across all nodes, it will become consistent over time if no new updates occur. The system sacrifices instant consistency in order to achieve better performance and scalability. 

## Normal Form

Normal Form refers to a set of guidelines in relational database design that help eliminate redundancy and dependency problems. By organizing data into increasingly strict levels called normal forms, a database becomes more efficient, consistent, and scalable, reducing anomalies during insertion, deletion, and update operations. School management systems, which deal with varied data like students, classes, teachers, and fees, often rely on normalization to maintain clean and consistent databases. 

## First Normal Form (1NF / FNF)

First Normal Form (1NF) requires that each table column contains only atomic (indivisible) values and each record must be unique. It ensures that repeating groups or arrays are not present in any field. 

Example: In a school management system, instead of storing multiple contact numbers in a single cell of a “Students” table (e.g., Contact = “98765…, 98989…”), these numbers are divided into separate rows or fields so that each column holds a single value, ensuring every student’s record is cleanly formatted under 1NF rules. 

## Second Normal Form (2NF / SNF)

Second Normal Form (2NF) builds on the first by ensuring there is no partial dependency; that is, non-key attributes must depend on the entire primary key rather than just part of it. 

Example: In a school database, suppose there is a table storing StudentID, SubjectID, and TeacherName. If TeacherName depends only on SubjectID and not on the combination of StudentID and SubjectID, this violates 2NF. So, the table is split: one table contains SubjectID and TeacherName, and other stores the StudentID and SubjectID mapping, thus eliminating partial dependency and satisfying 2NF. 

## Third Normal Form (3NF / TNF)

Third Normal Form (3NF) requires that tables be in 2NF and that all the non-key attributes depend only on the primary key, not on other non-key attributes (i.e., no transitive dependency). 

Example: In a school management system, a table containing StudentID, ClassID, and ClassTeacherPhone might cause a transitive dependency because ClassTeacherPhone actually depends on ClassID, not directly on StudentID. Separating class information into a new table with ClassID, ClassTeacher, and ClassTeacherPhone, and linking students only by ClassID ensures that all data stored in the student table relates directly to the student as primary key, meeting 3NF. 

## Fourth Normal Form (4NF / FNF) 

Fourth Normal Form (4NF) focuses on eliminating multi-valued dependencies. A table is in 4NF if it is in 3NF and does not contain two or more independent and multivalued data facts about an entity. 

Example: In a school system, if a table lists StudentID with multiple Hobbies and multiple Languages, then combinations of hobbies and languages show up redundantly, creating a multivalued dependency problem. To convert this into 4NF, two separate tables should be created: one for StudentID–Hobby and another for StudentID–Language, preserving independence between hobbies and languages per student. 

## Fifth Normal Form (5NF / FNF) 

Fifth Normal Form (5NF), also called Projection Join Normal Form (PJNF), ensures that a table is broken down into smaller tables so that they can be joined without creating redundant data. It addresses cases where information can be reconstructed from smaller pieces without loss but storing them together results in redundancy. 

Example: In a school management database, suppose a table stores which Teachers teach a Subject in a particular Class. If teachers may teach different subjects in different classes, redundancy may creep in. Instead, breaking this into three separate tables — one mapping Teacher–Subject, another mapping Subject–Class, and a third linking Teacher–Class — and then joining them through appropriate queries eliminates redundancies, ensuring the system adheres to 5NF. 

## My Structured Query Language (MySQL)

MySQL is an open-source relational database management system (RDBMS) developed by Oracle Corporation, based on Structured Query Language (SQL). It is widely used for managing and organizing data in web applications due to its speed, reliability, and ease of use.  

MySQL follows a client-server architecture, where the MySQL server manages databases and responds to queries from client programs. It supports standard SQL commands for creating, reading, updating, and deleting data, and is popularly used with PHP and Apache in the LAMP stack for dynamic website development. 

MySQL is usually case-insensitive for table and column names (especially on Windows), meaning SELECT Name and select name are treated the same. However, on Linux systems MySQL can become case-sensitive depending on the filesystem and lower_case_table_names settings. 

MySQL is typically used for web applications and small to medium-scale systems due to its simplicity and speed. Oracle SQL offers more advanced features such as built-in support for PL/SQL, complex transaction controls, real application clusters (RAC), and extensive backup and recovery tools. MySQL performs exceptionally well for read-heavy workloads and simple queries used commonly in web applications. MySQL supports stored procedures and triggers, but its procedural capabilities are limited compared to Oracle. 

## Q1. What Is Database? 

A database is an organized collection of interrelated data stored in a structured format that enables efficient retrieval, insertion, deletion, and management of information. It allows users to organize data into tables, rows, columns, and indexes, making it easier to quickly access and manage relevant information. Databases also offer distinct APIs for performing various operations such as creating, managing, and searching data. Widely used databases include MySQL, Oracle, MongoDB, PostgreSQL, and SQL Server. MySQL, in particular, is known for its reliability, ease of use, and strong community support. 

## Q2. What is DBMS (Database Management System)? 

The software which is used to manage database is called Database Management System (DBMS). For Example, MySQL, Oracle etc. are popular commercial DBMS used in different applications. 

## 03. What are the different types of SQL languages used in a DBMS? 

1. **DDL (Data Definition Language)** Used to define and modify the structure of database objects like tables, indexes, and schemas. Common DDL commands include CREATE, ALTER, DROP, and TRUNCATE.  

2. **DML (Data Manipulation Language)** Used for manipulating data within tables. It includes commands like SELECT, INSERT, UPDATE, and DELETE for retrieving and modifying data. 

3. **DCL (Data Control Language)** Used to control access to data and manage user permissions within the database. Common DCL commands are GRANT, REVOKE. 

4. **TCL (Transaction Control Language)** Deals with the transactions within a database, ensuring the integrity of the data. Common TCL commands include COMMIT, ROLLBACK, SAVEPOINT, SET TRANSACTION. 

5. **DQL (Data Query Language)** Focused specifically on querying the data. The main DQL command is SELECT. 

* Stored Procedures and functions are pre-compiled SQL statements that can be executed as a unit. Stored procedures allow for better performance and security, as well as the reuse of logic within the database.  

* Triggers are Special types of procedures that automatically execute in response to certain events (like INSERT, UPDATE, or DELETE operations) on a table.  

* Indexes are the Structures that improve the speed of data retrieval operations on a database table, making queries more efficient. 

* Views are the Virtual tables that provide a way to simplify complex queries by creating a predefined result set from one or more tables, which can be queried as if it were a table. 

* Normalization is a process in DBMS to minimize redundancy and dependency by organizing fields and table relations in a database.  

## Q4. In DBMS which tasks are allowed to do certain operations? 

Data Definition which helps in creation, modification and removal of definitions that define the organization of data in database. Data Updating which helps in insertion, modification and deletion of the actual data in the database.  Data Retrieval which helps in retrieval of data from the database which can be used by applications for various purposes. 

## Q5. What is User Administration? 

It helps in registering and monitoring users, enforcing data security, monitoring performance, maintaining data integrity, dealing with concurrency control and recovering information corrupted by unexpected failure. 

## Q6. What is My SQL? 

My SQL is a database management system software used for managing the relational database. It is an open-source database software which is supported by Oracle. It is fast, scalable, and easy to use database management system in comparison with Microsoft SQL Server and Oracle Database. It is commonly used in conjunction with PHP scripts for creating powerful and dynamic server-side or web-based enterprise applications. 

## Q7. Features Of My SQL? 

It allows us to implement database operations on tables, rows, columns, and indexes. It defines the database relationship in the form of tables (collection of rows and columns), also known as relations. It provides the Referential Integrity between rows or columns of various tables. It allows us to updates the table indexes automatically. It uses many SQL queries and combines useful information from multiple tables for the end-users.  

## Q8. Advantages Of My SQL? 

It is a cross platform. It used with multiple languages like JAVA, PHP, node js, python, C#. MySQL software is open source. MySQL is RDBMS. MySQL database server is fast, reliable, scalable and easy to use. MySQL server works in client/server or embedded systems. 

## Q9. Difference between SQL & No SQL? 

### SQL: 

1. It is a domain-specific language used to manage data stored in a relational database which requires a fixed schema. Examples: Oracle, MySQL, PostgreSQL, MSSQL, etc. 

2. SQL has a fixed database schema that uses a set of rules that govern the integrity and consistency of data in relational and tabular form. 

3. SQL is a structured query language, as the name implies. Although there are many different dialects in SQL, they all share the same grammar and syntax.  

4. SQL databases are known to be vertically scalable. It adds more power to the underlying cluster or server for CPU, memory, and storage processing.  

### No SQL: 

1. It is a scalable and easy-to-use non-relational database management system which does not require a fixed schema. Examples: MongoDB, HBase, Cassandra, Redis, CouchBase, etc. 

2. NoSQL has a dynamic database schema that uses column-oriented, document-based, graph databases and key-value pairs.  

3. The dynamic nature of NoSQL databases allows for the representation of varying structures, as it places less emphasis on preparation and gives freedom in creating new fields with varying syntax and methods across databases.  

4. NoSQL databases are horizontally scalable, implying that NoSQL adds additional nodes or servers to share some load.  

## Q10. What is normalization? 

Normalization is the process of organizing a relational database's structure to reduce data redundancy, improve data integrity, and optimize its performance. The primary goal of normalization is to eliminate anomalies in the data and create a better database design by dividing large tables into smaller, related ones and defining relationships between them. 

## Q11. What is My SQL Clustering? 

MySQL clustering, also known as MySQL Cluster or MySQL NDB Cluster, is a high-availability, scalable, and distributed database architecture that ensures fault tolerance and automatic data partitioning across multiple nodes. 

## My SQL Data Types

### String Data Type

1. char () = 0 to 255				 

2. varchar () = 0 to 65,535			

3. binary () = 0 to 255				

4. varbinary () = 0 to 65,535			

5. tinytext () = 255 character			

6. text () = 65,535 bytes				

7. mediumtext () = 16,777,215 character	

8. longtext = 4,294,967,295 character

9. tinyblob = 255 bytes

10. blob () = 65,535 bytes

11. mediumblob () = 16,777,215 bytes

12. longblob () = 4,294,967,295 bytes

13. enum (v1, v2, …) = list up to 65,535 values

14. set (v1, v2, ….) = list up to 64 values

### Numeric Data Type

1. bit () = 1 to 64						

2. tinyint () = -128 to 127					

3. int () = -2,147,483,648 to 2,147,483,647		

4. integer () = 2,147,483,648 to 2,147,483,647	

5. smallint () = -32,768 to 32,767			

6. mediumint () = -83,88,608 to 83,88,607		

7. bigint () = -922,337,203,685,447,758,808 to 922,337,203,685,447,758,807

8. bool = 0 / 1

9. boolean = 0 / 1

10. Float (p) = 255.568

11. double (size, d) = 255.568

12. decimal (size, d) = size = 60, d = 30

13. dec (size, d) = size = 60, d = 30 

## Date & Time Data Type

1. date = 1000-01-01 to 9999-12-31 = (year-month-date) 

2. datetime (fsp) = year-month-date hour: minute: second 

3. timestamp (fsp) = year-month-date hour: minute: second 

4. time (fsp) = hour: minute: second 

5. year = four-digit format -> 1901 




