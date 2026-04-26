# car-data-lakehouse
In this project, you will build a complete Data Lakehouse from scratch using Databricks and the Medallion Architecture

### stucture
```
cars-lakehouse-project/
│
├── notebooks/
|
├── setup/
│   │   ├── init_catalog_data.ipynb
|   |   
│   ├── bronze/
│   │   ├── ingest_raw_data.ipynb
│   │
│   ├── silver/
│   │   ├── clean_transform.ipynb
│   │
│   ├── gold/
│   │   ├── business_aggregations.ipynb
│
├── pipelines/
|
│── setup/
│   ├── init_catalog.py
|   |
|   ├──bronze/
│   │   ├── ingest.py
│   │
│   ├── silver/
│   │   ├── transform.py
│   │
│   ├── gold/
│   │   ├── aggregate.py
│
├── sql/
│   ├── bronze/
│   │   ├── create_raw_tables.sql
│   ├── silver/
│   │   ├── clean_tables.sql
│   ├── gold/
│   │   ├── analytics.sql
│
├── workflows/                # ❗ orchestration layer (Airflow / Databricks Jobs)
│   ├── airflow/
│   │   ├── cars_pipeline_dag.py
│   ├── databricks_jobs/
│   │   ├── job_config.json
│
├── configs/
├── tests/
├── utils/
├── README.md
└── requirements.txt

```

