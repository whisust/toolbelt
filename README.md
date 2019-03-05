# toolbelt
List of stuff I use, know of, master, saw once on HN.
This is more of a reminder of what I know, for my future self to not forget.

### Languages
- Python, working with 2.7 right now, did a lot of 3.6 -> mostly for ML stuff, can be great for quick scripting though
- Scala 2.12 -> functional programming, safe team development experience, compiled, type safe, a bit slow but gives strong guarantees
  - Typelevel library family
  - Cats, i luv u
  - fs2 streams, i luv u
- Rust, learning -> bare metal performances with type safe and memory safe guarantees
- Clojure, learning -> learn too quickly prototype programs
- Javascript, should learn it a bit more -> learn it before learning a frontend framework, looking for vue
- Java up to 8 -> I just feel better and better not coding in java anymore
- Bash -> Automate all the things
- SQL -> because DB
- CQL -> because DB

### Databases
- Cassandra / Scylla -> Columnar db with horizontal scaling, can handle lot of write/read per sec, eventually consistent
- Postgres -> SQL database for the win, up to v10
- CDC -> capture data change, read db modifications at the source (wal) and create a read-only copy of what you want where you want
- Kafka -> Like cassandra but for data in movement, distributed streaming platform
- MySQL
- OracleDB

### Data Processing
- Batch processing / Data at rest 
  - Spark, standalone and cluster mode, Mesos and EMR (yarn)
- Stream processing / Data in movement
  - Beam model -> google way of doing stream processing
  - Flink -> use a Master and a worker to do things, state save
  - Kafka Streams -> Add state stores backed up in your kafka cluster, easy start/stop, add http server to query your state stores
- Kafka connect -> send stuff to kafka
- Hadoop -> Distributed processing

### Data Formats
- Parquet -> Columnar, schema-wearing, efficient data format, great for storing things
- Avro -> Byte format, serialzation, schema needed but not in data. Great for exchanging things
- Json -> human readable serilization format, easy to use but not space efficient
- CSV

### Cloud
- AWS yay we all love to use software that's 10 years old and not updated since 5... -> Datapipeline, EMR, S3, EC2, Route53, Cloudwatch, SNS, Lambda, Redshift
- DCOS -> datacenter os, deploy every kind of app on your cluster
- Marathon -> orchestrator for DCOS
- Mesos -> virtualize your resources pool

### Monitoring
- Datadog -> Store metrics, create dashboards, define alerting, forget everything about logs
- Metrics -> com.codahale.metrics.SharedMetricRegistries 
- Statsd -> Collect metrics at system level
- Pagerduty -> You liked that sweet weekend? Well here's a software crackdown you must solve now

### Delivery
- Docker -> bundle system dependencies together to ensure reproducible
- Jenkins -> Automate your builds and deployments

### Computer Science
- CAP theorem -> Consistency / Availability / Partition fault tolerant, pick two
- Partitioning featuring Replication -> Sort your data, make copies to be fault tolerant
- Stragglers -> What kind of ressources does your software require? Where can it be a problem if there is too much of this or not enough of that? How do you see it?
- Scheduling -> Given a pool of resource with constraints, how do you schedule your workloads to be the most efficient
- Costs of operations -> cache / ram / disk / network
- Parallelism / Concurrency

### Misc
- Zookeeper -> Distributed configuration and service discovery
- Hazelcast -> In memory, distributed cache

### Sotwares
- IntelliJ IDEA -> IDE efficient for compiled languages and useful for integrations; databasess conection, runs, repls, builds...
- Sublime Text -> Nice for text editing and file navigation, requires a bit of knowledge for keyboard shotcuts
- VSCode -> for not compiled languages
- terminal -> write stuff, make it work, never touch the mouse
- jq -> tool for using json in CLI
- curl / httpie -> http requests
- git -> git
- repls when available
- mvn, sbt, yarn (js), npm, cargo, leiningen, make -> build tools for their respective language
- autojump -> `cd` with superpowers
- fzf -> fuzzy history matcher

### Machine Learning
- Linear and logistic regressions
- XGBoost stuff
- Overfitting / Underfitting -> Do you have enough data? Do your models handle new inputs?
- Cross validation
- Bias
- Thompson model -> Update your distributions with every new success, efficient for online learning
- Data preparation -> here lies 80% of the work
