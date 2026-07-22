---
title: "AWS Vietnam Community Day - May 2026"
date: 2026-05-23
weight: 1
chapter: false
draft: false
pre: "<b>4.1.</b> "
---

# Bài thu hoạch “AWS Vietnam Community Day – May 2026”

## Thông Tin Sự Kiện

- **Tên sự kiện:** *AWS Vietnam Community Day – May 2026*
- **Ngày tham dự:** *23/05/2026*
- **Địa điểm:** *Tầng 26, Toà nhà Bitexco*
- **Đơn vị tổ chức:** *FCAJ - First Cloud AI Journey*
- **Hình thức tham dự:** *Trực tiếp*

## Mục Đích Của Sự Kiện

- Cập nhật những xu hướng mới trong lĩnh vực **Generative AI, Agentic AI và kiến trúc ứng dụng trên AWS**.
- Chia sẻ kinh nghiệm thực tế về cách thiết kế, triển khai và vận hành hệ thống AI trong môi trường doanh nghiệp.
- Giới thiệu các phương pháp tối ưu **hiệu năng, chi phí, bảo mật và độ tin cậy** cho ứng dụng thông qua Amazon CloudFront.
- Giúp người tham dự hiểu rõ vai trò của **context engineering**, multi-agent system, guardrails và khả năng kiểm soát tính bất định của mô hình ngôn ngữ lớn.
- Tạo cơ hội học hỏi từ các dự án thực tế, hoạt động hackathon và kinh nghiệm xây dựng sản phẩm trong thời gian giới hạn.
- Kết nối sinh viên, kỹ sư và các thành viên trong cộng đồng công nghệ AWS tại Việt Nam.

## Danh Sách Diễn Giả

- **Tinh Truong** - Platform Engineer, GoTymeX
- **Pham Ng Hai Anh** - G-AsiaPacific Vietnam, AWS Community Builder
- **Nguyen Tuan Thinh** - DevOps Engineer, First Cloud AI Journey
- **Team VIB** - Chia sẻ dự án UTMorpho tại LotusHacks 2026
- **Đào Đức** - Solution Architect, Cloud Kinetics
- **Cát Vy** - Senior Business Systems Analyst, VPBank

## Nội Dung Nổi Bật

### 1. Context Is Everything – Tầm Quan Trọng Của Context Khi Làm Việc Với AI

Bài trình bày nhấn mạnh rằng mô hình AI hiện nay đã có năng lực rất mạnh, nhưng chất lượng kết quả còn phụ thuộc lớn vào cách người dùng cung cấp **context**. Nhiều câu trả lời không đúng hướng, quá dài hoặc bỏ sót yêu cầu không hẳn do mô hình yếu mà do đầu vào chưa mô tả đầy đủ mục tiêu và ràng buộc.

Một context tốt nên bao gồm:

- **Mục tiêu:** Kết quả cuối cùng cần đạt được là gì.
- **Tình huống:** Người sử dụng là sinh viên, người mới học hay thành viên của một dự án thực tế.
- **Ràng buộc:** Công nghệ, ngân sách, thời gian, phong cách và định dạng đầu ra.
- **Thông tin liên quan:** Code, tài liệu, ví dụ, yêu cầu và bằng chứng cần thiết.

Bài trình bày cũng chỉ ra ba lỗi phổ biến:

- Đưa toàn bộ tài liệu, ảnh và ghi chú vào một lần khiến thông tin quan trọng bị chìm trong dữ liệu không liên quan.
- Cung cấp lại những điều AI đã có thể nhận biết từ tài liệu, nhưng không nói rõ cần thay đổi hoặc giải quyết vấn đề gì.
- Đặt yêu cầu quá chung chung, không có tiêu chí đánh giá kết quả.

Thông điệp quan trọng là **chất lượng context quan trọng hơn số lượng context**. Quá trình sử dụng AI đang chuyển từ một prompt đơn lẻ sang các hệ thống có khả năng lưu trữ, truy xuất context và ghi nhớ thông tin hữu ích theo thời gian. Một luồng xử lý đơn giản có thể gồm: **Store → Retrieve → Generate → Learn**.

### 2. Friendly AI Assistant With Amazon Quick

