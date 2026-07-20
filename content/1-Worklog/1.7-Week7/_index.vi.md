---
title: "Worklog Tuần 7"
date: 2026-07-10
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---


### Mục tiêu tuần 7:

* Hiểu các dịch vụ cơ sở dữ liệu trên AWS.
* Tìm hiểu Amazon RDS, Aurora, DynamoDB và ElastiCache.
* Nắm được cách kết nối ứng dụng với database và cách chọn database theo nhu cầu.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Học tổng quan về database trên AWS.<br>- Ôn lại các khái niệm relational database, NoSQL database, cache và data migration. | 01/06/2026 | 01/06/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html |
| 3 | - Tìm hiểu Amazon RDS và Amazon Aurora.<br>- Ghi chú DB engine, DB instance class, storage, backup, Multi-AZ và DB Subnet Group. | 02/06/2026 | 02/06/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html |
| 4 | - Tìm hiểu các bước tạo RDS database instance.<br>- Tìm hiểu Security Group cho database và cách cho phép EC2/Application kết nối tới RDS. | 03/06/2026 | 03/06/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html |
| 5 | - Tìm hiểu Amazon DynamoDB.<br>- Ghi chú Partition Key, Sort Key, Item, Attribute, scan/query và use case cho dữ liệu lịch sử review. | 04/06/2026 | 04/06/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html |
| 6 | - Tìm hiểu Amazon ElastiCache và vai trò của caching.<br>- So sánh RDS, DynamoDB và ElastiCache ở mức tổng quan.<br>- Tổng hợp lựa chọn DynamoDB cho phần lưu lịch sử review trong đồ án. | 05/06/2026 | 05/06/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html |

### Gợi ý các bước thực hiện lab trong tuần 7:

* Create a VPC for database lab.
* Create EC2 Security Group.
* Create RDS Security Group.
* Create DB Subnet Group.
* Create RDS database instance.
* Review application deployment connecting to database.
* Explore DynamoDB console.
* Review DynamoDB backup and design patterns.

### Kết quả đạt được tuần 7:

* Hiểu được sự khác nhau giữa relational database và NoSQL database.
* Nắm được các thành phần cơ bản khi tạo RDS.
* Hiểu cách Security Group ảnh hưởng đến kết nối database.
* Biết DynamoDB phù hợp để lưu metadata, trạng thái và lịch sử review.
* Chuẩn bị được cơ sở để dùng DynamoDB trong hệ thống AI AWS Architecture Reviewer.


---