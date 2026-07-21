---
title: "Worklog Week 7"
date: 2026-07-10
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---


### Objectives for Week 7:

* Understand database services on AWS.
* Learn about Amazon RDS, Aurora, DynamoDB, and ElastiCache.
* Understand how applications connect to databases and how to choose a database based on requirements.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Study the overview of databases on AWS.<br>- Review relational database, NoSQL database, cache, and database migration concepts. | 01/06/2026 | 01/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000006.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html |
| Tuesday | - Learn about Amazon RDS and Amazon Aurora.<br>- Take notes on DB engine, DB instance class, storage, backup, Multi-AZ, and DB Subnet Group. | 02/06/2026 | 02/06/2026 | https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html<br>https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html |
| Wednesday | - Learn the steps to create an RDS database instance.<br>- Learn about Security Group for database and how to allow EC2/Application to connect to RDS. | 03/06/2026 | 03/06/2026 | https://000005.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_VPC.WorkingWithRDSInstanceinaVPC.html |
| Thursday | - Learn about Amazon DynamoDB.<br>- Take notes on Partition Key, Sort Key, Item, Attribute, Scan/Query, and the use case for review history data. | 04/06/2026 | 04/06/2026 | https://000039.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html |
| Friday | - Learn about Amazon ElastiCache and the role of caching.<br>- Compare RDS, DynamoDB, and ElastiCache at an overview level.<br>- Summarize why DynamoDB is suitable for storing review history in the project. | 05/06/2026 | 05/06/2026 | https://docs.aws.amazon.com/AmazonElastiCache/latest/dg/WhatIs.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html |

### Lab implementation steps for Week 7:

* Prepare VPC, subnets, and Security Group for the database lab.
* Create a DB Subnet Group that includes subnets in multiple Availability Zones if the lab requires it.
* Create a Security Group for RDS and only allow connections from the Security Group of EC2 or the application.
* Create an RDS database instance, choose a suitable engine such as MySQL or MariaDB, and configure username/password and storage.
* Check the RDS endpoint and try connecting from EC2 or a demo application.
* Learn basic RDS backup, snapshot, and restore.
* Open the DynamoDB Console and create a test table with a suitable Partition Key.
* Add items, view items, try basic Scan/Query operations, and observe how data is stored in key-value/document format.
* Summarize why DynamoDB is suitable for review history data in the project.

### Results achieved in Week 7:

* Understood the difference between relational database and NoSQL database.
* Understood the basic components required when creating RDS.
* Understood how Security Group affects database connectivity.
* Learned that DynamoDB is suitable for storing metadata, status, and review history.
* Prepared the foundation for using DynamoDB in the AI AWS Architecture Reviewer system.


---