Phiên trình bày giới thiệu cách sử dụng Amazon Quick Suite để hỗ trợ người dùng doanh nghiệp thực hiện các công việc thường ngày. Những khó khăn phổ biến bao gồm việc phải thu thập thông tin từ nhiều nguồn, cần chuyên gia phân tích dữ liệu chuyên ngành và phải lặp lại nhiều tác vụ thủ công tốn thời gian.

Amazon Quick Suite được mô tả như một môi trường thống nhất, kết hợp:

- Dữ liệu nội bộ của doanh nghiệp, file do người dùng tải lên, cơ sở dữ liệu và data warehouse.
- Kiến thức bên ngoài, web search và các mô hình trên Amazon Bedrock.
- Nhiều data connector và hành động tích hợp với ứng dụng bên thứ ba.
- Dashboard, chat, research, insight và các luồng automation.
- Các cơ chế quản trị như access control, guardrails, bảo mật dữ liệu và tuân thủ quy định.

Use case minh họa là một **PM Assistant** có thể tự động tạo biên bản cuộc họp, gửi email cho các bên liên quan và lên lịch cuộc họp tiếp theo. Qua đó, AI không chỉ dùng để hỏi đáp mà còn có thể tham gia trực tiếp vào quy trình nghiệp vụ và thực hiện hành động theo luồng được thiết kế.

### 3. From Edge to Origin – CloudFront as Your Foundation

Bài trình bày cho thấy Amazon CloudFront không chỉ là một dịch vụ CDN mà còn có thể đóng vai trò là lớp nền tảng phía trước ứng dụng để tối ưu **chi phí, bảo mật, độ tin cậy và hiệu năng**.

#### Tối ưu và kiểm soát chi phí

Phiên trình bày giới thiệu mô hình flat-rate pricing nhằm giúp khách hàng dễ dự đoán chi phí hơn so với việc hoàn toàn phụ thuộc vào lưu lượng sử dụng. Các gói có thể kết hợp nhiều thành phần như CDN, WAF, bảo vệ DDoS, DNS, logging và quyền lợi lưu trữ.

CloudFront còn giúp giảm tải cho origin bằng caching, request collapsing và compression. Khi số request đến origin giảm, hệ thống có thể tiết kiệm tài nguyên trên Load Balancer, EC2 và cơ sở dữ liệu.

#### Bảo mật hệ thống

Các khả năng bảo mật được đề cập gồm:

- Phân tán việc phòng thủ DDoS tại các edge location và chặn traffic không mong muốn gần nguồn phát sinh.
- Tích hợp AWS Shield và AWS WAF.
- Sử dụng HTTPS, TLS và mutual TLS cho các tình huống cần xác thực hai chiều.
- Ẩn origin bằng VPC Origin, Origin Access Control hoặc giới hạn firewall chỉ nhận traffic từ CloudFront.
- Thêm custom header bí mật để hạn chế hành vi truy cập trực tiếp vào origin.
- Kiểm soát truy cập theo vị trí địa lý.
- Bảo vệ nội dung bằng Signed URL hoặc Signed Cookie.

#### Tăng độ tin cậy

CloudFront có thể tiếp tục trả nội dung đã cache khi origin tạm thời không phản hồi, sử dụng origin failover để chuyển sang origin dự phòng và cung cấp custom error page nhằm duy trì trải nghiệm thân thiện với người dùng.

#### Cải thiện hiệu năng

Các kỹ thuật được giới thiệu gồm kiến trúc caching nhiều tầng, HTTP/3, compression, persistent connection đến origin và xử lý logic tại edge bằng CloudFront Functions hoặc Lambda@Edge. Những cơ chế này giúp giảm latency, giảm số lần kết nối đến origin và tăng tốc độ phản hồi của ứng dụng.

### 4. UTMorpho – Building an AI Product in 36 Hours

Bài chia sẻ kể lại hành trình xây dựng **UTMorpho** trong 36 giờ tại LotusHacks 2026. Ý tưởng xuất phát từ một khó khăn thực tế: nhiều công cụ AI có thể tạo giao diện, nhưng mỗi lần cần sửa một chi tiết, người dùng phải nhập prompt lại. Quá trình re-prompt có thể làm thay đổi màu sắc, khoảng cách, bố cục và tiêu tốn thêm token.

