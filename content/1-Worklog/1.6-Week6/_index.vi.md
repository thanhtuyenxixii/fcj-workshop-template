---
title: "Tuần 6: Triển khai ECS Fargate & CI/CD"
date: 2026-07-06
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

## 06/07/2026 - 12/07/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Triển khai Container ứng dụng lên Amazon ECS Fargate và tự động hóa quy trình CI/CD qua Azure DevOps / GitHub Actions.

## Bối cảnh

Tuần 6 vận hành ứng dụng trên nền tảng Serverless Container bằng AWS Fargate giúp không cần quản lý máy chủ EC2 thủ công.

## Trọng tâm học tập AWS

- **Kiến trúc Amazon ECS:** Task Definitions, Task Execution Roles, Services và Clusters.
- **AWS Fargate:** Cơ chế chạy Container Serverless.
- **CI/CD Pipeline:** Tự động hóa build Docker Image, push ECR và cập nhật ECS Service.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 06/07/2026 | Tạo ECS Task Definition liên kết với Image trên ECR (0.5 vCPU, 1GB RAM). |
| 07/07/2026 | Khởi tạo ECS Cluster và triển khai Service trên Fargate thuộc Private Subnet. |
| 08/07/2026 | Cấu hình Pipeline CI/CD trên Azure DevOps / GitHub Actions. |
| 09/07/2026 | Tự động hóa build Image, đẩy lên ECR và Trigger cập nhật ECS khi có commit mới. |
| 10/07/2026 | Kiểm thử quy trình cập nhật không gián đoạn (Rolling Update). |
| 11/07/2026 - 12/07/2026 | Thu thập log chạy Pipeline và cập nhật báo cáo. |

## Hoạt động kỹ thuật

- Khai báo ECS Task Definition chứa biến môi trường trỏ về S3 Bucket.
- Xây dựng Pipeline tự động chạy kiểm thử, đóng gói Docker và cập nhật ECS.

## Kết quả đạt được (Deliverables)

- **ECS Fargate Cluster hoạt động ổn định.**
- **Tuyến CI/CD tự động hóa 100% từ Git đến AWS.**
- **Kiểm thử cập nhật ứng dụng Rolling Update thành công.**

## Thách thức & Giải pháp

**Thách thức:** ECS Task trên Private Subnet không kéo được Image từ ECR về.

**Giải pháp:** Kiểm tra lại tuyến định tuyến NAT Gateway và cấu hình ECR VPC Endpoint.

## Đóng góp cho Dự án

Đảm bảo mô-đun đánh giá AI Agent luôn được cập nhật tự động mỗi khi bổ sung tính năng mới.

## Tài liệu tham khảo

- [Amazon ECS Developer Guide](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/Welcome.html)
- [AWS Fargate Overview](https://aws.amazon.com/fargate/)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.7-week7/)
