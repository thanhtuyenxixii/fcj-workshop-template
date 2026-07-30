---
title: "Tuần 3: Lưu trữ S3 & VPC Endpoints"
date: 2026-06-15
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

## 15/06/2026 - 21/06/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Xây dựng cấu trúc lưu trữ Amazon S3 cho dữ liệu AI Agent và thiết lập kết nối nội bộ qua S3 VPC Gateway Endpoints.

## Bối cảnh

Tuần 3 tập trung chuẩn bị kho lưu trữ dữ liệu log hành vi của AI Agent và đảm bảo các máy chủ nội bộ truy cập S3 qua đường truyền riêng của AWS.

## Trọng tâm học tập AWS

- **Cấu trúc Amazon S3:** Phân chia Prefix (`raw-agent-logs/`, `processed-features/`, `model-artifacts/`).
- **Bảo mật S3:** Bật mã hóa SSE-S3, Cấu hình Bucket Policy và Block Public Access.
- **S3 VPC Gateway Endpoints:** Định tuyến dữ liệu S3 trực tiếp qua mạng nội bộ AWS.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 15/06/2026 | Triển khai EC2 kiểm thử trong Private Subnet. |
| 16/06/2026 | Khởi tạo S3 Bucket, chia Prefix và bật mã hóa SSE-S3. |
| 17/06/2026 | Cấu hình S3 Bucket Policy chỉ cho phép IAM Roles của dự án truy cập. |
| 18/06/2026 | Triển khai S3 VPC Gateway Endpoint và gắn vào Private Route Table. |
| 19/06/2026 | Kiểm thử đọc/ghi dữ liệu S3 từ EC2 riêng tư không có Internet. |
| 20/06/2026 - 21/06/2026 | Thiết lập Lifecycle Rules và lưu trữ minh chứng. |

## Hoạt động kỹ thuật

- Khởi tạo Bucket `ai-agent-risk-data-store-ap-southeast-1` có bật Versioning.
- Gắn S3 Gateway Endpoint vào Private Route Table để truyền dữ liệu an toàn.

## Kết quả đạt được (Deliverables)

- **S3 Bucket được mã hóa và phân chia Prefix chuẩn.**
- **S3 VPC Gateway Endpoint hoạt động ổn định.**
- **Kiểm thử đọc/ghi S3 nội bộ thành công.**

## Thách thức & Giải pháp

**Thách thức:** Kiểm thử đọc/ghi S3 từ máy chủ Private không có Internet.

**Giải pháp:** Sử dụng VPC Gateway Endpoint giúp kết nối thẳng tới S3 mà không cần qua Internet.

## Đóng góp cho Dự án

Tạo kho lưu trữ an toàn tuyệt đối cho toàn bộ dữ liệu mẫu và mô hình AI Agent.

## Tài liệu tham khảo

- [Amazon S3 Developer Guide](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)
- [VPC Endpoints for S3](https://docs.aws.amazon.com/vpc/latest/privatelink/vpc-endpoints-s3.html)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.4-week4/)
