---
title: "Worklog Tuần 9"
date: 2026-07-10
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Mục tiêu tuần 9:

* Bắt đầu tìm hiểu và xác định hướng thực hiện đồ án nhóm.
* Phân tích yêu cầu hệ thống và lựa chọn đề tài AI AWS Architecture Reviewer.
* Xác định các dịch vụ AWS chính cần sử dụng trong kiến trúc đồ án.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Họp nhóm bắt đầu giai đoạn làm đồ án.<br>- Trao đổi các hướng đề tài có thể triển khai trên AWS.<br>- Thống nhất tập trung vào bài toán hỗ trợ phân tích sơ đồ kiến trúc AWS bằng AI. | 15/06/2026 | 15/06/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html |
| 3 | - Phân tích yêu cầu hệ thống AI AWS Architecture Reviewer.<br>- Xác định input là ảnh sơ đồ kiến trúc và output là kết quả review, cost estimation và report.<br>- Ghi chú các chức năng chính: upload diagram, analyze architecture, estimate cost, generate report, view history. | 16/06/2026 | 16/06/2026 | https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://docs.aws.amazon.com/lambda/latest/dg/welcome.html |
| 4 | - Nghiên cứu các dịch vụ phù hợp cho frontend/backend.<br>- Lựa chọn S3 + CloudFront cho frontend, API Gateway + Lambda cho backend upload, DynamoDB cho lịch sử review. | 17/06/2026 | 17/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/website-hosting-cloudfront-walkthrough.html<br>https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html<br>https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html |
| 5 | - Tìm hiểu EventBridge và Step Functions cho workflow tự động.<br>- Ghi chú luồng S3 Object Created → EventBridge → Step Functions → Lambda processing. | 18/06/2026 | 18/06/2026 | https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-what-is.html<br>https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html |
| 6 | - Tìm hiểu Amazon Bedrock và khả năng dùng model AI để phân tích ảnh kiến trúc.<br>- Xác định các Lambda xử lý chính: AI Analyzer, Cost Tool, PDF Generator.<br>- Tổng hợp kiến trúc dự kiến của đồ án. | 19/06/2026 | 19/06/2026 | https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/aws-cost-management/latest/APIReference/Welcome.html |

### Gợi ý các bước thực hiện lab trong tuần 9:

* Review Serverless Automation with AWS Lambda.
* Review API Gateway and Lambda integration.
* Review EventBridge event-driven architecture.
* Review Step Functions workflow orchestration.
* Review Amazon Bedrock for AI-based analysis.
* Review DynamoDB as metadata/history storage.

### Kết quả đạt được tuần 9:

* Nhóm đã xác định đề tài AI AWS Architecture Reviewer.
* Xác định được input/output và các chức năng chính của hệ thống.
* Lựa chọn được các dịch vụ AWS chính cho kiến trúc.
* Xây dựng được luồng xử lý tổng quan từ upload đến tạo báo cáo.
* Chuẩn bị được nền tảng để chia việc và triển khai ở tuần tiếp theo.


---