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
| 2 | - Học tổng quan về database trên AWS.<br>- Ôn lại các khái niệm relational database, NoSQL database, cache và database migration. | 01/06/2026 | 01/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000006.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html |
| 3 | - Tìm hiểu Amazon RDS và Amazon Aurora.<br>- Ghi chú DB engine, DB instance class, storage, backup, Multi-AZ và DB Subnet Group. | 02/06/2026 | 02/06/2026 | https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html<br>https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html |
| 4 | - Tìm hiểu các bước tạo RDS database instance.<br>- Tìm hiểu Security Group cho database và cách cho phép EC2/Application kết nối tới RDS. | 03/06/2026 | 03/06/2026 | https://000005.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_VPC.WorkingWithRDSInstanceinaVPC.html |
| 5 | - Tìm hiểu Amazon DynamoDB.<br>- Ghi chú Partition Key, Sort Key, Item, Attribute, Scan/Query và use case cho dữ liệu lịch sử review. | 04/06/2026 | 04/06/2026 | https://000039.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html |
| 6 | - Tìm hiểu Amazon ElastiCache và vai trò của caching.<br>- So sánh RDS, DynamoDB và ElastiCache ở mức tổng quan.<br>- Tổng hợp lựa chọn DynamoDB cho phần lưu lịch sử review trong đồ án. | 05/06/2026 | 05/06/2026 | https://docs.aws.amazon.com/AmazonElastiCache/latest/dg/WhatIs.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html |

### Các bước thực hiện lab trong tuần 7:

* Chuẩn bị VPC, subnet và Security Group cho bài lab database.
* Tạo DB Subnet Group gồm các subnet thuộc nhiều Availability Zone nếu lab yêu cầu.
* Tạo Security Group cho RDS, chỉ cho phép kết nối từ Security Group của EC2 hoặc ứng dụng.
* Tạo RDS database instance, chọn engine phù hợp như MySQL hoặc MariaDB, cấu hình username/password và storage.
* Kiểm tra endpoint của RDS và thử kết nối từ EC2 hoặc ứng dụng demo.
* Tìm hiểu backup, snapshot và restore của RDS ở mức cơ bản.
* Vào DynamoDB Console, tạo table thử nghiệm với Partition Key phù hợp.
* Thêm item, xem item, thử Scan/Query cơ bản và quan sát cách dữ liệu được lưu dưới dạng key-value/document.
* Tổng hợp lý do DynamoDB phù hợp cho dữ liệu lịch sử review trong đồ án.

### Kết quả đạt được tuần 7:

* Hiểu được sự khác nhau giữa relational database và NoSQL database.
* Nắm được các thành phần cơ bản khi tạo RDS.
* Hiểu cách Security Group ảnh hưởng đến kết nối database.
* Biết DynamoDB phù hợp để lưu metadata, trạng thái và lịch sử review.
* Chuẩn bị được cơ sở để dùng DynamoDB trong hệ thống AI AWS Architecture Reviewer.


---