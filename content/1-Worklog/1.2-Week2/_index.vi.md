---
title: "Worklog Tuần 2"
date: 2026-07-10
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---


### Mục tiêu tuần 2:

* Hiểu Amazon VPC và các thành phần mạng cơ bản trên AWS.
* Nắm được vai trò của Subnet, Route Table, Internet Gateway, NAT Gateway, Security Group và Network ACL.
* Biết cách đọc mô hình mạng cơ bản và xác định luồng kết nối trong VPC.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Học tổng quan về Amazon VPC.<br>- Tìm hiểu CIDR block, public subnet, private subnet.<br>- Ghi chú vai trò của VPC trong việc cô lập tài nguyên trên AWS. | 27/04/2026 | 27/04/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html |
| 3 | - Tìm hiểu Subnet và Route Table.<br>- Phân biệt public subnet và private subnet dựa trên route đến Internet Gateway.<br>- Vẽ lại mô hình VPC đơn giản gồm 1 public subnet và 1 private subnet. | 28/04/2026 | 28/04/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html |
| 4 | - Tìm hiểu Internet Gateway và NAT Gateway.<br>- Ghi chú luồng truy cập Internet từ public subnet và private subnet.<br>- Tìm hiểu khi nào cần NAT Gateway và các yếu tố có thể phát sinh chi phí. | 29/04/2026 | 29/04/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html |
| 5 | - Tìm hiểu Security Group và Network ACL.<br>- So sánh Security Group stateful và Network ACL stateless.<br>- Ghi chú cách mở inbound/outbound rule an toàn. | 30/04/2026 | 30/04/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html |
| 6 | - Tìm hiểu VPC Resource Map và cách kiểm tra kết nối giữa các thành phần trong VPC.<br>- Tổng hợp các bước tạo VPC, subnet, route table, IGW và security group.<br>- Ghi lại checklist cấu hình mạng cơ bản cho một ứng dụng web trên AWS. | 01/05/2026 | 01/05/2026 | https://cloudjourney.awsstudygroup.com/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html |

### Gợi ý các bước thực hiện lab trong tuần 2:

* Create VPC.
* Create Subnet.
* Create an Internet Gateway.
* Create Route Table for outbound Internet routing via Internet Gateway.
* Create Security Groups.
* Create EC2 Instances in Subnets.
* Test connection.
* Create NAT Gateway.

### Kết quả đạt được tuần 2:

* Hiểu được VPC là mạng ảo cô lập dùng để triển khai tài nguyên AWS.
* Phân biệt được public subnet và private subnet.
* Nắm được vai trò của route table trong điều hướng traffic.
* Hiểu cách Security Group và Network ACL kiểm soát truy cập mạng.
* Có khả năng mô tả luồng kết nối Internet cơ bản trong một VPC.


---