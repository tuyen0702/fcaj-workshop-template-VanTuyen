---
title: "Worklog Tuần 5"
date: 2026-07-10
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---


### Mục tiêu tuần 5:

* Hiểu cách phân phối nội dung website bằng Amazon CloudFront.
* Tìm hiểu thêm Lightsail, EC2 Auto Scaling, CloudWatch và các dịch vụ hỗ trợ triển khai ứng dụng.
* Biết cách kết hợp S3 Static Website với CloudFront trong mô hình frontend.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Học về Content Delivery Network và vai trò của Amazon CloudFront.<br>- Tìm hiểu Edge Location, cache, origin và distribution. | 18/05/2026 | 18/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000058.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html |
| 3 | - Tìm hiểu cách dùng CloudFront với S3 Static Website.<br>- Ghi chú origin domain, default root object, cache behavior và HTTPS endpoint. | 19/05/2026 | 19/05/2026 | https://000058.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/website-hosting-cloudfront-walkthrough.html |
| 4 | - Tìm hiểu Amazon Lightsail và trường hợp dùng Lightsail để triển khai nhanh ứng dụng.<br>- So sánh EC2 và Lightsail ở mức tổng quan. | 20/05/2026 | 20/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/lightsail/latest/userguide/what-is-amazon-lightsail.html |
| 5 | - Tìm hiểu EC2 Auto Scaling và khái niệm scaling ứng dụng.<br>- Ghi chú Launch Template, Auto Scaling Group, scaling policy và health check. | 21/05/2026 | 21/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html |
| 6 | - Tìm hiểu CloudWatch cơ bản để theo dõi tài nguyên.<br>- Tổng hợp vai trò của S3, CloudFront, EC2/Lightsail và CloudWatch trong mô hình web app. | 22/05/2026 | 22/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html |

### Các bước thực hiện lab trong tuần 5:

* Chuẩn bị một S3 bucket đã có website tĩnh hoặc một origin có thể truy cập được.
* Vào CloudFront Console và tạo Distribution mới.
* Cấu hình Origin Domain trỏ về S3 website endpoint hoặc S3 bucket origin theo yêu cầu lab.
* Cấu hình Default cache behavior, Viewer protocol policy và Allowed HTTP methods.
* Thiết lập Default root object là index.html nếu dùng website tĩnh.
* Chờ distribution chuyển sang trạng thái Deployed, sau đó truy cập CloudFront domain để kiểm tra website.
* Kiểm tra cache bằng cách thay đổi file trong S3 và quan sát thời gian cập nhật trên CloudFront.
* Tìm hiểu thêm Lightsail để triển khai ứng dụng nhanh và EC2 Auto Scaling để mở rộng số lượng instance khi tải tăng.
* Tổng hợp các chỉ số CloudWatch cần theo dõi khi website được phân phối qua CloudFront.

### Kết quả đạt được tuần 5:

* Hiểu được CloudFront giúp phân phối nội dung gần người dùng hơn thông qua edge locations.
* Nắm được khái niệm origin, distribution và cache behavior.
* Biết cách kết hợp S3 và CloudFront để host frontend tĩnh.
* Hiểu ở mức tổng quan vai trò của Lightsail, Auto Scaling và CloudWatch.
* Chuẩn bị được nền tảng cho phần triển khai frontend đồ án sau này.


---