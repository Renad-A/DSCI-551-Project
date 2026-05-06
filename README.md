# DuckDB Analytical Application

## Overview

This project explores how DuckDB executes analytical queries and how its internal design affects query behavior and performance. It demonstrates how database internals such as columnar storage and vectorized execution influence analytical workloads.

---

## Features

- Analytical queries using DuckDB
- Execution plan analysis using `EXPLAIN ANALYZE`
- Demonstration of columnar storage and vectorized execution
- Query comparisons (aggregation, filtering, time-based analysis)

---

## Dataset

This project uses the **Superstore** dataset, scaled to approximately **200,000 rows** to simulate a larger analytical workload.

### Files

| File | Description |
|------|-------------|
| `cleaned superstore dataset.csv` | Original cleaned dataset (~9,993 rows) — **included in the repo** |
| `superstore_scaled.csv` | Scaled dataset (~199,860 rows) — **generated automatically by the notebook** |

### Important

- `cleaned_superstore_dataset.csv` must be present in the **same directory as the notebook** before running any cells. The notebook loads it using a relative path, so moving it will cause an error.
- `superstore_scaled.csv` does **not** need to be downloaded or created manually — it is generated when cell [1] is executed.
- Run all cells **in order** from top to bottom. Cell [1] must complete successfully before any subsequent queries can run.

---

## Environment Setup

1. Clone the repository:

```bash
git clone https://github.com/Renad-A/DSCI-551-Project.git
cd DSCI-551-Project
```

2. Install required packages:

```bash
pip install duckdb pandas jupyter
```

---

## Project Configuration

No additional configuration is required.

- The project uses an **in-memory DuckDB instance**
- The dataset is included (`cleaned_superstore_dataset.csv`)
- A scaled dataset is generated automatically in the notebook

---

## Run the Application

1. Launch Jupyter Notebook:

```bash
jupyter notebook
```

2. Open the notebook:

```
DuckDB_internals.ipynb
```

---

## Reproduce Results

To reproduce results, run the notebook from start to finish. The notebook will:

1. Load and scale the dataset
2. Create a DuckDB in-memory database
3. Execute queries
4. Display results and execution plans using `EXPLAIN ANALYZE`

All outputs (tables, runtimes, and execution plans) will be generated automatically.
