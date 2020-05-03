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

### CASSANDRA VS. MONGODB

		 | Plugin | README |
| ------ | ------ | ------ |
| ------ || Dropbox | [plugins/dropbox/README.md][PlDb] |
| ------ || GitHub | [plugins/github/README.md][PlGh] |
| ------ || Google Drive | [plugins/googledrive/README.md][PlGd] |
| ------ || OneDrive | [plugins/onedrive/README.md][PlOd] |
| ------ || Medium | [plugins/medium/README.md][PlMe] |
| ------ || Google Analytics | [plugins/googleanalytics/README.md][PlGa] |




In computer programming, create, read, update, and delete[1] (CRUD) are the four basic functions of persistent storage.[2] Alternate words are sometimes used when defining the four basic functions of CRUD, such as retrieve instead of read, modify instead of update, or destroy instead of delete. CRUD is also sometimes used to describe user interface conventions that facilitate viewing, searching, and changing information; often using computer-based forms and reports. 