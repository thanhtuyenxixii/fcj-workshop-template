---
title: "Event 2"
date: 2024-01-02
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

## Event 2: AWS Enterprise Cloud Architectures & Industry Application

| Thuộc tính | Chi tiết |
|---|---|
| Tên sự kiện | AWS: Enterprise Cloud Architectures and Industry Application |
| Thời gian | 01:30 PM, ngày 04/07/2026 |
| Địa điểm | Tầng 26, Tòa nhà Bitexco Financial, 02 Hải Triều, Phường Sài Gòn, TP. Hồ Chí Minh |
| Đơn vị đồng hành | Cloud Kinetics & Renova Cloud |
| Vai trò | Người tham dự |
| Mục đích tham gia | Học hỏi kiến trúc Cloud Doanh nghiệp & Mở rộng kết nối |
| Ca làm việc | Full-time |
| Họ và tên sinh viên | Bùi Thanh Tuyền |
| Trường Đại học | Trường Đại học Bách khoa - ĐHQG TP.HCM (HCMUT) |
| Mã số sinh viên | 2353284 |

## Tổng quan sự kiện

Sự kiện chuyên đề **AWS: Enterprise Cloud Architectures and Industry Application** là một hội thảo chuyên sâu tập trung vào cách thiết kế, chuyển đổi và vận hành các hệ thống Điện toán đám mây cấp Doanh nghiệp (Enterprise Cloud). Với sự tham gia của các chuyên gia tư vấn đến từ **Cloud Kinetics** và **Renova Cloud**—hai đối tác Premier/Advanced Partner hàng đầu của AWS—hội thảo mang đến cái nhìn thực tế về hành trình đưa các hệ thống CNTT truyền thống lên AWS, tối ưu hóa chi phí vận hành (FinOps), bảo mật đa tầng và ứng dụng Data/AI vào bài toán kinh doanh quy mô lớn.

Tham dự sự kiện này giúp mình lấp đầy khoảng trống giữa kiến thức lý thuyết học ở trường và thực tế triển khai Cloud tại các tập đoàn lớn. Những chia sẻ về bài toán thực tế (Use cases) từ các ngành Tài chính, Bán lẻ và Sản xuất đã mang lại tư duy thiết kế hệ thống có khả năng mở rộng (Scalability), tính sẵn sàng cao (High Availability) và chuẩn bảo mật nghiêm ngặt.

## Các Chủ đề Thảo luận & Diễn giả

Sự kiện được chia thành các phiên trình bày kỹ thuật và thảo luận bàn tròn với các nội dung trọng tâm:

| Đơn vị / Diễn giả | Chủ đề trình bày chính |
|---|---|
| Đại diện AWS | Định hướng Kiến trúc Đám mây Doanh nghiệp chuẩn Khung AWS Well-Architected Framework |
| Chuyên gia Cloud Kinetics | Chiến lược Chuyển đổi số (Cloud Migration) & Tối ưu hóa Chi phí vận hành (FinOps) |
| Chuyên gia Renova Cloud | Xây dựng Hạ tầng Hiện đại (Modern Infrastructure), DevOps & Bảo mật Doanh nghiệp trên AWS |
| Phiên Thảo luận Bàn tròn | Giải quyết thách thức về Tuân thủ bảo mật, Data Mesh và Ứng dụng Generative AI trong Doanh nghiệp |

## Các Kiến thức Trọng tâm Thu hoạch được

### 1. Kiến trúc Chuẩn Doanh nghiệp (AWS Well-Architected Framework)

Phiên chia sẻ nhấn mạnh tầm quan trọng của việc áp dụng **AWS Well-Architected Framework** dựa trên 6 trụ cột cốt lõi khi thiết kế hệ thống lớn:
- **Tối ưu hóa Chi phí (Cost Optimization):** Sử dụng Right-sizing, Auto Scaling, Spot Instances và các gói Savings Plans.
- **Hiệu năng & Khả năng Mở rộng (Performance Efficiency):** Thiết kế hệ thống nhượng quyền Serverless, Caching đa lớp và Database phù hợp với mục đích sử dụng (Purpose-built Databases).
- **Độ tin cậy (Reliability):** Thiết kế kiến trúc Multi-AZ, Multi-Region và xây dựng quy trình Khôi phục sau thảm họa (Disaster Recovery - DR).
- **Bảo mật (Security):** Áp dụng mô hình Least Privilege, mã hóa dữ liệu At-rest/In-transit và quản lý định danh tập trung (AWS IAM Identity Center).
- **Vận hành Xuất sắc & Tối ưu Bền vững:** Tự động hóa hạ tầng bằng Infrastructure as Code (IaC) và giám sát tập trung.

