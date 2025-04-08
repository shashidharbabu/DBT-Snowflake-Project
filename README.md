# 📘 dbt Project: Session Summary with Snowflake

## Project Overview

This project demonstrates a dbt pipeline connected to Snowflake. It focuses on building input models using CTEs, transforming them into an output summary, applying snapshots, and testing key fields.

---

## Tasks Completed

### 1. dbt Project Initialization
- Created a dbt project named `build_mau`.
- Configured to work with the Snowflake connector.

### 2. Input Models
- Created two input models:
  - `user_session_channel`
  - `session_timestamp`
- Both are implemented using Common Table Expressions (CTEs).

### 3. Output Model
- Created `session_summary` by joining the input models.
- Includes calculated session duration.

### 4. Snapshot Setup
- Added snapshot for the `session_summary` table.
- Uses the `timestamp` strategy based on `session_end`.

### 5. Data Tests
- Applied two tests to the `session_id` field in `session_summary`:
  - `unique`
  - `not_null`

---


- Shashidhar Babu P V D (018174494)