UTMorpho được xây dựng với mục tiêu:

- Tạo một UI component hoạt động được từ prompt, thay vì chỉ tạo ảnh mockup.
- Cho phép chỉnh sửa trực tiếp text, màu sắc, spacing và layout trên canvas.
- Chỉ thay đổi đúng thành phần được chọn, hạn chế design drift.
- Sử dụng smart diff để thay đổi nhỏ chỉ tiêu tốn lượng token tương ứng.
- Hỗ trợ xuất kết quả sang React.

Quá trình phát triển được chia thành các giai đoạn: thiết lập repository và quyền truy cập AWS, dựng backend cơ bản, tích hợp AI, phát triển inline editor, đồng bộ state, xử lý lỗi, cắt giảm tính năng không cần thiết, hoàn thiện demo và luyện tập phần pitching.

Các bài học nổi bật gồm:

- Ý tưởng tốt thường xuất phát từ một vấn đề mà chính nhóm phát triển đã gặp phải.
- Trong thời gian giới hạn, cần bảo vệ luồng demo chính thay vì cố hoàn thành quá nhiều tính năng.
- Sự tin tưởng và khả năng phối hợp của đội nhóm có thể quan trọng hơn việc xây dựng một quy trình phức tạp.
- Token và chi phí AI cần được xem là một ràng buộc thiết kế sản phẩm.
- AI có thể được xem như một thành viên hỗ trợ nhóm thay vì chỉ là một thư viện được gọi qua API.

### 5. Non-Determinism of “Deterministic” LLM Settings

Phiên trình bày giải thích cách mô hình ngôn ngữ lớn tạo kết quả từng token thông qua logit, softmax và các tham số như **Temperature, Top-P và Top-K**.

Về lý thuyết, khi đặt `temperature = 0`, mô hình sẽ chọn token có xác suất cao nhất và được kỳ vọng tạo ra cùng một kết quả cho cùng một prompt. Tuy nhiên, trong môi trường triển khai thực tế, cấu hình này không bảo đảm hệ thống hoàn toàn deterministic.

Các nguyên nhân chính được đề cập gồm:

- Phép toán số thực trên GPU có thể tạo sai khác rất nhỏ tùy theo thứ tự tính toán song song.
- Những sai khác nhỏ trong logit có thể làm thay đổi token được chọn.
- Nhà cung cấp thường gom request của nhiều người dùng thành batch để tối ưu GPU.
- Cấu trúc batch và các kỹ thuật tối ưu inference có thể làm kết quả thay đổi giữa các lần chạy.

Điều này ảnh hưởng đến các ứng dụng yêu cầu structured output, regression testing, prompt evaluation, benchmarking và những hệ thống có mức độ rủi ro cao.

Một số hướng giảm thiểu:

- Chạy cùng một yêu cầu nhiều lần và sử dụng majority voting.
- Giới hạn không gian đầu ra bằng JSON mode, function calling, schema hoặc grammar.
- Kiểm tra và xác thực output trước khi đưa sang bước tiếp theo.
- Thiết kế hệ thống với giả định rằng kết quả AI mang tính xác suất.
- Self-host mô hình khi cần kiểm soát sâu hạ tầng inference.
- Thực hiện testing nhiều lần trên các tình huống và bộ dữ liệu khác nhau.

Bài học quan trọng là `temperature = 0` chỉ loại bỏ một phần tính ngẫu nhiên trong quá trình sampling, chứ không loại bỏ mọi nguồn gây ra sự khác biệt của kết quả.

### 6. Enterprise-Grade Multi-Agent System – Startup Credit Scoring

Bài trình bày sử dụng bài toán chấm điểm tín dụng cho startup để minh họa sự khác biệt giữa single-agent và multi-agent system.

Hệ thống chấm điểm tín dụng truyền thống thường dựa vào lịch sử tài chính dài, tài sản thế chấp, doanh thu ổn định và biểu mẫu chuẩn hóa. Trong khi đó, startup thường chỉ có thời gian hoạt động ngắn, chưa có lịch sử tín dụng, tài sản chủ yếu là trí tuệ, đội ngũ và mức độ tăng trưởng. Dữ liệu còn phân tán trên nhiều lĩnh vực như tài chính, thị trường, đội ngũ và traction.

