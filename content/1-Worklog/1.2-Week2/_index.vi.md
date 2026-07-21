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
| 2 | - Học Module về Amazon Virtual Private Cloud.<br>- Tìm hiểu khái niệm VPC, CIDR block, public subnet và private subnet.<br>- Ghi chú vai trò của VPC trong việc cô lập tài nguyên trên AWS. | 27/04/2026 | 27/04/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html <br> https://www.youtube.com/watch?v=O5CIvG0Wt78&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=28 |
| 3 | - Tìm hiểu Subnet và Route Table.<br>- Phân biệt public subnet và private subnet dựa trên route đến Internet Gateway.<br>- Vẽ lại mô hình VPC đơn giản gồm public subnet và private subnet. | 28/04/2026 | 28/04/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/configure-subnets.html |
| 4 | - Tìm hiểu Internet Gateway và NAT Gateway.<br>- Ghi chú luồng truy cập Internet từ public subnet và private subnet.<br>- Tìm hiểu khi nào cần NAT Gateway và các yếu tố có thể phát sinh chi phí. | 29/04/2026 | 29/04/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html<br>https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-gateway.html |
| 5 | - Tìm hiểu Security Group và Network ACL.<br>- So sánh Security Group theo cơ chế stateful và Network ACL theo cơ chế stateless.<br>- Ghi chú cách mở inbound/outbound rule an toàn. | 30/04/2026 | 30/04/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/vpc-security-groups.html<br>https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html |
| 6 | - Tìm hiểu VPC Resource Map và cách kiểm tra kết nối giữa các thành phần trong VPC.<br>- Tổng hợp các bước tạo VPC, subnet, route table, Internet Gateway và Security Group.<br>- Ghi lại checklist cấu hình mạng cơ bản cho một ứng dụng web trên AWS. | 01/05/2026 | 01/05/2026 | https://000003.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html |

### Các bước thực hiện lab trong tuần 2:

* Vào VPC Console và chọn đúng Region thực hành, ví dụ ap-southeast-1.
* Tạo VPC mới, khai báo IPv4 CIDR block phù hợp, ví dụ 10.0.0.0/16.
* Tạo public subnet và private subnet, gắn từng subnet vào Availability Zone phù hợp.
* Tạo Internet Gateway, attach vào VPC và thêm route 0.0.0.0/0 trỏ đến Internet Gateway cho public route table.
* Tạo NAT Gateway trong public subnet và cấu hình private route table đi Internet thông qua NAT Gateway nếu cần.
* Tạo Security Group cho EC2/web server, chỉ mở các port cần thiết như SSH, HTTP hoặc HTTPS.
* Tìm hiểu Network ACL, kiểm tra inbound/outbound rule và phân biệt với Security Group.
* Tạo EC2 trong subnet để kiểm tra kết nối mạng, sau đó cleanup tài nguyên không dùng để tránh phát sinh chi phí.

### Kết quả đạt được tuần 2:

* Hiểu được VPC là mạng ảo cô lập dùng để triển khai tài nguyên AWS.
* Phân biệt được public subnet và private subnet.
* Nắm được vai trò của Route Table trong điều hướng traffic.
* Hiểu cách Security Group và Network ACL kiểm soát truy cập mạng.
* Có khả năng mô tả luồng kết nối Internet cơ bản trong một VPC.


---