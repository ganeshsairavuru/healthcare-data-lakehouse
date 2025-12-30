# Azure Healthcare Claims Analytics Pipeline (PoC)

End-to-end ELT pipeline demonstrating enterprise-grade processing of synthetic healthcare claims data using Azure-native tools.

## Objective
Simulate real-world healthcare claims processing: ingest raw claims, clean and transform, apply quality checks, aggregate for analytics, and store in Delta Lake — designed with scalability, governance, and compliance (HIPAA patterns) in mind.

## Architecture Overview
- Raw CSV → Azure Data Lake (simulated locally/DBFS)
- Processing → PySpark on Databricks
- Storage → Delta Lake tables
- Quality → Custom validation rules
- Output → Aggregated analytics tables ready for Power BI / Synapse

## Tech Stack
- Azure Databricks
- PySpark & Spark SQL
- Delta Lake
- Python (pandas for quick exploration)

## Key Features & Outcomes
- Cleaned and validated 10,000+ synthetic claims records
- Removed nulls/duplicates and standardized diagnosis codes
- Created yearly and provider-level cost summaries
- 100% data quality on critical fields post-processing
- Delta Lake enables ACID transactions and time travel

## Project Structure
- data/                        # Raw synthetic claims
- notebooks/                   # Main pipeline notebook
- screenshots/                 # Visual results

## How to Run (Databricks Community Edition or Local Spark)
1. Upload `data/synthetic_claims.csv` to DBFS or local path
2. Open and run `notebooks/healthcare_claims_pipeline.ipynb.`
3. View Delta tables and output summaries

Built by Ganesh Sai Ravuru  
Data Engineer | Multi-Cloud Specialist
