# Awesome Cassandra [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome [Apache Cassandra](http://cassandra.apache.org/) packages and resources. Maintained by Rahul Singh of [Anant](http://anant.us). Feel free contact me if you'd like to collaborate on this and other awesome lists. [Awesome Cassandra](https://github.com/Anant/awesome-cassandra) , [Awesome Solr](https://github.com/Anant/awesome-solr), [Awesome Lucene](https://github.com/Anant/awesome-lucene)

## Contents

- [General](#general) 
<!-- TODO: list out concept subject titles here and link -->
- [Packages](#packages)
  - [Libraries](#interfaces)  Programming Language Specific Libs for Cassandra.
  - [Tools](#tools) Applications / Tools that work with Cassandra.
  - [Projects](#projects) Other projects that use Cassandra.
  
- [Resources](#resources) 
  - [Documentation](#documentation) Official / unofficial documentation. 
  - [Books](#books) Popular books about Cassandra.
  - [Tutorials](#tutorials) Step by step tutorials on Cassandra.
  - [Web Sites](#web-sites) Sites ( not blogs ) on Cassandra.
  - [Blogs](#blogs) from Cassandra experts.
  - [Videos](#videos) Videos on Cassandra.
  - [Slides](#slides) Slides on Cassandra / related technologies.

## General

### Cassandra 
- [Apache Cassandra](http://cassandra.apache.org/) Manage massive amounts of data, fast, without losing sleep.

### Cassandra History
- [IDG: 10 Years of Apache Cassandra](https://www.idgconnect.com/abstract/30973/apache-cassandra)
- [ZDNet: Apache Cassandra Turns 10](https://www.zdnet.com/article/apache-cassandra-turns-10/)

### Cassandra Use Cases 
- [Datastax Academy: Brief Introduction to Apache Cassandra](https://academy.datastax.com/resources/brief-introduction-apache-cassandra)
- [Kaa application based on Raspberry Pi and DHT11 sensor](https://github.com/pyroalf/kaa-cassandra-sample) - Cassandra IoT usecase with Raspberry Pi and a DHT11 Sensor

### Cassandra Distributions
- [Datastax](https://www.datastax.com/) - Most widely used commercial distribution of Apache Cassandra, integrated with Apache Spark (for SparkSQL, analytics), Apache Solr (for secondary index), Apache TinkerPop based Graph stored in Cassandra, and OpsCenter.
- [Elassandra](http://www.elassandra.io/): Elassandra = Elasticsearch as a Cassandra secondary index.
- [ScyllaDB](https://github.com/scylladb/scylla)- NoSQL data store using the seastar framework, compatible with Apache Cassandra 
- [YugaByte Database](https://github.com/YugaByte/yugabyte-db) - YugaByteDB is a transactional, high-performance database for building distributed cloud services. It supports Cassandra-compatible and Redis-compatible APIs, with PostgreSQL in Beta.
- [Microsoft Azure Cosmos DB: Apache Cassandra API](https://docs.microsoft.com/en-us/azure/cosmos-db/cassandra-introduction) - Azure Cosmos DB provides the Cassandra API (preview) for applications that are written for Apache Cassandra that need premium capabilities.

### Relational / Other -> Cassandra
- [RDBMS to NoSQL](http://www.datastax.com/relational-database-to-nosql): Your roadmap to understanding whether NoSQL is right for you.
- [MySQL to C*](http://planetcassandra.org/mysql-to-cassandra-migration/): mysql to cassandra migration guide
- [Real-Time Replication from MySQL to Cassandra](https://mcbguru.blog/2014/02/27/real-time-replication-from-mysql-to-cassandra/)

### Using Cassandra

<!-- - TODO:: cassandra installation tutorials in local, docker, cloud (do, aws, azure, gcp)) -->

- [Installing the Cassandra / Spark OSS Stack](https://tobert.github.io/post/2014-07-15-installing-cassandra-spark-stack.html)
- [Install Cassandra and Spark](http://tobert.github.io/post/2014-07-15-installing-cassandra-spark-stack.html): quick user guide for integration with Cassandra and Spark
<!-- - TODO:: compiling cassandra -->
<!-- - TODO:: running cassandra -->
<!-- - TODO:: using cql -->
- [The Cassandra Query Language](http://cassandra.apache.org/doc/latest/cql/)
<!-- - TODO:: using zeppelin with cassandra -->
- [tghe LIMIT Clause in Apache Cassandra might not work as you think](http://thelastpickle.com/blog/2017/03/07/The-limit-clause-in-cassandra-might-not-work-as-you-think.html)
<!-- - TODO:: getting data in / out of cassandra -->
- [Building a Performant API using Go and Cassandra](https://getstream.io/blog/building-a-performant-api-using-go-and-cassandra/)
- [Cassandra Data Copy Tool](https://github.com/wildengineer/cassandra-data-copy-tool)- Java tool to copy data from one cassandra table to another
- [Spring Data Cassandra Examples](https://github.com/jxblum/spring-data-cassandra-examples) - Examples for the Spring Data Cassandra Project.
<!-- - TODO:: using spark with cassandra -->
- [Introduction to Spark & Cassandra](http://rustyrazorblade.com/post/2015/2015-01-02-intro-to-spark-and-cassandra/) 

- [From Cassandra to S3, with Spark](https://objectpartners.com/2016/11/30/from-cassandra-to-s3-with-spark/)
- [Import CSV files with spark](https://github.com/markthebault/importCSVSparkCassandra) - How to import a file from S3 into cassandra using spark

### Cassandra Data Modeling
- [Basic Rules Of Cassandra Data Modeling](http://www.datastax.com/dev/blog/basic-rules-of-cassandra-data-modeling): Picking the right data model is the hardest part of using Cassandra. If you have a relational background, CQL will look familiar, but the way you use it can be very different.
<!-- - TODO:: sql v. cql-->
- [Cassandra Query Language : CQL vs. SQL](https://medium.com/@alexbmeng/cassandra-query-language-cql-vs-sql-7f6ed7706b4c)
- [CQL: This is not the SQL you are Looking For](https://www.slideshare.net/aploetz/cql-this-is-not-the-sql-you-are-loooking-for)
- [A Deep Look at the CQL Where Clause](https://www.datastax.com/dev/blog/a-deep-look-to-the-cql-where-clause)
<!-- - TODO:: query driven methodology -->
<!-- - TODO:: schema designs / examples-->
- [killrvideo-sample-schema](https://github.com/pmcfadin/killrvideo-sample-schema) - Sample Cassandra CQL Schema for a Youtube clone.
- [Spring Data Cassandra Examples](https://github.com/jxblum/spring-data-cassandra-examples/blob/master/src/main/resources/cassandra-example-schema.cql)
<!-- - TODO:: data modeling problems -->
- [Common Problems in Cassandra Data Models](https://blog.anant.us/common-problems-cassandra-data-models/) - Presentation and Article on wide partions, tombstones, and data skew.
- [Casandra Time Series Data Modeling for Massive Scale](http://thelastpickle.com/blog/2017/08/02/time-series-data-modeling-massive-scale.html)

### Cassandra Architecture
<!-- - TODO: - Data Centers and Racks -->
<!-- - TODO: - Gossip and Failure Detection -->
<!-- - TODO: - Snitches -->
<!-- - TODO: - Rings and Tokens -->
<!-- - TODO: - Virtual Nodes -->
<!-- - TODO: - Partitioners -->
<!-- - TODO: - Replication Strategies -->
<!-- - TODO: - Consistency Levels -->
<!-- - TODO: - Queries and Coordinator Nodes -->
<!-- - TODO: - Memtables, SSTables, and Commit Logs -->

- [Introduction To The Apache Cassandra 3.x Storage Engine](http://thelastpickle.com/blog/2016/03/04/introductiont-to-the-apache-cassandra-3-storage-engine.html) - The 3.x storage engine makes it easier for Cassandra to get bytes off disk.
- [Dropping columns in Apache Cassandra 3.0](http://thelastpickle.com/blog/2016/02/18/dropping-columns.html)

<!-- - TODO: - Caching -->
<!-- - TODO: - Hinted Handoff -->

- [Hinted Handoff and GC Grace Demystified](http://thelastpickle.com/blog/2018/03/21/hinted-handoff-gc-grace-demystified.html) - Tuning the balance between GC Grace and Hinted Handoff.
<!-- - TODO: - Lightweight Transactions and Paxos -->
<!-- - TODO: - Tombstones -->
- [Deletes an Tombstones](http://thelastpickle.com/blog/2011/05/15/Deletes-and-Tombstones.html) - Explains how deletes create tombstones in Cassandra and what they are. 
- [About Deletes and Tombstones in Cassandra](http://thelastpickle.com/blog/2016/07/27/about-deletes-and-tombstones.html) - Deleting distributed and replicated data from a system such as Apache Cassandra is far trickier than in a relational database.
- [Null bindings on prepared statements and undesired tombstone creation](http://thelastpickle.com/blog/2016/09/15/Null-bindings-on-prepared-statements-and-undesired-tombstone-creation.html) - Good follow up to the last article on Tombstones.
- [Undetecetable tombstones in Apache Cassandra](http://thelastpickle.com/blog/2018/07/05/undetectable-tombstones-in-apache-cassandra.html) - Indepth analysis of cell and range tombstones. 
- [Common Problems with Cassandra Tombstones](https://opencredo.com/cassandra-tombstones-common-issues/) - "Large Number of Tombstones Causes Latency and Heap Pressure"
<!-- - TODO: - Bloom Filters -->
<!-- - TODO: - Compaction -->
- [Understanding the Nuance of Compaction in Apache Cassandra](http://thelastpickle.com/blog/2017/03/16/compaction-nuance.html) - Overview of how Cassandra manages data on disk.
<!-- - TODO: - Anti-Entropy, Repair, and Merkle Trees -->
<!-- - TODO: - Staged Event-Driven Architecture (SEDA) -->
<!-- - TODO: - Managers and Services -->
<!-- - TODO: - System Keyspaces -->

### Cassandra Monitoring
- [Resources for Monitoring Datastax, Cassandra, Spark, & Solr Performance](https://blog.anant.us/resources-for-monitoring-datastax-cassandra-spark-solr-performance/)
- [How to Monitor Cassandra](https://www.datadoghq.com/blog/how-to-monitor-cassandra-performance-metrics/): A guide to help you monitor Cassandra performance and work metrics regardles of which monitoring tool you choose to use.
- [Cassandra metrics and their use in Grafana](https://medium.com/@mlowicki/cassandra-metrics-and-their-use-in-grafana-1f0dc33f9cca)
- [Monitoring Cassandra with Prometheus](https://www.robustperception.io/monitoring-cassandra-with-prometheus)
- [Monitoring Cassandra With Grafana And Influx DB](https://blog.pythian.com/monitoring-cassandra-grafana-influx-db/)
- [Cassandra Monitoring - Introduction (1/2)](https://softwaremill.com/cassandra-monitoring-part-1/)
- [Cassandra Monitoring - Graphite/InfluxDB & Grafana on Docker (1/2)](https://softwaremill.com/cassandra-monitoring-part-2/)
- [Monitoring Cassandra using Intel Snap and Grafana](http://thelastpickle.com/blog/2017/04/13/monitoring-cassandra-using-intel-snap.html) - This blog post describes how to monitor Apache Cassandra using the Intel Snap open source telemetry framework.

### Cassandra Maintenance
- [Running commands cluster-wide without any management tool](http://thelastpickle.com/blog/2016/03/21/running-commands-cluster-wide.html) - Some tips and tricks to do basic Cluster operations without tools like Chef, Ansible, or Salt.
<!-- - TODO:: Health Check -->
<!-- - TODO:: Basic Maintenance -->
- [Limiting Nodetool Parallel Threads](http://thelastpickle.com/blog/2017/08/14/limiting-nodetool-parallel-threads.html) - Little known tool to do nodetool operations with less resources.
<!-- - TODO:: Adding Nodes -->
- [Bootstrapping Cassandra Nodes](http://thelastpickle.com/blog/2017/05/23/auto-bootstrapping-part1.html) - Indepth article on how to add nodes to a running Cassandra cluster.
<!-- - TODO:: Handling Node Failure -->
- [Node Replacement without Bootstrapping](http://thelastpickle.com/blog/2018/02/21/replace-node-without-bootstrapping.html) - How to avoid the long bootstrapping process.
<!-- - TODO:: Upgrading Cassandra -->
<!-- - TODO:: Backup and Recovery -->
- [Cassandra Backup and Restore - Backup in AWS using EBS Volumes](http://thelastpickle.com/blog/2018/04/03/cassandra-backup-and-restore-aws-ebs.html) - Indepth article about Backup and recovery in AWS.
- [Cassandra backup util](https://github.com/instaclustr/cassandra-backup) - https://github.com/instaclustr/cassandra-backup
<!-- - TODO:: SSTable Utilities -->
- [sstable tools](https://github.com/tolbertam/sstable-tools) - A toolkit for parsing, creating and doing other fun stuff with Cassandra 3.x SSTables.
- [cassandra-sstable-tools](https://github.com/instaclustr/cassandra-sstable-tools) - Tools for working with sstables
<!-- - TODO:: Maintenance Tools 
  - OpsCenter
  - Reaper
  - TableAnalyzer
-->
### Cassandra Performance Tuning
- [Jon Haddad: Cassandra Summit Recap - Diagnosing Problems in Production](http://rustyrazorblade.com/2014/09/cassandra-summit-recap-diagnosing-problems-in-production/)
- [Ryan Svihla's Cassandra 2.0 checklist](https://medium.com/@foundev/my-cassandra-diagnostics-checklist-brain-dump-599a2b95b118)
- [Amy's Cassandra 2.1 tuning guide](https://tobert.github.io/pages/als-cassandra-21-tuning-guide.html)
- [Secret HotSpot option improving GC pauses on large heaps](http://blog.ragozin.info/2012/03/secret-hotspot-option-improving-gc.html)
- [DSE 5.1: Tuning Java Resource](https://docs.datastax.com/en/dse/5.1/dse-admin/datastax_enterprise/operations/opsTuneJVM.html)
- [Analyzing Cassandra Performance with Flame Graphs](http://thelastpickle.com/blog/2018/01/16/cassandra-flame-graphs.html) - Visually examining Cassandra performance visually using Flamegraphs. 
- [Garbage Collection Tuning for Cassandra](http://thelastpickle.com/blog/2018/04/11/gc-tuning.html) - Optimizing garbage collection for better performance.

<!-- - TODO:: Managing Performance -->
- [Cassandra Node Diagnostics Tools](https://github.com/smartcat-labs/cassandra-diagnostics) - Monitoring and audit power kit for Apache Cassandra.
<!-- - TODO:: Caching -->
<!-- - TODO:: Memtables -->
<!-- - TODO:: Commit Logs -->
<!-- - TODO:: SSTables -->
<!-- - TODO:: Hinted Handoff -->
<!-- - TODO:: Compaction -->
- [TWCS part 1 - how does it work and when should you use it?](http://thelastpickle.com/blog/2016/12/08/TWCS-part1.html) - Best suited for time series data that expires, Time Window Compaction Strategy comes with some caveats.
- [Performing User Defined Compactions in Apache Cassandra](http://thelastpickle.com/blog/2016/10/18/user-defined-compaction.html) - This is a process by which we tell Cassandra to create a compaction task for one or more tables explicitly. 
<!-- - TODO:: Concurrency and Threading -->
<!-- - TODO:: Networking and Timeouts -->
<!-- - TODO:: JVM Settings -->
<!-- - TODO:: Using cassandra-stress -->
- [Graphing cassandra-stress](http://thelastpickle.com/blog/2015/10/23/cassandra-stress-and-graphs.html) - Benchmarking schemas and configuration changes using the cassandra-stress tool, before pushing such changes out to production is one of the things every Cassandra developer should know and regularly practice.
- [Modeling real life workloads with cassandra-stress is hard](http://thelastpickle.com/blog/2017/02/08/Modeling-real-life-workloads-with-cassandra-stress.html) - 
<!-- - TODO:: Using Gatling -->
- [Gatling DSE Stress](https://github.com/datastax/gatling-dse-stress)
- [Gatling DSE Plugin for Gatling Load injector](https://github.com/datastax/gatling-dse-plugin) - This project is a plugin for the Gatling load injector. It adds CQL support in Gatling for Datastax Enterprise. It allows for benchmarking Datastax Enterprise features, including DSE Graph Fluent API.
- [Gatling DSE Stress Simulation Catalog](https://github.com/datastax/gatling-dse-simcatalog) - The goal of the repo is to provide a sample of the Gatling DSE Stress Framework's usage. Feel free to submit a pull request with example simulations.

### Cassandra Security
- [Hardening Cassandra Step by Step: Part 1](http://thelastpickle.com/blog/2015/09/30/hardening-cassandra-step-by-step-part-1-server-to-server.html) - Inter-Node Encryption (And a Gentle Intro to Certificates)
<!-- - TODO:: Authentication and Authorization -->
- [LDAP Authenticator for Apache Cassandra](https://github.com/instaclustr/cassandra-ldap) - This is a pluggable authentication implementation for Apache Cassandra, providing a way to authenticate and create users based on a configured LDAP server. 
<!-- - TODO:: Encryption -->
<!-- - TODO:: JMX Security -->
<!-- - TODO:: Disk -->
- [Encrypting EC2 ephemeral volumes with LUKS and AWS KMS](https://www.whaletech.co/2016/04/07/encryption-ephemeral-volumes-with-kms.html) - The example used here is Cassandra data stored on ephemeral disks.
<!-- - TODO:: System -->
<!-- - TODO:: Network -->

### Deploying Cassandra
<!-- - TODO:: Planning a Cluster Deployment -->
<!-- - TODO:: Container Deployment -->
- [Docker Meet Cassandra. Cassandra Meet Docker](http://thelastpickle.com/blog/2018/01/23/docker-meet-cassandra.html) Article reviewing how to setup a complete Cassandra application with monitoring on Docker.
- [Example code from the Docker Meet Cassandra Article](https://github.com/thelastpickle/docker-cassandra-bootstrap)
- [Docker-Cassandra](https://github.com/nicolasff/docker-cassandra): A set of scripts and config files to run a Cassandra cluster from Docker.
- [Cassandra & Zeppelin Notebook on Docker](https://github.com/academyofdata/cassandra-zeppelin): Docker-Compose script for Cassandra + Zeppelin setup.
- [Packer: Cassandra Image](https://github.com/cloudurable/cassandra-image) - Cassandra Image using Packer for Docker and EC2 AMI. Covers managing EC2 Cassandra clusters with Ansible.
- [Cassandra Docker](https://github.com/instaclustr/cassandra-docker) - This is the Instaclustr public docker image for Apache Cassandra. It contains docker images for Cassandra 3.0 and 3.11.1.
- [Cassandra / Elassandra Docker](https://github.com/zegelin/cassandra-docker) - Apache Cassandra and Elassandra docker images.

<!-- - TODO:: Container Orchestration -->
- [Kubernetes Cassandra Operator](https://github.com/instaclustr/cassandra-operator) - The Cassandra operator manages Cassandra clusters deployed to Kubernetes and automates tasks related to operating an Cassandra cluster.
- [Running Cassandra on DC/OS (Mesos)](http://thelastpickle.com/blog/2016/05/07/dcos.html) -  This blog will show how to setup DC/OS in the Amazon cloud, how to install Apache Cassandra on a DC/OS cluster, and finally new ways to interact with and Apache Cassandra after it is installed.
<!-- - TODO:: Cloud Deployment -->
- [How To Setup A Highly Available Multi-AZ Cassandra Cluster On AWS EC2](http://highscalability.com/blog/2016/8/1/how-to-setup-a-highly-available-multi-az-cassandra-cluster-o.html)
<!-- - TODO:: Cloud Automations -->
- [CloudFormation Cassandra AWS](https://github.com/LoyaltyOne/cassandra-aws)- A cassandra cluster for development using Cloud Formation

### Integrating with Cassandra
- [Building a Streaming Data Hub with Elasticsearch, Kafka and Cassandra](http://thenewstack.io/building-streaming-data-hub-elasticsearch-kafka-cassandra/)
- [Docker container for Kafka - Spark streaming - Cassandra](https://github.com/Yannael/kafka-sparkstreaming-cassandra) - This Dockerfile sets up a complete streaming environment for experimenting with Kafka, Spark streaming (PySpark), and Cassandra.
- [sample KafkaSparkCassandra](https://github.com/instaclustr/sample-KafkaSparkCassandra) - Introductory sample scala app using Apache Spark Streaming to accept data from Kafka and write a summary to Cassandra.
- [sample Spark Cassandra with SSL](https://github.com/instaclustr/sample-SparkCassandrawithSSL) - Simple sample job illustrating the use of Spark to execute Apache Spark analytics with Cassandra with SSL connection.



<!-- - TODO:: ESB -->
<!-- - TODO:: Streaming -->
<!-- - TODO:: ETL -->
<!-- - TODO:: CDC -->

#### Spark
- [DataStax Spark Cassandra Connector](https://github.com/datastax/spark-cassandra-connector): This library lets you expose Cassandra tables as Spark RDDs, write Spark RDDs to Cassandra tables, and execute arbitrary CQL queries in your Spark applications.
- [Stratio Deep (deprecated)](https://github.com/Stratio/stratio-deep): Deep is a thin integration layer between Apache Spark and several NoSQL datastores. We actually support Apache Cassandra and MongoDB, but in the near future we will add support for sever other datastores.
- [sample Spark Job Server Cassandra](https://github.com/instaclustr/sample-SparkJobserverCassandra) - Simple sample job illustrating the use of Spark Jobserver to execute Apache Spark analytics with Cassandra.
- [fluxcapacitor/pipeline](https://github.com/fluxcapacitor/pipeline): End-to-End, Real-time, Advanced Analytics Big Data Reference Pipeline using Spark, Spark SQL, Spark ML, GraphX, Spark Streaming, Kafka, NiFi, Cassandra, ElasticSearch, Redis, Tachyon, HDFS, Zeppelin, iPython/Jupyter Notebook, Tableau, Twitter Algebird.


#### Search / Secondary Indexes 
- [Tuning DSE Search](http://www.datastax.com/dev/blog/tuning-dse-search) Tuning DSE Search – Indexing latency and query latency
- [Elassandra](http://www.elassandra.io/): Elassandra = Elasticsearch as a Cassandra secondary index.
- [Cassandra Lucene Index](https://github.com/Stratio/cassandra-lucene-index):  Lucene based secondary indexes for Cassandra
- OLD - [Solandra](https://github.com/tjake/Solandra): Solandra is a real-time distributed search engine built on Apache Solr and Apache Cassandra.
- [cassandra-trigger](https://github.com/gradeup/cassandra-trigger) - Cassandra trigger to push realtime updates to elasticsearch

## Packages


### Libraries
- [DataStax Java Driver](https://github.com/datastax/java-driver): A Java client driver for Apache Cassandra. 
- [DataStax C++ Driver](https://github.com/datastax/cpp-driver): A modern, feature-rich, and highly tunable C/C++ client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's native protocol and Cassandra Query Language v3. http://datastax.github.io/cpp-driver/
- [DataStax Python Driver](https://github.com/datastax/python-driver): A modern, feature-rich and highly-tunable Python client library for Apache Cassandra (2.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax Ruby Driver](https://github.com/datastax/ruby-driver) : A Ruby client driver for Apache Cassandra. This driver works exclusively with the Cassandra Query Language version 3 (CQL3) and Cassandra's native protocol.
- [DataStax NodeJS Driver](https://github.com/datastax/nodejs-driver): A modern, feature-rich and highly tunable Node.js client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax C# Driver](https://github.com/datastax/csharp-driver) A modern, feature-rich and highly tunable C# client library for Apache Cassandra (1.2+) and DataStax Enterprise (3.1+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
- [DataStax PHP Driver](https://github.com/datastax/php-driver): DataStax PHP Driver for Apache Cassandra http://datastax.github.io/php-driver/
- [Achilles](http://doanduyhai.github.io/Achilles/): Achilles is an open source Persistence Manager for Apache Cassandra,with the features like Advanced bean mapping (compound primary key, composite partition key, timeUUID...),Native collections and map support,and so.
- [phpcassa](https://github.com/thobbs/phpcassa): PHP client library for Apache Cassandra
- [Caffinitas](http://caffinitas.org/mapper/): Caffinitas is an advanced object mapper for Apache Cassandra which has been especially designed to work with Datastax Java Driver 2.1+ against Apache Cassandra 2.1, 2.0 or 1.2.
- [Spring Data for Apache Cassandra](http://projects.spring.io/spring-data-cassandra/) -  Spring Data for Apache Cassandra offers a familiar interface to those who have used other Spring Data modules in the past.
- [gocql](https://github.com/gocql/gocql) - Package gocql implements a fast and robust Cassandra client for the Go programming language.
- OLD - [Netflix Astyanax](https://github.com/Netflix/astyanax): Astyanax is a high level Java client for Apache Cassandra, based on Thrift protocol. Not maintained.

### Tools
- [Cassandra Reaper](http://cassandra-reaper.io/): Automated repairs for Apache Cassandra. Supports all versions. 
- [cstar perf](https://github.com/datastax/cstar_perf) Apache Cassandra performance testing platform
- [Spark Cassandra Stress](https://github.com/datastax/spark-cassandra-stress) A tool for testing the DataStax Spark Connector against Apache Cassandra or DSE
- [trireme](https://github.com/o19s/trireme): Migration tool providing support for Apache Cassandra, DataStax Enterprise Cassandra, & DataStax Enterprise Solr.
- [cqlmigrate](https://github.com/sky-uk/cqlmigrate) -  Cassandra CQL migration tool. cqlmigrate is a library for performing schema migrations on a cassandra cluster.
- [cassandra-migration-tool-java](https://github.com/smartcat-labs/cassandra-migration-tool-java) - Cassandra migration tool for java is a lightweight tool used to execute schema and data migration on Cassandra database. 
- [Web: Cassandra Calculator](https://www.ecyrd.com/cassandracalculator/): A simple calculator to see how size / replication factor affect the system's consistency.
- [Cassandra-web](http://avalanche123.com/cassandra-web/) - A web interface for Apache Cassandra
https://github.com/rohitsakala/CassandraRestfulAPI
- [CassanddraRestfulAPI](https://github.com/rohitsakala/CassandraRestfulAPI) - CassandraRestfulAPI project exposes the cassandra data tables with the help of Restful API.
- [Netflix: Staash](https://github.com/Netflix/staash) - A language-agnostic as well as storage-agnostic web interface for storing data into persistent storage systems, the metadata layer abstracts a lot of storage details and the pattern automation APIs take care of automating common data access patterns.


### Admin / Monitor
- [DataStax OpsCenter](http://www.datastax.com/what-we-offer/products-services/datastax-opscenter): Simplified management for DataStax Enterprise and Cassandra database clusters.
- [Cassandra Cluster Admin](https://github.com/sebgiroux/Cassandra-Cluster-Admin): Cassandra Cluster Admin is a GUI tool to help people administrate their Apache Cassandra cluster.
- [Cassandra StatD Agent](https://github.com/lookout/cassandra-statsd-agent): Java Agent for Cassandra integration with StatsD 
- [Cassandra Scripts](https://github.com/bart613/cassandra): Python based cassandra ops scripts to monitor cfstats. 
- [Cassandra-Tools](https://github.com/CrowdStrike/cassandra-tools): Python Fabric scripts to help automate the launching and managing of cluster testing on AWS. 
- [Cassandra Opstools](https://github.com/spotify/cassandra-opstools): Generic scripts to review and monitor cassandra, from Spotify.  
- [CCM: Cassandra Cluster Manager)](https://github.com/pcmanus/ccm): A script/library to create, launch and remove an Apache Cassandra cluster on localhost.
- [Cassandra Nagios](https://github.com/causes/cassandra-nagios): Perl Based scripts to get metrics for monitoring using Jolokia.
- [Cassandra Log Tools](https://github.com/erickramirezDSE/cass_log_tools): Simple scripts for working with Apache Cassandra logs.
- [Cassandra CFStats to CSV Parser](https://github.com/jlacefie/cfstats-csv-parser): Converts the output of CFStats to CSV. 
- [Netflix-Priam](https://github.com/Netflix/Priam)Co-Process for backup/recovery, Token Management, and Centralized Configuration management for Cassandra.


### Queues / Schedulers
- [CMB](https://github.com/Comcast/cmb): A highly available, horizontally scalable queuing and notification service compatible with AWS SQS and SNS
- [CassieQ](https://github.com/paradoxical-io/cassieq): A Distributed queue built off of Cassandra.
- [Cherami](https://eng.uber.com/cherami/) : Distributed, scalable, durable, and highly available message queue system.
- [scheduler](https://github.com/PagerDuty/scheduler) : A Scala library for scheduling arbitrary code to run at an arbitrary time.



### Logging 
- [cassandra-log4j-appender](https://github.com/datastax/cassandra-log4j-appender): Cassandra appenders for Log4j

### Open Source Applications 
- [Twissandra](https://github.com/twissandra/twissandra) - Twissandra is an example project, created to learn and demonstrate how to use Cassandra. Running the project will present a website that has similar functionality to Twitter.
- [FiloDB](https://github.com/filodb/FiloDB) - High-performance distributed analytical database + Spark SQL queries + built for streaming.
- [ChronoServer](https://github.com/cyngn/ChronoServer) - A test server for sampling how long it takes mobile & web clients to make various types of requests to a server doing common request patterns. 

## Resources 

### Documentation 
- [Apache Cassandra Documentation](http://cassandra.apache.org/doc/) Definitive documentation for all published versions. 
- [DataStax Documentation](http://docs.datastax.com/en/landing_page/doc/landing_page/current.html) Documentation and Drivers from DataStax 

### Courses 
- [DataStax Academy](https://academy.datastax.com/): Free online courses on Cassandra

### Communities
- [Apache Cassandra Users Mailing List](http://www.mail-archive.com/user@cassandra.apache.org/)
- [Apache Cassandra Developers Mailing List](http://www.mail-archive.com/dev@cassandra.apache.org/)
- [Apache Cassandra Commits Mailing List](http://www.mail-archive.com/commits@cassandra.apache.org/)
- [Datastax Academy Slack](https://academy.datastax.com/slack)
- [Cassandra Slack](https://cassandra-slack.herokuapp.com/)
- [StackOverflow: Cassandra](https://stackoverflow.com/questions/tagged/cassandra)
- [StackOverflow: cql](https://stackoverflow.com/questions/tagged/cql)
- [StackOverflow: spark-cassandra-connector](https://stackoverflow.com/questions/tagged/spark-cassandra-connector)
- [Quora: Cassandra](https://www.quora.com/topic/Cassandra-database)
- [Meetups: Cassandra](https://www.meetup.com/topics/cassandra/?_cookie-check=mHgLvBy3N6Cke1RU)

### Blogs
- [Datastax](https://www.datastax.com/blog)
- [Datastax Academy](https://academy.datastax.com/developer-blog)
- [Codecentric](https://blog.codecentric.de/)
- [Pythian](https://www.pythian.com/blog/)
- [Instaclustr](https://www.instaclustr.com/blog/) 
- [Cassandra Zone](https://cassandra-zone.com/) - Findings and musings on Apache Cassandra
- [Altheroot:Cassandra](https://blog.alteroot.org/categories/cassandra/index.html)
- [OpenCredo:Cassandra](https://opencredo.com/tag/cassandra/)
- [DOAN DuyHai's Blog: Cassandra](http://www.doanduyhai.com/blog/?cat=57)
- [Amy Tobert](https://tobert.github.io/)
- [Christopher Batey: Cassandra](http://batey.info/cassandra.html)
- [Distributed Bytes:Cassandra](https://distributedbytes.timojo.com/search/label/cassandra)
- [The Netflix Tech Blog](https://medium.com/netflix-techblog)
- [Anant](https://blog.anant.us/tag/datastax/)

### Videos 
- [Best Practices for Running Cassandra on AWS](https://www.youtube.com/watch?v=IuJldwJLyFM)
- [Monitoring Cassandra: Don't Miss a Thing (Alain Rodriguez, The Last Pickle) | C* Summit 2016](https://www.youtube.com/watch?v=Q9AAR4UQzMk)
- [GumGum: Multi-Region Cassandra in AWS](https://academy.datastax.com/resources/Multi-Region-Cassandra-in-AWS)

### Slides
- [Cassandra DataTables Using Restful API](https://www.slideshare.net/SimranKedia2/cassandra-datatables-using-restful-api) A case on how to create a performant API using Python / Flash.
- [HAPI Cassandra](https://github.com/victorcouste/hapi-cassandra) A simple REST API with hapi nodejs framework on top of a Apache Cassandra database  
- [GumGum: Multi-Region Cassandra in AWS](https://www.slideshare.net/planetcassandra/gumgum-multiregion-cassandra-in-aws)
- [CQL: This is not the SQL you are Looking For](https://www.slideshare.net/aploetz/cql-this-is-not-the-sql-you-are-loooking-for)
- [Hardening cassandra for compliance or paranoia](https://www.slideshare.net/zznate/hardening-cassandra-for-compliance-or-paranoia)
- [Securing Cassandra](https://www.slideshare.net/planetcassandra/securing-cassandra-the-right-way)