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

## SIMILARITIES BETWEEN CASSANDRA AND MONGODB

- both are NoSQL Databases
- they do not replace 


1.  Expressive Object Model
MongoDB supports a rich and expressive object model. Objects can have properties and objects can be nested in one another (for multiple levels). This model is very “object-oriented” and can easily represent any object structure in your domain. You can also index the property of any object at any level of the hierarchy – this is strikingly powerful! Cassandra, on the other hand, offers a fairly traditional table structure with rows and columns. Data is more structured and each column has a specific type which can be specified during creation.

Verdict: If your problem domain needs a rich data model, then MongoDB hosting is a better fit for you.
 

2.  Secondary Indexes
Secondary indexes are a first-class construct in MongoDB. This makes it easy to index any property of an object stored in MongoDB even if it is nested. This makes it really easy to query based on these secondary indexes. Cassandra has only cursory support for secondary indexes. Secondary indexes are also limited to single columns and equality comparisons. If you are mostly going to be querying by the primary key then Cassandra will work well for you.

Verdict:  If your application needs secondary indexes and needs flexibility in the query model then MongoDB is a better fit for you.
 

3.  High Availability
MongoDB supports a “single master” model. This means you have a master node and a number of slave nodes. In case the master goes down, one of the slaves is elected as master. This process happens automatically but it takes time, usually 10-40 seconds. During this time of new leader election, your replica set is down and cannot take writes. This works for most applications but ultimately depends on your needs. Cassandra supports a “multiple master” model. The loss of a single node does not affect the ability of the cluster to take writes – so you can achieve 100% uptime for writes.

Verdict: If you need 100% uptime Cassandra is a better fit for you.
 

4.  Write Scalability
MongoDB with its “single master” model can take writes only on the primary. The secondary servers can only be used for reads. So essentially if you have three node replica set, only the master is taking writes and the other two nodes are only used for reads. This greatly limits write scalability. You can deploy multiple shards but essentially only 1/3 of your data nodes can take writes. Cassandra with its “multiple master” model can take writes on any server. Essentially your write scalability is limited by the number of servers you have in the cluster. The more servers you have in the cluster, the better it will scale.

Verdict: If write scalability is your thing, Cassandra is a better fit for you.
 

5.  Query Language Support
Cassandra supports the CQL query language which is very similar to SQL. If you already have a team of data analysts they will be able to port over a majority of their SQL skills which is very important to large organizations. However CQL is not full blown ANSI SQL – It has several limitations (No join support, no OR clauses) etc. MongoDB at this point has no support for a query language. The queries are structured as JSON fragments.

Verdict: If you need query language support, Cassandra is the better fit for you.
 

6.  Performance Benchmarks
Let’s talk performance.  At this point, you are probably expecting a performance benchmark comparison of the databases.  I have deliberately not included performance benchmarks in the comparison. In any comparison, we have to make sure we are making an apples-to-apples comparison.

1.  Database model - The database model/schema of the application being tested makes a big difference. Some schemas are well suited for MongoDB and some are well suited for Cassandra. So when comparing databases it is important to use a model that works reasonably well for both databases.
2.  Load characteristics – The characteristics of the benchmark load are very important. E.g. In write-heavy benchmarks, I would expect Cassandra to smoke MongoDB. However, in read-heavy benchmarks, MongoDB and Cassandra should be similar in performance.
3.  Consistency requirements  - This is a tricky one. You need to make sure that the read/write consistency requirements specified are identical in both databases and not biased towards one participant.  Very often in a number of the ‘Marketing’ benchmarks, the knobs are tuned to disadvantage the other side. So, pay close attention to the consistency settings.

One last thing to keep in mind is that the benchmark load may or may not reflect the performance of your application. So in order for benchmarks to be useful, it is very important to find a benchmark load that reflects the performance characteristics of your application. Here are some benchmarks you might want to look at:
- NoSQL Performance Benchmarks
- Cassandra vs. MongoDB vs. Couchbase vs. HBase

7.  Ease of Use
If you had asked this question a couple of years ago MongoDB would be the hands-down winner. It’s a fairly simple task to get MongoDB up and running. In the last couple of years, however, Cassandra has made great strides in this aspect of the product. With the adoption of CQL as the primary interface for Cassandra, it has taken this a step further – they have made it very simple for legions of SQL programmers to use Cassandra very easily.

Verdict: Both are fairly easy to use and ramp up.
 

8.  Native Aggregation
MongoDB has a built-in Aggregation framework to run an ETL pipeline to transform the data stored in the database. This is great for small to medium jobs but as your data processing needs become more complicated the aggregation framework becomes difficult to debug. Cassandra does not have a built-in aggregation framework. External tools like Hadoop, Spark are used for this.

9.  Schema-less Models
In MongoDB, you can choose to not enforce any schema on your documents. While this was the default in prior versions in the newer version you have the option to enforce a schema for your documents.  Each document in MongoDB can be a different structure and it is up to your application to interpret the data. While this is not relevant to most applications, in some cases the extra flexibility is important. Cassandra in the newer versions (with CQL as the default language) provides static typing. You need to define the type of very column upfront.



|| MongoDB | Cassandra |
| ------ | ------ | ------ |
|Expresive Object Model | MongoDB supports a rich and expressive object model. Objects can have properties and objects can be nested in one another (for multiple levels). This model is very “object-oriented” and can easily represent any object structure in your domain. You can also index the property of any object at any level of the hierarchy – this is strikingly powerful!  | Cassandra, on the other hand, offers a fairly traditional table structure with rows and columns. Data is more structured and each column has a specific type which can be specified during creation.|
|Secondary Indexes| Secondary indexes are a first-class construct in MongoDB. This makes it easy to index any property of an object stored in MongoDB even if it is nested. This makes it really easy to query based on these secondary indexes.  | Cassandra has only cursory support for secondary indexes. Secondary indexes are also limited to single columns and equality comparisons. If you are mostly going to be querying by the primary key then Cassandra will work well for you. |
|High Availability| MongoDB supports a “single master” model. This means you have a master node and a number of slave nodes. In case the master goes down, one of the slaves is elected as master. This process happens automatically but it takes time, usually 10-40 seconds. During this time of new leader election, your replica set is down and cannot take writes. This works for most applications but ultimately depends on your needs.  | Cassandra supports a “multiple master” model. The loss of a single node does not affect the ability of the cluster to take writes – so you can achieve 100% uptime for writes.|




In computer programming, create, read, update, and delete[1] (CRUD) are the four basic functions of persistent storage.[2] Alternate words are sometimes used when defining the four basic functions of CRUD, such as retrieve instead of read, modify instead of update, or destroy instead of delete. CRUD is also sometimes used to describe user interface conventions that facilitate viewing, searching, and changing information; often using computer-based forms and reports. 