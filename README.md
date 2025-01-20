**Concepts about Database require for Backend Development:**

![image](https://github.com/codebyalisher/Database--All-Concepts/assets/62823194/44a91914-51c0-4fca-839b-ee9d29598e0b)
✒️

**What is a database?** In simple and easy words ,The Physical storage of data on device.

**How is data related?** To sustain the real world record for various purposes ,data is necessary.

**Alternative types of databases:** Object database ,Graph, JSON and document. These can be Relational and non relational Databases.

**What is the RDBMS:** It is a system that is used to control and manage the different operations on databases.

**Architecture of the RDBMS(Relational Data Base Management System) :** There are 3 levels

**1-External Level:** It consists of views/results of data to client.

**2-Conceptual Level:** this level defined the structural/logical storage of data.

**3-Internal Level:** It is the physical storage of data in database on device.

**What is the OODB (Object Oriented Data Base):** it is a system that is used to manage the complex structure data.

**Roles: There are Three roles;**

**1-Database Programmer:** defined how to store the objects ,state and behaviours.

**2-Database Administrator:** Grant or revoke the access of data from database.

**3-Client-User:** The person who retrieve the data from the database which is relevant to his request.

**Architectural Layers:**

**Interaction layer**(through which user/client connect with the application).

**Application layer:** This is the layer which actually run the app.

**Administrative layer:** Where the Roles and task and permissions are managed.

**Security layer:** Where authentication mostly happened.

**Virtual layer:** Here virtually things are handled.

**Paging layer:** The layer that connects with database to retrieve or store the data and to perform the other operations.

**What is Structured Query Language?** The language that is used to perform the operations on database is called structured query language.

**Types of SQL Languages**: **DDL(Data Definition Language)** this is used to create the database and ,truncate the database ,to create the tables and to delete the tables from the database.

**DML(Data Manipulation Language)** This type of language is used to read the data, update, delete , and creation of data in the tables.

**DCL(Data Control Language)** this type of language is used to do he tasks like security, administrative level and granting and revoking the access of data from the database.

**TCL(Transaction Control Language)** This language Is used to generate the transaction/reports from the database/data .It is also administrative level.

**Advantages of SQL:** Easy to maintain the real world data using this language in database.

**SQL syntax introduction:** The statement which is written using query is called syntex.

**Fields:** Value or item is hold/stored.

**Records/row:** Collection of fields (attributes or columns).

**Files:** Collection of records is called file (a file can be Database ,tables or a table) .

**What are tables in databases?** Table is a object or entity of a database.it gives the structure to store the data.

**Types of keys in a database table:** **Primary key** is used to make the field specific for the entity.

**Foreign key:** is used to refers or to create the connection between the tables. I .e create table tblename(cn,dtype ,primary key(cn) ; foreign key(cn) reference childtablename(cn))

**Numeric data types:** Int,Decimal

**String data types:** string

Default values:

**CREATE and DROP database:** Create dbname ,DROP dbname;

**CREATE TABLE statement:** create table tablename;

**ALTER TABLE statement:** alter table tablename

**INSERT statement:** insert tablename (cn,cn) values(v,v)

**SELECT statement:** select \* from tablename

**INSERT INTO SELECT statement:** insert into tablename(cn,cn) values(v1,v2)

**Updating data:** alter table tablename where cn=value, set cn=newvalue

**Deleting data:** alter table tablename where cn=value,

Create, Read, Update and Delete (CRUD) Operations

✒️

**SQL Arithmetic Operators: +,-,/,\***

Operators in use:

**SQL Comparison operators:** (=.\<,\>,=\>)

**ORDER BY clause:** to arrange/sort the values/result in the specific order either in ascending or descending of the spcified column i.e.alphabetically or in numbering of that clmn.

** Group By clause:** to get the result on the behalf of repeated/same values for the specified columns .used for aggregate funcions

**WHERE clause:** To perform the queries on the condition base.

**SELECT DISTINCT clause:** distinct shows the once of duplicate values

**Aggregate Functions:** min(),max(),sum(),avg(),

**Like:** select\* from tablename where cn like%a,a%,-a%,a-%,[a-z,\*,\#,%]

**Between/In:** select \* from tablename where cn btween value AND value. IN is the shorthand of the OR operator.

**Having:** it is used when where cant be used with aggerigate functions i.e. select\* from tablename having count(cn)\>5 order by cn asc/desc

**JOINS(INNER,LEFT,RIGHT,FULL JOIN):** select cn,cn from table inner join tablename on cn=cn,joins mean to get result on the matching of the values with respect to the specified tables 

**CASE:** select cn,cn case when cn\>30 then ‘message’ when cn\<20 then ‘message’ else ‘message’ end

**STORED PROCEEDURE:** To write the query again and again ,write once and call it again and again.

Create procedure procedurename as select\* from tablename go; exec procedure name

✒️

**Database schema:** The code that we write for the creation of database is called database schema.

**Schema in use:** through this code database operations are performed on the actual physical stored data in the database.

**Types of database schema:** relational in It tables ,tables are connect with each other by a relationship. Non-relational In which data is stored in a file .

**Table relationships:**

**One -to-one:** in this type of relationship one attribute of one table is connected with the other attribute of the other table.

**One-to-many:** here one attribute of one table is connected to many attributes of the other tables.

**Many-to-many:** in this many attributes of the tables are connected with the others tables attributes.

**Many-to-one:** here many attributes of the tables are connected to the one attribute of the other table.

**Primary key:** It is used to make the entity specific by selecting the field.

**Foreign key:** It is used to make the connection between tables

Finding entitites:

**What is database normalization?** Normalization is a process to make the data redundancy free or to avoid the ambiguity in the data.

**Anomaly:** It occurs on the following :

**Insertion Anomaly:** It occurs when items/attributes are inserted into relation database without the existence of other attributes.

**Deletion Anomaly**: It occurs when deleting the one part of the data and it deletes the other necessary information from database.

**Updation anomaly:** it occurs when same items with same values repeated without linking each other.

**First normal form 1NF:** it is done when a attribute/column contain two or more values and those values are separated by making a new row but with the same key.

**Second normal form 2NF**: table first it should in 1NF form. Then converts the table into two parts, in one table those values will be kept with the same primary key in which all those attributes have duplicates values, and in second table rest all the values of all the others attributes will be kept with the same primary key.

**Third normal form 3NF**.In this first table should be in the 2NF form. In it table is also normalized into two parts but on the behalf of two strong dependent attributes, mean one table will contain these two strong dependent attributes and the other table will contain the rest attributes but one attribute from these two strong dependent attributes will also be in the second table ,so that these two tables will make connection with each other .

**Fourth Normal form 4NF**: in this table should in the 3NF form ,the difference is that in this form the process of 3NF form will be repeated for every strong dependent attribute.
