---
title: "Worklog Tuần 11"
date: 2026-07-10
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---


### Mục tiêu tuần 11:

* Triển khai các thành phần xử lý tự động cho đồ án.
* Cấu hình S3 Input Bucket, DynamoDB, EventBridge, Step Functions, AI Analyzer Lambda và Cost Tool Lambda.
* Kiểm thử luồng workflow tự động sau khi người dùng upload file.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Họp nhóm báo cáo tiến độ thực hiện.<br>- Kiểm tra lại upload backend, S3 Input Bucket và DynamoDB review history table.<br>- Bổ sung các field cần thiết cho item review: reviewId, fileName, status, uploadDate, updatedAt. | 29/06/2026 | 29/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html<br>https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html<br>https://chatgpt.com/ |
| 3 | - Cấu hình S3 Input Bucket gửi sự kiện Object Created sang EventBridge.<br>- Tạo EventBridge rule bắt sự kiện upload file mới từ bucket input. | 30/06/2026 | 30/06/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/EventBridge.html<br>https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-rules.html<br>https://chatgpt.com/ |
| 4 | - Tạo Step Functions state machine để điều phối AI Workflow.<br>- Thiết kế các state: AnalyzeArchitectureWithAI, EstimateCost, GenerateReport.<br>- Cấu hình input/output path giữa các state. | 01/07/2026 | 01/07/2026 | https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html<br>https://docs.aws.amazon.com/step-functions/latest/dg/concepts-amazon-states-language.html<br>https://chatgpt.com/ |
| 5 | - Triển khai AI Analyzer Lambda.<br>- Cấu hình quyền đọc S3 Input Bucket và quyền gọi Amazon Bedrock.<br>- Kiểm thử Lambda đọc ảnh từ S3 và trả về danh sách dịch vụ AWS phát hiện được. | 02/07/2026 | 02/07/2026 | https://docs.aws.amazon.com/lambda/latest/dg/welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://chatgpt.com/ |
| 6 | - Triển khai Cost Tool Lambda.<br>- Gọi AWS Price List API để lấy giá các dịch vụ có mapping.<br>- Kết hợp Bedrock để tạo nhận xét và đề xuất tối ưu chi phí.<br>- Kiểm thử Step Functions chạy qua Analyzer và Cost Tool. | 03/07/2026 | 03/07/2026 | https://docs.aws.amazon.com/aws-cost-management/latest/APIReference/Welcome.html<br>https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html<br>https://chatgpt.com/ |

### Các bước thực hiện lab trong tuần 11:

* Vào S3 Input Bucket, bật Amazon EventBridge trong phần Properties để bucket gửi sự kiện sang EventBridge.
* Tạo EventBridge rule với event pattern bắt sự kiện Object Created từ bucket input.
* Cấu hình target của EventBridge rule là Step Functions state machine.
* Dùng input transformer để truyền bucket, key và region sang workflow.
* Tạo Step Functions state machine gồm các bước AnalyzeArchitectureWithAI, EstimateCost và GenerateReport.
* Tạo AI Analyzer Lambda, cấu hình MODEL_ID và BEDROCK_REGION.
* Cấp quyền cho AI Analyzer Lambda đọc object từ S3 Input Bucket và gọi Bedrock model.
* Test AI Analyzer bằng event mẫu gồm bucket, key và region.
* Tạo Cost Tool Lambda, cấu hình quyền pricing:GetProducts và bedrock:InvokeModel.
* Test Step Functions bằng một object đã upload và kiểm tra output của từng state.

### Kết quả đạt được tuần 11:

* EventBridge có thể bắt sự kiện upload file từ S3 Input Bucket.
* Step Functions có thể điều phối các Lambda theo đúng thứ tự.
* AI Analyzer Lambda kết nối được Amazon Bedrock để phân tích kiến trúc.
* Cost Tool Lambda có thể tính chi phí ước tính cho một số dịch vụ AWS phổ biến.
* Nhóm kiểm thử được workflow tự động đến bước phân tích và tính chi phí.


---
