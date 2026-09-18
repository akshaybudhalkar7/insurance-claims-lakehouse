# Insurance Claims Lakehouse — Documentation

Documentation for an insurance claims and policy analytics platform built on
Postgres CDC → Debezium → Kafka → S3 → Snowflake → dbt, orchestrated with Airflow.

Published with [Mintlify](https://mintlify.com).

## What the platform does

Insurers need loss-ratio, reserving and claims-operations reporting that is
**point-in-time accurate** — an auditor can ask what the reserve figure was on a
past date, and the answer has to be reproducible. That single requirement is what
drives every architectural decision here: change data capture rather than nightly
snapshots, an append-only raw layer, and idempotent incremental loads.

## Contents

| Section | Covers |
| --- | --- |
| Overview | The business problem, system architecture, ingestion paths |
| Concepts | How CDC, WAL/replication slots and replica identity actually work |
| Build Log | What was built at each stage, and the reasoning behind each decision |
| Reference | Verification queries and a troubleshooting catalogue |

## Local preview

```bash
npm i -g mint
mint dev
```

Opens at http://localhost:3000.
