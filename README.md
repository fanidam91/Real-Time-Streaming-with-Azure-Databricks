Real-time Data Processing with Azure Databricks (and Event Hubs)
This notebook demonstrates the below architecture to build real-time data pipelines. Solution Architecture
<img width="574" height="207" alt="Screenshot 2025-09-01 234024" src="https://github.com/user-attachments/assets/289cacb2-7c2b-4484-8000-4bccc90441bf" />


Data Sources: Streaming data from IoT devices or social media feeds. (Simulated in Event Hubs)
Ingestion: Azure Event Hubs for capturing real-time data.
Processing: Azure Databricks for stream processing using Structured Streaming.
Storage: Processed data stored Azure Data Lake (Delta Format).
Visualisation: Data visualized using Power BI.
Azure Services Required
Databricks Workspace (Unity Catalog enabled)
Azure Data Lake Storage (Premium)
Azure Event Hub (Basic Tier)
Azure Databricks Configuration Required
Single Node Compute Cluster: 12.2 LTS (includes Apache Spark 3.3.2, Scala 2.12)
Maven Library installed on Compute Cluster: com.microsoft.azure:azure-eventhubs-spark_2.12:2.3.22
