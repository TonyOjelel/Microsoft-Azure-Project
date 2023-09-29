You can create such a diagram using various diagramming tools or software like Microsoft Visio, Lucidchart, draw.io, or even hand-draw it on paper.

Here's a textual representation of a simple data flow diagram for the project:

```
        +-------------------+        +-----------------------+
        |    Xero API      |        |   Unleashed API       |
        +--------+----------+        +-----------+-----------+
                 |                             |
                 |                             |
                 v                             v
        +--------+----------+        +-----------+-----------+
        | Azure Data Factory|        | Azure Data Factory    |
        |   Data Ingestion  |        |   Data Ingestion      |
        +--------+----------+        +-----------+-----------+
                 |                             |
                 |                             |
                 v                             v
        +--------+----------+        +-----------+-----------+
        |Azure Data Lake    |        |Azure Data Lake Storage|
        |   Storage         |        |                       |
        +--------+----------+        +-----------+-----------+
                 |                             |
                 |                             |
                 v                             v
        +--------+----------+        +-----------+-----------+
        |Azure SQL Database |        |Azure SQL Database     |
        |   Data Warehouse  |        |                       |
        +-------------------+        +-----------------------+
                 |                             |
                 |                             |
                 v                             v
        +-------------------+        +-----------------------+
        |   Power BI        |        |   Excel               |
        |   Data Analysis   |        |   Data Analysis       |
        +-------------------+        +-----------------------+
```

In this diagram:

- Data is collected from Xero and Unleashed using Azure Data Factory for data ingestion.
- The data is stored in Azure Data Lake Storage for further processing.
- Azure SQL Database or Data Warehouse is used for structured data storage.
- Power BI and Excel are connected to Azure SQL Database/Data Warehouse for data analysis and reporting.

You can use a diagramming tool to create a visual representation of this data flow according to your project's specific architecture and requirements.