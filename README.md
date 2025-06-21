![Medallion Data Architecture Animated GIF](https://github.com/danmca19/Medallion_Data_Architecture/blob/main/Gemini_Generated_Image_yylm17yylm17yylm.png)

Project Overview
This project focuses on building an automated data pipeline using Databricks to consolidate, clean, and enrich raw data. The goal is to transform disparate raw data into a structured and valuable format, ready for advanced analytics, Business Intelligence (BI), and Machine Learning (ML) applications. The pipeline adheres to the Medallion Architecture (Bronze, Silver, Gold layers), ensuring data quality, reliability, and accessibility.

What Was Done
The project implements a robust data pipeline, moving data through three distinct layers:

1. Bronze Layer (Raw Data Ingestion)
This is the initial landing zone for raw, untransformed data. Data is ingested as-is, preserving its original format and history.

Notebooks:
01_Primeira_Camada.ipynb: Sets up the initial environment and databases.
02_Tabela_Bronze_Clientes.ipynb: Ingests raw customer data into the Bronze layer.
03_Tabela_Bronze_Produtos.ipynb: Ingests raw product data into the Bronze layer.
04_Tabela_Bronze_Transacoes.ipynb: Ingests raw transaction data into the Bronze layer.
2. Silver Layer (Cleaned & Conformed Data)
In this layer, raw data from the Bronze layer undergoes cleaning, filtering, and basic transformations. Data is structured, de-duplicated, and conformed to common standards, preparing it for deeper analysis.

Notebooks:
05_Segunda_Camada.ipynb: Prepares the environment for the Silver layer.
06_Tabela_Silver_Clientes.ipynb: Cleans and transforms customer data, moving it to the Silver layer.
07_Tabela_Silver_Produtos.ipynb: Cleans and transforms product data, moving it to the Silver layer.
08_Tabela_Silver_Transacoes.ipynb: Cleans and transforms transaction data, moving it to the Silver layer.
3. Gold Layer (Business-Ready Data)
The Gold layer contains highly refined, aggregated, and enriched data, optimized for specific business use cases. This data is suitable for direct consumption by business users, data scientists, and reporting tools. It often involves joins between different Silver tables and the creation of aggregated metrics.

Notebooks:
09_Camada_Final.ipynb: Prepares the environment for the Gold layer.
10_Tabela_Gold.ipynb: Consolidates and enriches data from the Silver layer to create the final business-ready tables (e.g., customer segments, product performance, aggregated transactions).
Key Technologies Used
Databricks: Unified analytics platform used for running all notebooks and managing the data pipeline.
Apache Spark: Powering the data processing and transformations within Databricks.
Delta Lake: Providing ACID transactions, scalable metadata handling, and data versioning for reliable data lakes.
SQL/Python: Used for data manipulation, cleaning, and querying within the notebooks.
What Can Be Analyzed
After running the complete pipeline, the Gold layer tables provide a rich dataset for various analytical purposes, including but not limited to:

Customer Segmentation: Analyze dsa_gold_table_segmentos_clientes to understand different customer groups based on their purchasing behavior and other attributes.
Product Performance: Evaluate product sales, popularity, and other metrics from the aggregated product data.
Transaction Trends: Identify patterns, peak seasons, and other insights from the consolidated transaction data.
Business Intelligence Reporting: The Gold tables are ideal for building dashboards and reports in BI tools.
Machine Learning Model Training: The clean and enriched data serves as an excellent foundation for training ML models for tasks such as churn prediction, recommendation systems, or sales forecasting.
How to Run the Project
Databricks Workspace: Ensure you have access to a Databricks workspace.
Import Notebooks: Import all .ipynb files into your Databricks workspace.
Configure Cluster: Attach the notebooks to a Databricks cluster (ensure it has the necessary runtime for Delta Lake).
Execute Notebooks Sequentially: Run the notebooks in numerical order (01_... to 10_...). Each notebook builds upon the previous one, creating and refining the data layers.Project Overview
This project focuses on building an automated data pipeline using Databricks to consolidate, clean, and enrich raw data. The goal is to transform disparate raw data into a structured and valuable format, ready for advanced analytics, Business Intelligence (BI), and Machine Learning (ML) applications. The pipeline adheres to the Medallion Architecture (Bronze, Silver, Gold layers), ensuring data quality, reliability, and accessibility.

What Was Done
The project implements a robust data pipeline, moving data through three distinct layers:

1. Bronze Layer (Raw Data Ingestion)
This is the initial landing zone for raw, untransformed data. Data is ingested as-is, preserving its original format and history.

Notebooks:
01_Primeira_Camada.ipynb: Sets up the initial environment and databases.
02_Tabela_Bronze_Clientes.ipynb: Ingests raw customer data into the Bronze layer.
03_Tabela_Bronze_Produtos.ipynb: Ingests raw product data into the Bronze layer.
04_Tabela_Bronze_Transacoes.ipynb: Ingests raw transaction data into the Bronze layer.
2. Silver Layer (Cleaned & Conformed Data)
In this layer, raw data from the Bronze layer undergoes cleaning, filtering, and basic transformations. Data is structured, de-duplicated, and conformed to common standards, preparing it for deeper analysis.

Notebooks:
05_Segunda_Camada.ipynb: Prepares the environment for the Silver layer.
06_Tabela_Silver_Clientes.ipynb: Cleans and transforms customer data, moving it to the Silver layer.
07_Tabela_Silver_Produtos.ipynb: Cleans and transforms product data, moving it to the Silver layer.
08_Tabela_Silver_Transacoes.ipynb: Cleans and transforms transaction data, moving it to the Silver layer.
3. Gold Layer (Business-Ready Data)
The Gold layer contains highly refined, aggregated, and enriched data, optimized for specific business use cases. This data is suitable for direct consumption by business users, data scientists, and reporting tools. It often involves joins between different Silver tables and the creation of aggregated metrics.

Notebooks:
09_Camada_Final.ipynb: Prepares the environment for the Gold layer.
10_Tabela_Gold.ipynb: Consolidates and enriches data from the Silver layer to create the final business-ready tables (e.g., customer segments, product performance, aggregated transactions).
Key Technologies Used
Databricks: Unified analytics platform used for running all notebooks and managing the data pipeline.
Apache Spark: Powering the data processing and transformations within Databricks.
Delta Lake: Providing ACID transactions, scalable metadata handling, and data versioning for reliable data lakes.
SQL/Python: Used for data manipulation, cleaning, and querying within the notebooks.
What Can Be Analyzed
After running the complete pipeline, the Gold layer tables provide a rich dataset for various analytical purposes, including but not limited to:

Customer Segmentation: Analyze dsa_gold_table_segmentos_clientes to understand different customer groups based on their purchasing behavior and other attributes.
Product Performance: Evaluate product sales, popularity, and other metrics from the aggregated product data.
Transaction Trends: Identify patterns, peak seasons, and other insights from the consolidated transaction data.
Business Intelligence Reporting: The Gold tables are ideal for building dashboards and reports in BI tools.
Machine Learning Model Training: The clean and enriched data serves as an excellent foundation for training ML models for tasks such as churn prediction, recommendation systems, or sales forecasting.
How to Run the Project
Databricks Workspace: Ensure you have access to a Databricks workspace.
Import Notebooks: Import all .ipynb files into your Databricks workspace.
Configure Cluster: Attach the notebooks to a Databricks cluster (ensure it has the necessary runtime for Delta Lake).
Execute Notebooks Sequentially: Run the notebooks in numerical order (01_... to 10_...). Each notebook builds upon the previous one, creating and refining the data layers.
