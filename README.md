# Overview of Database Types
  
**Overview:** This guide covers 9 popular database types (*note: DB solutions can cover multiple categories, and the following is not an exhaustive list of database solutions and how many categories they overlap in*):

#### Table of Contents:

1. [Popular Database Types (with examples)](#popular-db)
2. [Database Use Cases](#use-cases)
3. [Scaling Features](#scaling)
4. [Supplemental Resources](#supplemental)
  
<hr />
  
## 1. <a name="popular-db">Popular Database Types (with examples)</a>
  
* **Columnar Databases**
    - [Amazon Redshift](https://aws.amazon.com/redshift/): Intended for big data queries and analytics.
    - [Apache Cassandra](https://cassandra.apache.org/_/index.html): Handles massive data volumes with high availability and fault tolerance. Intended for high speed settings (e.g., e-commerce, CMSes, social media).
    - [Apache HBase](https://hbase.apache.org/): Used to handle big data, social media, and IoT apps, with dashboards for real-time analytics.
    - [ClickHouse](https://clickhouse.com/): Popular for online analytical processing in large data settings, with dashboard-accessible insights.
    - [Google Bigtable](https://cloud.google.com/bigtable): Processes financial, marketing, and time-series data.
* **Document-Based Databases**
    - [Amazon DocumentDB](https://aws.amazon.com/documentdb/): Enables quick scaling of memory and computational resources for Amazon's Virtual Private Cloud.
    - [Apache CouchDB](https://couchdb.apache.org/): Can operate database servers via virtual machines and other servers.
    - [MongoDB](https://www.mongodb.com/): Builds highly scalable and available web apps. Utilized by MERN and MEAN Stack Developers.
    - [RavenDB](https://ravendb.net/): Includes a cloud service for handling administrative tasks (e.g., user security, hardware installations/maintenance).
    - [RethinkDB](https://rethinkdb.com/): Useful for tracking real-time changes and applying block/non-block requests.
* **Graph-Based Databases**
    - [Amazon Neptune](https://aws.amazon.com/neptune/): Builds and executes apps that handle connected datasets (e.g., network security, fraud detection, recommendation engine apps).
    - [ArangoDB](https://arangodb.com/): Enables data integration for relationship and activity analysis. A popular solution for fraud monitoring/detection apps.
    - [Azure Cosmos DB](https://azure.microsoft.com/en-us/products/cosmos-db): Builds AI-enabled, web, mobile, and other apps that handle large quantities of data.
    - [Neo4j](https://neo4j.com/): Detects data patterns and provides data persistence and querying for complex relationships.
    - [OrientDB](https://orientdb.org/): Utilized for big data processing while providing scalability and flexibility. A popular solution for social networks, banks, and fraud prevention/detection systems.
* **In-Memory Databases**
    - [Memcached](https://memcached.org/): Supports database load balancing and increases speed/processing efficiency of web apps.
    - [Microsoft Azure (OLTP)](https://learn.microsoft.com/en-us/azure/architecture/data-guide/relational-data/online-transaction-processing): Records real-time interactions and allows the data to be queried for quick decision making.
    - [Redis](https://redis.io/): Can be utilized dynamically (as a cache, database, or message broker).
    - [SAP HANA](https://www.sap.com/products/data-cloud/hana/what-is-sap-hana.html): Utilized for diverse operations (e.g., advanced analytics, custom app development and deployment, managing processes).
    - [Volt Active Data](https://www.voltactivedata.com/): Empowers enterprises with high scalability, without compromising data or data processing.
* **NoSQL Databases**
    - [Actian NoSQL Object Database](https://www.actian.com/databases/nosql/): Provides transactional storage of data via object-oriented programming languages, which serve as data definition languages.
    - [Apache Cassandra](https://cassandra.apache.org/_/index.html):  Handles massive data volumes with high availability and fault tolerance. Intended for high speed settings (e.g., e-commerce, CMSes, social media).
    - [Apache HBase](https://hbase.apache.org/): Used to handle big data, social media, and IoT apps, with dashboards for real-time analytics.
    - [Couchbase](https://www.couchbase.com/): Manages sessions, provides user profiles in real-time, and can store data for offline operations via mobile apps.
    - [MongoDB](https://www.mongodb.com/): Builds highly scalable and available web apps. Utilized by MERN and MEAN Stack Developers.
    - [Redis](https://redis.io/): Can be utilized dynamically (as a cache, database, or message broker).
* **Object-Oriented Databases**
    - [Actian NoSQL Object Database](https://www.actian.com/databases/nosql/): Provides transactional storage of data via object-oriented programming languages, which serve as data definition languages.
    - [Actian db4o (Legacy Technology)](https://dbdb.io/db/db4o): Intended for .NET and Java developers. Discontinued since October 2014.
    - [GemStone/S](https://gemtalksystems.com/products/gs64/): Supports mission-critical apps, integrating the Smalltalk programing language for development, deployment, and management.
    - [ObjectDB](https://www.objectdb.com/): Relies on two Java APIs (JDO and JPA) instead of utilizing a proprietary API and implementing an ORM as an intermediary.
    - [ZODB](https://zodb.org/en/latest/): Provides data persistence and transparency for Python objects.
* **Relational Databases**
    - [CockroachDB](https://www.cockroachlabs.com/): Popular for cloud-based software-as-a-service apps, financial systems, Kubernetes (k8s) services, OLTP, and transactional platform solutions.
    - [Microsoft SQL Server](https://www.microsoft.com/en-us/sql-server): Provides data persistence and data fetching for diverse workloads, including client-based and cloud-based apps.
    - [Oracle MySQL](https://www.mysql.com/): Utilized by content management systems (such as for academic purposes), e-commerce stores, embedded systems, and web apps.
    - [PostgreSQL](https://www.postgresql.org/): A highly portable database solution with an active international support community. Capable of handling diverse workloads and providing high availability even when many concurrent users are present.
    - [SQLite](https://www.sqlite.org/): An embedded database solution, rather than a standalone app. A popular choice for embedded systems, operating systems, smart phones, and web browsers. 
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
  
## 4. <a name="supplemental">Supplemental Resources</a>
  
* *[Data Repositories Overview Guide](https://github.com/chaseofthejungle/data-repositories-overview)*
* *[List of Apache Databases](https://projects.apache.org/projects.html?category#database)*
* *[MongoDB Official Website](https://www.mongodb.com/)*
