---
title: "Worklog Tuần 10"
date: 2026-07-10
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Mục tiêu tuần 10:

* Họp nhóm phân chia công việc cho từng thành viên.
* Thiết kế kiến trúc tổng thể cho đồ án và phân tách backend/frontend.
* Triển khai các thành phần nền tảng: S3 Static Website, CloudFront, API Gateway và Lambda Upload Service.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Họp nhóm phân chia công việc thực hiện cho từng thành viên.<br>- Xác định phạm vi phụ trách: frontend, upload backend, AI workflow, cost tool, report generator và tài liệu. | 22/06/2026 | 22/06/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/ <br> https://chatgpt.com/ |
| 3 | - Thiết kế kiến trúc tổng thể của hệ thống.<br>- Vẽ luồng xử lý: React Frontend → API Gateway → Lambda Upload Service → S3 Input Bucket → DynamoDB. | 23/06/2026 | 23/06/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html <br> https://chatgpt.com/ |
| 4 | - Cấu hình S3 Static Website cho frontend.<br>- Chuẩn bị file build React và cấu hình bucket phục vụ nội dung tĩnh.<br>- Kiểm tra đường dẫn website sau khi upload frontend. | 24/06/2026 | 24/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html <br> https://chatgpt.com/ |
| 5 | - Cấu hình CloudFront distribution cho frontend.<br>- Thiết lập origin trỏ về S3, default root object và kiểm tra truy cập qua CloudFront domain. | 25/06/2026 | 25/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/website-hosting-cloudfront-walkthrough.html <br> https://chatgpt.com/ |
| 6 | - Thiết kế và triển khai API Gateway + Lambda Upload Service.<br>- Cấu hình route POST /upload, xử lý multipart upload, validate file, lưu file vào S3 và lưu metadata vào DynamoDB. | 26/06/2026 | 26/06/2026 | https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop.html<br>https://docs.aws.amazon.com/lambda/latest/dg/python-handler.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html <br> https://chatgpt.com/ |

### Các bước thực hiện lab trong tuần 10:

* Tạo S3 bucket dùng để host frontend, upload file build của React sau khi chạy build.
* Bật Static Website Hosting hoặc chuẩn bị S3 origin cho CloudFront tùy theo hướng triển khai.
* Tạo CloudFront distribution, cấu hình origin trỏ đến S3 và kiểm tra domain CloudFront.
* Tạo S3 Input Bucket để lưu file kiến trúc do người dùng upload.
* Tạo DynamoDB table lưu lịch sử review, dùng partition key reviewId.
* Tạo Lambda Upload Service, cấu hình biến môi trường INPUT_BUCKET, TABLE_NAME, MAX_FILE_SIZE_MB và ALLOWED_ORIGINS.
* Tạo IAM role cho Lambda có quyền PutObject vào S3 Input Bucket và PutItem vào DynamoDB.
* Tạo API Gateway HTTP API, thêm route POST /upload và tích hợp với Lambda Upload Service.
* Cấu hình CORS để frontend có thể gọi API Gateway.
* Test upload bằng frontend hoặc curl, kiểm tra file trong S3 và item metadata trong DynamoDB.

### Kết quả đạt được tuần 10:

* Nhóm đã phân chia được công việc rõ ràng.
* Thiết kế được kiến trúc tổng thể của đồ án.
* Cấu hình được frontend hosting bằng S3 và CloudFront.
* Tạo được API Gateway route cho upload file.
* Lambda Upload Service có thể upload file vào S3 Input Bucket và lưu metadata ban đầu vào DynamoDB.


---