Một single agent có thể gặp các giới hạn:

- Context quá lớn.
- Kiến thức chuyên môn bị dàn trải.
- Không có cơ chế kiểm tra và phản biện chéo.
- Trở thành single point of failure.

Giải pháp được đề xuất là một **virtual credit committee** gồm nhiều agent chuyên biệt:

- **Manager Agent:** Điều phối toàn bộ quy trình.
- **Financial Analyst:** Phân tích cash flow, burn rate và unit economics.
- **Market Analyst:** Đánh giá thị trường, cạnh tranh và thời điểm.
- **Team Evaluator:** Đánh giá founder, đội ngũ và kinh nghiệm.
- **Risk Assessor:** Phân tích rủi ro và biện pháp giảm thiểu.
- **Compliance Agent:** Kiểm tra chính sách và quy định.

Các agent có thể chạy song song, phản biện kết quả và tạo đầu ra gồm credit score, risk rating, confidence và audit trail.

Để chuyển từ POC sang hệ thống enterprise-grade, bài trình bày đề xuất sáu nhóm yếu tố:

- **Security:** Authentication, encryption và secrets management.
- **Data Governance:** PII handling, data residency và audit logging.
- **Network:** VPC isolation, private endpoint và zero-trust.
- **Operations:** Monitoring, incident response và disaster recovery.
- **Human Factors:** Training, runbook và knowledge transfer.
- **Compliance:** Quy định ngành, chính sách nội bộ và chứng nhận.

Guardrails nên được triển khai xuyên suốt:

- **Input guardrails:** Content filtering, PII detection, prompt injection prevention và rate limiting.
- **Processing guardrails:** Token budget, timeout, model selection và tool permission.
- **Output guardrails:** Validation, hallucination detection, bias checking và compliance verification.

Luồng triển khai tham khảo sử dụng container, Amazon ECR, Amazon Bedrock, API Gateway, VPC, IAM, AWS Secrets Manager, CloudWatch, X-Ray và Infrastructure as Code. Việc triển khai nên được chia thành các giai đoạn foundation, integration, pilot và scale.

## Những Gì Học Được

### Làm Việc Hiệu Quả Với AI

- Một prompt tốt cần thể hiện rõ mục tiêu, context, ràng buộc và tiêu chí thành công.
- Không nên đưa toàn bộ dữ liệu vào mô hình; cần truy xuất đúng phần thông tin liên quan.
- Memory và retrieval giúp hệ thống AI duy trì ngữ cảnh tốt hơn qua nhiều lần tương tác.
- Đầu ra của LLM cần được xem là kết quả xác suất và phải có bước kiểm tra.

### Thiết Kế Hệ Thống AI

- Single agent phù hợp với workflow tuyến tính và phạm vi chuyên môn hẹp.
- Multi-agent phù hợp hơn khi bài toán có nhiều miền kiến thức, cần phản biện và audit.
- Guardrails phải được thiết kế ở cả input, processing và output.
- Security, governance, observability và compliance cần được xem xét ngay từ đầu.
- Token usage, latency và chi phí inference là các ràng buộc kiến trúc quan trọng.

### Kiến Trúc Và Vận Hành Trên AWS

- CloudFront có thể được sử dụng như lớp bảo vệ và tối ưu ở phía trước ứng dụng.
- Caching, request collapsing và edge computing giúp giảm tải cho origin.
- OAC, VPC Origin, WAF, Shield, TLS và Signed URL hỗ trợ xây dựng nhiều lớp bảo mật.
- Monitoring, audit trail, IAM least privilege và Infrastructure as Code là những thành phần cần thiết của hệ thống production.

### Phát Triển Sản Phẩm Và Làm Việc Nhóm

- Nên bắt đầu từ vấn đề thực tế thay vì cố tìm một ý tưởng quá lớn.
- Trong thời gian giới hạn, cần ưu tiên MVP và luồng demo quan trọng nhất.
- Team synchronization và khả năng phân chia công việc rõ ràng giúp tăng tốc độ thực hiện.
- Cần sẵn sàng cắt giảm tính năng để bảo đảm sản phẩm cốt lõi hoạt động ổn định.

