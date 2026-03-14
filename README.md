1️⃣ Real-Time Stock Market Data Analytics Pipeline
Project Overview

This project implements a real-time stock market analytics pipeline using serverless and event-driven cloud services. The system ingests stock market data in real time, processes the data to detect trends, stores structured records for quick lookup, and sends notifications when specific conditions are met.

The architecture is designed to be scalable, automated, and cost-efficient.

AWS Services Used

Amazon Kinesis Data Streams – Ingests real-time stock data.

AWS Lambda – Processes incoming stock events.

Amazon DynamoDB – Stores structured stock records.

Amazon S3 – Stores raw stock data for historical analysis.

Amazon Athena – Queries data stored in S3.

Amazon Simple Notification Service – Sends alerts via email/SMS.

AWS Identity and Access Management – Manages permissions.

Architecture

Workflow of the system:

Stock Data Producer
        ↓
Kinesis Data Stream
        ↓
Lambda Function
        ↓
DynamoDB (Store Processed Data)
        ↓
SNS (Send Alerts)

Raw Data → S3 → Athena (Query for Analysis)
Features

Real-time data ingestion

Event-driven processing

Serverless architecture

Historical data analysis

Automated notifications

2️⃣ End-to-End Serverless Data Pipeline
Project Overview

This project demonstrates how to build a fully automated serverless data pipeline on AWS. Raw CSV data is uploaded to cloud storage, automatically processed and cataloged, and then visualized using a business intelligence dashboard.

The pipeline enables data transformation, querying, and visualization without managing servers.

AWS Services Used

Amazon S3 – Stores raw datasets.

AWS Lambda – Triggers workflow automation.

AWS Glue – Runs crawlers and ETL jobs to prepare data.

Amazon Athena – Queries processed datasets.

Amazon QuickSight – Builds dashboards for data visualization.

AWS Identity and Access Management – Manages roles and permissions.

Architecture
CSV Upload
    ↓
Amazon S3
    ↓
Lambda Trigger
    ↓
AWS Glue Crawler
    ↓
AWS Glue ETL Job
    ↓
Amazon Athena Query
    ↓
Amazon QuickSight Dashboard
Features

Automated data ingestion

ETL data transformation

Serverless data analytics pipeline

SQL-based data querying

Interactive business dashboards
3️⃣ Automated Receipt Processing System
Project Overview

This project builds an automated receipt processing system using cloud AI and serverless services. When a receipt image or PDF is uploaded, the system automatically extracts structured information such as store name, total amount, tax, and purchase date.

The extracted data is stored in a database and a notification email is sent once processing is completed.

AWS Services Used

Amazon S3 – Stores uploaded receipt images and PDFs.

AWS Lambda – Automates the workflow.

Amazon Textract – Extracts structured text from receipts.

Amazon DynamoDB – Stores extracted receipt information.

Amazon Simple Email Service – Sends email notifications after processing.

AWS Identity and Access Management – Handles permissions.

Architecture
Receipt Upload
     ↓
Amazon S3
     ↓
Lambda Trigger
     ↓
Amazon Textract
     ↓
Extracted Data
     ↓
DynamoDB
     ↓
Email Notification (SES)
Features

Automated receipt data extraction

OCR-based document processing

Event-driven automation

Structured data storage

Email notifications
