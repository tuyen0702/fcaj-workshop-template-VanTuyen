---
title: "Worklog Tuần 6"
date: 2026-07-10
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---


### Mục tiêu tuần 6:

* Hiểu các khái niệm bảo mật cơ bản trên AWS.
* Nắm Shared Responsibility Model, IAM, Cognito, KMS, Security Hub và best practice bảo mật.
* Biết cách tổ chức quyền truy cập tài nguyên AWS an toàn hơn.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Học Shared Responsibility Model.<br>- Phân biệt trách nhiệm bảo mật của AWS và trách nhiệm của người dùng khi triển khai hệ thống. | 25/05/2026 | 25/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000005.awsstudygroup.com/vi/<br>https://aws.amazon.com/compliance/shared-responsibility-model/ |
| 3 | - Học IAM chuyên sâu hơn: user, group, role, policy, permission boundary ở mức khái niệm.<br>- Ghi chú nguyên tắc least privilege và tránh dùng root user cho công việc hằng ngày. | 26/05/2026 | 26/05/2026 | https://000002.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html |
| 4 | - Tìm hiểu IAM Policy và cách đọc policy JSON.<br>- Tìm hiểu Allow, Deny, Action, Resource, Condition.<br>- Ghi chú cách phân quyền Lambda truy cập S3/DynamoDB theo phạm vi cụ thể. | 27/05/2026 | 27/05/2026 | https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html |
| 5 | - Tìm hiểu Amazon Cognito, KMS và Security Hub ở mức tổng quan.<br>- Ghi chú trường hợp sử dụng Cognito cho xác thực, KMS cho mã hóa và Security Hub cho kiểm tra bảo mật. | 28/05/2026 | 28/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html<br>https://docs.aws.amazon.com/kms/latest/developerguide/overview.html<br>https://docs.aws.amazon.com/securityhub/latest/userguide/what-is-securityhub.html |
| 6 | - Tìm hiểu một số S3 Security Best Practices.<br>- Tổng hợp checklist bảo mật: MFA, IAM least privilege, bucket policy, encryption, logging và kiểm soát public access. | 29/05/2026 | 29/05/2026 | https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-best-practices.html |

### Các bước thực hiện lab trong tuần 6:

* Vào IAM Console và tạo IAM user theo nội dung lab nếu cần thực hành user riêng.
* Tạo IAM Group và gắn policy phù hợp cho nhóm, ưu tiên quyền tối thiểu theo nhu cầu lab.
* Tạo IAM Policy dạng JSON, đọc kỹ các thành phần Effect, Action, Resource và Condition.
* Tạo IAM Role cho dịch vụ AWS như EC2 hoặc Lambda nếu lab yêu cầu service truy cập tài nguyên khác.
* Thử Switch Role hoặc kiểm tra quyền của user sau khi gắn policy.
* Tạo một policy giới hạn quyền để quan sát cách IAM kiểm soát hành động được phép hoặc bị từ chối.
* Kiểm tra S3 bucket security: Block Public Access, bucket policy và encryption.
* Tìm hiểu KMS key dùng để mã hóa dữ liệu và Security Hub dùng để tổng hợp cảnh báo bảo mật.
* Xóa user/key/policy thử nghiệm nếu không còn dùng để tránh rủi ro bảo mật.

### Kết quả đạt được tuần 6:

* Hiểu được mô hình chia sẻ trách nhiệm bảo mật trên AWS.
* Nắm được IAM là thành phần quan trọng để kiểm soát quyền truy cập.
* Biết cách đọc policy JSON cơ bản.
* Hiểu vai trò của Cognito, KMS và Security Hub ở mức tổng quan.
* Biết cần giới hạn quyền theo từng service và từng tài nguyên khi triển khai Lambda.


---