## Ứng Dụng Vào Project AI AWS Architecture Reviewer

### Cải Thiện Context Cho Quá Trình Phân Tích

- Bổ sung metadata cùng với ảnh kiến trúc như loại workload, mục tiêu hệ thống, môi trường triển khai và yêu cầu ưu tiên.
- Chỉ gửi đến Bedrock các tài liệu và quy tắc liên quan đến kiến trúc đang được đánh giá.
- Xác định rõ output schema gồm detected services, Well-Architected findings, security risks, cost estimation và recommendations.
- Lưu các thông tin hữu ích theo từng `reviewId` để phục vụ truy xuất và theo dõi lịch sử.

### Mở Rộng Theo Hướng Multi-Agent

Trong phiên bản mở rộng, hệ thống có thể được tách thành các agent chuyên biệt:

- Agent nhận diện dịch vụ AWS trong diagram.
- Agent đánh giá AWS Well-Architected Framework.
- Agent phân tích security và compliance.
- Agent ước tính và tối ưu chi phí.
- Agent tổng hợp kết quả và tạo báo cáo cuối cùng.

Một manager agent có thể điều phối các agent, kiểm tra kết quả và xử lý trường hợp các agent đưa ra đánh giá khác nhau.

### Tăng Bảo Mật Và Hiệu Năng Cho Website

- Đặt CloudFront phía trước S3 frontend và API phù hợp.
- Sử dụng OAC để hạn chế truy cập trực tiếp vào S3 bucket.
- Kết hợp AWS WAF để lọc request bất thường và giới hạn tốc độ.
- Bật HTTPS, compression và HTTP/3 nếu phù hợp.
- Cân nhắc Signed URL cho các báo cáo chỉ được phép tải trong khoảng thời gian nhất định.
- Theo dõi access log, WAF log và CloudWatch metric để phát hiện sự cố.

## Trải Nghiệm Trong Event

Tham gia **AWS Vietnam Community Day – May 2026** giúp tôi tiếp cận nhiều góc nhìn khác nhau, từ cách giao tiếp hiệu quả với AI đến thiết kế kiến trúc cloud và đưa hệ thống AI vào môi trường doanh nghiệp.

### Kiến Thức Có Tính Liên Kết Cao

Các phiên trình bày tuy đề cập những chủ đề khác nhau nhưng có sự liên kết rõ ràng. Một hệ thống AI tốt cần bắt đầu bằng context chính xác, xử lý được tính bất định của mô hình, có kiến trúc agent phù hợp và được bảo vệ bởi các lớp security, governance và monitoring.

### Nhiều Tình Huống Thực Tế

Các case study về PM Assistant, UTMorpho và startup credit scoring giúp tôi hiểu cách chuyển kiến thức kỹ thuật thành một sản phẩm có giá trị. Nội dung không chỉ giới thiệu dịch vụ AWS mà còn trình bày vấn đề, quyết định kiến trúc, giới hạn và hướng triển khai thực tế.

### Thay Đổi Cách Nhìn Về AI

Tôi nhận ra rằng AI không phải thành phần có thể hoạt động ổn định chỉ bằng một prompt. Để xây dựng một ứng dụng AI đáng tin cậy, cần có context management, output validation, guardrails, logging, testing và cơ chế xử lý khi kết quả thay đổi.

### Bài Học Cho Quá Trình Làm Project

Kinh nghiệm xây dựng UTMorpho trong 36 giờ cho thấy việc xác định đúng vấn đề và tập trung vào luồng chính quan trọng hơn số lượng tính năng. Đây là bài học hữu ích cho quá trình phát triển project nhóm, đặc biệt trong giai đoạn hoàn thiện demo và chuẩn bị thuyết trình.

> Tổng thể, sự kiện đã cung cấp cho tôi cả kiến thức kỹ thuật, kinh nghiệm phát triển sản phẩm và tư duy triển khai hệ thống AI trong thực tế. Những nội dung về context engineering, CloudFront, LLM non-determinism, multi-agent architecture và enterprise guardrails có thể được áp dụng trực tiếp vào quá trình hoàn thiện project AI AWS Architecture Reviewer.
