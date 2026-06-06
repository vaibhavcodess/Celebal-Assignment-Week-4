This assignment demonstrates an end-to-end Azure Data Engineering pipeline using Azure Storage Account and Azure Data Factory (ADF).

First, a Resource Group and Azure Storage Account were created in the Azure Portal. Two Blob Containers named source-container and destination-container were created. The Superstore CSV dataset was uploaded into the source-container.

Azure Data Factory was then created to build the data pipeline. A Linked Service was configured to establish connectivity between ADF and Azure Blob Storage. Source and destination datasets were created using DelimitedText format for handling the CSV file.

A pipeline named pl_superstore_pipeline was developed using two activities:

1. Get Metadata activity – used to validate file existence and retrieve file information.
2. Copy Data activity – used to copy the CSV file from source-container to destination-container.

The pipeline was executed successfully using Debug mode, and execution was monitored through the Monitor tab in ADF Studio. IAM roles such as Reader and Contributor were also assigned to ensure proper access control between services.

The final output confirmed successful metadata validation and file transfer from source to destination container in Azure Blob Storage.
