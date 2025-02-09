# Overview of Database Types
  
**Overview:** This guide covers 9 popular database types (*note: DB solutions can cover multiple categories, and the following is not an exhaustive list of database solutions and how many categories they overlap in*):

#### Table of Contents:

1. [Popular Database Types (with examples)](#popular-db)
2. [Database Use Cases](#use-cases)
3. [Scaling Features](#scaling)
  
<hr />
  
## 1. <a name="popular-db">Popular Database Types (with examples)</a>
  
* **Columnar Databases**
    - Amazon Redshift
    - Apache Cassandra
    - Apache HBase
    - ClickHouse
    - Google Bigtable
* **Document-Based Databases**
    - Amazon DocumentDB
    - CouchDB
    - MongoDB
    - RavenDB
    - RethinkDB
* **Graph-Based Databases**
    - Amazon Neptune
    - ArangoDB
    - Azure Cosmos DB
    - Neo4j
    - OrientDB
* **In-Memory Databases**
    - Memcached
    - Microsoft SQL Server In-Memory (OLTP)
    - Redis
    - SAP HANA
    - VoltDB
* **NoSQL Databases**
    - Apache Cassandra
    - Apache HBase
    - Couchbase
    - MongoDB
    - Redis
* **Object-Oriented Databases**
    - db4o
    - GemStone/S
    - ObjectDB
    - Versant Object Database
    - ZODB
* **Relational Databases**
    - CockroachDB
    - Microsoft SQL Server
    - MySQL
    - Oracle (various products)
    - PostgreSQL
    - SQLite
* **Time-Oriented Databases**
    - Druid
    - InfluxDB
    - OpenTSDB
    - Prometheus
    - TimescaleDB
* **Vector-Based Databases**
    - Chroma
    - Milvus
    - Pinecone
    - Qdrant
    - Weaviate
  
<hr />

## 2. <a name="use-cases">Database Use Cases</a>
  
Before diving into specific use cases for each type of database, several factors should be considered. These include: cost of operations (can the organization cover it, and is there a more efficacious alternative?), employee/team expertise (will it take significant training to implement the database solution?), whether it makes sense to host services in-house or via a cloud provider, whether scalability is a significant concern (such as it is for streaming services and some embedded/IoT environments), and if one's organization is prepared to back up and recover data, or install and maintain backup/recovery solutions corresponding to the selected database solution.
  
*Use cases for these nine database types include...*
  
| Database Type | Use Cases |
| ------- | ------- |
| **Columnar** | Business intelligence (BI), data warehousing, significant analytics and enterprise-level reporting needs. |
| **Document Based** | Content management, JSON and JSON-like data, fast development deadlines, need for flexibile schematics. |
| **Graph Based** | Social bookmarking, networking, and recommendation-based sites, interconnected data needs, pattern recognition. |
| **In Memory** | Need for instant/real-time performance and processing, data caching, and temporary storage of data. | 
| **NoSQL** | Quick response times/low latency, instant/real-time analytics, constantly-evolving data, server scalability needs. |
| **Object Oriented** | Integration with object-oriented languages (e.g., Java), hierarchy-based data objects, long-term object storage/persistence. |
| **Relational** | ACID compliance (important for large enterprises and essential services), data integrity, sophisticated joins/transactions of multi-table data, structured data. |
| **Time Oriented** | Time-series analytics, monitoring and metrics, sensor-related and IoT/embedded system data, data sequencing/patterns. |
| **Vector Based** | Quick retrieval, machine learning (including complex tasks), similarity searching. |

<hr />  

## 3. <a name="scaling">Scaling Features</a>
  
Four of the unique ways that databases scale (and can handle increasing traffic/data requests) include...
    
| Feature | Explanation |
| ------ | ------ |
| **Indexing** | This is the use of 'pointers', in which keys in memory (indexes, or indices) are mapped to rows/records in a table. |
| **Caching** | By searching for data in a memory cache, performance of reads can be improved (no need to request data from a database, preserving time and memory). |
| **Sharding** | This splits rows/records and columns/fields across multiple servers/devices, potentially providing load balancing. |
| **Replications** | This also provides load balancing by replicating data (for reading purposes) across multiple servers/devices. Write responsibilities can still be allocated to one database (the 'primary' database) to preserve data integrity. |
  
TODO: Add overviews for each example in Section 1.
