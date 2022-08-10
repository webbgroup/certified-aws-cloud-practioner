# Databases

* Database
* Tables
* Row
* Fields/Columns

- MSSQL
- Oracle
- MySQL
- PostGreSQL
- Amazon Aurora (Proprietary)
- MariaDB

RDS
* Multiple Availability Zones - For Disaster Recovery
* Read Replicas - For Performance

So if you have DB1 in AZ1, connection string will failover to AZ2

5 Copies of your live Database

# Non Relational Databases
* Collection = Table
* Document = Row
* Key Value Pairs = Fields

```
id_
firstname
surname
Age
address: [
	street:
	suburb
]
```

* The columns in the table can vary
* This will not affect other rows in the database

# DynamoDB  - Amazons NonRelational DB

OLTP - Standard queries - CRUD.

OLAP - Summing. Analytics away from Processing. Business Tools Very large complex Tool sets.

Data Warehousing databases use different type of architecture both.


# RedShift - OLAP built for analysis

Amazon's Data Warehousing is called RedShift.

# ElastiCache

1. Web-service and makes it easy to deploy operate and scale in memory cache.
2. Caches the most common queries, and those will be stored in Elasticashe.

- Memcached
- Redis
