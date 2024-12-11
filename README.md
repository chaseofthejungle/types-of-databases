# Overview of Database Types
This guide covers 9 popular database types (*note: DB solutions can cover multiple categories, and the following is not an exhaustive list of database solutions and how many categories they overlap in*):
  
* Columnar Databases
  + *Examples Include:* Amazon Redshift, Apache Cassandra, Apache HBase, ClickHouse, Google Bigtable.
* Document-Based Databases
  + *Examples Include:* Amazon DocumentDB, CouchDB, MongoDB, RavenDB, RethinkDB.
* Graph-Based Databases
  + *Examples Include:* Amazon Neptune, ArangoDB, Azure Cosmos DB, Neo4j, OrientDB.
* In-Memory Databases
  + *Examples Include:* Memcached, Microsoft SQL Server In-Memory (OLTP), Redis, SAP HANA, VoltDB.
* NoSQL Databases
  + *Examples Include:* Apache Cassandra, Apache HBase, Couchbase, MongoDB, Redis.
* Object-Oriented Databases
  + *Examples Include:* db4o, GemStone/S, ObjectDB, Versant Object Database, ZODB.
* Relational Databases
  + *Examples Include:* CockroachDB, Microsoft SQL Server, MySQL, Oracle (various products), PostgreSQL, SQLite.
* Time-Oriented Databases
  + *Examples Include:* Druid, InfluxDB, OpenTSDB, Prometheus, TimescaleDB.
* Vector-Based Databases
  + *Examples Include:* Chroma, Milvus, Pinecone, Qdrant, Weaviate.
<br />
  
Before diving into specific use cases for each type of database, several factors should be considered. These include: cost of operations (can the organization cover it, and is there a more efficacious alternative?), employee/team expertise (will it take significant training to implement the database solution?), whether it makes sense to host services in-house or via a cloud provider, whether scalability is a significant concern (such as it is for streaming services and some embedded/IoT environments), and if one's organization is prepared to back up and recover data, or install and maintain backup/recovery solutions corresponding to the selected database solution.
  
*Use cases for these nine database types include...*
  
| Database Type | Use Cases |
| ------- | ------- |
| `Columnar` | Business intelligence (BI), data warehousing, significant analytics and enterprise-level reporting needs. |
| `Document-Based` | Content management, JSON and JSON-like data, fast development deadlines, need for flexibile schematics. |
| `Graph-Based` | Social bookmarking, networking, and recommendation-based sites, interconnected data needs, pattern recognition. |
| `In-Memory` | Need for instant/real-time performance and processing, data caching, and temporary storage of data. | 
| `NoSQL` | Quick response times/low latency, instant/real-time analytics, constantly-evolving data, server scalability needs. |
| `Object-Oriented` | Integration with object-oriented languages (e.g., Java), hierarchy-based data objects, long-term object storage/persistence. |
| `Relational` | ACID compliance (important for large enterprises and essential services), data integrity, sophisticated joins/transactions of multi-table data, structured data. |
| `Time-Oriented` | Time-series analytics, monitoring and metrics, sensor-related and IoT/embedded system data, data sequencing/patterns. |
| `Vector-Based` | Quick retrieval, machine learning (including complex tasks), similarity searching. |
