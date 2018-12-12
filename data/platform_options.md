# Existing options for building a data pipeline

This document began in 2013 as a survey of the landscape of "Big Data" offerings. I've added to and updated it over the years, but is by no means complete (and may contain inaccuracies). Pull requests welcome for corrections and additions!

# Systems and Frameworks

### Spark

[Apache Spark](http://spark.apache.org/) is a fast and general engine for large-scale data processing.

### Storm

[Apache Storm](https://storm.incubator.apache.org/) is a free and open source distributed realtime computation system.

### Hindsight

[Hindsight](http://mozilla-services.github.io/hindsight/) is an open source stream processing software system developed by Mozilla. It was implemented as a successor to [Heka](http://hekad.readthedocs.org/).

### CloudWatch

[Amazon CloudWatch](http://aws.amazon.com/cloudwatch/) is a monitoring service for AWS cloud resources and the applications you run on AWS.

### Fluentd

[Fluentd](http://www.fluentd.org/) is an open source data collector designed for processing high-volume data streams.

### ELK Stack (ElasticSearch Logstash Kibana)

By combining the massively popular [Elasticsearch, Logstash and Kibana](http://www.elasticsearch.org/overview/) we have created an end-to-end stack that delivers actionable insights in real-time from almost any type of structured and unstructured data source.

### Flume

[Flume](http://flume.apache.org/) is a distributed, reliable, and available service for efficiently collecting, aggregating, and moving large amounts of log data.

### Disco

[Disco](http://disco.readthedocs.org/en/latest/intro.html) is an implementation of mapreduce for distributed computing.

### Inferno (DDS - Disco Distributed FS)

[Inferno](http://inferno.readthedocs.org/en/latest/index.html) is an open-source python map/reduce library, powered by [Disco.](http://discoproject.org/)

### Samza

[Apache Samza](http://samza.incubator.apache.org/) is a distributed stream processing framework.

### Hadoop

The Apache [Hadoop](http://hadoop.apache.org/) software library is a framework that allows for the distributed processing of large data sets across clusters of computers using simple programming models.

Hadoop is kind of a container/base for many other projects, such as HBase, Hive, Spark (see above), Mahout, Pig, Tez, ...

- [http://www.cloudera.com/content/cloudera/en/home.html](http://www.cloudera.com/content/cloudera/en/home.html)
- [Tez](http://tez.apache.org/) - The Apache Tez project is aimed at building an application framework which allows for a complex directed-acyclic-graph of tasks for processing data.
- [http://hortonworks.com/](http://hortonworks.com/)
- [http://www.jethrodata.com/home](http://www.jethrodata.com/home)
- [http://www.platfora.com/](http://www.platfora.com/)
- [http://www.splicemachine.com/](http://www.splicemachine.com/)
- [http://sqrrl.com/](http://sqrrl.com/)
- [Cascading](http://www.cascading.org/projects/cascading/) is an application development platform for building Data applications on Apache Hadoop. The data processing APIs define data processing flows. The APIs exposed provide a rich set of capabilities that allow you to think in terms of the data and the business problem such as sort, average, filter, merge etc.
- [http://gethue.com/](http://gethue.com/) Hue is a Web interface for analyzing data with Apache Hadoop.

### Graylog

[Graylog2](http://www.graylog2.org/) is an integrated log capture and analysis solution for operational intelligence. Non Graylog2-authored components include MongoDB for metadata and Elasticsearch for log file storage and text search.

### Suro

[Suro](https://github.com/netflix/suro) is a data pipeline service for collecting, aggregating, and dispatching large volume of application events including log data.

http://techblog.netflix.com/2013/12/announcing-suro-backbone-of-netflixs.html

### Manta

[Manta](https://github.com/joyent/manta/) is an open-source, HTTP-based object store that uses OS containers to allow running arbitrary compute on data at rest (i.e., without copying data out of the object store). General overview [here](http://queue.acm.org/detail.cfm?id=2645649).

### Flink

[Flink](https://flink.apache.org/) is a[streaming dataflow engine](https://flink.apache.org/features.html#unified-stream-amp-batch-processing) that provides data distribution, communication, and fault tolerance for distributed computations over data streams. One interesting feature is that it provides the option of [“exactly once” message delivery](https://flink.apache.org/features.html) (and out-of-order events).

### Nifi

[Apache Nifi](http://nifi.apache.org/) is an easy to use, powerful, and reliable system to process and distribute data. Nifi supports powerful and scalable directed graphs of data routing, transformation, and system mediation logic.

### Panda / PNDA

[PNDA](http://panda.cisco.com/overview) is an Open source Platform for Network Data Analytics from Cisco.

### Streamlio

[Streamlio](https://www.streaml.io/) is Enterprise-grade, unified, end-to-end real-time solution. Uses Pulsar, Heron, and BookKeeper (linked below).

### Snowplow

[Snowplow](https://github.com/snowplow/snowplow/wiki/Technical-architecture) is an enterprise-strength marketing and product analytics platform. It does three things:

1. Identifies your users, and tracks the way they engage with your website or application
2. Stores your users' behavioural data in a scalable "event data warehouse" you control: in Amazon S3 and (optionally) Amazon Redshift or Postgres
3. Lets you leverage the biggest range of tools to analyze that data, including big data tools (e.g. Spark) via EMR or more traditional tools e.g. Looker, Mode, Caravel, Re:dash to analyze that behavioural data

### StreamSets

[StreamSets](https://streamsets.com/) is the industry’s first data operations platform. With StreamSets data operations platform you can efficiently develop batch and streaming dataflows, operate them with full visibility and control, and easily evolve your architecture over time.

### Snap

[Snap](http://snap-telemetry.io/) is a powerful open telemetry framework. Easily collect, process, and publish telemetry data at scale.

### DataFusion

[DataFusion](https://datafusion.rs/): Modern Distributed Compute Platform implemented in Rust. Code on [github](https://github.com/datafusion-rs/datafusion)

# Components

## Serialization Formats

See [serialization](serialization.md).

### Mesos

[Apache Mesos](http://mesos.apache.org/) is a cluster manager that simplifies the complexity of running applications on a shared pool of servers.

### Kafka

[Apache Kafka](http://kafka.apache.org/) is publish-subscribe messaging rethought as a distributed commit log.

[https://wikitech.wikimedia.org/wiki/Analytics/Cluster/Logging_Solutions_Overview](https://wikitech.wikimedia.org/wiki/Analytics/Cluster/Logging_Solutions_Overview)

### Chronicle Queue

[Persisted Queue](http://openhft.net/products/chronicle-queue/), fast enough to record everything.

### Sawzall

[Sawzall](http://en.wikipedia.org/wiki/Sawzall_%28programming_language%29) is a procedural domain-specific programming language, used by Google to process large numbers of individual log records.

### Druid

[Druid](http://druid.io/docs/0.7.1.1/) is an open-source analytics data store designed for OLAP queries on timeseries data (trillions of events, petabytes of data). Druid provides cost-effective and always-on real-time data ingestion, arbitrary data exploration, and fast data aggregation.

### Aerospike

[Aerospike](http://www.aerospike.com/docs/architecture/) is a distributed, scalable NoSQL database.

[http://highscalability.com/blog/2014/8/18/1-aerospike-server-x-1-amazon-ec2-instance-1-million-tps-for.html](http://highscalability.com/blog/2014/8/18/1-aerospike-server-x-1-amazon-ec2-instance-1-million-tps-for.html)

### NuoDB

[NuoDB](http://www.nuodb.com/) is a distributed database offering a rich SQL implementation and true ACID transactions. Designed for the modern datacenter, and as a scale-out cloud database, NuoDB is the NewSQL solution you need to simplify application deployment.

### ElasticSearch

[ElasticSearch](http://www.elasticsearch.org/overview/elasticsearch) is distributed restful search and analytics

### Logstash

[logstash](http://logstash.net/) is a tool for managing events and logs. You can use it to collect logs, parse them, and store them for later use (like, for searching).

### Kibana

[Kibana](http://www.elasticsearch.org/overview/kibana/) lets you visualize logs and time-stamped data.

### Redshift

[Amazon Redshift](http://aws.amazon.com/redshift/) is a fast, fully managed, petabyte-scale data warehouse solution that makes it simple and cost-effective to efficiently analyze all your data using your existing business intelligence tools.

### Riemann

[Riemann](http://riemann.io/index.html) aggregates events from your servers and applications with a powerful stream processing language.

### Mahout

The [Apache Mahout](https://mahout.apache.org/) project's goal is to build a scalable machine learning library.

### H20

[H2O](http://0xdata.com/h2o/) is the world’s fastest in-memory platform for machine learning and predictive analytics on big data.

### Presto

[Presto](http://prestodb.io/) is an open source distributed SQL query engine for running interactive analytic queries against data sources of all sizes ranging from gigabytes to petabytes.

### Sensu

[Sensu](http://sensuapp.org/) is often described as the “monitoring router”. Essentially, Sensu takes the results of “check” scripts run across many systems, and if certain conditions are met; passes their information to one or more “handlers”.

### dCache

[dCache](http://www.dcache.org/) A system for storing and retrieving huge amounts of data, distributed among a large number of heterogenous server nodes, under a single virtual filesystem tree with a variety of standard access methods.

### Cockroach

[Cockroach](https://github.com/cockroachdb/cockroach/blob/master/README.md) is a distributed key/value datastore which supports ACID transactional semantics and versioned values as first-class features. The primary design goal is global consistency and survivability, hence the name. Cockroach aims to tolerate disk, machine, rack, and even datacenter failures with minimal latency disruption and no manual intervention. Cockroach nodes are symmetric; a design goal is one binary with minimal configuration and no required auxiliary services.

### TaskCluster

[TaskCluster](http://docs.taskcluster.net/) is a set of components that manages task queuing, scheduling, execution and provisioning of resources. It was designed to run automated builds and test at Mozilla.

### LMAX

[LMAX](http://martinfowler.com/articles/lmax.html) is a platform aimed at processing events (it’s intended for financial trading) at high speed with low latency. The “disruptor” is [open source](https://github.com/LMAX-Exchange/disruptor).

### Charted

[Charted](http://flowingdata.com/2014/11/26/chart-data-quickly-with-open-source-charted/) is a stripped down charting tool for quick & dirty visualizations of publicly accessible data.  May be of use for things like public data exported to S3.

### Atlas

[Atlas](http://techblog.netflix.com/2014/12/introducing-atlas-netflixs-primary.html) is a telemetry-recording and display tool from Netflix.

### AWS Lambda

[AWS Lambda](http://aws.amazon.com/lambda/) is a compute service that runs your code in response to events and automatically manages the compute resources for you, making it easy to build applications that respond quickly to new information.[[1]](http://awsadvent.tumblr.com/post/105710082739/aws-advent-2014-exploring-aws-lambda)

### Tachyon

[Tachyon](http://tachyon-project.org/index.html) is a memory-centric distributed file system enabling reliable file sharing at memory-speed across cluster frameworks, such as Spark and MapReduce. It achieves high performance by leveraging lineage information and using memory aggressively. Tachyon caches working set files in memory, thereby avoiding going to disk to load datasets that are frequently read. This enables different jobs/queries and frameworks to access cached files at memory speed.

### VoltDB

[VoltDB](https://www.voltdb.com/overview) is an in-memory, operational database built to rapidly import, operate on, and then export HUGE amounts of data at lightning speed.

### Microsoft Bond

[Bond](https://github.com/Microsoft/bond) is a cross-platform framework for working with schematized data. It supports cross-language de/serialization and powerful generic mechanisms for efficiently manipulating data.

### Streamtools

[Streamtools](http://blog.nytlabs.com/streamtools/docs/) is a graphical toolkit for dealing with streams of data. Streamtools makes it easy to explore, analyse, modify and learn from streams of data.

### Fenzo

[Fenzo](https://github.com/Netflix/Fenzo) is a scheduler Java library for Apache Mesos frameworks that supports plugins for scheduling optimizations and facilitates cluster autoscaling.

### Luigi

[Luigi](https://github.com/spotify/luigi) is a Python (2.7, 3.3, 3.4) package that helps you build complex pipelines of batch jobs. It handles dependency resolution, workflow management, visualization, handling failures, command line integration, and much more.

### Kubernetes

[Kubernetes](http://blog.kubernetes.io/) is an open source Container Cluster orchestration framework that was started by Google in 2014.

### Airflow

[Airflow](https://github.com/apache/incubator-airflow) is a platform to programmatically author, schedule and monitor workflows.

### DistributedLog

[DistributedLog](http://distributedlog.io/html/index.html) (DL) is a high-performance, replicated log service, offering durability, replication and strong consistency as essentials for building reliable distributed systems.

### Apache Beam

[Apache Beam](https://beam.apache.org/get-started/beam-overview/) is an open source, unified programming model that you can use to create a data processing pipeline. You start by building a program that defines the pipeline using one of the open source Beam SDKs. The pipeline is then executed by one of Beam’s supported distributed processing back-ends, which include[Apache Apex](http://apex.apache.org),[Apache Flink](http://flink.apache.org),[Apache Spark](http://spark.apache.org), and [Google Cloud Dataflow](https://cloud.google.com/dataflow).

### AWS Glue

[AWS Glue](https://aws.amazon.com/glue/) is a fully managed ETL service that makes it easy to move data between your data stores. AWS Glue simplifies and automates the difficult and time consuming data discovery, conversion, mapping, and job scheduling tasks.

### Pachyderm

[Pachyderm](http://www.pachyderm.io/) is a data lake that offers complete version control for data and leverages the container ecosystem to provide reproducible data processing.

### Apache Bookkeeper

[BookKeeper](https://bookkeeper.apache.org/) is a scalable, fault-tolerant, and low-latency storage service optimized for real-time workloads

### Apache Pulsar

[Apache Pulsar](https://pulsar.incubator.apache.org) (incubating) provides pub-sub messaging scalable out to millions of topics.

### Heron

[Heron](https://twitter.github.io/heron) provides topology-based real-time stream processing.

### Prometheus

[Prometheus](https://github.com/prometheus) is an open-source systems monitoring and alerting toolkit.

### Kudu

[Kudu](https://kudu.apache.org/overview.html) is a hadoop-compatible storage layer to enable fast analytics on fast data.

### Kylin

[Apache Kylin](http://kylin.apache.org/)™ is an open source Distributed Analytics Engine designed to provide SQL interface and multi-dimensional analysis (OLAP) on Hadoop/Spark supporting extremely large datasets.

### MatrixDS

[MatrixDS](http://matrixds.com/) is the data project workbench. MatrixDS is Github meets Docker for data scientists and data analysts. Designed from the ground up for the data community, we are a place to build, share and manage data projects at any scale.

### Split.io

[Split](https://www.split.io/product/) helps product teams make smarter decisions by enabling them to turn every feature roll-out into an experiment.

### Proteus

Netifi [Proteus](https://netifi.com/proteus.html) is the next-generation reactive microservices platform that allows developers to focus on their product by transparently providing API management, routing, service discovery, predictive load balancing, and ultra low latency RPC.

### ClickHouse

[ClickHouse](https://clickhouse.yandex/) is an open source column-oriented database management system capable of real time generation of analytical data reports using SQL queries.

### MQTT

[MQTT](http://mosquitto.org/man/mqtt-7.html) is a lightweight publish/subscribe messaging protocol. It is useful for use with low power sensors, but is applicable to many scenarios.

### Roughtime

[Roughtime](https://roughtime.googlesource.com/roughtime) is a project that aims to provide secure time synchronisation.

### Great Expectations

[Great Expectations](https://github.com/great-expectations/great_expectations) is a framework that helps teams save time and promote analytic integrity with a new twist on automated testing: pipeline tests. Pipeline tests are applied to data (instead of code) and at batch time (instead of compile or deploy time). Blog post: ["Down with pipeline debt"](https://medium.com/@expectgreatdata/down-with-pipeline-debt-introducing-great-expectations-862ddc46782a)

### Sia

[Sia](https://sia.tech/) is a decentralized storage platform secured by blockchain technology. The Sia Storage Platform leverages underutilized hard drive capacity around the world to create a data storage marketplace that is more reliable and lower cost than traditional cloud storage providers.

### Mixpanel

[Mixpanel](https://mixpanel.com/): Understand every user's journey. Acquire, engage, and retain with actionable user analytics.

### DBT

[dbt](https://docs.getdbt.com/docs/overview) (data build tool) is a productivity tool that helps analysts get more done and produce higher quality results.

Analysts commonly spend 50-80% of their time modeling raw data—cleaning, reshaping, and applying fundamental business logic to it. dbt empowers analysts to do this work better and faster.

### InfluxDB

[InfluxDB](https://www.influxdata.com/time-series-platform/influxdb/) is used as a data store for any use case involving large amounts of timestamped data, including DevOps monitoring, application metrics, IoT sensor data, and real-time analytics. Conserve space on your machine by configuring InfluxDB to keep data for a defined length of time, automatically expiring & deleting any unwanted data from the system. InfluxDB also offers a SQL-like query language for interacting with data.

### StreamX

[StreamX](https://github.com/qubole/streamx) is a kafka-connect based connector to copy data from Kafka to Object Stores like Amazon s3, Google Cloud Storage and Azure Blob Store. It focusses on reliable and scalable data copying. It can write the data out in different formats (like parquet, so that it can readily be used by analytical tools) and also in different partitioning requirements.

### Databricks Delta

[Databricks Delta](https://databricks.com/blog/2017/10/25/databricks-delta-a-unified-management-system-for-real-time-big-data.html) is a unified data management system to simplify large-scale data management.

### Apache Arrow

[Apache Arrow](https://arrow.apache.org/) is a cross-language development platform for in-memory data.

### TrailDB

[TrailDB](http://traildb.io/) is an efficient tool for storing and querying series of events.


# Ideas and Research

### Mortar

[Mortar: Wide-Scale Stream Processing](http://cseweb.ucsd.edu/~kyocum/synsys/mortar_wide-scale_stream_pr.html). Mortar is a light-weight distributed stream processing engine for federated systems.

### Borealis

[Borealis: Distributed Stream Processing Engine](http://cs.brown.edu/research/borealis/public/). Borealis is a distributed stream processing engine that is being developed at Brandeis University, Brown University, and MIT.

### MillWheel

[MillWheel: Fault-Tolerant Stream Processing at Internet Scale](http://research.google.com/pubs/pub41378.html)

### Megastore

[Megastore: Providing Scalable, Highly Available Storage for Interactive Services](http://research.google.com/pubs/pub36971.html)

### Spanner

[Spanner](https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf)



# ** Ruled out **

### S4

[S4](http://incubator.apache.org/s4/) is a general-purpose, distributed, scalable, fault-tolerant, pluggable platform that allows programmers to easily develop applications for processing continuous unbounded streams of data.

Ruled out because: dead project.


### Scribe

[Scribe](https://github.com/facebookarchive/scribe) is a server for aggregating log data streamed in real time from a large number of servers.

Ruled out because: dead project.

[https://wikitech.wikimedia.org/wiki/Analytics/Cluster/Logging_Solutions_Overview](https://wikitech.wikimedia.org/wiki/Analytics/Cluster/Logging_Solutions_Overview)



# Other Commercial Offerings

- Kinesis
    - [Amazon Kinesis](http://aws.amazon.com/kinesis/) is a fully managed service for real-time processing of streaming data at massive scale.
    - Ruled out because: payload size too small, data retention too short.
- [Velocidata](http://velocidata.com/)
    - Hardware enhanced data transformation claiming to be 100 to 1000x faster than conventional ETL processes. Essentially, VelociData gives you a purpose-built supercomputer in a 4U form factor at a monthly or annual cost that radically transforms the economics of Big Data, analytics and BI.
- [Sisense](http://www.sisense.com/)
    - End to end BI product highly optimized for x64 architectures enabling a single commodity server to deliver the same data processing power as a (Hadoop) cluster made up of 10 individual nodes.
- [Splunk](http://www.splunk.com/)
    - Platform for Operational Intelligence. Customers use Splunk to search, monitor, analyze and visualize machine data. By monitoring and analyzing everything from customer clickstreams and transactions to network activity and call records, Splunk Enterprise turns your machine data into valuable insights.
- [Google Cloud Dataflow](http://googlecloudplatform.blogspot.com/2014/06/sneak-peek-google-cloud-dataflow-a-cloud-native-data-processing-service.html)
    - Not available yet
- [Azure Stream Analytics](https://gigaom.com/2014/10/29/microsoft-adds-stream-processing-and-pipeline-tools-to-azure/)
    - Part of Microsoft’s Azure cloud platform.
- [Cirro](http://www.cirro.com/)
    - Cirro’s Next Generation Data Federation allows organizations to ask questions and harvest value previously unavailable in disconnected corporate data silos. Cirro can spread a query across multiple data sources and use the local processing capability located where each of the sources resides to help resolve the query.
- [Alpine Data Labs](http://alpinenow.com/)
    - Basically BI for the non-developer: “Alpine Chorus 5.0 is the world's only advanced analytics platform that is 100% visual, web-based, collaborative and optimized for Big Data.”
- [logentries](https://logentries.com/)
    - Log Management Built for the Cloud. Fast Search & Real-time Log Processing. Centralized search, aggregation, and correlation. See query results in seconds. Connect Distributed Systems, Apps & Users. Process log data in any format, connect with any system, and share with any team. Smarter Analytics, Quicker Insights
- [papertrail](https://papertrailapp.com/)
    - Frustration-free log management.
- [Jethro](https://jethro.io/)
    - A SQL-on-Hadoop engine, Jethro acts as a BI-on-Hadoop acceleration layer that speeds up big data query performance for BI tools like Tableau, Qlik and Microstrategy from any data source like Hadoop or Amazon S3.
- [Periscope](https://www.periscopedata.com/blog) announced their [Unified Data Platform](https://www.periscopedata.com/blog/unified-data-platform) in 2017.
- [Sentry](https://sentry.io/welcome/) Open-source error tracking that helps developers monitor and fix crashes in real time. Iterate continuously. Boost efficiency. Improve user experience.

# Bibliography

1. [http://jasonwilder.com/blog/2013/11/19/fluentd-vs-logstash/](http://jasonwilder.com/blog/2013/11/19/fluentd-vs-logstash/)
2. [http://highscalability.com/blog/2014/8/18/1-aerospike-server-x-1-amazon-ec2-instance-1-million-tps-for.html](http://highscalability.com/blog/2014/8/18/1-aerospike-server-x-1-amazon-ec2-instance-1-million-tps-for.html)
3. [https://wikitech.wikimedia.org/wiki/Analytics/Cluster/Logging_Solutions_Overview](https://wikitech.wikimedia.org/wiki/Analytics/Cluster/Logging_Solutions_Overview)
4. Databricks [https://www.youtube.com/watch?v=dJQ5lV5Tldw](https://www.youtube.com/watch?v=dJQ5lV5Tldw)
5. [http://sqrrl.com/](http://sqrrl.com/)
6. [http://www.splicemachine.com/](http://www.splicemachine.com/)
7. [http://www.platfora.com/](http://www.platfora.com/)
8. [http://www.crn.com/slide-shows/applications-os/240164423/the-10-coolest-big-data-products-of-2013.htm?itc=nextpage](http://www.crn.com/slide-shows/applications-os/240164423/the-10-coolest-big-data-products-of-2013.htm?itc=nextpage)
9. [http://www.knime.org/](http://www.knime.org/)
10. [http://www.zdatainc.com/2014/09/apache-storm-apache-spark/](http://www.zdatainc.com/2014/09/apache-storm-apache-spark/)
11. [http://techblog.netflix.com/2014/10/using-presto-in-our-big-data-platform.html](http://techblog.netflix.com/2014/10/using-presto-in-our-big-data-platform.html)
12. [The Big Data Information Architecture](http://insideanalysis.com/wp-content/uploads/2014/07/BDIAReportFINAL.pdf)
13. [http://highlyscalable.wordpress.com/2013/08/20/in-stream-big-data-processing/](http://highlyscalable.wordpress.com/2013/08/20/in-stream-big-data-processing/)
14. [Storm vs Spark](http://www.zdatainc.com/2014/09/apache-storm-apache-spark/)
15. [http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis](http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis)
16. [https://aws.amazon.com/blogs/aws/dynamodb-streams-preview/](https://aws.amazon.com/blogs/aws/dynamodb-streams-preview/)
17. http://blog.confluent.io/2015/03/04/turning-the-database-inside-out-with-apache-samza/
18. [Prometheus vs. other time-series databases](https://prometheus.io/docs/introduction/comparison/)
19. [Workflow Managers](https://github.com/erikbern/workflow-managers)