---
title: "Worklog Tuần 4"
date: 2026-07-10
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---


### Mục tiêu tuần 4:

* Hiểu các dịch vụ lưu trữ trên AWS, tập trung vào Amazon S3.
* Biết cách tạo S3 Bucket, upload object, cấu hình quyền truy cập và Static Website Hosting.
* Nắm các khái niệm cơ bản về bucket policy, object key, versioning và storage class.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Học tổng quan về các dịch vụ lưu trữ trên AWS.<br>- Tìm hiểu Amazon S3, S3 Bucket, Object, Object Key, Region và Storage Class. | 11/05/2026 | 11/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html |
| 3 | - Tìm hiểu tạo S3 Bucket và upload object.<br>- Tìm hiểu Block Public Access, Object Ownership và quyền truy cập object. | 12/05/2026 | 12/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html |
| 4 | - Tìm hiểu S3 Static Website Hosting.<br>- Ghi chú index document, error document và bucket website endpoint.<br>- Thử cấu hình website tĩnh với file HTML đơn giản. | 13/05/2026 | 13/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html |
| 5 | - Tìm hiểu bucket policy và cách cấp quyền đọc object cho website tĩnh.<br>- Tìm hiểu CORS trong S3 và trường hợp cần cấu hình CORS cho frontend. | 14/05/2026 | 14/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/example-bucket-policies.html<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/cors.html |
| 6 | - Tìm hiểu S3 Versioning, lifecycle và một số best practice lưu trữ.<br>- Tổng hợp các bước triển khai static website bằng S3.<br>- Ghi chú các lỗi thường gặp khi truy cập S3 website. | 15/05/2026 | 15/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/Versioning.html<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lifecycle-mgmt.html |

### Các bước thực hiện lab trong tuần 4:

* Vào S3 Console, chọn Create bucket và đặt tên bucket duy nhất toàn cầu.
* Chọn Region phù hợp, ví dụ ap-southeast-1, sau đó cấu hình Object Ownership và Block Public Access theo yêu cầu lab.
* Upload các file website tĩnh như index.html, error.html, CSS, JavaScript hoặc hình ảnh.
* Vào Properties của bucket, bật Static website hosting và khai báo index document/error document.
* Tạo bucket policy cho phép public read object nếu lab yêu cầu website truy cập công khai.
* Kiểm tra website endpoint được S3 cung cấp và test bằng trình duyệt.
* Bật Bucket Versioning để theo dõi phiên bản object khi upload lại file.
* Tìm hiểu Lifecycle rule để chuyển hoặc xóa object cũ nếu cần tối ưu lưu trữ.
* Tắt public access hoặc xóa bucket sau khi hoàn tất lab nếu không tiếp tục sử dụng.

### Kết quả đạt được tuần 4:

* Hiểu được cách S3 lưu trữ dữ liệu dưới dạng object.
* Biết cấu trúc Bucket, Object và Object Key.
* Nắm được các bước cơ bản để bật Static Website Hosting.
* Hiểu bucket policy và public access ảnh hưởng đến khả năng truy cập website.
* Biết S3 có thể được dùng làm nơi lưu trữ frontend hoặc file upload trong đồ án.


---
