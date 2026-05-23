Project X — Mini Data Mart & ETL Pipeline
📊  Consolidated data mart built from 5+ source systems to enable faster, reliable compliance reporting

Data Mart	SQL · Python	ETL Pipeline	BFSI

📝 Overview
Project X is a mini data warehouse and ETL pipeline built for the Compliance team at a financial institution. It consolidates data from 5+ heterogeneous source systems into a single unified data mart, enabling faster, more reliable consolidated reporting and reducing reconciliation time significantly.

✨ Key Features
▸	Data extraction from 5+ source systems with schema normalization
▸	Incremental loading logic — only processes new/changed records for efficiency
▸	Fact and dimension table design following star schema principles
▸	Automated reconciliation checks — flags discrepancies between source and mart
▸	Power BI-ready output layer for dashboard consumption

🛠 Tech Stack
SQL (MySQL)  ·  Python (pandas, sqlalchemy)  ·  Star Schema Design  ·  Data Modeling  ·  Power BI

📈 Results
▸	✅  Consolidated 5+ fragmented data sources into a single queryable mart
▸	✅  Reduced report generation time from hours to minutes
▸	✅  Improved stakeholder confidence in data accuracy through automated reconciliation

📁 Project Structure
project-x/
├── schema/
│   ├── fact_transactions.sql
│   └── dim_customers.sql
├── etl/
│   ├── extract.py
│   ├── transform.py
│   └── load.py
├── reconciliation/
│   └── checks.py
└── README.md

🚀 Getting Started
# Clone the repo
git clone https://github.com/krisanumanna/project-x-datamart

# Set up schema
mysql -u root -p < schema/fact_transactions.sql

# Run full ETL
python etl/extract.py && python etl/transform.py && python etl/load.py
