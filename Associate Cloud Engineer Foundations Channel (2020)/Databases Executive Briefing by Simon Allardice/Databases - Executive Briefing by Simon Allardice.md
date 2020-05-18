# VIDEO: DATABASES EXECUTIVE BRIEFING 
## By Simon Allardice

My notes from the video and the hive.
* Link: https://app.pluralsight.com/channels/player?courseId=e4d99c97-d616-40c8-949a-bcc8f92dcdd7&channelId=d441e420-64fb-45b7-bcda-9b738f9a08e3
* Link: https://the-hive.bbd.co.za/course/db

## The Problem Databases solve:

Databases solve the problem of having data:

* that will grow and change over time 
* that must be shared, fast, searchable, reliable
* is interdependent
* that must be consistent and protected and secure

These problems are solved by using a DBMS - Database Management System
(The software used to create, define and manage databases.)

# Relational Databases
## What is a Relational Database?

A Highly structured data file that allows data input, organisation and retrieval. It uses tables to store, sort and filter data. Important key features are: 

* organized around records
* data points are columns in a table
* relationships are enforced with constraints
* indexing data brings hi-speed access
* SQL is used to get data in and out of the db
* triggers, views, stored procs & materialized views may also be supported

## Constraints in Relational Databases

Constraints can be defined as rules that data must adhere to before it can inserted into a table on the database. Common examples of constraints:

* Primary key constraints – Responsible for enforcing entity integrity for a specific column
* Foreign key constraints – Responsible for enforcing referential integrity of a record
* Unique constraints – Responsible for preventing the duplication of data
* Check constraints – Responsible for specific value checking, i.e. only certain values are allowed
* Default Values – Responsible for providing a value should one not be available, i.e. if there was no value specified for a column, it ensures that a default value is inserted. E.g. Current Date.

## What is Referential Integrity?

Referential Integrity is a relational database concept. In the words of Simon Allardice it is "making sure data remains valid and consistent across related tables". In other words,any foreign key field must agree with the primary key that is referenced by the foreign key.Thus, any primary key field changes must be applied to all foreign keys, or not at all. The same restriction applies to foreign keys. Referential integrity is how relational databases ensure the prevention of orphaned data. 

# Database Development

Data modeling is often the first step in database development and object-oriented programming. Data modeling involves a progression from conceptual model to logical model to physical schema. Data Modelling forms part of the development life cycle. It is important to understand the data before modeling a database. 

# Transactions

A database transaction is similar to a real life transaction. In essence, its the idea of giving something and getting something back in return. 

A formal definition of a transaction; a sequence of operations performed as a single unit logical unit of work. A transaction has four key properties that is a abbreviated as ACID.

A = Atomic => all the work in the transaction is treated as a single unit. Either it is all performed or none of it is.

C = Consistent => a completed transaction leaves the database in a consistent internal state. If the data was valid before the transaction it will be valid after. 

I = Isolated => the transaction sees the database in a consistent state. This transaction operates on a consistent view of the data. If two transactions try to update the same table, one will go first and then the other will follow.

D = Durability => the results of the transaction are permanently stored in the system. What is done stays done. 

ACID is the 4 key factors to consider when determining the success of a transaction. 

Although Relational Databases can be hugely beneficial, there can a few impacting drawbacks in the Agile world we live in today with its lack of flexibilty. 