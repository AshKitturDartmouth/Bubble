# Bubble
Financial Services Data Platform

A financial research platform that ingests live and historical market data and financial documents, processes them into analytical datasets, and enables both quantitative analysis and document intelligence via RAG.

The platform continuously ingests tick-level market data and financial data through streaming and batch pipelines. For data ingestion, utilizes multithreading. Batch workflows are orchestrated using Airflow DAGs, which coordinate Spark, dbt, and Python jobs to transform and validate data.

The resulting data is stored in two systems: an analytical warehouse (DuckDB + dbt) for SQL-based analysis and feature generation, and a vector store (Qdrant) that powers RAG-based question answering over financial documents.

Tech Stack: Python, PySpark, Airflow, Docker, Jenkins, dbt, DuckDB, Linux, and QDrant.
