# EX-07-Overview-of-DynamoDB-in-AWS

## Aim
To understand and perform basic operations in Amazon DynamoDB, including table creation, item insertion, querying, and experimenting with simple data operations using the AWS SDK.

---

## Objectives
1. Set up an Amazon DynamoDB table.
2. Perform basic CRUD (Create, Read, Update, Delete) operations in DynamoDB.
3. Explore querying and scanning techniques.
4. Use the AWS SDK to interact with DynamoDB programmatically.

---

## Introduction
Amazon DynamoDB is a fully managed NoSQL database service provided by AWS. It's designed for high-performance applications requiring low-latency access to large volumes of data, making it ideal for use cases like web applications, IoT, and mobile backends. DynamoDB offers flexibility with its schema-less design and supports both key-value and document data structures.

---

## Required Tools
- AWS Account with DynamoDB access.
- AWS Management Console for web-based interactions.
- [AWS SDK for Python (Boto3)](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) for programmatic access.

---

## Instructions

### 1. Setting Up the Environment
   - Log into the AWS Management Console.
   - Navigate to **DynamoDB** under the **Database** section.

![db0](https://github.com/user-attachments/assets/3396a860-f7c0-4658-a100-1d112ba2003e)


### 2. Creating a Table in DynamoDB
   - Go to **Create Table**.
   - Enter a **Table Name**, such as `ExperimentTable`.
   - Define the **Partition Key** (e.g., `ItemID`) and optionally a **Sort Key** (e.g., `Timestamp`).
   - Configure **Read/Write Capacity** settings based on expected load.
   - Click on **Create Table** to finalize.

<img width="1163" alt="db1" src="https://github.com/user-attachments/assets/8777b591-5063-4ab5-a6fc-42ed7c33cbde">


### 3. Inserting Items
   - Select the created table and go to the **Items** tab.
   - Click on **Create Item**.
   - Add attributes such as `ItemID`, `Description`, `Status`, etc.
   - Click **Save** to store the item.

![db4](https://github.com/user-attachments/assets/1d6ff9d8-f5f4-459b-baf9-dcb0718f249f)



### 4. Querying Data
   - Navigate to the **Items** tab of your table.
   - Click **Query** to search by the primary key.
   - Specify filters (e.g., by `Status` or `Timestamp`) for more refined results.

![db2](https://github.com/user-attachments/assets/fe452d2b-8c4f-43d0-91a5-1058bab4bb29)


### 5. Experimenting with Advanced Features
Global Secondary Indexes (GSI): Set up GSIs for querying non-primary attributes.
DynamoDB Streams: Enable streams to capture and process real-time changes.
Auto Scaling: Configure read/write auto-scaling for dynamic workloads.

### RESULTS

  Successfully create a DynamoDB table and manage data entries, Efficiently use DynamoDB’s querying and filtering options to retrieve data.
