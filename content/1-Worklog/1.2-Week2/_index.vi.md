---
title: "Tuần 2: Mạng VPC & Bảo mật IAM"
date: 2026-06-08
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

## 08/06/2026 - 14/06/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Thiết kế hạ tầng mạng VPC tùy chỉnh và cấu hình các IAM Execution Roles cho các dịch vụ AI/ML.

## Bối cảnh

Tuần 2 tập trung cô lập môi trường mạng và thiết lập phân quyền tối thiểu trước khi triển khai mô hình Machine Learning.

## Trọng tâm học tập AWS

- **Amazon VPC Subnetting:** Quy hoạch CIDR (`10.0.0.0/16`) trên 2 Availability Zones.
- **Định tuyến & Gateways:** Cấu hình Internet Gateway cho Public Subnet và NAT Gateway cho Private Subnet.
- **Security Groups & NACLs:** Thiết lập rào chắn bảo mật Stateful và Stateless.
- **Service Roles:** Viết IAM Trust Policy cho phép SageMaker và Lambda truy cập S3 an toàn.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 08/06/2026 | Quy hoạch dải mạng CIDR và thiết kế sơ đồ Subnet. |
| 09/06/2026 | Khởi tạo VPC tùy chỉnh, 2 Public Subnets và 2 Private Subnets tại `ap-southeast-1`. |
| 10/06/2026 | Cấu hình Internet Gateway, NAT Gateway và cập nhật Route Tables. |
| 11/06/2026 | Thiết lập Security Groups cô lập tầng ứng dụng nội bộ. |
| 12/06/2026 | Tạo IAM Execution Roles (`SageMaker-Execution-Role`, `Lambda-Inference-Role`). |
| 13/06/2026 - 14/06/2026 | Kiểm thử tính cô lập của mạng và hoàn thiện sơ đồ VPC. |

## Hoạt động kỹ thuật

- Triển khai VPC (`10.0.0.0/16`) trên 2 AZs (`ap-southeast-1a`, `ap-southeast-1b`).
- Chặn truy cập trực tiếp từ Internet vào Private Subnet nhưng cho phép kết nối ra ngoài qua NAT Gateway.
- Phân quyền tối thiểu cho IAM Execution Roles.

## Kết quả đạt được (Deliverables)

- **Hạ tầng VPC tùy chỉnh đã hoàn thành.**
- **Hệ thống định tuyến Route Table & NAT Gateway hoạt động chuẩn xác.**
- **IAM Roles cho Lambda và SageMaker sẵn sàng.**

## Thách thức & Giải pháp

**Thách thức:** Tối ưu chi phí duy trì NAT Gateway trên tài khoản Student.

**Giải pháp:** Dùng AWS CLI script để xóa NAT Gateway khi không thử nghiệm và tạo lại khi cần.

## Đóng góp cho Dự án

Đảm bảo dữ liệu huấn luyện và log của AI Agent được bảo vệ hoàn toàn trong mạng nội bộ.

## Tài liệu tham khảo

- [Amazon VPC User Guide](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)
- [AWS IAM Policies](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.3-week3/)
