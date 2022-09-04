## Mongo and Mongoose

**Reading**

[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

**Fill in the chart below with five differences between SQL and NoSQL databases:**


| SQL  | NoSQL |
| ------------- | ------------- |
| primarily called as Relational Databases (RDBMS).  | primarily called as non-relational or distributed database.  |
| table based databases, represent data in form of tables which consists of n number of rows of data  | document based, key-value pairs, graph databases or wide-column stores.  |
| predefined schema  | dynamic schema for unstructured data.  |
| vertically scalable, by increasing the horse-power of the hardware.   | horizontally scalable, by increasing the databases servers in the pool of resources to reduce the load.  |
| uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful.  | (Unstructured Query Language). The syntax of using UnQL varies from database to database.  |
| examples: MySql, Oracle, Sqlite, Postgres and MS-SQL.  | examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb  |
| good fit for the complex query intensive environment  | don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.  |
| SQL are not best fit for hierarchical data storage.   | NoSQL fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data, highly preferred for large data set. |
| vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server.  | horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.  |
| best fit for heavy duty transactional type applications, as it is more stable and promises the atomicity as well as integrity of the data. | While you can use NoSQL for transactions purpose, it is still not comparable and sable enough in high load and for complex transactional applications.  |
| For support: Excellent support are available for all SQL database from their vendors. There are also lot of independent consultations who can help you with SQL database for a very large scale deployments.   | For some NoSQL database you still have to rely on community support, and only limited outside experts are available for you to setup and deploy your large scale NoSQL deployments.  |
| properties: SQL databases emphasizes on ACID properties ( Atomicity, Consistency, Isolation and Durability)  | NoSQL database follows the Brewers CAP theorem ( Consistency, Availability and Partition tolerance )  |
| DB types: On a high-level, we can classify SQL databases as either open-source or close-sourced from commercial vendors.  | can be classified on the basis of way of storing data as graph databases, key-value store databases, document store databases, column store database and XML databases.  |


**What kind of data is a good fit for an SQL database?**
SQL databases are best fit for heavy duty transactional type applications.

**Give a real world example.**

**What kind of data is a good fit a NoSQL database?**
kind contains key-pair value, like object

**Give a real world example.**

**Which type of database is best for hierarchical data storage?**
SQL is a better

**Which type of database is best for scalability?**
NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.


**Videos**
[SQL vs NoSQL or MySQL vs MongoDB](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y) 

**What does SQL stand for?**
Structured Query Language.

**What is a relational database?**
A relational database (RDBMS) is a type of database that stores and provides access to data points that are related to one another.

**What type of structure does a relational database work with?**
 logical data structures—the data tables, views, and indexes—are separate from the physical storage structures.

**What is a 'schema'?**
A database schema defines how data is organized within a relational database; this is inclusive of logical constraints such as, table names, fields, data types, and the relationships between these entities.

**What is a NoSQL database?**
"not only SQL") are non-tabular databases and store data differently than relational tables. NoSQL databases come in a variety of types based on their data model. The main types are document, key-value, wide-column, and graph. They provide flexible schemas and scale easily with large amounts of data and high user loads.

**How does it work?**
NoSQL databases store data in documents rather than relational tables.

**What is inside of a Mongo database?**
MongoDB stores data records as documents (specifically BSON documents) which are gathered together in collections.

**Which is more flexible - SQL or MongoDB? and why.**
there are some limitations of SQL Databases that have been observed over the years which are overcome with NoSQL Database options such as MongoDB. MongoDB offers faster query processing but with an increased load and system requirements.

**What is the disadvantage of a NoSQL database?**
NoSQL databases don't have the reliability functions which Relational Databases have (basically don't support ACID).



