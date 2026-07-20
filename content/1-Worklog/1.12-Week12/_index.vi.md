---
title: "Worklog Tuần 12"
date: 2026-07-10
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---


### Mục tiêu tuần 12:

* Hoàn thiện AI Workflow của đồ án.
* Triển khai PDF Generator Lambda, S3 Report Bucket, ReportLab Layer và cập nhật DynamoDB sau khi phân tích hoàn tất.
* Kiểm thử toàn bộ luồng và hoàn thiện báo cáo.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Triển khai PDF Generator Lambda.<br>- Nhận analysis result và cost result từ Step Functions.<br>- Gọi Amazon Bedrock để tạo nội dung final review cho báo cáo. | 06/07/2026 | 06/07/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html |
| 3 | - Cấu hình S3 Report Bucket để lưu report-data.json, report.html và report.pdf.<br>- Viết logic upload report lên S3 theo cấu trúc reports/{reviewId}/. | 07/07/2026 | 07/07/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html<br>https://docs.aws.amazon.com/lambda/latest/dg/welcome.html |
| 4 | - Tạo ReportLab Layer cho Lambda để xuất file PDF.<br>- Bổ sung font DejaVuSans để hỗ trợ hiển thị tiếng Việt trong PDF.<br>- Gắn layer vào PDF Generator Lambda và kiểm thử tạo PDF. | 08/07/2026 | 08/07/2026 | https://docs.aws.amazon.com/lambda/latest/dg/chapter-layers.html<br>https://docs.aws.amazon.com/lambda/latest/dg/welcome.html |
| 5 | - Bổ sung logic cập nhật lịch sử review trong DynamoDB sau khi tạo report thành công.<br>- Cập nhật status từ uploaded sang completed, lưu score, detectedServices, recommendations, risks, costResult và reportFiles. | 09/07/2026 | 09/07/2026 | https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html<br>https://docs.aws.amazon.com/lambda/latest/dg/welcome.html |
| 6 | - Kiểm thử toàn bộ luồng từ frontend upload file đến Step Functions, Bedrock analysis, cost estimation, report generation và hiển thị lịch sử trên frontend.<br>- Họp nhóm hoàn thiện báo cáo, rà soát hình ảnh minh họa và chuẩn bị nội dung trình bày. | 10/07/2026 | 10/07/2026 | https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-what-is.html<br>https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html |

### Gợi ý các bước thực hiện lab trong tuần 12:

* Create S3 Report Bucket.
* Create PDF Generator Lambda.
* Configure Lambda environment variables: REPORT_BUCKET, TABLE_NAME, MODEL_ID, BEDROCK_REGION.
* Create and attach ReportLab Layer.
* Register Vietnamese font in ReportLab.
* Update DynamoDB review history after workflow completed.
* Verify report-data.json, report.html and report.pdf in S3.
* Verify completed review on frontend.
* Finalize internship report and project documentation.

### Kết quả đạt được tuần 12:

* PDF Generator Lambda tạo được báo cáo HTML/PDF.
* S3 Report Bucket lưu được các file báo cáo theo từng reviewId.
* ReportLab Layer hoạt động và hỗ trợ tạo file PDF.
* DynamoDB review history được cập nhật sau khi workflow hoàn tất.
* Frontend có thể hiển thị lịch sử review và trạng thái completed.
* Nhóm hoàn thiện báo cáo và kiểm thử luồng chính của đồ án.