### 2. Chiến dịch Dịch chuyển Hạ tầng (Cloud Migration at Scale)

Chuyên gia từ **Cloud Kinetics** đã chia sẻ về chiến lược dịch chuyển quy mô lớn cho các doanh nghiệp legacy theo mô hình **6 Rs** (Rehost, Replatform, Refactor, Repurchase, Retain, Retire):
- **Giai đoạn Đánh giá & Chuẩn bị (Landing Zone):** Xây dựng môi trường AWS Multi-Account chuẩn hóa bằng AWS Control Tower và AWS Organizations để quản lý tài nguyên và chi phí riêng biệt giữa các môi trường Dev, Staging, Prod.
- **Chiến lược Chuyển đổi:** Tối ưu hóa việc chuyển từ Lift-and-Shift (Rehost) sang mô hình Cloud-Native (Refactor) bằng cách đóng gói ứng dụng thành Container (ECS/EKS) hoặc chuyển sang Serverless.

### 3. Thực thi FinOps & Quản trị Chi phí Cloud

Một điểm nóng tại hội thảo là bài toán quản lý chi phí khi quy mô Cloud tăng trưởng nhanh. **Cloud Kinetics** đã giới thiệu văn hóa FinOps (Financial Operations) giúp kết hợp giữa đội ngũ Kỹ thuật, Tài chính và Kinh doanh:
- Sử dụng **AWS Cost Explorer** và **AWS Budgets** để đặt ngưỡng cảnh báo chi phí tự động.
- Gắn tag (Cost Allocation Tags) chi tiết cho từng tài nguyên để phân bổ chi phí chuẩn xác cho từng phòng ban/dự án.
- Tự động tắt các tài nguyên thử nghiệm (Dev/Test) ngoài giờ làm việc để tránh lãng phí.

### 4. Bảo mật & Tuân thủ Doanh nghiệp từ Renova Cloud

Chuyên gia từ **Renova Cloud** đã làm rõ cách xây dựng mô hình bảo mật Chống chịu sâu (Defense-in-Depth):
- **Bảo mật Mạng:** Sử dụng AWS Transit Gateway, AWS WAF, AWS Shield và Amazon VPC Peering/PrivateLink để cô lập luồng dữ liệu nội bộ khỏi Internet công cộng.
- **Quản lý Định danh & Truy cập:** Kết hợp Okta/Active Directory với AWS IAM để triển khai xác thực SSO và MFA bắt buộc.
- **Giám sát & Tuân thủ:** Tự động ghi log bằng AWS CloudTrail, Amazon GuardDuty và đánh giá tuân thủ cấu hình tự động qua AWS Config.

### 5. Hiện đại hóa Dữ liệu & AI trong Doanh nghiệp

Phiên thảo luận phân tích xu hướng dịch chuyển từ các kho dữ liệu tập trung (Data Warehouse) sang kiến trúc **Data Mesh** và **Data Lakehouse** trên AWS (kết hợp Amazon S3, AWS Glue, Amazon Redshift và Amazon Athena). 

Nội dung cũng cập nhật cách các doanh nghiệp tích hợp Generative AI vào quy trình vận hành thông qua **Amazon Bedrock**, giúp khai thác dữ liệu nội bộ an toàn mà không lo bị rò rỉ dữ liệu doanh nghiệp ra bên ngoài.

## Trải nghiệm Cá nhân tại Sự kiện

