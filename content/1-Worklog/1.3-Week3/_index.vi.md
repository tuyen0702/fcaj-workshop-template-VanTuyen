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
| 2 | - Học tổng quan về Amazon EC2 và vai trò của EC2 trong kiến trúc cloud.<br>- Tìm hiểu Instance Type, vCPU, RAM, instance family và cách chọn instance phù hợp. | 04/05/2026 | 04/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html |
| 3 | - Tìm hiểu AMI, hệ điều hành, root volume và vòng đời EC2 instance.<br>- Ghi chú các trạng thái EC2: pending, running, stopped và terminated. | 05/05/2026 | 05/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html |
| 4 | - Tìm hiểu Key Pair và các cách remote vào EC2.<br>- Tìm hiểu SSH cho Linux instance và RDP cho Windows instance.<br>- Ghi chú vấn đề phân quyền file key khi dùng SSH trên Windows. | 06/05/2026 | 06/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html |
| 5 | - Tìm hiểu Amazon EBS, root volume, data volume và snapshot.<br>- Tìm hiểu User Data dùng để chạy script khi EC2 khởi tạo.<br>- Ghi chú cách dùng User Data để cài web server cơ bản. | 07/05/2026 | 07/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html |
| 6 | - Tìm hiểu EC2 Metadata và vai trò của IAM Role for EC2.<br>- Tổng hợp quy trình tạo EC2 instance từ Console.<br>- Ghi lại checklist bảo mật cơ bản khi triển khai EC2. | 08/05/2026 | 08/05/2026 | https://000004.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instancedata-data-retrieval.html<br>https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_use_switch-role-ec2.html |

### Các bước thực hiện lab trong tuần 3:

* Vào EC2 Console, chọn Launch Instance và đặt tên instance theo nội dung lab.
* Chọn AMI phù hợp, ví dụ Amazon Linux hoặc Ubuntu, sau đó chọn instance type nhỏ như t2.micro/t3.micro nếu phù hợp Free Tier.
* Tạo hoặc chọn Key Pair để kết nối SSH, tải file .pem và lưu ở thư mục an toàn.
* Cấu hình Network Settings: chọn VPC, subnet và Security Group cho phép SSH từ IP cá nhân.
* Kiểm tra phần Storage, root volume và dung lượng EBS được gắn vào instance.
* Khởi tạo instance, chờ trạng thái running và kiểm tra Public IPv4 address/Public DNS.
* Dùng SSH để kết nối vào EC2, kiểm tra hệ điều hành bằng các lệnh cơ bản như hostname, uname, df -h.
* Thử đọc EC2 metadata hoặc kiểm tra IAM Role nếu instance được gắn role.
* Dừng hoặc terminate instance sau khi hoàn tất lab để tránh phát sinh chi phí.

### Kết quả đạt được tuần 3:

* Hiểu được vai trò của EC2 trong nhóm dịch vụ Compute.
* Nắm được các thành phần cần cấu hình khi tạo EC2 instance.
* Biết cách kết nối SSH/RDP vào EC2 ở mức cơ bản.
* Hiểu vai trò của EBS volume và snapshot.
* Biết User Data có thể tự động hóa cài đặt phần mềm khi instance khởi tạo.


---
