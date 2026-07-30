---
title: "Tuần 5: Đóng gói Container với Docker & Amazon ECR"
date: 2026-06-29
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

## 29/06/2026 - 05/07/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS.

## Mục tiêu

Đóng gói mô-đun đánh giá rủi ro AI Agent bằng Docker và lưu trữ Container Image trên Amazon ECR.

## Bối cảnh

Tuần 5 đóng gói toàn bộ mã nguồn Python, thư viện PyTorch và script xử lý dữ liệu thành Docker Container để đảm bảo tính nhất quán khi triển khai lên Cloud.

## Trọng tâm học tập AWS

- **Tối ưu Dockerfile:** Kỹ thuật Multi-stage build và chọn Base Image nhẹ (`python-slim`).
- **Docker Compose:** Điều phối ứng dụng đa container để kiểm thử cục bộ.
- **Amazon ECR:** Tạo Private Registry, đăng nhập qua AWS CLI và quản lý Image Tags.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 29/06/2026 | Chuẩn bị danh sách thư viện Python (`torch`, `boto3`, `scikit-learn`). |
| 30/06/2026 | Viết Dockerfile tối ưu cho Risk Scoring Engine. |
| 01/07/2026 | Build và kiểm thử chạy Docker Container cục bộ. |
| 02/07/2026 | Khởi tạo Private ECR Repository `ai-agent-risk-evaluator`. |
| 03/07/2026 | Đăng nhập ECR qua AWS CLI và đẩy (push) Image lên Cloud. |
| 04/07/2026 - 05/07/2026 | Bật tính năng quét lỗ hổng bảo mật (Image Scanning) trên ECR. |

## Hoạt động kỹ thuật

- Viết Dockerfile tối ưu dung lượng cho mô-đun Python PyTorch.
- Đẩy Docker Images chứa các Tag (`v1.0.0`, `latest`) lên ECR.

## Kết quả đạt được (Deliverables)

- **Dockerfile chuẩn hóa cho bộ mô hình AI.**
- **Private Amazon ECR Repository đi vào hoạt động.**
- **Docker Image được tải lên ECR thành công.**

## Thách thức & Giải pháp

**Thách thức:** Dung lượng Docker Image quá lớn do chứa thư viện PyTorch mặc định.

**Giải pháp:** Sử dụng bản PyTorch CPU-only giúp giảm hơn 60% dung lượng Image.

## Đóng góp cho Dự án

Tạo ra các đóng gói Container chuẩn bị cho việc triển khai linh hoạt trên hạ tầng Serverless ECS Fargate.

## Tài liệu tham khảo

- [Docker Documentation](https://docs.docker.com/)
- [Amazon ECR User Guide](https://docs.aws.amazon.com/AmazonECR/latest/userguide/what-is-ecr.html)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.6-week6/)
