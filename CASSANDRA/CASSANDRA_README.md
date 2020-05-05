# CASSANDRA

## TELL ME ABOUT CASSANDRA 

* Cassandra, or more specifically [Apache Cassandra](https://cassandra.apache.org), is an open-source distributed NoSQL database.  Cassandra delivers outstanding performance due to its distributed node design.  
* This design leads to a linear increase in both read and write performance as more nodes are added.  
* Another benefit to the design is that each node is identical because data is replicated across all nodes, meaning no single node represents a point of failure.  
* Based on Cassandra’s design, the CAP theorem would indicate that Cassandra focuses on the A and P guarantees – A for Availability and P for Partition tolerance – while sacrificing Consistency.

<< CAP THEOREM DIAGRAM>> 


### WHAT IS NOSQL DATABASE? 

- There are two types of databases, [Relational](https://en.wikipedia.org/wiki/Relational_database) or SQL Database and NoSQL Database. 
- Relational Database provides a mechanism to store and retrieve data through tabular relations. In other words, it consists of relational data. 
- Whereas, NoSQL database consists of non-relational data. This NoSQL database has a few advantages over SQL or Relational Database. They can handle a huge amount of data and support easy replication and also have a simple API. In this different data structures are used as compared to the relational database.

* Cassandra shares some design qualities with popular NoSQL databases such as [Amazon’s DynamoDB](https://aws.amazon.com/dynamodb/) and [Google’s Big Table](https://cloud.google.com/bigtable/). 
* Cassandra is a Column store database like Google’s Big Table.  

[KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)

### WHAT IS APACHE CASSANDRA?

- Apache Cassandra is an example of NoSQL Database. It is a distributed, decentralized and an open-source database or a storage system. It is basically used for managing very large amounts of structured data. There is no single point of failure, providing highly available services.

- However, Cassandra is also similar to Amazon’s DynamoDB in that it uses a key-value system in which the keys point to column families that represent the structure of the stored data.  
- Unlike Big Table and DynamoDB, Cassandra takes a different approach to query its data.  Cassandra employs a query language that shares many similarities to SQL called the Cassandra Query Language.  CQL helps ease the onboarding of developers who are already familiar with SQL with.  Let’s take a look at the CQL syntax.

### WHAT MAKES CASSANDRA AWESOME?

- _Massively Scalable Architecture_: Cassandra has a masterless design where all nodes are at the same level which provides operational simplicity and easy scale out.
- _Masterless Architecture_: Data can be written and read on any node.
- _Linear Scale Performance_: As more nodes are added, the performance of Cassandra increases.
- _No Single point of failure_: Cassandra replicates data on different nodes that ensures no single point of failure.
- _Fault Detection and Recovery_: Failed nodes can easily be restored and recovered.
- _Flexible and Dynamic Data Model_: Supports datatypes with Fast writes and reads.
- _Data Protection_: Data is protected with commit log design and build in security like backup and restore mechanisms.
- _Tunable Data Consistency_: Support for strong data consistency across distributed architecture.
- _Multi Data Center Replication_: Cassandra provides feature to replicate data across multiple data center.
- _Data Compression_: Cassandra can compress up to 80% data without any overhead.
- _Cassandra Query language_: Cassandra provides query language that is similar like SQL language. It makes very easy for relational database developers moving from relational database to Cassandra.

### CASSANDRA VS. MONGODB


|| MongoDB | Cassandra |
| ------ | ------ | ------ |
|Expresive Object Model | MongoDB supports a rich and expressive object model. Objects can have properties and objects can be nested in one another (for multiple levels). This model is very “object-oriented” and can easily represent any object structure in your domain. You can also index the property of any object at any level of the hierarchy – this is strikingly powerful!  | Cassandra, on the other hand, offers a fairly traditional table structure with rows and columns. Data is more structured and each column has a specific type which can be specified during creation.|
|Secondary Indexes| Secondary indexes are a first-class construct in MongoDB. This makes it easy to index any property of an object stored in MongoDB even if it is nested. This makes it really easy to query based on these secondary indexes.  | Cassandra has only cursory support for secondary indexes. Secondary indexes are also limited to single columns and equality comparisons. If you are mostly going to be querying by the primary key then Cassandra will work well for you. |
|High Availability| MongoDB supports a “single master” model. This means you have a master node and a number of slave nodes. In case the master goes down, one of the slaves is elected as master. This process happens automatically but it takes time, usually 10-40 seconds. During this time of new leader election, your replica set is down and cannot take writes. This works for most applications but ultimately depends on your needs.  | Cassandra supports a “multiple master” model. The loss of a single node does not affect the ability of the cluster to take writes – so you can achieve 100% uptime for writes.|




In computer programming, create, read, update, and delete[1] (CRUD) are the four basic functions of persistent storage.[2] Alternate words are sometimes used when defining the four basic functions of CRUD, such as retrieve instead of read, modify instead of update, or destroy instead of delete. CRUD is also sometimes used to describe user interface conventions that facilitate viewing, searching, and changing information; often using computer-based forms and reports. 