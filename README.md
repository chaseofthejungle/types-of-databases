# Overview of Database Types
  
**Overview:** This guide covers 9 popular database types (*note: DB solutions can cover multiple categories, and the following is not an exhaustive list of database solutions and how many categories they overlap in*):

#### Table of Contents:

1. [Popular Database Types (with examples)](#popular-db)
2. [Database Use Cases](#use-cases)
3. [Scaling Features](#scaling)
4. [Supplemental Resource](#supplemental)
  
<hr />
  
## 1. <a name="popular-db">Popular Database Types (with examples)</a>
  
* **Columnar Databases**
    - [Amazon Redshift](https://aws.amazon.com/redshift/)
    - [Apache Cassandra](https://cassandra.apache.org/_/index.html)
    - [Apache HBase](https://hbase.apache.org/)
    - [ClickHouse](https://clickhouse.com/)
    - [Google Bigtable](https://cloud.google.com/bigtable)
* **Document-Based Databases**
    - [Amazon DocumentDB](https://aws.amazon.com/documentdb/)
    - [Apache CouchDB](https://couchdb.apache.org/)
    - [MongoDB](https://www.mongodb.com/)
    - [RavenDB](https://ravendb.net/)
    - [RethinkDB](https://rethinkdb.com/)
* **Graph-Based Databases**
    - [Amazon Neptune](https://aws.amazon.com/neptune/)
    - [ArangoDB](https://arangodb.com/)
    - [Azure Cosmos DB](https://azure.microsoft.com/en-us/products/cosmos-db)
    - [Neo4j](https://neo4j.com/)
    - [OrientDB](https://orientdb.org/)
* **In-Memory Databases**
    - [Memcached](https://memcached.org/)
    - [Microsoft Azure (OLTP)](https://learn.microsoft.com/en-us/azure/architecture/data-guide/relational-data/online-transaction-processing)
    - [Redis](https://redis.io/)
    - [SAP HANA](https://www.sap.com/products/data-cloud/hana/what-is-sap-hana.html)
    - [Volt Active Data](https://www.voltactivedata.com/)
* **NoSQL Databases**
    - [Actian NoSQL Object Database](https://www.actian.com/databases/nosql/)
    - [Apache Cassandra](https://cassandra.apache.org/_/index.html)
    - [Apache HBase](https://hbase.apache.org/)
    - [Couchbase](https://www.couchbase.com/)
    - [MongoDB](https://www.mongodb.com/)
    - [Redis](https://redis.io/)
* **Object-Oriented Databases**
    - [Actian NoSQL Object Database](https://www.actian.com/databases/nosql/)
    - [db4o (Legacy Technology)](https://dbdb.io/db/db4o)
    - [GemStone/S](https://gemtalksystems.com/products/gs64/)
    - [ObjectDB](https://www.objectdb.com/)
    - [ZODB](https://zodb.org/en/latest/)
* **Relational Databases**
    - [CockroachDB](https://www.cockroachlabs.com/)
    - [Microsoft SQL Server](https://www.microsoft.com/en-us/sql-server)
    - [Oracle MySQL](https://www.mysql.com/)
    - [PostgreSQL](https://www.postgresql.org/)
    - [SQLite](https://www.sqlite.org/)
* **Time-Oriented Databases**
    - [Apache Druid](https://druid.apache.org/)
    - [InfluxDB](https://www.influxdata.com/)
    - [OpenTSDB](https://opentsdb.net/)
    - [Prometheus](https://prometheus.io/)
    - [TimescaleDB](https://www.timescale.com/)
* **Vector-Based Databases**
    - [Chroma](https://www.trychroma.com/)
    - [Milvus](https://milvus.io/)
    - [Pinecone](https://www.pinecone.io/)
    - [Qdrant](https://qdrant.tech/)
    - [Weaviate](https://weaviate.io/)
  
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
  
<hr />
  
## 4. <a name="supplemental">Supplemental Resource</a>
  
[Data Repositories Overview Guide](https://github.com/chaseofthejungle/data-repositories-overview)
