# BigQuery Scheduled Query

This Java program runs a daily BigQuery query to insert deduplicated usage data into a partitioned and clustered table.

## Components

- BigQuery query logic in Java
- (Recommended) Cloud Function or Cloud Run to host the logic
- Cloud Scheduler to trigger the endpoint daily

## Usage

Run locally:

```bash
mvn compile exec:java -Dexec.mainClass="com.example.BigQueryScheduledQuery"
