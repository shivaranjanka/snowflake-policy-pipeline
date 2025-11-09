# 🚀 Automated Insurance Policy Data Pipeline (AWS S3 → Snowflake)

This project demonstrates end‑to‑end ingestion and CDC in Snowflake using **Snowpipe**, **Streams**, and **Tasks**.
It loads policy data from **AWS S3** into **Snowflake**, merges incremental changes, and builds a validation report.

## Quick Start
1) Run `scripts/01_create_stage_and_pipe.sql`
2) Run `scripts/02_create_streams_and_tasks.sql`
3) (Optional) Run `scripts/03_validation_check.sql`
4) Upload `data/policy_data_day1.csv` to your S3 bucket configured in the Stage.
5) Watch data auto‑ingest via Snowpipe and Task merge hourly.

> Replace `MY_S3_INTEGRATION` and `s3://insurance-data/` with your real values.
