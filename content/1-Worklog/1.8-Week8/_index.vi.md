---
title: "Worklog Tuần 8"
date: 2026-07-10
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---


### Mục tiêu tuần 8:

* Hiểu giám sát, vận hành và tối ưu hệ thống trên AWS.
* Tìm hiểu CloudWatch Logs, CloudWatch Alarms, SNS, Resource Tags, AWS Budgets và Cost Management.
* Biết cách dùng log và alarm để theo dõi hệ thống serverless.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Học tổng quan về vận hành hệ thống trên AWS.<br>- Tìm hiểu CloudWatch Metrics, CloudWatch Logs và CloudWatch Dashboard. | 08/06/2026 | 08/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html |
| 3 | - Tìm hiểu CloudWatch Alarms và cách đặt ngưỡng cảnh báo.<br>- Ghi chú các chỉ số thường theo dõi: errors, duration, invocations, throttles, CPU và memory. | 09/06/2026 | 09/06/2026 | https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/AlarmThatSendsEmail.html |
| 4 | - Tìm hiểu Amazon SNS và cách gửi thông báo khi có sự kiện hoặc alarm.<br>- Ghi chú mô hình CloudWatch Alarm → SNS → Email notification. | 10/06/2026 | 10/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/sns/latest/dg/welcome.html |
| 5 | - Tìm hiểu Resource Tags, Resource Groups và cách dùng tag để tổ chức tài nguyên.<br>- Ghi chú tag theo project, environment, owner và cost center. | 11/06/2026 | 11/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/tag-editor/latest/userguide/tagging.html |
| 6 | - Tìm hiểu AWS Budgets, Cost Management và hướng tối ưu chi phí.<br>- Ghi chú các hướng: right-sizing, tắt tài nguyên không dùng, kiểm soát data transfer và dùng storage class phù hợp. | 12/06/2026 | 12/06/2026 | https://docs.aws.amazon.com/cost-management/latest/userguide/what-is-costmanagement.html |

### Các bước thực hiện lab trong tuần 8:

* Vào CloudWatch Console để xem Metrics của các tài nguyên đã tạo như EC2, Lambda hoặc S3 nếu có dữ liệu.
* Mở CloudWatch Logs để kiểm tra log group và log stream của Lambda hoặc dịch vụ liên quan.
* Tạo CloudWatch Alarm mẫu dựa trên một metric phù hợp như Lambda Errors hoặc EC2 CPUUtilization.
* Tạo SNS Topic, thêm email subscription và xác nhận email subscription.
* Kết nối CloudWatch Alarm với SNS Topic để gửi thông báo khi alarm chuyển trạng thái.
* Gắn tag cho tài nguyên theo các khóa như Project, Environment, Owner hoặc CostCenter.
* Tìm hiểu AWS Budgets và tạo budget cảnh báo chi phí nếu cần.
* Tổng hợp các cách tối ưu chi phí: tắt tài nguyên không dùng, right-sizing, kiểm soát data transfer và dọn dẹp tài nguyên sau lab.

### Kết quả đạt được tuần 8:

* Hiểu CloudWatch là dịch vụ quan trọng để giám sát tài nguyên và ứng dụng.
* Nắm được cách CloudWatch Logs hỗ trợ debug Lambda.
* Hiểu cách SNS có thể dùng để gửi thông báo qua email.
* Biết dùng tag để tổ chức và quản lý tài nguyên theo project.
* Nắm được các nguyên tắc tối ưu chi phí cơ bản khi học và thực hành AWS.


---
