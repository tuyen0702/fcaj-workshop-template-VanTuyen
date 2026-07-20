---
title: "Worklog Tuần 3"
date: 2026-07-10
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---


### Mục tiêu tuần 3:

* Hiểu Amazon EC2 và nhóm dịch vụ Compute trên AWS.
* Nắm được các thành phần khi tạo EC2: AMI, Instance Type, Key Pair, Security Group, EBS, User Data và Metadata.
* Biết cách khởi tạo, kết nối và quản lý EC2 instance ở mức cơ bản.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Học tổng quan về Amazon EC2 và vai trò của EC2 trong kiến trúc cloud.<br>- Tìm hiểu instance type, vCPU, RAM, family và cách chọn instance phù hợp. | 04/05/2026 | 04/05/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html |
| 3 | - Tìm hiểu AMI, hệ điều hành, root volume và vòng đời EC2 instance.<br>- Ghi chú các trạng thái EC2: pending, running, stopped, terminated. | 05/05/2026 | 05/05/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html |
| 4 | - Tìm hiểu Key Pair và các cách remote vào EC2.<br>- Tìm hiểu SSH cho Linux instance và RDP cho Windows instance.<br>- Ghi chú vấn đề phân quyền file key khi dùng SSH trên Windows. | 06/05/2026 | 06/05/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html |
| 5 | - Tìm hiểu Amazon EBS, root volume, data volume và snapshot.<br>- Tìm hiểu User Data dùng để chạy script khi EC2 khởi tạo.<br>- Ghi chú cách dùng User Data để cài web server cơ bản. | 07/05/2026 | 07/05/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html |
| 6 | - Tìm hiểu EC2 Metadata và vai trò của IAM Role for EC2.<br>- Tổng hợp quy trình tạo EC2 instance từ Console.<br>- Ghi lại checklist bảo mật cơ bản khi triển khai EC2. | 08/05/2026 | 08/05/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html<br>https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html |

### Gợi ý các bước thực hiện lab trong tuần 3:

* Create EC2 instance.
* Configure Security Group for EC2.
* Connect to EC2 using SSH.
* Review EBS volume.
* Test User Data script.
* Explore EC2 instance metadata.
* Review IAM Role for EC2.

### Kết quả đạt được tuần 3:

* Hiểu được vai trò của EC2 trong nhóm dịch vụ Compute.
* Nắm được các thành phần cần cấu hình khi tạo EC2 instance.
* Biết cách kết nối SSH/RDP vào EC2 ở mức cơ bản.
* Hiểu vai trò của EBS volume và snapshot.
* Biết User Data có thể tự động hóa cài đặt phần mềm khi instance khởi tạo.


---