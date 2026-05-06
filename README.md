# DuckDB Analytical Application

## Overview
This project explores how DuckDB executes analytical queries and how its internal design affects query behavior and performance. It demonstrates how database internals such as columnar storage and vectorized execution influence analytical workloads.

---

## Features
- Analytical queries using DuckDB
- Execution plan analysis using EXPLAIN ANALYZE
- Demonstration of columnar storage and vectorized execution
- Query comparisons (aggregation, filtering, time-based analysis)

---

## Dataset
This project uses the Superstore dataset.

The dataset was scaled to approximately 200,000 rows to simulate a larger analytical workload.

---

## Requirements

Install dependencies:

```bash
pip install duckdb pandas
