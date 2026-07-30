---
title: "Tuần 1: Khởi động & Nền tảng AWS"
date: 2026-06-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

## 01/06/2026 - 07/06/2026

**Hình thức làm việc:** Tự thực hiện kết hợp thảo luận nhóm.
**Chương trình:** Workforce Bootcamp - First Cloud AI Journey.
**Người hướng dẫn (Mentor):** Tự quản lý tiến độ với sự hỗ trợ từ tài liệu AWS và cộng đồng.

## Mục tiêu

Nắm rõ yêu cầu thực tập, chọn đề tài dự án kỹ thuật và xây dựng kiến thức nền tảng AWS để chuẩn bị cho việc triển khai dự án.

## Bối cảnh

Tuần đầu tiên tập trung làm quen với lộ trình thực tập AWS First Cloud AI Journey. Do làm việc theo hình thức tự quản lý, việc xác định mục tiêu hàng tuần, lưu trữ minh chứng và dựng khung báo cáo Hugo được ưu tiên ngay từ đầu.

## Trọng tâm học tập AWS

- **AWS Global Infrastructure:** Nghiên cứu Region, Availability Zone và nhất quán chọn Region `ap-southeast-1`.
- **AWS IAM & Bảo mật:** Ôn tập cấu trúc IAM Policy, Role, Trust Relationship và nguyên tắc phân quyền tối thiểu.
- **Shared Responsibility Model:** Phân định trách nhiệm bảo mật giữa AWS và người dùng.
- **Tổng quan S3 & CloudWatch:** Tìm hiểu lưu trữ theo Prefix trên S3 và cơ chế ghi log trên CloudWatch.

## Chi tiết công việc hàng ngày

| Ngày | Công việc đã thực hiện |
|---|---|
| 01/06/2026 | Nghiên cứu yêu cầu báo cáo thực tập và tạo cấu trúc thư mục Hugo. |
| 02/06/2026 | Tìm hiểu hạ tầng toàn cầu AWS, thiết lập AWS CLI và AWS Budgets. |
| 03/06/2026 | Ôn tập IAM, Shared Responsibility Model và phân quyền trên Cloud. |
| 04/06/2026 | Chốt đề tài: Đánh giá rủi ro cho AI Coding Agent (Risk Scoring). |
| 05/06/2026 | Phác thảo sơ đồ dịch vụ AWS MVP (S3, SageMaker, Lambda, API Gateway). |
| 06/06/2026 - 07/06/2026 | Tổng hợp tài liệu tham khảo và lưu trữ minh chứng Tuần 1. |

## Hoạt động kỹ thuật

- Thiết lập môi trường phát triển cục bộ với VS Code, Git, AWS CLI và Hugo.
- Xác định sơ đồ luồng dữ liệu: Log sự kiện Agent -> S3 -> SageMaker Model -> Lambda -> API Gateway.

## Kết quả đạt được (Deliverables)

- **Đã chốt đề tài thực tập.**
- **Đã dựng xong khung báo cáo Hugo.**
- **Đã phác thảo sơ đồ kiến trúc MVP.**

## Thách thức & Giải pháp

**Thách thức:** Khoanh vùng phạm vi đề tài AI/Cloud sao cho vừa sức với tài khoản AWS Student.

**Giải pháp:** Giới hạn MVP vào việc đánh giá rủi ro dựa trên log hành vi của AI Agent, đảm bảo tính khả thi cao.

## Đóng góp cho Dự án

Đặt nền móng lý thuyết và kiến trúc để chuyển đổi bài toán đánh giá rủi ro AI Agent sang mô hình Cloud-native.


## Tài liệu tham khảo

- [AWS Cloud Practitioner Essentials](https://aws.amazon.com/training/digital/aws-cloud-practitioner-essentials/)
- [AWS IAM Best Practices](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)

---

[Quay lại Worklog](/1-worklog/) | [Tuần tiếp theo](/1-worklog/1.2-week2/)
