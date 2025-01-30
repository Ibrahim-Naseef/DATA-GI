# Git

**Git** is a version control system which is used to track changes made in a code or file.

- Track history
- Collaborators
- Fast and Secure

## Configuring Git

It is used to set username and mail so we can keep track that changes can be made from diffrent mail id.

- git config --global user.name "Name"
- git config --global user.mail "Mail@"
- git config list

## Git Commands

- **clone** : used to download repo from github to local machine
  `git clone <link>

- **status** : displays staus of code or file

  1. untracked : new files which are not added
  2. modified : file that content are changed
  3. staged : file is ready to be commited
  4. unmodified : didnt change any content of file

- **add** : To add the modified file to staged state
  `git add <file>`

- **commit** : Keeps records of all changes
  `git commit -m <message>`

- **push** : Upload local changes made in repo to remote repo
  `git push origin main`

- **pull** : pull chnaged remote repo into the local
  `git pull origin main`

- **Pull request** : This is done manually in github.In this the user can check who made changes and iis it useful and then he can merge.

- **Fork** : To copy the other user repo and edit it.

## To create new Repo in Local and Upload it to Remote Repo

1. Create a new Repo. `mkdir NewRepo`
2. Change directory to that new Repo. `cd Newrepo`
3. Run `git init` command to initialize it as an Git Repository
4. Add files that are required.
5. Make a new repo in github
6. Run `git remote add origin <-git repo link->` to add to remote system.
7. Run `git remote -v` to confirm the path

## Git Branches

Git Branches are useful when multiple developers works on same Project to add diffrent features wuthout interrupting/waiting other developers to complete their work

- `git branch` : Lists all the availible branches of repo.
- `git checkout <-BranchName->` : To Switch between Branches
- `git checkout -b <-Branch Name->` : To create new Branch and swicth to that Branch.
- `git branch -d` : To Delete a Branch
- `git diff <-BranchName->` : Comapres the diffrence between 2 Repository

## Git Merge

It is used to combine the changes made in one branch to the main bracnch

- `git merge <-Branch Name->` : Combine the present brach with mentioned branch
- **Merge Conflict** : It occurs when same line is chnaged in 2 branches and we try to merge it.
  - Solution : Manually select original/new/both changes

---

# Azure Devops

It consist of a tools and services for software develpoment lifecycle management.

- End to End integration
- Scalibility
- Multi Platform Supports
- Security
- Extensibility

Main 5 types

1. Boards
2. Repos
3. Pipelines
4. Test Plans
5. Artifacts

1.**Boards**:

- Its a project Management tool for tracking work items,bugs and features
- We can assign task to any team members
- We can highlight task based on its priority

  2.**Repos**

- A version control system to manage code using git ot TFVC
- Code collaboration through Pull requsts
- Branch and Merge supports

  3.**Pipelines** :

- Its a CI/CD platform to build test, and deploy applications across multiple flatforms
- Supports Multiple Languages and platforms
- To Deploy the appplication

  4.**Test Plans**:

- A testing solution to plan,execute and track manual tests
- To check the application is working fine
- Test case management and Execution

  5.**Artifacts** :

- A repository for managing and sharing packages like NuGet,npm, Maven and Python
- Supports packets versioning
- Used to integrate with CI/CD pipelines

---

# Big Data

Big data refers to the massive datasets that are too large and cant be processed by using traditional data processing Methods.
It is characterized by 3V

1. Volume : Refers to large amount of data collected by various sources like social media, sensors, machine.
2. Velocity : It describes speed at which data is generated and processed
3. Variety : diffrent types of data formats such as text,images,videos and logs

## Types of data:

1. **Structured Data**
2. **Unstuctured Data**
3. **Semi-Stuctured Data**

4. **Structured Data**:
   It is highly organized and stored in a predefined format,making it easy to search and analyze.

- Follows tabular formats
- Easy searchable using SQL
- Predefined Data schema

2. **Unstuctured Data**:
   They lacks a predefined format making it harder to search and analyze.

- Do not follow a specific structure or schema
- Requires advanced tool like ML for analysis
- Eg: Emails,audio,images and video files

3. **Semi-Stuctured Data**:
   It comes between structured and unstructured data. It has some level of organization but lacks a strict schema, making it more flexible than structured data

- Does not conform to a rigid structure but contains tags or markers to separate elements
- Flexible, allowing data to evolve over time
- Eg : json,xml,log files from applications

## Tools and Technologies

It involves frameworks, platforms, and tools that help in processing and analyzing these massive datasets

1. **Distributed Storage**:

- Hadoop HDFS: For distributed storage
- Amazon S3, Google Cloud Storage, Azure Blob Storage

2. **Distributed Processing**:

- Apache Spark: In-memory distributed data processing
- Hadoop MapReduce: Batch processing framework

3. **Data Streaming**:

- Apache Kafka: For real-time data ingestion
- Apache Flink or Apache Storm: For stream processing

4. **Database Systems**:

- NoSQL: MongoDB, Cassandra, HBase
- SQL: Amazon Redshift, Google BigQuery

---

# Data Analytics

It is the process of examining datasets to uncover patterns, trends, and insights that can help in decision-making
It combines statistical techniques, tools, and technologies to analyze and interpret data

## Types of Data Analytics

1. **Descriptive Analytics**

- To summarize and describe historical data
- Key Question: "What happened?"
- Techniques: - Data visualization (charts, graphs, dashboards) - Summary statistics (mean, median, variance)
  -Example: A sales dashboard showing monthly revenue trends

2. **Diagnostic Analytics**

- To identify the causes of specific events or patterns
- Key Question: "Why did it happen?"
- Techniques:
  - Drill-down analysis
  - Correlation and regression analysis
- Example: Identifying why website traffic dropped in a specific month

3. **Predictive Analytics**

- To forecast future outcomes based on historical data
- Key Question: "What is likely to happen?"
- Techniques:
  - Machine learning models
  - Time series analysis
- Example: Predicting customer churn in a subscription-based business

4. **Prescriptive Analytics**

- To recommend actions to achieve desired outcomes
- Key Question: "What should we do?"
- Techniques:
  - Optimization algorithms
  - Scenario analysis
- Example: Suggesting the best pricing strategy to maximize profit

## Steps in the Data Analytics Process

1. **Data Collection**: Gathering raw data from various sources like databases, APIs, or sensors
2. **Data Cleaning**: Handling missing values, removing duplicates, and ensuring data consistency
3. **Data Exploration**: Using visualization and statistical methods to understand the data
4. **Data Analysis**: Applying techniques like clustering, classification, or regression
5. **Interpretation**: Deriving insights and making data-driven decisions
6. **Visualization and Reporting**: Presenting findings using dashboards or reports

---

# Data Pipeline

A data pipeline is a set of tools and processes for collecting, processing, and delivering data from one or more sources to a destination where it can be analyzed and used

## How it works

1. **Extract**: Data is extracted from various sources
2. **Transform**: The data is cleaned, enriched, or modified
3. **Load**: The data is stored in a data store, such as a data warehouse or data lake

## Types od Data pipelines

- **Batch pipelines**
  Collect large amounts of data and process it in chunks at scheduled intervals. This is useful when insights from large amounts of data aren't needed immediately.

- **Streaming data pipelines**
  Process data as soon as it becomes available. This is useful for applications that require immediate data processing, such as fraud detection

- **ETL pipelines**
  Extract raw data from various sources, transform it into a single format, and load it into a target system

- **ELT pipelines**
  Similar to ETL pipelines, but with a different sequence of steps. In ELT, data is first loaded into a target system and then transformed

---

# Devops

DevOps combines development (Dev) and operations (Ops) to increase the efficiency, speed, and security of software development and delivery compared to traditional processes

## How does DevOps work?

1. **Collaboration**
   DevOps encourages collaboration between development, IT operations, quality engineering, and security teams

2. **Automation**
   DevOps uses tools and practices to automate manual tasks, such as testing, to reduce errors and speed up delivery

3. **Continuous feedback**
   DevOps encourages a culture of continuous feedback so teams can quickly adapt and improve

4. **Security**
   DevOps uses tools like automated security testing to ensure software is secure throughout the development lifecycle

---

# DataOps

DataOps is a set of practices that improve the management of data by automating processes and encouraging collaboration
It's based on agile software engineering and DevOps practices

## Key Components of a DataOps Pipeline

- **Data Ingestion** : Extract data from multiple sources.
- **Data Transformation** : Clean, preprocess, and enrich data.
- **Data Validation** : Perform schema validation, quality checks, and unit testing.
- **Data Deployment** : Automate deployment of data models, dashboards, APIs.
- **Data Monitoring** : Ensure data reliability, consistency, and performance.

---

# Data Warehousing

## Introduction

It is the process of collecting, storing, and managing large volumes of structured data from multiple sources for analysis and reporting.

## Characteristics of Data Warehouses

- **Subject-Oriented**: Organizes data around key business areas like sales, finance, or marketing
- **Integrated**: Combines data from different sources into a consistent format
- **Time-Variant**: Maintains historical data to track changes over time
- **Non-Volatile**: Data is stable and does not change after being stored

## Data Warehouse Architecture

1. **Source Layer**: Extracts data from transactional systems, logs, and APIs
2. **ETL (Extract, Transform, Load) Process**: Extracts, transforms, and loads data into the warehouse
3. **Data Storage Layer**: Stores processed data in relational databases or data lakes
4. **Data Mart**: A subset of the data warehouse focused on a specific business function
5. **BI & Reporting Layer**: Provides tools for analysis, reporting, and visualization

## Types of Data Warehouses

- **Enterprise Data Warehouse (EDW)**: Centralized warehouse for the entire organization
- **Operational Data Store (ODS)**: Stores real-time operational data for short-term analysis
- **Data Marts**: Small-scale warehouse focusing on a specific department

---

# Data Lake

## Introduction

It is a centralized storage system that allows storing structured, semi-structured, and unstructured data at any scale
It enables data ingestion, storage, processing, and analytics in a flexible and scalable manner.

## Characteristics of Data Lakes

- **Scalability**: Can handle massive volumes of data
- **Schema-on-Read**: Data is stored in its raw format and structured when accessed
- **Multi-Format Support**: Stores structured, semi-structured, and unstructured data
- **Cost-Effective**: Uses cheap storage solutions like cloud-based object storage
- **Supports Advanced Analytics**: Integrates with AI, ML, and BI tools

## Data Lake Architecture

1. **Ingestion Layer**: Collects data from different sources (databases, IoT devices, APIs, logs, etc.)
2. **Storage Layer**: Stores raw data in distributed storage system
3. **Processing Layer**: Transforms data using big data frameworks like Apache Spark or Hadoop
4. **Analytics Layer**: Provides tools for reporting, machine learning, and business intelligence
5. **Access & Security Layer**: Manages data access, encryption, and governance policies

## Data Lake Zones

- **Raw Zone**: Stores raw, unprocessed data from various sources
- **Cleansed Zone**: Stores transformed and cleaned data for further processing
- **Curated Zone**: Stores structured data for business intelligence and analytics
- **Sandbox Zone**: Provides a workspace for data scientists and analysts to experiment

---

# AWS (Amazon Web Services)

## Introduction

It is a cloud computing platform that provides a wide range of scalable and on-demand cloud services, including computing power, storage, networking, databases, and security.

## Benefits of AWS

- **Scalability**
- **Cost-Effective**
- **Security**
- **Global Reach**
- **Flexibility**

## AWS Global Infrastructure

- **Regions**: Geographically isolated areas with multiple data centers
- **Availability Zones (AZs)**: Multiple, isolated locations within a region.
- **Edge Locations**: Used for caching and reducing latency (Content Delivery Network - CDN)

## Core AWS Services

1.  **AWS EC2 (Elastic Compute Cloud)**

- Virtual servers in the cloud.
- Scalable, pay-as-you-go.
- Supports different instance types.

2.  **AWS S3 (Simple Storage Service)**

- Object storage for any type of data.
- Multiple storage classes (Standard, IA, Glacier).
- Secure and scalable.

3.  **AWS IAM (Identity and Access Management)**

- Manages user access and permissions.
- Uses policies and roles for security.
- Multi-factor authentication (MFA) support.

4.  **AWS EBS (Elastic Block Store)**

- Persistent block storage for EC2.
- Supports SSD & HDD types.
- Snapshots for backup.

5.  **AWS EFS (Elastic File System)**

- Scalable file storage for multiple EC2 instances.
- Fully managed, automatic scaling.
- Supports NFS (Network File System).

6.  **AWS Glue**

- Managed ETL (Extract, Transform, Load) service.
- Used for data preparation and transformation.
- Serverless and integrates with AWS analytics.

7.  **AWS RDS (Relational Database Service)**

- Managed database service (MySQL, PostgreSQL, SQL Server, etc.).
- Automated backups and scaling.
- Multi-AZ for high availability.

8.  **AWS CloudWatch**

- Monitors AWS resources and applications.
- Provides logs, metrics, and alerts.
- Helps in troubleshooting and optimization.
