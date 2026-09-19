# Insurance Claims Lakehouse — Documentation

The story of how an insurance claims data platform captures change from Postgres
into Kafka, and where it goes from there.

Postgres CDC → Debezium → Kafka → S3 → Snowflake → dbt, orchestrated with Airflow.

Published with [Mintlify](https://mintlify.com).

## Local preview

```bash
npm i -g mint
mint dev
```

Opens at http://localhost:3000.