Tham dự sự kiện do AWS, Cloud Kinetics và Renova Cloud phối hợp tổ chức mang lại cho mình một góc nhìn rất chuyên nghiệp về ngành tư vấn Điện toán đám mây (Cloud Consulting). Mình đã có cơ hội:
- Trực tiếp quan sát cách các Solution Architect đại diện cho Partner tư vấn và giải quyết các bài toán hóc chuẩn doanh nghiệp.
- Học hỏi tư duy chọn lựa dịch vụ AWS dựa trên bài toán chi phí và độ phức tạp vận hành thay vì chỉ chọn theo xu hướng công nghệ.
- Mở rộng mạng lưới kết nối (Networking) với các anh chị kỹ sư, chuyên gia tuyển dụng và các bạn sinh viên cùng đam mê trong cộng đồng AWS.

## Các Bài học Chuyên môn Cốt lõi

- **Hạ tầng là Mã nguồn (IaC):** Việc quản lý hệ thống doanh nghiệp bắt buộc phải sử dụng các công cụ IaC như AWS CDK, Terraform hoặc CloudFormation để đảm bảo tính đồng nhất và khả năng nhân bản nhanh chóng.
- **Bảo mật là Ưu tiên số 1 (Security First):** Mọi thiết kế kiến trúc Cloud phải bắt đầu từ việc phân quyền tối thiểu (Least Privilege) và bảo vệ dữ liệu ngay từ đầu, không phải là bước bổ sung sau khi hoàn thành hệ thống.
- **Văn hóa FinOps:** Kỹ sư Cloud giỏi không chỉ xây dựng được hệ thống chạy tốt, mà còn phải biết xây dựng hệ thống với chi phí tối ưu nhất cho doanh nghiệp.
- **Tư duy Multi-Account:** Không bao giờ gộp chung tất cả ứng dụng vào một tài khoản AWS duy nhất; cần phân chia tài khoản bằng AWS Organizations để quản trị an toàn.

## Giá trị Thực tế Áp dụng vào Dự án Thực tập

Sự kiện mang lại những góc nhìn rất giá trị để mình hoàn thiện dự án thực tập **AI Coding Agent Risk Scoring on AWS SageMaker**:
- **Thiết kế Hạ tầng Chuẩn:** Áp dụng kiến trúc bảo mật với VPC Endpoints và Private Subnets cho SageMaker Endpoint và AWS Lambda, giúp ngăn chặn truy cập trái phép từ Internet.
- **Quản lý Chi phí Endpoint:** Vận dụng bài học FinOps để chọn đúng kích thước Instance (`ml.m5.xlarge`) cho SageMaker Inference và viết script tự động xóa Endpoint khi không sử dụng (Clean-up) để tránh phát sinh chi phí ngoài ý muốn.
- **Chuẩn hóa Giám sát:** Áp dụng mô hình giám sát tập trung qua Amazon CloudWatch Logs/Metrics và cấu hình cảnh báo tự động khi phát hiện đợt truy cập bất thường vào scoring API.

## Xác minh Đăng ký Participant

| Thuộc tính xác minh | Thông tin ghi nhận |
|---|---|
| Họ và tên sinh viên | Bùi Thanh Tuyền |
| Email chính | tuyen.bui2005@hcmut.edu.vn |
| Số điện thoại liên hệ | 0387697447 |
| Trường Đại học | Trường Đại học Bách khoa - ĐHQG TP.HCM (HCMUT) |
| Mã số sinh viên | 2353284 |
| Ngày đăng ký | Ngày 04 tháng 07 năm 2026 |
| Ca đăng ký | Fulltime |
| Vị trí / Tầng | Tầng 26 |
| Mục đích | Tham dự sự kiện |

## Minh chứng Tham dự

Do không chụp ảnh cá nhân trong thời gian diễn ra hội thảo, minh chứng tham dự chính thức được xác minh thông qua bản ghi lịch sử điểm danh trên Hệ thống Portal FCAJ dưới đây. Bản ghi xác nhận thông tin đăng ký và lượt check-in của mình cho ca 01:30 chiều ngày 13/06/2026 tại địa điểm Tầng 26.

![Minh chứng điểm danh trên Portal FCAJ cho Event 2 ngày 13/06/2026](static/images/events/event2.jfif)

---

[Quay lại Sự kiện Trước](/4-eventparticipated/4.1-event1/) | [Sự kiện Tiếp theo](/4-eventparticipated/4.3-event3/)
