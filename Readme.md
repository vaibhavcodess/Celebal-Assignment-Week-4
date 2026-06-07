# Azure ETL Superstore Pipeline

This project is a basic end-to-end ETL pipeline built using Azure Data Factory and Azure Blob Storage.

The pipeline takes a CSV file from a source blob container, checks the file metadata, and copies the file into another blob container using Azure Data Factory activities.

## Services Used

* Azure Resource Group
* Azure Storage Account
* Azure Blob Containers
* Azure Data Factory
* IAM Role Assignment

## Dataset

Dataset used:

* Superstore Sales CSV Dataset

## Workflow

1. Created a Resource Group in Azure
2. Created a Storage Account
3. Created two Blob Containers:

   * source-container
   * destination-container
4. Uploaded CSV file into source-container
5. Created Azure Data Factory
6. Connected Blob Storage using Linked Service
7. Created Source and Destination datasets
8. Added Get Metadata activity
9. Added Copy Data activity
10. Executed and monitored the pipeline

## Pipeline Flow

```text id="6jlwmv"
Source CSV File
      ↓
Get Metadata Activity
      ↓
Copy Data Activity
      ↓
Destination Container
```

## Output

The pipeline successfully copied the CSV file from the source container to the destination container.

## Screenshots

Project screenshots are available as .png images.

## Author

Vaibhav Singh
