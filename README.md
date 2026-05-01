# Apache Flink (flink)

Apache Flink is an open-source framework and distributed processing engine for stateful computations over unbounded and bounded data streams. It is designed to run in all common cluster environments and to perform computations at in-memory speed and at any scale. Flink supports event-time processing, exactly-once semantics, layered APIs (SQL, Table, DataStream, ProcessFunction), and is widely used for real-time analytics, event-driven applications, and continuous ETL pipelines.

Beyond its programming APIs, Flink exposes a REST API on the JobManager Dispatcher that allows external systems to query cluster status, submit and manage jobs, trigger savepoints and checkpoints, upload and run JARs, and inspect metrics, accumulators, and exception histories. The same REST endpoints power the Flink Web UI, making the REST API the primary programmatic interface for operating a Flink cluster.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/flink/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Big Data
- Distributed Computing
- Real-Time Analytics
- Stream Processing
- Workflows

## APIs

### Apache Flink REST API

The Flink REST API is exposed by the JobManager Dispatcher and provides monitoring and management capabilities for a Flink cluster. The API covers cluster configuration, JobManager environment and metrics, job lifecycle (submit, list, cancel, stop), checkpoint and savepoint management, JAR upload and execution, dataset operations, and TaskManager inspection.

Endpoint categories include:

- **Cluster** — `/cluster`, `/config`, `/jobmanager/config`, `/jobmanager/environment`, `/jobmanager/logs`, `/jobmanager/metrics`, `/jobmanager/thread-dump`
- **Jobs** — `/jobs`, `/jobs/:jobid`, `/jobs/overview`, `/jobs/metrics`, `/jobs/:jobid/accumulators`, `/jobs/:jobid/exceptions`, `/jobs/:jobid/config`
- **Checkpoints & Savepoints** — `/jobs/:jobid/checkpoints`, `/jobs/:jobid/checkpoints/config`, `/jobs/:jobid/checkpoints/details/:checkpointid`
- **JARs** — `/jars`, `/jars/upload`, `/jars/:jarid/plan`, `/jars/:jarid/run`, `/jars/:jarid`
- **Datasets** — `/datasets`, `/datasets/:datasetid`
- **TaskManagers** — `/taskmanagers`, `/taskmanagers/:id/metrics`, `/taskmanagers/:id/logs`

**Documentation:** [https://nightlies.apache.org/flink/flink-docs-stable/docs/ops/rest_api/](https://nightlies.apache.org/flink/flink-docs-stable/docs/ops/rest_api/)

## Common Properties

- [Website](https://flink.apache.org/)
- [Documentation](https://nightlies.apache.org/flink/flink-docs-stable/)
- [REST API Documentation](https://nightlies.apache.org/flink/flink-docs-stable/docs/ops/rest_api/)
- [GitHub Repository](https://github.com/apache/flink)
- [Blog](https://flink.apache.org/posts/)
- [Community](https://flink.apache.org/community/)

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-04-28

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
